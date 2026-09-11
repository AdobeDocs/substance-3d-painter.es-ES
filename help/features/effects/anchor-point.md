---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/effects/anchor-point.html"
breadcrumb-title: ''
description: Aprenda a utilizar los efectos de punto de anclaje en Substance 3D Painter para hacer referencia a texturas de otras capas para una composición avanzada.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Anchor Point
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Punto de anclaje
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# Punto de anclaje

Un punto de ancla es una forma de exponer cualquier recurso o elemento de la pila de capas y hacer referencia a él en diferentes áreas de la pila de capas para diferentes propósitos y con un conjunto diferente de ajustes. Te abren todo un nuevo conjunto de posibilidades, te permiten enlazar de forma eficaz capas o máscaras y hacer que un solo punto de ancla afecte a varios aspectos de tu proyecto, lo que transforma a Substance 3D Painter en una experiencia verdaderamente no lineal.

>[!NOTE]
>
> Solo se puede hacer referencia a un punto de ancla dentro de la misma textura que se ha creado. La creación de vínculos entre un anclaje y sus referencias no es posible en los conjuntos de texturas.

## Adición de un punto de ancla

Punto de anclaje está disponible en el menú Efectos. Se pueden añadir en capas y máscaras.

![](../../assets/add-anchor-point.png)

## Uso de un punto de ancla como referencia

Otra capa puede hacer referencia a un punto de ancla: esto creará una instancia del contenido del punto de ancla en la capa que hace referencia a él.

Los puntos de ancla se pueden utilizar como referencia en los siguientes recursos:

* Capa de relleno
* Efecto de relleno
* Entrada de un filtro de substancia (Efecto, Procedimiento, Generador)

![](../../assets/anchor-point-resource.png)

Solo se pueden usar como referencias los puntos de ancla que estén **debajo** de la capa que hace referencia a ella.\
Si mueve un punto de ancla por encima de una capa que haga referencia a él, se romperá la referencia. Puede deshacer esta acción si desea cancelarla.

![](../../assets/layer-broken.png)![](../../assets/reference-broken.png)

## Búsqueda de referencias para un punto de ancla

Al hacer clic en un punto de ancla, puede ver en las propiedades la lista de capas en las que este punto de ancla se utiliza como referencia.

![](../../assets/references.png)

## Buscar un punto de ancla

Cuando utilice una capa/efecto de relleno con un punto de ancla como referencia, puede saltar al punto de ancla.

![](../../assets/jump-to-anchor-point.png)
