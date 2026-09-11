---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-is-not-recognized.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo solucionar problemas de reconocimiento de GPU en Substance 3D Painter para habilitar el rendimiento y la aceleración de hardware adecuados.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU is not recognized
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La GPU no se reconoce
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%

---


# La GPU no se reconoce

![](../../../assets/not-recognized-gpu.png){width="500px"}

Algunos usuarios de **NVIDIA Optimus** pueden tener problemas para hacer que Substance 3D Painter se ejecute en la GPU correcta. Una solución alternativa es establecer las siguientes claves en el Registro de Windows en 0:

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
