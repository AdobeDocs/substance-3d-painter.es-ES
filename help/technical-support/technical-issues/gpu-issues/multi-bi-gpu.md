---
breadcrumb-title: ""
description: Aprenda a configurar Substance 3D Painter para sistemas con varias GPU y dos GPU con el fin de optimizar el rendimiento de procesamiento.
title: MultiBi-GPU
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
