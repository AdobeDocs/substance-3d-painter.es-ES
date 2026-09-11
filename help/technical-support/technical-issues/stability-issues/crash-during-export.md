---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-during-export.html"
breadcrumb-title: ''
description: Aprenda a corregir bloqueos de Substance 3D Painter durante las operaciones de exportación para obtener flujos de trabajo de exportación de textura fiables.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash during export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bloqueo durante la exportación
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---


# Bloqueo durante la exportación

Algunos casos específicos pueden hacer que Substance 3D Painter se bloquee durante la exportación, especialmente con una resolución muy alta (como 4K u 8K). A continuación se muestra una lista de las fuentes más comunes de este problema.

## TDR (Detección y recuperación de tiempo de espera)

La detección y recuperación de tiempo de espera (TDR) es un mecanismo de seguridad de Microsoft Windows que evita que una GPU bloquee el sistema con un cálculo interminable. Lamentablemente, este mecanismo es demasiado restrictivo para Substance 3D Painter de forma predeterminada.

Para obtener más información, consulte: [bloqueo de controladores de GPU con cálculos largos (bloqueo TDR)](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html).

## Poca memoria virtual

La exportación puede consumir una gran cantidad de RAM (memoria del equipo), en cuyo caso el sistema intentará recuperar la memoria virtual si el sistema se queda sin RAM. La memoria virtual suele ser memoria adicional almacenada en unidades de disco duro. Si el tamaño de la memoria virtual es demasiado pequeño, Substance 3D Painter generará un bloqueo porque se quedó sin memoria total.

Para obtener más información, consulte: [Bloqueo con poca memoria virtual](crash-with-low-virtual-memory.md).

## Falta de espacio en disco

Desde la introducción de Sparse Virtual Textures (SVT), Substance 3D Painter puede transmitir en el disco parte de la memoria caché para equilibrar el rendimiento. Si no hay suficiente espacio libre en el disco, puede que se produzca un bloqueo porque la aplicación no pudo transferir y escribir en él.

La ubicación de la caché se puede mover desde la carpeta predeterminada de archivos temporales del sistema. Para obtener más información, consulte: [Texturas virtuales dispersas](../../../features/sparse-virtual-textures.md).

## Frecuencia de GPU sobreacelerada

Las GPU sobreaceleradas a menudo pueden ser más inestables porque se ejecutan en frecuencias no diseñadas inicialmente por el constructor de la GPU. Es posible que ayude a desactivar la sobreaceleración durante un tiempo.

Para obtener más información, consulte: [Bloqueo al trabajar con GPU sobreacelerada](../gpu-issues/crash-when-working-with-overclocked-gpu.md).
