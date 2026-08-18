---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/interface/layer-stack/geometry-mask.html"
breadcrumb-title: ''
description: Aprenda a utilizar máscaras de geometría en Substance 3D Painter para enmascarar capas en función de la geometría de malla y las propiedades de la superficie.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Geometry mask
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Máscara de geometría
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 1%

---


# Máscara de geometría

![](../../assets/geometry-mask.png)\
La máscara de geometría es una máscara secundaria en capas que permite enmascarar una capa en función de la geometría del modelo 3D del conjunto de texturas asociado. Se puede enmascarar por nombres de malla o por mosaicos UV.

## Información general

La máscara de geometría funciona especificando qué parte del modelo 3D debe aplicar la capa mediante una lista de inclusión/exclusión.

La máscara de geometría es una herramienta útil para descartar rápidamente gran parte de la geometría del modelo 3D. Ofrece varias ventajas a la máscara de pintura:

* Normalmente, es más rápido configurar y utilizar los modos de selección de ventanilla.
* Ofrece mejores prestaciones, ya que la geometría se puede descartar por completo al generar las texturas.
* No es destructivo y se actualizará cuando el modelo 3D cambie después de una reimportación.
* Permite pintar la geometría que se encuentra debajo de la geometría enmascarada, lo que permite pintar partes ocultas.
* Al igual que la máscara de pintura, la máscara geométrica se puede aplicar a un grupo para que afecte a varias capas a la vez.

### Estados de icono

El icono de máscara de geometría puede indicar en qué estado se encuentra:

| Icono | Descripción |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-default.png"/></div> | No se ha excluido ninguna geometría, la capa se aplica a toda la malla del conjunto de texturas asociado. Este es el estado predeterminado de cualquier capa o carpeta nueva. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-selection.png"/></div> | Se han excluido uno o más nombres de malla. El número indica la cantidad de elementos restantes que la capa sigue afectando. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-uvtiles.png"/></div> | Se han excluido uno o más mosaicos UV. El número indica la cantidad de elementos restantes que la capa sigue afectando. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-empty.png"/></div> | No se incluyen nombres de malla, la capa no tendrá ningún efecto real. |

## Edición de la máscara de geometría

Para modificar la máscara de geometría de una capa determinada, basta con hacer clic en el icono específico. Para salir del modo de edición, simplemente haz clic en otra parte de la capa, como el contenido o la máscara de pintura:

![](../../assets/geo-mask-editing.gif)

### Tipos de máscara

La máscara de geometría admite dos tipos de enmascaramiento:

| Tipo | Descripción |
| --- | --- |
| **Mosaicos UV** | El enmascaramiento se realiza especificando qué número de azulejo UV (UDIM) debe incluirse. Este es el método de mayor rendimiento, ya que permite descartar completamente una textura de ser computada. |
| **Nombres de malla** | El enmascaramiento se realiza especificando qué submalla debe incluirse en el modelo 3D. La geometría se agrupa por nombre de malla. |

### Acciones de pila de capas

![](../../assets/geo-mask-actions.png)

El estado de la máscara de geometría se puede modificar rápidamente desde la pila de capas directamente haciendo clic con el botón derecho en el icono.

Ofrece las siguientes acciones:

| Acción | Descripción |
| --- | --- |
| **Copiar máscara de geometría** | Copie el tipo y la selección de la máscara de geometría de la capa dada. |
| **Pegar en máscara de geometría.** | Pegue las propiedades de máscara de geometría copiadas anteriormente. |
| **Incluir todos** | Marque todos los elementos de la máscara dada como seleccionados. |
| **Excluir todo** | Marque todos los elementos de la máscara dada como no seleccionados. |

## Pintura mediante geometría enmascarada

Cuando se han excluido partes de la geometría, se pueden ocultar en la ventana gráfica. Esto permite pintar sobre la geometría que anteriormente estaba por debajo y no accesible.

Para ocultar la geometría excluida, utilice el botón situado en la parte superior de la ventana gráfica en la barra de herramientas contextual:

![](../../assets/hide-excluded-geo-button.png)

En el ejemplo siguiente, el modelo 3D se ha dividido en dos objetos: una parte superior e inferior. De forma predeterminada, los trazos de pincel entran en conflicto con todos los objetos. excluyendo la parte superior, ahora solo es posible pintar la parte inferior de forma exclusiva.

>[!NOTE]
>
> La lista de inclusión/exclusión de la máscara geométrica es dinámica; si se cambia su estado, se activará un nuevo cálculo de los trazos de pincel en la capa. Esto permite ajustar la máscara sin perder los trazos de pincel al volver a importar una malla con nuevos azulejos UV o si los nombres de la malla han cambiado. Sin embargo, también significa que los trazos de pincel no están horneados, por lo que cualquier cambio en la máscara de geometría podría provocar una proyección de pincel incorrecta posteriormente.

| Visual | Descripción |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/no-geo-excluded.jpg" width="420px"/></div> | No se ha excluido ninguna geometría en la máscara de geometría; la capa de pintura en la que se ha realizado el trazo de pincel blanco colisiona con toda la geometría.El botón **Ocultar geometría excluida** está deshabilitado. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-excluded-hidden.jpg" width="420px"/></div> | La parte superior se ha excluido de la máscara de geometría y el trazo de pincel blanco solo entra en conflicto con la parte inferior de la geometría.El botón **Ocultar geometría excluida** está habilitado. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-excluded-visible.jpg" width="420px"/></div> | La parte superior se ha excluido de la máscara de geometría y el trazo de pincel blanco solo entra en conflicto con la parte inferior de la geometría.El botón **Ocultar geometría excluida** está deshabilitado. |
