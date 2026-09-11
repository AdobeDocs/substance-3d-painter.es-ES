---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/eraser.html"
breadcrumb-title: ''
description: Usa la herramienta Borrador de Substance 3D Painter para eliminar la pintura y las texturas de tus modelos en 3D con un control de precisión.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Eraser
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Borrador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 1%

---


# Borrador

El Borrador es una herramienta de pintura que borra/oculta lo que han pintado anteriormente otras herramientas. Esta herramienta solo afecta a una capa cada vez.

El Borrador comparte parámetros y comportamientos comunes con la herramienta Pintura. Para obtener más información sobre el pincel, los controles alfa y de galería de símbolos echan un vistazo a la [página de la herramienta Pintura](paint-brush.md).

>[!NOTE]
>
> Técnicamente, **el borrador no quita realmente la información**. Solo tiene que devolver a cero la capa alfa, que borrará u ocultará la información de pintura anterior. Esto significa:
> 
> * Cualquier trazo de pincel anterior que se haya pintado se sigue calculando cuando se vuelve a abrir un proyecto antes de que se apliquen los trazos de pincel con el borrador.
> * Un Substance puede recuperar la información de pintura si ignora la información alfa
> 
> Por esta razón, a veces es más recomendable **eliminar una capa y volver a crearla** en lugar de usar el borrador, ya que puede mejorar el rendimiento.

## Material

Al borrar información, es posible que solo afecte a canales específicos.

>[!NOTE]
>
> A diferencia de la herramienta de Pintura, el Borrador solo permite definir qué canales se verán afectados. No es posible cargar un recurso desde la bandeja para que afecte a cada canal.

* Si todos los canales están activados, el borrador eliminará la información dentro de todos los canales:

  ![](../../assets/eraser-all-channels-selection.png)

  ![](../../assets/erase-all-channel-optim.gif){width="325px"}
* Si se seleccionan canales específicos, el borrador eliminará información solo de esos canales:

  ![](../../assets/eraser-one-channel-selection.png)

  ![](../../assets/erase-one-channel-optim.gif){width="325px"}
