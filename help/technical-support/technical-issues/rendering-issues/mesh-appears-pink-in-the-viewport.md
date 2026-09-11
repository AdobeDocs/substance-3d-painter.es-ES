---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-appears-pink-in-the-viewport.html"
breadcrumb-title: ''
description: Aprenda a corregir el aspecto de la malla rosa en la ventana gráfica de Substance 3D Painter para restaurar la representación de material adecuada.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh appears pink in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La malla aparece de color rosa en la ventana gráfica
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---


# La malla aparece de color rosa en la ventana gráfica

![](../../../assets/pink-mesh.jpg){width="400px"}

La malla puede aparecer **rosada** dentro del área de visualización porque el **sombreador** que se usó para dibujarla **ya no se compila** (como se indica en la **ventana de registro** ). Esto puede deberse a que el sombreador no es compatible con la última versión de la API del sombreador.

A continuación se indica cómo solucionarlo:

* Para **sombreadores predeterminados**: Siga el procedimiento paso a paso de la página [Actualizando un sombreado](../../../interface/shader-settings/updating-a-shader.md).
* Para **sombreador personalizado**: consulta el mensaje de error en la ventana de registro, así como la página [API del sombreador](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).
