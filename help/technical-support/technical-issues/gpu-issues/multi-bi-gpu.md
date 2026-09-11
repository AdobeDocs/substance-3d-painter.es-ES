---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/multi-bi-gpu.html"
breadcrumb-title: ''
description: Aprenda a configurar Substance 3D Painter para sistemas con varias GPU y dos GPU con el fin de optimizar el rendimiento de procesamiento.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > MultiBi-GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MultiBi-GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

---


# Multi/Bi-GPU

Algunas configuraciones de GPU y/o modelos de GPU no son compatibles con Substance 3D Painter y darán lugar a inestabilidad y bloqueos. A continuación se muestra una lista de las configuraciones no compatibles :

| ***Configuración*** | ***Solución*** |
| --- | --- |
| **Nvidia SLI / AMD Crossfire** (puentes de tarjetas gráficas) | Deshabilite SLI o Crossfire en la configuración del controlador de la GPU. |
| **Bi-GPU** (dos chipsets GPU en una tarjeta gráfica) | Deshabilite el uso de los dos chipsets GPU en la configuración de controladores para solo uno. |
