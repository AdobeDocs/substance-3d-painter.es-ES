---
breadcrumb-title: ""
description: Acceda a la referencia del API del sombreador del Alpha Lib de Substance 3D Painter para trabajar con canales alfa y transparencia en sombreadores personalizados.
title: Alpha Lib - API del sombreador
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '72'
ht-degree: 0%
---

# Alpha Lib - API del sombreador

## lib-alpha.glsl

**Funciones públicas:** *alphaKill*

```
import lib-sampler.glsl 

import lib-random.glsl
```


Mapa de opacidad, proporcionado por el motor.

```
//: param auto channel_opacity 

uniform SamplerSparse opacity_tex;
```


umbral de prueba del Alpha.

```
//: param custom { 

//:   "default": 0.33, 

//:   "label": "Alpha threshold", 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float alpha_threshold;
```


Alpha prueba tramado.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Alpha dithering", 

//:   "group": "Common Parameters" 

//: } 

uniform bool alpha_dither;
```


Emular prueba alfa : descarte el fragmento actual si su opacidad está por debajo de un umbral definido por el usuario. Se debe llamar DESPUÉS de las llamadas de muestreo de textura: puede romper los derivados

```
void alphaKill(float alpha) 

{ 

  float threshold = alpha_dither ? getBlueNoiseThresholdTemporal() : alpha_threshold; 

  if (alpha < threshold) discard; 

} 

 

void alphaKill(SparseCoord coord) 

{ 

  alphaKill(getOpacity(opacity_tex, coord)); 

} 

 
```
