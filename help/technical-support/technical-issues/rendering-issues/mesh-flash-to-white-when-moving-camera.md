---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.html"
breadcrumb-title: ''
description: Aprenda a corregir el parpadeo de la malla a blanco al mover la cámara en la ventana gráfica de Substance 3D Painter para un procesamiento estable.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh flash to white when moving camera
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parpadeo de malla en blanco al mover la cámara
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Parpadeo de malla en blanco al mover la cámara

![](../../../assets/white-flash-svt-optim.gif){width="300px"}

Con los proyectos antiguos que se mueven por la cámara en la ventana gráfica, es posible que se muestren brevemente destellos blancos creados por texturas blancas o vacías. Esto se debe a que el sistema [Texturas virtuales dispersas](https://substance3d.adobe.com/display/DRAFTPAINTER/Sparse+Virtual+Textures) (SVT) se basa en configuraciones de sombreador específicas que los sombreadores más antiguos no utilizan.

Para deshacerse del flash blanco, simplemente **actualiza** el **sombreador del proyecto**:

* Para **sombreadores predeterminados**: Siga el procedimiento paso a paso de la página [Actualizando un sombreado](../../../interface/shader-settings/updating-a-shader.md).
* Para **sombreadores personalizados**: echa un vistazo a los mensajes de error del registro, así como a la página [API del sombreador](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).
