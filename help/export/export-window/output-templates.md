---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export/export-window/output-templates.html"
breadcrumb-title: ''
description: Aprenda a utilizar las plantillas de salida en la ventana de exportación de Substance 3D Painter para configurar los formatos y los nombres de exportación de las texturas.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Export window > Output templates
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Plantillas de salida
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 2%

---


# Plantillas de salida

![](../../assets/export-output-template.png){width="500px"}

La pestaña Plantilla de salida le permite administrar y crear nuevas Plantillas de salida. Puede utilizar Plantillas de salida para modificar los nombres, los formatos y la configuración de las texturas exportadas.

## Lista de ajustes preestablecidos

![](../../assets/export-preset-list.png)

La lista Ajustes preestablecidos muestra todas las Plantillas de salida disponibles. Esta lista incluye una colección de [Plantillas de salida predeterminadas](../export-presets/default-presets.md), así como cualquier plantilla personalizada que haya creado.

En esta lista, las plantillas se pueden <b>crear</b>, <b>cambiar de nombre</b>, <b>duplicar,</b> o <b>eliminar</b>.

| Acción | Visual | Descripción |
| --- | --- | --- |
| **Duplicar** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_image" src="../../assets/preset-duplicate.png"/></div> | Crear una copia de la plantilla de salida seleccionada actualmente en la lista. |
| **Quitar** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_image" src="../../assets/preset-remove.png"/></div> | Quitar la plantilla de salida seleccionada actualmente en la lista.  **Nota:** La eliminación de una plantilla no se puede deshacer. |
| **Agregar** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_image" src="../../assets/preset-add.png"/></div> | Añada una nueva plantilla de salida vacía. |
| **Haga doble clic** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c1_image" src="../../assets/rename-preset.gif"/></div> | Cambie el nombre de la plantilla de salida seleccionada. |
| **Clic con el botón derecho** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c1_image" src="../../assets/right-click.gif"/></div> | Haga clic con el botón derecho en una plantilla para abrir el menú contextual, donde puede eliminar, cambiar el nombre o duplicar una plantilla. |

## Lista de mapas de salida

![](../../assets/export-preset-config.png)

En esta sección se enumeran todas las texturas que generará la plantilla y su composición.

### Asignar tipos y palabras clave

La línea superior muestra todos los tipos de textura que se pueden realizar:

| Botón | Visual | Descripción |
| --- | --- | --- |
| **Gris** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c1_image" src="../../assets/export-type-gray.png"/></div> | Añada un nuevo mapa de escala de grises. |
| **RGB** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c1_image" src="../../assets/export-type-rgb.png"/></div> | Añada un nuevo mapa de color de RGB. |
| **R+G+B** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_image" src="../../assets/export-type-r-g-b.png"/></div> | Añada un nuevo mapa de RGB con 3 ranuras individuales en escala de grises. |
| **RGB+A** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c1_image" src="../../assets/export-type-rgb-a.png"/></div> | Añada una nueva asignación de RGB y una ranura alfa (en escala de grises). |
| **R+G+B+A** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c1_image" src="../../assets/export-type-r-g-b-a.png"/></div> | Añada un nuevo mapa RGBA con 4 ranuras individuales en escala de grises. |

>[!NOTE]
>
> Algunos tipos se pueden combinar o contraer cuando están vacíos o comparten la misma asignación de entrada:
> 
> ![](../../assets/split-collapse.gif)

### Nombre del mapa

![](../../assets/outputmap-name.png)

Se puede asignar un nombre a cada textura mediante una convención de nomenclatura personalizada. Se pueden agregar algunas palabras clave (con la ayuda del botón **$**) para que la aplicación las reemplace automáticamente cuando se genere el archivo final:

| Palabra clave | Descripción |
| --- | --- |
| **$proyecto** | Se reemplaza por el nombre del archivo de proyecto (.spp). |
| **$mesh** | Se reemplaza por el nombre del archivo de malla (archivo de malla de entrada, como .fbx) |
| **$textureset** | Se sustituye por el nombre del material/conjunto de texturas a partir del que se genera la textura. |
| **$udim** | Se reemplaza por el número de UDIM a partir del cual se genera una textura. |
| **$colorSpace** | Se reemplaza por el nombre del espacio de color utilizado para el canal dado (RGB o G, ignora Alpha). |

### Asignar formato de archivo y profundidad de bits

![](../../assets/outputmap-file-format-bit-depth.png)

La primera lista desplegable se puede utilizar para especificar el formato de archivo de la asignación de salida actual.

El segundo menú desplegable se utiliza para especificar la profundidad de bits del mapa de salida. La profundidad de bits depende del formato de archivo seleccionado. Consulte [Configuración de exportación](export-settings.md) para obtener más información.

>[!NOTE]
>
> Para que el formato y la configuración de profundidad de bits se tengan en cuenta al exportar, asegúrese de que el tipo de archivo en la configuración general esté establecido en **Según la plantilla de salida**.

## Lista de mapas de origen

![](../../assets/export-map-list.png)

### Mapas de entrada

La lista de asignación de entrada reagrupa todos los canales que se pueden agregar mediante la configuración de [Conjunto de texturas](../../interface/texture-set/texture-set-settings.md).

>[!NOTE]
>
> Los canales de **usuario** se basan en su nombre original (**usuario\_x**), los nombres personalizados se omiten.

### Mapas de malla

Los mapas de malla son las texturas hechas un bake:

| Nombre | Descripción |
| --- | --- |
| **Normal** | mapa de normales hecho un bake. |
| **Espacio normal del mundo** | Espacio hecho un bake normal del mundo. |
| **ID** | ID hecho un bake. |
| **oclusión de ambiente** | oclusión ambiental hecha un bake |
| **Curvatura** | Curvatura hecha un bake. |
| **Posición** | Posición hecha un bake. |
| **Thickness** | thickness hecho un bake. |
| **Height** | height hecho un bake. |
| **Normales dobladas** | Horneado doblado normales. |

### Mapas convertidos

Los mapas convertidos son mapas generados por la aplicación desde otro origen:

| Nombre | Descripción |
| --- | --- |
| **OpenGL de normal** | Mapa normal combinado en formato OpenGL de la normal horneada y el canal normal del conjunto de texturas. |
| **DirectX normal** | Mapa de normales combinado en formato DirectX de la normal hecha un bake y el canal normal del conjunto de texturas. |
| **OA mixta** | Oclusión de ambiente combinada de la oclusión de ambiente horneada y el canal de oclusión de ambiente del conjunto de texturas. |
| **Difusión** | textura de Difuso generada a partir del canal **Color base** y **Metálico** (las áreas metálicas se reemplazan por un color negro). |
| **Specular** | textura de specular generada a partir del **Color base** y el canal **Metallic**. |
| **Brillo** | Textura brillante generada a partir del inverso del canal de rugosidad. |
| **Unity4 Difuso** | Obsoleto. textura de Difuso generada a partir del canal **Color base** para que coincida con los sombreadores de Unity 4. |
| **Brillo Unity4** | Obsoleto. Textura brillante generada a partir del canal **Roughness** y **Metallic** para que coincida con los sombreadores Unity 4. |
| **Reflejo** | Texturas donde el blanco indica un material dieléctrico y otros colores como materiales metálicos. |
| **1/o** | Textura que contiene 1 dividida por el valor **IOR**. **IOR** se genera a partir del mapa metálico: 1,4 para dieléctricos, 100 para metales (color negro). |
| **Brillo<sup>2</sup>** | Versión cuadrada del canal **Brillo** (**Brillo** \* **Brillo**) |
| **f0** | Textura que contiene un valor de reflectancia de 0 (0,04 para dielétricos y 1,0 para metálicos). |
