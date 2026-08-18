---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/interface/viewport/2d-view.html"
breadcrumb-title: ''
description: Aprenda a utilizar la vista 2D en Substance 3D Painter para ver y editar texturas en el espacio UV para pintar texturas con precisión.
helpx_creative_field: ""
helpx_description: Painter > Interface > Viewport > 2D view
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Vista 2D
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Vista 2D

![](../../assets/2d-view.jpg){width="450px"}

La vista 2D muestra las Islas de UV de malla del [conjunto de texturas](../texture-set/texture-set.md) seleccionado actualmente. Permite ver las texturas de la pila de capas, pero también pintar en las Islas de UV de malla.

## Modo de visualización

![](../../assets/display-mode-1.png)

En la parte superior derecha de la ventana gráfica se encuentra el menú desplegable del modo de visualización. Este control permite cambiar la información que debe estar visible en la ventana gráfica. Permite mostrar canales individuales, mapas de malla o el resultado final del material con iluminación.

## Información del eje

![](../../assets/2d-axis.png)

En la parte inferior derecha de la ventana gráfica se encuentra **Axis Information**, que indica la dirección de los ejes bidimensionales. En el caso de la vista 2D los ejes son U y V.

## Información del azulejo UV

![](../../assets/2d-view-button.png)

Junto al **Modo de visualización** se encuentra el botón **Información de mosaico UV**, que permite mostrar u ocultar información relacionada con los mosaicos UV. Este botón no está visible en los proyectos normales.

## Flujo de trabajo del proyecto

En función del flujo de trabajo definido al crear un proyecto, la vista 2D puede tener un aspecto y un comportamiento diferentes:

| *Flujo de trabajo del proyecto* | *Comportamientos* |
| --- | --- |
| **Proyecto normal** | Con un proyecto normal, solo se puede pintar el UV con el rango UV [0-1]. Cualquier cosa fuera de este rango será visible, pero no será interactiva.En este ejemplo, solo se pueden pintar las Islas de UV de la izquierda (con el fondo gris claro detrás). <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-regular.jpg" width="500px"/></div> |
| **Proyecto de mosaico UV** | Con el proyecto de azulejo UV, cada gama UV es un nuevo conjunto de texturas, que se puede pintar en. La vista 2D también muestra una cuadrícula para ver mejor cómo está organizado cada mosaico. Cada mosaico tendrá asignado un número UDIM. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-uvtiles.jpg" width="500px"/></div> |
