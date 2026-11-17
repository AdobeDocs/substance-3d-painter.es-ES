---
breadcrumb-title: ""
description: Aprenda a utilizar entradas basadas en malla en efectos personalizados para Substance 3D Painter para crear efectos de textura que tengan en cuenta la geometría.
title: Entrada basada en malla
user-guide-description: ""
user-guide-title: ""
source-git-commit: 4432887b652896f77fc3c99010436ef44aeb8a3e
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 1%
---

# Entrada basada en malla

La entrada basada en malla es la textura que proporciona el motor de Substance 3D Painter extraída de la malla dentro del proyecto actual. Estas texturas se pueden utilizar para crear efectos avanzados basados en la topología de malla.

>[!NOTE]
>
> Esta información de malla se basa en la propia topología y no tiene en cuenta el mapa de malla (texturas hechas un bake).
> 
> La entrada proporcionada por el motor es una textura de punto flotante de 32 bits que se reducirá o se fijará al valor de la entrada en el gráfico del Substance.

| Información de malla | Identificador | Uso | Descripción |
| --- | --- | --- | --- |
| *Posición (RGB)* | **mesh\_position** | **meshPosition** | Recupere una textura que contenga la posición del vértice. |
| *Espacio normal mundial (RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | Recupere una textura que contenga el vértice normal en el espacio de entorno. |
| *Tangente espacial mundial (RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | Recupere una textura que contenga la tangente del vértice en el espacio de entorno. |
| *Bitangent espacial mundial (RGB)* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | Recupere una textura que contenga el vértice bi-tangente (bi-normal) en el espacio de entorno. |
| *Tamaño de texto (escala de grises)* | **mesh\_texel\_size** | **meshTexelSize** | Recupere una textura que contenga el tamaño del texel (diferencia entre la densidad de píxeles y la malla UV). |
| *Máscara UV (escala de grises)* | **mesh\_uv\_mask** | **meshUVMask** | Recupere una textura como máscara negra (exterior) y blanca (interior) de las Islas de UV de malla. |
| *Vecino UV (RGB)* | **mesh\_uv\_vecino** | **meshUVNeighbor** | Recupere una textura con dos datos. El interior de las Islas de UV almacena coordenadas UV regulares. El exterior de las Islas de UV almacena las coordenadas UV del píxel del otro lado de las costuras UV. Esta textura se puede utilizar para crear efectos perfectos. |
