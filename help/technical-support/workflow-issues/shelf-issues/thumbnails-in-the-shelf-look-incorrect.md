---
breadcrumb-title: ""
description: Aprenda a corregir la visualización incorrecta de miniaturas en la estantería de Substance 3D Painter para garantizar vistas previas precisas de los recursos.
title: Las miniaturas del estante tienen un aspecto incorrecto
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
