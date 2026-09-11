---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/content/creating-custom-effects/generic-filter.html"
breadcrumb-title: ''
description: Aprenda a crear efectos de filtro genéricos para que Substance 3D Painter aplique filtros de textura y procesamiento de imágenes personalizados.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Generic filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Filtro genérico
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---


# Filtro genérico

Se aplicará un efecto genérico en todos los canales del documento, incluida la opacidad. Un filtro genérico puede ser:

* **escala de grises**, se aplicará a cada componente (R, G, B y A) de cada canal (color base, metálico, rugosidad, etc.)
* **color**, se aplicará en el canal en color tal cual o se convertirá internamente a escala de grises para afectar a los canales en escala de grises

El nodo de entrada del efecto debe tener **identificador** o **uso** definido **entrada** y su nodo de salida debe tener **salida**. Tenga en cuenta que los filtros basados en **color** no se pueden usar en la máscara de una capa, solo los filtros de **escala de grises** serán compatibles.

>[!NOTE]
>
> Es posible usar **usage** o **identificador** en un nodo de entrada (el uso tiene la prioridad).

Ejemplo :

![](../../assets/generic-filter.png)![](../../assets/generic-rgba.png){width="575px"}
