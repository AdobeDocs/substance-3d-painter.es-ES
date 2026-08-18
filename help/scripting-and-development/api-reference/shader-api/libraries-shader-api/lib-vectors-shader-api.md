---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-vectors-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador Vectores de labios de Substance 3D Painter para trabajar con operaciones vectoriales en sombreados personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Vectors - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Vectores Lib - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---


# Vectores Lib - API del sombreador

## lib-vectors.glsl

**Funciones públicas:** *computeLocalFrame* *getEyeVec* *tangentSpaceToWorldSpace* *worldSpaceToTangentSpace*

Importar desde biblioteca

```
import lib-normal.glsl
```


Qué vista está sombreada.

```
//: param auto is_2d_view 

uniform bool is2DView;
```


Qué tipo de proyección se utiliza.

```
//: param auto is_perspective_projection 

uniform bool is_perspective;
```


Posición de los ojos en el espacio mundial.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


Orientación de la cámara en el espacio internacional.

```
//: param auto world_camera_direction 

uniform vec3 camera_dir; 

 

//: param auto facing 

uniform int facing; 

 

bool isBackFace() { 

  return facing == -1 || (facing == 0 && !gl_FrontFacing); 

}
```


Calcular el vector de ojo espacial mundial

```
vec3 getEyeVec(vec3 position) { 

  return is_perspective ? 

    normalize(camera_pos - position) : 

    -camera_dir; 

}
```


Convertir un vector de espacio tangente a espacio de mundo

```
vec3 tangentSpaceToWorldSpace(vec3 vecTS, V2F inputs) { 

  return normalize( 

    vecTS.x * inputs.tangent + 

    vecTS.y * inputs.bitangent + 

    vecTS.z * inputs.normal); 

}
```


Conversión de un vector del espacio de entorno al espacio tangente

```
vec3 worldSpaceToTangentSpace(vec3 vecWS, V2F inputs) { 

  // Assume the transformation is orthogonal 

  return normalize(vecWS * mat3(inputs.tangent, inputs.bitangent, inputs.normal)); 

}
```


Marco local del vértice en el espacio mundial

```
struct LocalVectors { 

  vec3 vertexNormal; 

  vec3 tangent, bitangent, normal, eye; 

};
```


Calcular el fotograma local a partir de la normal del espacio del mundo personalizado y el ángulo de anisotropía

```
LocalVectors computeLocalFrame(V2F inputs, vec3 normal, float anisoAngle) { 

  LocalVectors vectors; 

  vectors.vertexNormal = inputs.normal; 

  vectors.normal = normal; 

 

  // Flip the normals for back facing polygons 

  if (isBackFace()) { 

    vectors.vertexNormal = -vectors.vertexNormal; 

    vectors.normal = -vectors.normal; 

  } 

 

  vectors.eye = is2DView ? 

    vectors.normal : // In 2D view, put view vector along the normal 

    getEyeVec(inputs.position); 

 

  // Trick to remove black artifacts 

  // Backface ? place the eye at the opposite - removes black zones 

  if (dot(vectors.eye, vectors.normal) < 0.0) { 

    vectors.eye = reflect(vectors.eye, vectors.normal); 

  } 

 

  // Create a local frame for BRDF work 

  vec3 tangent = normalize( 

    inputs.tangent 

    * vectors.normal * dot(inputs.tangent, vectors.normal) 

  ); 

  vec3 bitangent = normalize( 

    inputs.bitangent 

    * vectors.normal * dot(inputs.bitangent, vectors.normal) 

    * tangent * dot(inputs.bitangent, tangent) 

  ); 

 

  float cosAngle = cos(anisoAngle); 

  float sinAngle = sin(anisoAngle); 

  vectors.tangent = cosAngle * tangent - sinAngle * bitangent; 

  vectors.bitangent = cosAngle * bitangent + sinAngle * tangent; 

 

  return vectors; 

}
```


Calcular el marco local a partir de mallas y height de documentos y normales

```
LocalVectors computeLocalFrame(V2F inputs) { 

  // Get world space normal 

  vec3 normal = computeWSNormal(inputs.sparse_coord, inputs.tangent, inputs.bitangent, inputs.normal); 

  return computeLocalFrame(inputs, normal, 0.0); 

} 

 
```
