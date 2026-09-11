---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/fill-projections/spherical-projection.html"
breadcrumb-title: ''
description: Utilice proyección esférica en Substance 3D Painter para proyectar texturas de una esfera y ajustarlas alrededor de los objetos.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Spherical projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Proyección esférica
user-guide-description: ''
user-guide-title: ''
source-git-commit: 7e24e45387178db5efa813e64e4b86ac2ae2e5aa
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 2%

---


# Proyección esférica

![](../../assets/spherical-proj.jpg)

La Proyección esférica de relleno permite proyectar imágenes y patrones alrededor de un objeto. Puede resultar útil proyectar en objetos redondos o distorsionar la textura en patrones circulares.

## Propiedades

| Configuración | Descripción |
| --- | --- |
| **Filtrado** | Controla cómo se filtrará la textura o el material. Este ajuste puede afectar al aspecto de la textura cuando se repite varias veces. Si los valores de escala son altos y se utiliza un filtro diferente al predeterminado, el resultado puede ser más atractivo. Configuración actual disponible:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>HQ `\|` bilineal</strong> (predeterminado): Filtro bilineal avanzado que intenta mejorar la calidad de la textura cuando los valores de mosaico son altos.</li><li data-preserve-html="true"><strong>Bilineal `\|` Agudo</strong>: Filtro bilineal simple que suaviza ligeramente la textura pero intenta conservar los detalles.</li><li data-preserve-html="true"><strong>Más cercano</strong>: Sin filtrado, útil si el filtrado bilineal proporciona un resultado borroso y rompe detalles precisos. Puede introducir suavizado en la textura.</li></ul> |
| **Envolvimiento de UV** | Controle cómo se repite la textura dentro de la proyección. Los valores posibles son:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Ninguno</strong>: la textura no se repite. Cualquier cosa fuera de la textura es negro/transparente.</li><li data-preserve-html="true"><strong>Repetir horizontalmente</strong>: la textura solo se repite horizontalmente.</li><li data-preserve-html="true"><strong>Repetir verticalmente</strong>: la textura solo se repite verticalmente.</li><li data-preserve-html="true"><strong>Repetir</strong> (predeterminado): la textura se repite en ambos ejes.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-repeat.jpg" width="500px"/></div> |
| **Recorte de formas** | Defina si la textura proyectada debe ser visible fuera del área de proyección. Los valores posibles son:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Proyecto recortado a la forma</strong>: la proyección está confinada dentro del área de proyección.</li><li data-preserve-html="true"><strong>La proyección se extiende fuera de la forma</strong> (predeterminado): la proyección continúa más allá del área de proyección.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-shape-crop.jpg" width="500px"/></div> |

### Transformación UV

Los ajustes de transformación UV controlan la textura dentro de la proyección.

| *Configuración* | *Descripción* |
| --- | --- |
| **Escala** | Defina cuántas veces se repetirá la textura dentro de la proyección. |
| **Rotación** | Controle el ángulo de la textura aplicada a la proyección. |
| **Desplazamiento** | Controle el origen de la textura proyectada. El valor predeterminado significa que la textura se encuentra en el centro de la proyección. |

### Configuración de proyección 3D

Los ajustes de proyección 3D controlan la transformación de la proyección en el espacio 3D.

| Configuración | Descripción |
| --- | --- |
| **Desplazamiento** | Posición del origen de la proyección en el espacio 3D. Las unidades se basan en el cuadro delimitador de toda la escena. 0 es el centro de esta caja. |
| **Rotación** | Ángulos en grados para rotar toda la proyección en cada eje. |
| **Escala** | Tamaño de toda la proyección en cada eje. |

## Barra de herramientas contextual

Hay varias configuraciones y herramientas disponibles en la [barra de herramientas contextual](../../interface/toolbars.md) situada en la parte superior de la ventana gráfica que proporciona controles sobre el manipulador y la proyección:

| Icono | Nombre | Descripción |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_image" src="../../assets/icon-hide-manipulator.png" width="50px"/></div> | Mostrar/ocultar manipulador | Si está activado, el manipulador es visible y controlable en la ventana gráfica. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_image" src="../../assets/icon-manipulator-settings.png" width="50px"/></div> | Configuración del manipulador | Este menú contiene tres ajustes:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Tamaño de Manipulador</strong>: controle el tamaño del manipulador en la ventana gráfica.</li><li data-preserve-html="true"><strong>Pasos de cuadrícula</strong>: defina el tamaño del paso al realizar la conversión con una restricción.</li><li data-preserve-html="true"><strong>Pasos angulares</strong>: defina el ángulo del paso al rotar con una restricción.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-translate.png" width="50px"/></div> | Manipulador de traducción | Permita mover la proyección en la escena a lo largo de los ejes principales (X, Y, Z). |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-rotate.png" width="50px"/></div> | Manipulador de rotación | Permita girar la proyección en la escena a lo largo de los ejes principales (X, Y, Z). |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-scale.png" width="50px"/></div> | Manipulador de escala | Permite escalar la proyección en la escena a lo largo de los ejes principales (X, Y, Z). |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-surface.png" width="50px"/></div> | Manipulador de superficie | Permita mover la proyección ajustándola a la superficie del modelo 3D.  **Nota:** Este manipulador solo está disponible con los tipos de proyección Plano y Deformación. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-space.png" width="50px"/></div> | espacio del manipulador | Defina en qué espacio se realiza la transformación. Los valores posibles son:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Espacio local</strong>: los ejes se alinean con la transformación actual.</li><li data-preserve-html="true"><strong>Espacio mundial</strong>: los ejes se alinean con la escena.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | Reflejar en X | Voltear la transformación en el eje X. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Espejo en Y | Voltear la transformación en el eje Y. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-z.png" width="50px"/></div> | Reflejar en Z | Voltear la transformación en el eje Z. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r11-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-reset.png" width="50px"/></div> | Restablecer transformación | Restaurar la transformación de la proyección a su estado predeterminado. |

## Manipulador

Este manipulador de proyección solo está disponible en la [ventana gráfica 3D](../../interface/viewport/3d-view.md).

| Acción | Método abreviado | Descripción |
| --- | --- | --- |
| **Traducción** | Clic del ratón | Con el manipulador de Traducción, al hacer clic en los ejes se mueve la proyección:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Un eje</strong>: solo se mueve en una dirección de la proyección.</li><li data-preserve-html="true"><strong>Dos ejes</strong>: mueva la proyección en los planos alineados con los ejes.</li><li data-preserve-html="true"><strong>Tres ejes</strong>: mueva la proyección en el espacio de la cámara (plano orientado).</li></ul>   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-translate-2axes.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/3d-translate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Traducción restringida** | MAYÚS+Clic del ratón | Con el manipulador de traslación, mueva la proyección a lo largo de los ejes seleccionados, pero solo a intervalos específicos (paso a paso). El tamaño del intervalo se define mediante la configuración del manipulador. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate-step.gif" width="200px"/></div> |
| **Rotación** | Clic del ratón | Con el manipulador Rotación, al hacer clic en uno de los ejes, se gira la proyección. Haga clic entre los ejes para poder rotar todos los ejes al mismo tiempo.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-rotate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Restricción de rotación** | MAYÚS+Clic del ratón | Con el manipulador de rotación, hacer clic en un eje para rotar la proyección solo se producirá a intervalos específicos. El paso se define mediante un ángulo a través de los ajustes del manipulador. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate-step.gif" width="200px"/></div> |
| **Escala** | Clic del ratón | Con el manipulador Escala (Scale), al pulsar en un manejador de eje se cambia el tamaño de la proyección a lo largo del eje dado.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-one-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/scale-two-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/scale-3-axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Escala restringida** | MAYÚS+Clic del ratón | Con el manipulador Escala, al hacer clic en un manejador de eje mientras mantiene el método abreviado, la proyección cambiará de tamaño en pasos. El tamaño del paso es el mismo que para el manipulador de traducción. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-1-axis-constrained.gif" width="200px"/></div> |
| **Superficie** | Clic del ratón | Con el manipulador Superficie (Surface), si se pulsa y se arrastra sobre el modelo 3D, se ajustará a la superficie. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/surface.gif" width="200px"/></div> **Nota:** Este manipulador solo está disponible con los tipos de proyección **Planar** y **Deformar**. |
