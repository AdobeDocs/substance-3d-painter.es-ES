---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.html"
breadcrumb-title: ''
description: Obtenga más información sobre los requisitos de compatibilidad de controladores de GPU para Substance 3D Painter para garantizar un procesamiento y rendimiento estables.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU drivers compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Compatibilidad de controladores de GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 2%

---


# Compatibilidad de controladores de GPU

Esta página reagrupa información sobre los controladores de la GPU que pueden provocar problemas con Substance 3D Painter.

## Nvidia

En la siguiente tabla, se enumeran todas las versiones de controlador que producen problemas para la GPU Nvidia (modelos GeForce o Quadro):

| *Versión del controlador* | *Descripción del problema* |
| --- | --- |
| <b> 425.xx </b> | Artefactos de trazado de rayos de GPU. |
| <b> 429.xx o anterior </b> | Artefactos de bloque de textura negra. |
| <b> 435.xx o anterior </b> | Problemas de color sRGB al calcular texturas. |
| <b> 439.xx </b> | Texturas corruptas. |
| <b> 441.08 </b> | Problemas de bloqueo o estabilidad. |
| <b> 442.19 </b> | Problemas de bloqueo o estabilidad. |
| <b>528.09</b> | Bloqueo del sistema operativo. |
| <b>572.16 a 572.42</b> | Se producen defectos o se bloquean al hornear texturas. |

### AMD

| *Versión del controlador* | *Descripción del problema* |
| --- | --- |
| **20.7.x** a **20.11.2** | Las texturas fallan o se dañan. |
| **20.11.3** a **21.2.1** | Problemas de texturas, daños y problemas de bloqueo o estabilidad. |
| **21.2.3** a **21.6.1** | Problemas de bloqueo o estabilidad. |
