---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/workflow-issues/shelf-issues/thumbnails-in-the-shelf-look-incorrect.html"
breadcrumb-title: ''
description: Aprenda a corregir la visualización incorrecta de miniaturas en la estantería de Substance 3D Painter para garantizar vistas previas precisas de los recursos.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Shelf Issues > Thumbnails in the shelf look incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Las miniaturas del estante tienen un aspecto incorrecto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# Las miniaturas del estante tienen un aspecto incorrecto

Si las miniaturas de la estantería parecen ser diferentes de lo habitual, puede deberse al sombreador utilizado para procesar las previsualizaciones.

| Miniaturas rotas | Miniaturas normales |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-broken-preview.png"/></div> | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-normal-preview.png" width="300px"/></div> |

## 1 - Abra la ventana de configuración principal

Ve a **Editar** y haz clic en **Configuración** :

![](../../../assets/pref-menu.png)

## 2 - Retire el sombreador de vista previa de la plataforma

En la vista **General**, desplácese hacia abajo hasta que esté visible la sección &quot;Opciones de vista previa&quot;.\
Haga clic en el botón **cross** situado delante del &quot;**Sombreador de previsualización de material**&quot; para quitar el sombreador especificado actualmente.

![](../../../assets/remove-preview-shader.png){width="450px"}

## 3 - Reinicie Substance 3D Painter

Para regenerar las miniaturas de modo que tengan el aspecto correcto, Substance 3D Painter debe reiniciarse.
