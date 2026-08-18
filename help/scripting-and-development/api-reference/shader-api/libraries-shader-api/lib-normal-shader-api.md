---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-normal-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador Lib Normal de Substance 3D Painter para trabajar con mapas normales y normales de superficie en sombreadores personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Normal - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Normal - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---


# Lib Normal - API del sombreador

## lib-normal.glsl

**Funciones públicas:** *normalBlend* *normalBlendOriented* *normalFade* *normalUnpack* *normalFromBaseNormal* *normalFromNormal* *normalFromHeight* *getTSNormal* *computeWSBaseNormal* 0&rbrace;computeWSNormal **

Importar desde biblioteca

```
import lib-defines.glsl 

import lib-sparse.glsl
```


Todos los parámetros del motor son útiles para operaciones centradas en la normalidad.

```
//: param auto channel_height 

uniform SamplerSparse height_texture; 

//: param auto channel_normal 

uniform SamplerSparse normal_texture; 

//: param auto texture_normal 

uniform SamplerSparse base_normal_texture; 

//: param auto normal_blending_mode 

uniform int normal_blending_mode;
```


Se utiliza para invertir el eje Y del mapa normal

```
//: param auto normal_y_coeff 

uniform float base_normal_y_coeff;
```


Determinados empíricamente por nuestros artistas...

```
const float HEIGHT_FACTOR = 400.0;
```


Realizar la fusión entre 2 mapas normales

Esto se basa en la fusión de Whiteout http://blog.selfshadow.com/publications/blending-in-detail/

```
vec3 normalBlend(vec3 baseNormal, vec3 overNormal) 

{ 

  return normalize(vec3( 

    baseNormal.xy + overNormal.xy, 

    baseNormal.z  * overNormal.z)); 

}
```


Realizar una fusión orientada a detalles entre 2 mapas normales

Esto se basa en la fusión orientada a los detalles http://blog.selfshadow.com/publications/blending-in-detail/

```
vec3 normalBlendOriented(vec3 baseNormal, vec3 overNormal) 

{ 

  baseNormal.z += 1.0; 

  overNormal.xy = -overNormal.xy; 

  return normalize(baseNormal * dot(baseNormal,overNormal) - 

    overNormal*baseNormal.z); 

}
```


Devuelve un valor normal acoplado por un factor de atenuación

```
vec3 normalFade(vec3 normal,float attenuation) 

{ 

  if (attenuation<1.0 && normal.z<1.0) 

  { 

    float phi = attenuation * acos(normal.z); 

    normal.xy *= 1.0/sqrt(1.0-normal.z*normal.z) * sin(phi); 

    normal.z = cos(phi); 

  } 

 

  return normal; 

}
```


Desempaquetar una normal con canal alfa

```
vec3 normalUnpack(vec4 normal_alpha, float y_coeff) 

{ 

  if (normal_alpha.a == 0.0 || normal_alpha.xyz == vec3(0.0)) { 

    return vec3(0.0, 0.0, 1.0); 

  } 

 

  // Attenuation in function of alpha 

  vec3 normal = normal_alpha.xyz/normal_alpha.a * 2.0 - vec3(1.0); 

  normal.y *= y_coeff; 

  normal.z = max(1e-3, normal.z); 

  normal = normalize(normal); 

  normal = normalFade(normal, normal_alpha.a); 

 

  return normal; 

}
```


Desempaquetar un canal alfa normal con inversión Y

```
vec3 normalUnpack(vec4 normal_alpha) 

{ 

  return normalUnpack(normal_alpha, 1.0); 

}
```


Calcular el espacio de tangente normal desde el canal de height del documento

```
vec3 normalFromHeight(SparseCoord coord, float height_force) 

{ 

  // Normal computation using height map 

 

  // Determine gradient offset in function of derivatives 

  vec2 dfd = max(coord.dfdx,coord.dfdy); 

  dfd = max(dfd,height_texture.size.zw); 

 

  vec2 dfdx,dfdy; 

  textureSparseQueryGrad(dfdx, dfdy, height_texture, coord); 

  float h_r  = textureGrad(height_texture.tex, coord.tex_coord+vec2( dfd.x,  0    ), dfdx, dfdy).r; 

  float h_l  = textureGrad(height_texture.tex, coord.tex_coord+vec2(-dfd.x,  0    ), dfdx, dfdy).r; 

  float h_t  = textureGrad(height_texture.tex, coord.tex_coord+vec2(     0,  dfd.y), dfdx, dfdy).r; 

  float h_b  = textureGrad(height_texture.tex, coord.tex_coord+vec2(     0, -dfd.y), dfdx, dfdy).r; 

  float h_rt = textureGrad(height_texture.tex, coord.tex_coord+vec2( dfd.x,  dfd.y), dfdx, dfdy).r; 

  float h_lt = textureGrad(height_texture.tex, coord.tex_coord+vec2(-dfd.x,  dfd.y), dfdx, dfdy).r; 

  float h_rb = textureGrad(height_texture.tex, coord.tex_coord+vec2( dfd.x, -dfd.y), dfdx, dfdy).r; 

  float h_lb = textureGrad(height_texture.tex, coord.tex_coord+vec2(-dfd.x, -dfd.y), dfdx, dfdy).r; 

 

  vec2 dh_dudv = (0.5 * height_force) / dfd * vec2( 

    2.0*(h_l-h_r)+h_lt-h_rt+h_lb-h_rb, 

    2.0*(h_b-h_t)+h_rb-h_rt+h_lb-h_lt); 

 

  return normalize(vec3(dh_dudv, HEIGHT_FACTOR)); 

}
```


Ayudante para calcular el espacio de tangente normal a partir de normal base y un valor de height, y un detalle normal opcional.

```
vec3 getTSNormal(SparseCoord coord, vec3 normalFromHeight) 

{ 

  vec3 normal = normalBlendOriented( 

    normalUnpack(textureSparse(base_normal_texture, coord), base_normal_y_coeff), 

    normalFromHeight); 

 

  if (normal_texture.is_set) { 

    vec3 channelNormal = normalUnpack(textureSparse(normal_texture, coord)); 

    if (normal_blending_mode == BlendingMode_Replace) { 

      normal = normalBlendOriented(normalFromHeight, channelNormal); 

    } else if (normal_blending_mode == BlendingMode_NM_Combine) { 

      normal = normalBlendOriented(normal, channelNormal); 

    } 

  } 

 

  return normal; 

}
```


Ayudante para calcular el espacio de tangente normal a partir de la base normal y height, y un detalle opcional normal.

```
vec3 getTSNormal(SparseCoord coord) 

{ 

  float height_force = 1.0; 

  vec3 normalH = normalFromHeight(coord, height_force); 

  return getTSNormal(coord, normalH); 

}
```


Ayudante para calcular la normalidad espacial mundial a partir de la base espacial tangente normal.

```
vec3 computeWSBaseNormal(SparseCoord coord, vec3 tangent, vec3 bitangent, vec3 normal) 

{ 

  vec3 normal_vec = normalUnpack(textureSparse(normal_texture, coord), base_normal_y_coeff); 

  return normalize( 

    normal_vec.x * tangent + 

    normal_vec.y * bitangent + 

    normal_vec.z * normal 

  ); 

}
```


Ayudante para calcular la normalidad del espacio mundial a partir de la normalidad del espacio tangente dada por los ayudantes getTSNormal y el marco local de la malla.

```
vec3 computeWSNormal(SparseCoord coord, vec3 tangent, vec3 bitangent, vec3 normal) 

{ 

  vec3 normal_vec = getTSNormal(coord); 

  return normalize( 

    normal_vec.x * tangent + 

    normal_vec.y * bitangent + 

    normal_vec.z * normal 

  ); 

} 

 
```
