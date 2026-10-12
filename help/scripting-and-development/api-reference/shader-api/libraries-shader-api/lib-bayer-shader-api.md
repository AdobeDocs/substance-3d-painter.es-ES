---
breadcrumb-title: ""
description: Acceda a la referencia de API del sombreador de Lib Bayer para Substance 3D Painter para crear patrones de tramado de Bayer en sombreadores personalizados.
title: Lib Bayer - API del sombreador
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '32'
ht-degree: 0%
---

# Lib Bayer - API del sombreador

## lib-bayer.glsl

**Funciones públicas:** *bayerMatrix8*

```
float bayerMatrix8(uvec2 coords) { 

  return (float(bayer(coords.x, coords.y)) + 0.5) / 64.0; 

} 

 
```
