---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/toon-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador de caricatura de Substance 3D Painter para crear efectos de representación personalizados al estilo de caricatura.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Toon - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Toon - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# Toon - API del sombreador

## Sombreador de tonos básico

Importar desde bibliotecas.

```
import lib-sampler.glsl
```


Definimos la posición global de la luz

```
const vec3 light_pos = vec3(10.0, 10.0, 10.0);
```


**enlazamos** la posición del ojo del mundo del parám automático a nuestro uniforme **camera\_pos**.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


**Enlazamos** el canal del documento **color base** a nuestro uniforme **color base\_tex**.

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex;
```


**enlazamos** la **curvatura de malla** a nuestro **texto de curvatura\** uniforme. Si no hay ninguna curvatura disponible, se proporciona una textura transparente.

```
//: param auto texture_curvature 

uniform SamplerSparse curvature_tex;
```


Definimos un nuevo ajuste personalizado para este sombreador, junto con su valor predeterminado. Este se utiliza para ajustar el thickness del contorno, cuando está sombreado.

```
//: param custom { 

//:  "default": 0.4, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Unlit outline thickness" 

//: } 

uniform float unlit_outline_thickness;
```


Definimos un nuevo ajuste personalizado para este sombreador, junto con su valor predeterminado. Este se utiliza para ajustar el thickness del contorno, cuando está iluminado.

```
//: param custom { 

//:   "default": 0.1, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Lit outline thickness" 

//: } 

uniform float lit_outline_thickness;
```


Si preferimos usar la curvatura o no.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Use curvature" 

//: } 

uniform bool use_curvature;
```


Punto de entrada del sombreado.

```
void shade(V2F inputs) 

{
```


Calculamos algunos valores útiles.

```
  vec3 V = normalize(camera_pos - inputs.position); 

  vec3 N = normalize(inputs.normal); 

  vec3 L = normalize(light_pos - inputs.position); 

  float NdV = dot(N, V); 

  float NdL = max(0.0, dot(N, L));
```


**La prioridad** es realizar la **detección de esquema**. Permite al usuario elegir si prefiere utilizar el mapa de curvatura para la detección de contornos o no.

```
  if (use_curvature) { 

    float curv = textureSparse(curvature_tex, inputs.sparse_coord).r; 

    NdV = 1.0 - curv; 

  }
```


Si se alcanza la condición de contorno, salga con color negro.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  }
```


Aquí, realizamos una discretización de color en 4 pasos.

```
  vec3 color = getBaseColor(basecolor_tex, inputs.sparse_coord); 

  if (NdL > 0.75) { 

    color = color; 

  } else if (NdL > 0.5) { 

    color = color * 0.5; 

  } else if (NdL > 0.1) { 

    color = color * 0.1; 

  } 

  else
```


La reserva es negra.

```
    color = vec3(0.0); 

 

  diffuseShadingOutput(color); 

} 

 
```
