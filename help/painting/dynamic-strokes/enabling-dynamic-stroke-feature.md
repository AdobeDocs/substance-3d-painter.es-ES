---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/painting/dynamic-strokes/enabling-dynamic-stroke-feature.html"
breadcrumb-title: ''
description: Aprenda a habilitar la función de trazo dinámico en Substance 3D Painter para crear trazos de pincel flexibles con efectos variables.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Enabling Dynamic Stroke Feature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Activación de la función Trazo dinámico
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 2%

---


# Activación de la función Trazo dinámico

Para habilitar la función Trazos dinámicos, primero se necesita un recurso específico.

## Buscar recursos compatibles con Trazos dinámicos

Al examinar la ventana [Assets](../../interface/assets/assets.md), aparece un icono dedicado en la parte inferior derecha de una miniatura que indica el tipo de compatibilidad del recurso. Si no hay ningún icono visible, significa que el recurso no puede aprovechar la función.

| *Icono* | *Descripción* |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-dyn.png"/></div> | Este recurso puede utilizar uno o varios de los comportamientos siguientes:<ul data-preserve-html="true"><li data-preserve-html="true">Índice de sellos</li><li data-preserve-html="true">Tiempo</li><li data-preserve-html="true">Grano aleatorio</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-random.png"/></div> | Este recurso sólo expone el parámetro Raíz aleatoria. |

También es posible buscar recursos utilizando el campo de búsqueda en la estantería con las siguientes palabras clave :

* brazada dinámica
* semilla al azar

## Parámetros de trazos dinámicos

![](../../assets/dynamic-strokes-settings.png)

Cuando se ha cargado un recurso de trazo dinámico, se agrega una nueva lista de parámetros justo antes del grupo de parámetros Substance.

| *Parámetro* | *Descripción* |
| --- | --- |
| **Controles dinámicos** | Enumere los parámetros disponibles con el archivo de Substance que se utiliza actualmente. |
| **Inicio de sello** | Sólo está disponible si el recurso tiene el control dinámico &quot;Stamp Index&quot;. Indica a partir de qué valor debe comenzar el índice de los sellos dentro del trazo del pincel:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Desde el principio (0)</strong>: Predeterminado. El índice comienza desde cero en cada trazo nuevo.</li> <li data-preserve-html="true"><strong>Del índice aleatorio</strong>: El índice comienza con un valor aleatorio (con su máximo definido por el recuento cíclico de sello). Tenga en cuenta que los siguientes valores seguirán siendo secuenciales y no completamente aleatorios.</li> </ul> |
| **Recuento de ciclos de sello** | Sólo está disponible si el recurso tiene el control dinámico &quot;Stamp Index&quot;. Estos parámetros controlan cuándo Substance 3D Painter debe dejar de generar nuevas variaciones de Substance y empezar a reciclar las existentes. Este parámetro tiene un gran impacto en el rendimiento, por lo que puede obtener más información sobre [Rendimiento de trazos dinámicos](dynamic-stroke-performances.md). |
| **Tipo de semilla aleatoria** | Sólo está disponible si el recurso tiene el control dinámico &quot;Raíz aleatoria&quot;. Controla cómo debe cambiar la Raíz aleatoria:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Único</strong>: Predeterminado. Utilice un único valor Raíz aleatoria que se puede definir manualmente mediante los parámetros del Substance.</li> <li data-preserve-html="true"><strong>Aleatorio por trazo</strong>: Genera un nuevo valor de Raíz aleatoria para cada nuevo trazo de pincel.</li> <li data-preserve-html="true"><strong>Aleatorio por sello</strong>: Genera un nuevo valor de Raíz aleatoria para cada sello dentro de un trazo de pincel. <em><strong>Tenga cuidado con el parámetro, ya que puede ser muy caro</strong>.</em></li> </ul> |
| **Hora** | El control dinámico de tiempo no tiene ningún parámetro. El tiempo depende del tiempo que dure la pintura de un trazo de pincel. |

## Lista de herramientas compatibles

Los ajustes de Trazo dinámico solo están disponibles con las siguientes herramientas y contextos :

| *Tipo de herramienta* | *Ranura de recurso compatible* |
| --- | --- |
| **Pintura** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li><li data-preserve-html="true">Material</li></ul> |
| **Borrador** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li><li data-preserve-html="true">Material</li></ul> |
| **Proyección** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li></ul> |
| **Difuminado** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li></ul> |
| **Clonar** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li></ul> |

>[!NOTE]
>
> Los trazos dinámicos no son compatibles con **Partículas** , por lo que la función se deshabilita al usar cualquier herramienta en el modo Física.
