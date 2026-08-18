---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/clone-tool.html"
breadcrumb-title: ''
description: Utilice la herramienta Clonar de Substance 3D Painter para copiar detalles de textura de un área a otra y pintar la textura sin problemas.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Clone Tool
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Herramienta Clonar
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%

---


# Herramienta Clonar

Introducida en Substance 3D Painter 2, la herramienta Clonar comparte el mismo tipo de parámetros que la [herramienta de pintura](https://support.allegorithmic.com/documentation/display/SPDOC/Paint+brush) . Como su nombre indica, la herramienta Clonar le permite duplicar el contenido de una capa específica o la pila de capas completa de un punto a otro.

![](../../assets/clone-01.gif)

## Uso

La forma más sencilla de utilizar la herramienta Clonar es utilizarla en el contenido de una capa de pintura.

Esto se puede hacer en 2 pasos:

* Seleccione la ubicación de origen colocando el mouse en el modelo y presionando la tecla &quot;**V**&quot;.
* A continuación, coloque el ratón donde aparecerá el área duplicada y comience a pintar.

Es posible actualizar el origen en cualquier momento presionando &quot;**V**&quot; de nuevo.

![](../../assets/2018-06-12-18-11-59.png)

De forma predeterminada, al pintar con la herramienta Clonar, la ubicación de origen se actualiza cuando se libera el pincel. Al deshabilitar el botón utilizado para el &quot;**comportamiento de origen de clonación**&quot;, el origen volverá a su estado definido al pulsar &quot;**V**&quot;. Esto puede resultar útil al pintar varias veces con la misma área de origen.

Una forma más inteligente de usar la herramienta Clonar es crear una capa de pintura y configurar el modo de fusión de todos los canales como &quot;Pass through&quot;. Esto permitirá duplicar cualquier información de una manera no destructiva de todas las capas ubicadas debajo de la &quot;Capa de clonación&quot;. Las capas siguientes permanecen intactas y la capa Clonar tendrá en cuenta las modificaciones que se apliquen posteriormente:

![](../../assets/clone-02.gif)
