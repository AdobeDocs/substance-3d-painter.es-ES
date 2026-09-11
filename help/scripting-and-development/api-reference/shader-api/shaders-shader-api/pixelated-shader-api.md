---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/pixelated-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador pixeladas de Substance 3D Painter para crear efectos de representación pixelada personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Pixelated - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pixelado - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---


# Pixelado - API del sombreador

## Sombreador básico de pixelado

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


Punto de entrada del sombreador.

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


**La prioridad** es realizar la **detección de esquema**. Si se alcanza la condición de contorno, salga con color negro.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  } 

 

  vec3 baseColor = getBaseColor(basecolor_tex, inputs.sparse_coord);
```


Variación del tamaño de la máscara basada en la luminancia de color base

```
  float maskRadiusJitter = pow(dot(baseColor, vec3(0.3333)), 0.1);
```


Calcula un valor de máscara en función de la posición del espacio de pantalla del fragmento. Esto creará una cuadrícula como un patrón.

```
  float mask = pow(1.0 - length(fract(gl_FragCoord.xy / 7.0) - vec2(0.5)), maskRadiusJitter * 5.0) * 5.0;
```


Aquí, probamos el color base y aplicamos una atenuación difusa simple

```
  vec3 color = baseColor * NdL; 

 

  diffuseShadingOutput(mask * color); 

} 

 
```
