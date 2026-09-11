---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/tools-issues/normal-map-looks-incorrect-when-loaded-in-layer-or-tool-properties.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo solucionar problemas de visualización de mapa de normales en las propiedades de capa y herramienta de Substance 3D Painter para obtener detalles precisos de la superficie.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Normal map looks incorrect when loaded in layer or tool properties
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: El mapa de normales parece incorrecto cuando se carga en las propiedades de capa o herramienta
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%

---


# El mapa de normales parece incorrecto cuando se carga en las propiedades de capa o herramienta

Al cargar una capa normal en la herramienta actual de la capa de relleno, esta puede parecer incorrecta si se trata de un mapa de normales de OpenGL.\
La razón es bastante simple : el motor de Substance 3D Painter supone que los mapas de normales cargados son DirectXs de forma predeterminada.

Este comportamiento se puede editar fácilmente haciendo clic en la pequeña flecha junto al material de substance o el canal dedicado:

![](../../../assets/channel-format-override.png)
