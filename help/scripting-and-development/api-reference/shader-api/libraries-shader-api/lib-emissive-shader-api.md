---
breadcrumb-title: ""
description: Acceda a la referencia de API del sombreador de Emisivos Lib de Substance 3D Painter para crear materiales de emisivo y efectos brillantes.
title: Emisivos Lib - API del sombreador
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%
---

# Emisivos Lib - API del sombreador

## lib-emisivo.glsl

**Funciones públicas:** *pbrComputeEmissive*

Importar desde biblioteca

```
import lib-sparse.glsl
```


La textura del canal de emisivo.

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


Valor utilizado para ajustar la intensidad del emisivo.

```
//: param custom { 

//:   "default": 1.0, 

//:   "label": "Emissive Intensity", 

//:   "min": 0.0, 

//:   "max": 100.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float emissive_intensity;
```


Calcula el brillo del emisivo al ojo del espectador

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
