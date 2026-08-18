---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/viewport-issues/mesh-faces-disappear-when-looking-at-them-from-behind.html"
breadcrumb-title: ''
description: Obtenga más información sobre cómo corregir la desaparición de caras de malla cuando se visualizan desde detrás en la ventana gráfica de Substance 3D Painter para obtener una visibilidad de malla adecuada.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Mesh faces disappear when looking at them from behind
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Las caras de malla desaparecen al mirarlas desde atrás
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%

---


# Las caras de malla desaparecen al mirarlas desde atrás

De forma predeterminada, las mallas de la ventana gráfica pueden no mostrar la parte posterior de los polígonos de malla (cara posterior). Esto se debe a que el sombreador actual los selecciona.

Para mostrar la parte posterior de las caras, simplemente cambie el sombreador actual a **pbr-metal-rough-alpha-test** en la [configuración del sombreador](../../../interface/shader-settings/shader-settings.md).
