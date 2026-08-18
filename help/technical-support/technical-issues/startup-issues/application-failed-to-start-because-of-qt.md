---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/startup-issues/application-failed-to-start-because-of-qt.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo solucionar los errores de inicio de Substance 3D Painter causados por problemas del framework Qt para iniciar la aplicación correctamente.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Application failed to start because of Qt
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La aplicación no se pudo iniciar debido a Qt
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---


# La aplicación no se pudo iniciar debido a Qt

Al iniciar la aplicación, puede aparecer el siguiente mensaje de error:

&#x200B;>> 

Esta aplicación no se pudo iniciar porque no se pudo inicializar ningún complemento de la plataforma Qt. Si reinstala la aplicación, es posible que se solucione el problema.

Los complementos de plataformas disponibles son: minimal, off screen, webgl, windows.

Este error se puede producir porque otra variable de entorno definida por software entra en conflicto con la aplicación.

Asegúrese de eliminar las siguientes variables del entorno actual antes de iniciar la aplicación:

```
QT_PLUGIN_PATH 

QML2_IMPORT_PATH
```


>[!NOTE]
>
> Estas variables también se pueden heredar de un contexto de Python, por ejemplo con **pyinstaller**. Asegúrese de quitarlas del contexto en el que se inicia la aplicación.
