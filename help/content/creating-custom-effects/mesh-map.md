---
breadcrumb-title: ""
description: Aprenda a utilizar los mapas de malla en efectos personalizados para que Substance 3D Painter acceda a la información de textura basada en la geometría.
title: Mapa de malla
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 3%
---

# Mapa de malla

Para conectar automáticamente mapas de malla (texturas hechas un bake) cuando se agrega un efecto en una capa, se debe seguir una convención de nomenclatura específica.

>[!NOTE]
>
> Es posible usar **usage** o **identificador** en un nodo de entrada (el uso tiene la prioridad).

Esta es la convención de nomenclatura para cada mapa de malla:

| Mapa de malla | Uso | Identificador |
| --- | --- | --- |
| *Oclusión ambiental* | **ambientOcclusionBase** | **ambiente\_oclusión** |
| *ID* | **id** | **id** |
| *Curvatura* | **curvatura** | **curvatura** |
| *Normal* | **normalBase** | **normal\_base** |
| *Normales espaciales mundiales* | **normalWS** | **mundo\_espacio\_normales** |
| *Posición* | **posición** | **posición** |
| *Thickness* | **thickness** | **thickness** |
| *Height* | **heightBase** | **height\_base** |
| *Normales dobladas* | **bentNormalsBase** | **bent\_normals\_base** |
| *Opacidad* | **opacityBase** | **opacidad\_base** |
