---
breadcrumb-title: ""
description: Aprenda a corregir el parpadeo de la malla a blanco al mover la cámara en la ventana gráfica de Substance 3D Painter para un procesamiento estable.
title: Parpadeo de malla en blanco al mover la cámara
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%
---

# Parpadeo de malla en blanco al mover la cámara

![](../../../assets/white-flash-svt-optim.gif){width="300px"}

Con los proyectos antiguos que se mueven por la cámara en la ventana gráfica, es posible que se muestren brevemente destellos blancos creados por texturas blancas o vacías. Esto se debe a que el sistema [Texturas virtuales dispersas](https://substance3d.adobe.com/display/DRAFTPAINTER/Sparse+Virtual+Textures) (SVT) se basa en configuraciones de sombreador específicas que los sombreadores más antiguos no utilizan.

Para deshacerte del flash blanco, simplemente **actualiza** el **sombreador del proyecto**:

* Para **sombreadores predeterminados**: Siga el procedimiento paso a paso de la página [Actualizando un sombreador](../../../interface/shader-settings/updating-a-shader.md).
* Para **sombreadores personalizados**: echa un vistazo a los mensajes de error del registro, así como a la página [API del sombreador](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).
