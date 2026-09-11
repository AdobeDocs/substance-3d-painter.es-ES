---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-random-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador Lib Random para Substance 3D Painter para generar valores aleatorios en el desarrollo de sombreadores personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Random - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Aleatorio de labios - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---


# Aleatorio de labios - API del sombreador

## lib-random.glsl

**Funciones públicas:** *getBlueNoiseThreshold* *getBlueNoiseThresholdTemporal* *fibonacci1D* *fibonacci2D* *fibonacci2DeitheredTemporal*

Importar desde biblioteca

```
import lib-defines.glsl
```


Textura de ruido azul 2D que contiene valores escalares

```
//: param auto texture_blue_noise 

uniform sampler2D texture_blue_noise;
```


Resolución de textura de ruido azul

```
const ivec2 texture_blue_noise_size = ivec2(256);
```


Semilla aleatoria del marco actual

```
//: param auto random_seed 

uniform int alg_random_seed;
```


Obtenga un valor aleatorio uniforme basado en coordenadas de píxeles.

```
float getBlueNoiseThreshold() 

{ 

  return texture(texture_blue_noise, gl_FragCoord.xy / vec2(texture_blue_noise_size)).x + 0.5 / 65536.0; 

}
```


Obtenga un valor aleatorio uniforme basado en las coordenadas de píxeles y el ID de marco.

```
float getBlueNoiseThresholdTemporal() 

{ 

  return fract(getBlueNoiseThreshold() + M_GOLDEN_RATIO * alg_random_seed); 

}
```


Devuelve el número i *th* de la secuencia de fibonacci.

```
float fibonacci1D(int i) 

{ 

  return fract((float(i) + 1.0) * M_GOLDEN_RATIO); 

}
```


Devuelve la pareja i *th* de la secuencia de fibonacci. nbSample es necesario para obtener una distribución uniforme.

```
vec2 fibonacci2D(int i, int nbSamples) 

{ 

  return vec2( 

    (float(i)+0.5) / float(nbSamples), 

    fibonacci1D(i) 

  ); 

}
```


Devuelve la pareja i *th* de la secuencia de fibonacci. nbSample es necesario para obtener una distribución uniforme. Esta versión tiene una rotación pseudoaleatoria por marco y por píxel aplicada.

```
vec2 fibonacci2DDitheredTemporal(int i, int nbSamples) 

{ 

  vec2 s = fibonacci2D(i, nbSamples); 

  s.x += getBlueNoiseThresholdTemporal(); 

  return s; 

} 

 
```
