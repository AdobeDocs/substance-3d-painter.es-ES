---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/interface/assets/navigation.html"
breadcrumb-title: ''
description: Aprenda a navegar por el panel Activos en Substance 3D Painter para navegar y acceder a su biblioteca de recursos de manera eficiente.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Navigation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Navegación
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 1%

---


# Navegación

Existen varios medios de navegación en la ventana Activos: ruta de exploración, campo de búsqueda e icono de tipos de activos. Todos los tipos de navegación son co-dependientes, por lo que puede combinar esas búsquedas a su favor.\
Por ejemplo, si ha seleccionado Materiales en los iconos de tipo de recurso, pero ha utilizado la ruta de exploración para desplazarse a la carpeta Máscaras inteligentes, el panel Recursos no mostrará ningún resultado; tendrá que volver a Todas las bibliotecas si desea mostrar Materiales o anular la selección de Materiales si desea examinar las Máscaras inteligentes.

## Rastros

Las rutas de exploración le permiten navegar rápidamente por la biblioteca. Al hacer clic en las flechas, se muestra cómo se almacenan los recursos en el disco y se puede seleccionar cualquiera de las ubicaciones mostradas. Si está atenuado, significa que no hay activos del tipo seleccionado dentro de esa carpeta, pero aún puede navegar a esa ubicación.

![](../../assets/00-05-breadcrumbs.jpg)

## Campo de búsqueda

El campo de búsqueda se puede utilizar para filtrar los recursos que contienen la consulta con tipo. Tenga en cuenta que no sólo realiza búsquedas por el título de los recursos, sino también por su ubicación y cualquier etiqueta contenida en el recurso.\
Las búsquedas escritas también pueden ser más avanzadas que las palabras clave. Consulte [Consultas de búsqueda avanzada](advanced-search-queries.md).

![](../../assets/00-05-searchfield.jpg)

## Tipos de activos

>[!NOTE]
>
> Los iconos de tipos de activos se pueden seleccionar de varias formas manteniendo la tecla **Ctrl** al hacer clic.

La selección predeterminada es Materiales, pero al hacer clic en otros iconos de tipos de activos, se muestran otros tipos de recursos.

![](../../assets/00-05-assettypeicons.jpg)

| Tipos de activos | Descripción |
| --- | --- |
| Materiales <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1-1.png"/></div> | Contienen .sbsar importados como *material base* y materiales creados a partir de una capa de relleno (puede obtener más información sobre la creación de ajustes preestablecidos [aquí](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/creating-and-saving-a-preset-180191514.html)). Son materiales básicos que se pueden usar en capas de relleno y se aplicarán a toda la superficie de la malla o el conjunto de texturas. |
| Materiales inteligentes <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-7.png"/></div> | Contengan materiales más complejos que consten de varias capas guardadas dentro de una carpeta (los Materiales inteligentes también son ajustes preestablecidos que puede crear). Al igual que los materiales base, los Materiales inteligentes se aplicarán a la totalidad de su malla/conjunto de texturas, pero también tendrán en cuenta la información individual de la malla, como la curvatura, la Oclusión o cualquier otro detalle de la superficie. Para obtener estos detalles de la superficie y usar Materiales inteligentes correctamente, primero debe [hacer un bake](../../baking/baking.md) la malla. |
| Máscaras inteligentes <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-2.png"/></div> | Contienen máscaras más complejas que utilizan efectos o generadores de varias capas. Puedes [crear](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) ajustes preestablecidos de Máscaras inteligentes tú mismo.De forma similar a los Materiales inteligentes, las Máscaras inteligentes necesitan información hecha un bake de su malla para funcionar correctamente. |
| Filtros <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-3.png"/></div> | Contiene archivos .sbsar importados como *filter*.Los filtros son efectos que toman la textura que ya tienes y la transforman de alguna manera. Algunos filtros solo funcionan con información en blanco y negro, algunos solo con entradas de material, lo que significa que no todos los filtros se pueden usar en máscaras. |
| Pinceles <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-4.png"/></div> | Contiene pinceles, partículas y herramientas. Estos son todos los ajustes preestablecidos que se pueden [crear](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) en Painter.**Los pinceles** son ajustes preestablecidos básicos en blanco y negro que usan una alfa. Puede usar pinceles para realizar pinturas en cualquiera de los canales o en todos ellos, o en una máscara.**Las partículas** tienen las mismas características que los pinceles, pero también tienen un conjunto adicional de parámetros que simulan la interacción física con la malla. Pueden producir los efectos de derrames, goteos, lluvia o cualquier otro que requiera una simulación física.**Herramientas** puede contener el comportamiento Pincel o Partícula, pero además este ajuste preestablecido también se guarda con información de canales de material. |
| Alfas <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-5.png"/></div> | Contienen una variedad de alfa, así como varios fabricantes de pinceles que permiten [crear](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) pinceles con efectos más elaborados (similares a Photoshop, trazos dinámicos, rodillo de pintura). Los Alpha son imágenes en escala de grises en las que las partes negras aparecen transparentes cuando se usan. |
| Texturas <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-6.png"/></div> | Contiene grunges, procedimientos, mapas con bake, normales de superficie dura y LUT.**Grunges** son imágenes en escala de grises con ruidos y texturas interesantes. Se pueden utilizar para añadir variación a la superficie de la malla, ya sea mediante máscara o conectándolos directamente en un canal.Los **procedimientos** también son texturas en escala de grises que comprenden ruidos o incluso patrones regulares. Sin embargo, a diferencia de algunos grunges estáticos, los procedimientos son mapas de bits dinámicos que se pueden escalar sin repetición y tienen variaciones infinitas (mediante semilla aleatoria).**Mapas con bake** representan la información de superficie y forma extraída de la malla. Para obtener más información sobre cómo hacer un bake, consulte aquí.**Las normales de superficie dura** son detalles que puede marcar directamente en su malla mediante el canal Normal.**LUT** (tablas de búsqueda) son texturas de perfil de color que se pueden usar en la configuración de visualización para simular un comportamiento de perfil de color en la ventana gráfica. Puede obtener más información sobre los perfiles de color [aquí](../../features/post-processing/color-profile.md). |
| Mapas de entorno <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1.jpg"/></div> | Contienen imágenes importadas como *entorno* (normalmente .hdr o .exr). Los mapas de entorno son imágenes de fondo que generan automáticamente una configuración de iluminación. Puede utilizar un mapa de entorno arrastrándolo directamente a la ventana gráfica o a través de la configuración de visualización. |
