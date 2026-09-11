---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/mesh-based-input.html"
breadcrumb-title: ''
description: Aprenda a utilizar entradas basadas en malla en efectos personalizados para Substance 3D Painter para crear efectos de textura que tengan en cuenta la geometría.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Based Input
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Entrada basada en malla
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---


# Entrada basada en malla

La entrada basada en malla es la textura que proporciona el motor de Substance 3D Painter extraída de la malla dentro del proyecto actual. Estas texturas se pueden utilizar para crear efectos avanzados basados en la topología de malla.

>[!NOTE]
>
> Esta información de malla se basa en la topología en sí y no tiene en cuenta el mapa de malla (texturas horneadas).
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
