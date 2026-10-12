---
breadcrumb-title: ""
description: Obtenga información sobre cómo solucionar problemas de reconocimiento de GPU en Substance 3D Painter para habilitar el rendimiento y la aceleración de hardware adecuados.
title: La GPU no se reconoce
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%
---

# La GPU no se reconoce

![](../../../assets/not-recognized-gpu.png){width="500px"}

Algunos usuarios de **NVIDIA Optimus** pueden tener problemas para hacer que Substance 3D Painter se ejecute en la GPU correcta. Una solución alternativa es establecer las siguientes claves en el Registro de Windows en 0:

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
