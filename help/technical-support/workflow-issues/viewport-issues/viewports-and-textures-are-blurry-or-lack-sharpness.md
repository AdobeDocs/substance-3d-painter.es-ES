---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/workflow-issues/viewport-issues/viewports-and-textures-are-blurry-or-lack-sharpness.html"
breadcrumb-title: ''
description: Aprenda a corregir puntos de visión y texturas borrosos en Substance 3D Painter para garantizar una calidad visual nítida y clara.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Viewports and textures are blurry or lack sharpness
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Las ventanas gráficas y las texturas son borrosas o carecen de nitidez
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%

---


# Las ventanas gráficas y las texturas son borrosas o carecen de nitidez

Las ventanas gráficas pueden aparecer borrosas por diferentes razones.

## Configuración de pantallas de alta resolución de PPP (Retina)

De forma predeterminada, Substance 3D Painter reduce la resolución de la ventana gráfica en la pantalla alta PPP/Retina para mejorar el rendimiento.

Este comportamiento se puede cambiar en la [configuración principal](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/general-71008262.html) cambiando el parámetro **Escalado de ventana gráfica**.

## Filtrado de textura

Las ventanas gráficas usan mipmaps y filtrado de texturas para poder transmitir por streaming [Texturas virtuales dispersas](../../../features/sparse-virtual-textures.md) y mejorar el rendimiento. Esto puede dar lugar a texturas borrosas en algunos casos.

El filtrado de texturas se puede ajustar a través de la ventana Configuración de visualización en los parámetros [Configuración de la ventana gráfica](../../../interface/display-settings/viewport-settings.md).
