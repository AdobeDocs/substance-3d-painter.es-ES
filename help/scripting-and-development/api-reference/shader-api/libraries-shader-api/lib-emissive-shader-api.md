---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-emissive-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador Emisora de labios de Substance 3D Painter para crear materiales emisores y efectos brillantes.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Emissive - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Emisor Lib - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%

---


# Emisor Lib - API del sombreador

## lib-emissive.glsl

**Funciones públicas:** *pbrComputeEmissive*

Importar desde biblioteca

```
import lib-sparse.glsl
```


La textura del canal de emisión.

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


Valor utilizado para ajustar la intensidad de las emisiones.

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


Calcula el brillo emisor al ojo del espectador

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
