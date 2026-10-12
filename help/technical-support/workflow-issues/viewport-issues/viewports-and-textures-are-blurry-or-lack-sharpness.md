---
breadcrumb-title: ""
description: Aprenda a corregir puntos de visión y texturas borrosos en Substance 3D Painter para garantizar una calidad visual nítida y clara.
title: Las ventanas gráficas y las texturas son borrosas o carecen de nitidez
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
