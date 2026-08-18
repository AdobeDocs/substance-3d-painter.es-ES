---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-is-not-recognized-and-is-mentionned-as-gdi-generic.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo solucionar problemas de reconocimiento de GPU que se muestran como GDI genérico en Substance 3D Painter para una aceleración de GPU adecuada.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU is not recognized and is mentionned as GDI Generic
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La GPU no se reconoce y se menciona como GDI Generic
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---


# La GPU no se reconoce y se menciona como GDI Generic

Este problema es un poco complicado de seguir y puede deberse a varias fuentes:

* Si utiliza un equipo con NVIDIA Optimus, consulte el siguiente vínculo: [No se reconoce la GPU](gpu-is-not-recognized.md)
* Compruebe que el monitor esté conectado a la GPU principal (y que en Windows este monitor esté configurado como pantalla principal)
* Compruebe que la profundidad de bits de color de la pantalla principal esté establecida en 32 bits en Windows
* Si el problema persiste, intente volver a instalar de forma limpia los controladores de la GPU (desinstalación completa con limpieza de los restos en el registro de Windows).
