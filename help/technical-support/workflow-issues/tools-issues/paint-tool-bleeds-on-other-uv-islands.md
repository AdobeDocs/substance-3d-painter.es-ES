---
breadcrumb-title: ""
description: Aprenda a corregir el sangrado de la herramienta de pintura a través de las Islas de UV en Substance 3D Painter para mantener los límites de textura limpios.
title: La herramienta pintura se desvanece en otras Islas de UV
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '126'
ht-degree: 0%
---

# La herramienta pintura se desvanece en otras Islas de UV

Algunos comportamientos predeterminados de la [herramienta de Pintura](../../../features/effects/paint.md) pueden parecer contradictorios en algunas situaciones específicas. Substance 3D Painter es una aplicación que funciona principalmente en el espacio 3D, esto se aplica a la pintura también. La configuración predeterminada del pincel de pintura es intentar pintar sin interrupciones en todas las UV. Por esta razón, al interactuar con el Vista 2D, algunos resultados pueden parecer inesperados.

Para evitar el sangrado en otras Islas de UV al pintar en la Vista 2D, simplemente cambie el valor **Alignment** en los parámetros de la herramienta:

| *Modo de alineación* | *Vista previa* |
| --- | --- |
| **Ajuste de tangente** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-tangent-optim.gif"/></div> |
| **UV** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-uv.gif" width="450px"/></div> |
