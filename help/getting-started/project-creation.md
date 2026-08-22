---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/getting-started/project-creation.html"
breadcrumb-title: ''
description: Aprende a crear un nuevo proyecto en Substance 3D Painter para empezar a pintar texturas en tus modelos en 3D.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Project Creation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Creación de proyectos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 1%

---


# Creación de proyectos

![](../assets/v12_banner_project_window.jpg)

La <b>ventana Nuevo proyecto </b> te permite crear un archivo de proyecto para almacenar tu modelo 3D y su información de texturizado.

Se crea un nuevo [conjunto de texturas](../interface/texture-set/texture-set.md) por definición de material que se encuentre en el modelo 3D importado. Esto significa que se pueden importar varios objetos a través de un solo archivo (incluso con UV superpuestos) si tienen diferentes materiales.

## Crear un nuevo proyecto

Para crear un nuevo proyecto, haz clic en <b>Archivo > Nuevo</b> o usa el método abreviado de teclado <b>Ctrl + N</b>.

A continuación, se explican todos los parámetros disponibles en la ventana Nuevo proyecto.

### Configuración básica

| *Parámetro* | *Descripción* |
| --- | --- |
| **Archivo** | Haga clic en el botón &quot;Seleccionar&quot; para especificar un archivo de modelo 3D para cargar. [Aquí hay disponible una lista de formatos de archivo compatibles.](https://experienceleague.adobe.com/es/docs/substance-3d/general-knowledge/ecosystem/import-and-export-formats) |
| **Plantilla** | Especifique una plantilla que defina la configuración predeterminada del proyecto. Una plantilla contiene los siguientes parámetros:<ul data-preserve-html="true"> <li data-preserve-html="true">Ajustes del conjunto de texturas.</li> <li data-preserve-html="true">Ajustes de visualización.</li> <li data-preserve-html="true">Configuración de horneado.</li> <li data-preserve-html="true">Recursos de sombreado (incluidas texturas adjuntas).</li> <li data-preserve-html="true">Archivo de mapa de entorno.</li> </ul>  **Nota:** Las plantillas son <b>\*.spt</b> archivos creados a partir de un proyecto existente a través del [menú Archivo](../interface/main-menu/file-menu.md) y guardados dentro de la carpeta Activos para compartirlos fácilmente con los integrantes del equipo. |
| <b>Resolución</b> | Defina la resolución de textura por defecto del proyecto para cada conjunto de texturas. La resolución puede llegar a 4K (4096x4096 píxeles) cuando se trabaja dentro de la aplicación y a 8K (8192x8192 píxeles) cuando se exporta. La resolución se puede cambiar en cualquier momento más adelante mediante la [configuración del conjunto de texturas](../interface/texture-set/texture-set-settings.md).  **Nota:** La exportación de 8K requiere al menos 2,5 GB de VRam en la GPU para estar disponible. |

### Configuración específica de tipo de archivo

Cuando se selecciona un USD, otras configuraciones específicas del tipo de archivo quedan disponibles.

| *Parámetro* | *Descripción* |
| --- | --- |
| <b>Ámbito y variantes</b> | Seleccione una parte específica de un archivo USD. De forma predeterminada, se establece en &quot;Root&quot;, lo que significa que se utilizará todo el archivo USD para crear el proyecto de Painter.  <b>Cambiar...</b> abre una nueva ventana que muestra el contenido del USD. Si se detectan variantes, es posible seleccionar una variante específica para la creación de proyectos. El ámbito y las variantes se pueden cambiar después de crear el proyecto en la configuración de [Project configuration](../interface/project-configuration.md). Tenga en cuenta que:<ul data-preserve-html="true"> <li data-preserve-html="true">Solo la selección de variante de modelado tendrá algún impacto en el proyecto.</li> <li data-preserve-html="true">Las variantes anidadas dentro de variantes no se detectan actualmente.</li> </ul> |
| <b>Nivel de subdivisión</b> | Para la geometría que se debe subdividir, este ajuste le permite especificar cuánto desea subdividir la malla para texturizar en Painter. Si subdivision se establece explícitamente en &#39;none&#39; dentro del archivo USD, esta configuración estará atenuada.  La subdivisión se aplica después de desenvolver UV, por lo que esto no altera la forma de los UV de la malla. Los niveles de subdivisión se pueden cambiar después de crear el proyecto en la configuración de [Proyecto](../interface/project-configuration.md). |
| <b>Marco</b> | Para los archivos USD en los que se detectan animaciones, esta configuración le permite seleccionar el marco que se utilizará para crear su proyecto de Painter. Si no hay ninguna animación en el archivo USD seleccionado, esta configuración está atenuada. El marco se puede cambiar después de crear el proyecto en la configuración de [proyecto](../interface/project-configuration.md). |

### Configuración avanzada

| *Parámetro* | *Descripción* |
| --- | --- |
| **Formato de mapa de normales** | Define el Formato de mapa de normales del proyecto, puede ser<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (X+, Y-, Z+)</li><li data-preserve-html="true"><strong>OpenGL</strong> (X+, Y+, Z+)</li></ul>  **Nota:** Como recordatorio:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Unreal Engine</b> usa DirectX de forma predeterminada.</li> <li data-preserve-html="true"><b>Unity</b> usa OpenGL de forma predeterminada.</li> </ul> |
| **Calcular espacio tangente por fragmento** | Si se activa, los bitangents se calculan en el sombreador de fragmentos (píxeles) en lugar del sombreador de vértices. Este parámetro afecta a la forma en que el sombreador descodifica el mapa Normal en la ventana gráfica. Para cambiar esta configuración, será necesario volver a realizar el mapa Normal.  **Nota:** Como recordatorio:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>El motor irreal</b> necesita que esta configuración esté habilitada.</li> <li data-preserve-html="true"><b>Unity</b> necesita que esta configuración esté Deshabilitada (o habilitada si está utilizando el flujo de trabajo HDRP)</li> </ul> |

### Configuración de mosaico de UV (UDIM)

>[!NOTE]
>
> Esta configuración no se puede modificar una vez creado el proyecto.

| *Parámetro* | *Descripción* |
| --- | --- |
| **Usar flujo de trabajo de mosaico UV** | Si se marca, la malla importada se procesará de forma diferente para permitir pintar fuera del rango UV normal (0-1). Los proyectos que utilicen UDIM deben habilitar esta configuración. El procesamiento de la malla puede variar dependiendo de la configuración.   Para obtener más información, consulte la [documentación del mosaico UV](../features/uv-tiles/uv-tiles.md). |
| <b>Conservar diseño de azulejo UV por materiales y habilitar la pintura en azulejos</b> | Los mosaicos UV (UDIM) se importan y agrupan por asignación de material en la malla. Esto significa que un único conjunto de texturas puede contener varios mosaicos UV visibles en paralelo en la vista 2D. Los mosaicos UV que se encuentran dentro del mismo conjunto de texturas se pueden pintar a lo largo sin problemas.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c1_image_copy" src="../assets/uvtiles-paintacross.jpg" width="500px"/></div> |
| <b>Convertir mosaicos UV en conjuntos de texturas individuales (heredados)</b> | Los mosaicos UV (UDIM) se separan en conjuntos de texturas individuales y se les cambia el nombre, ignorando cualquier asignación de material. Cada mosaico UV se mueve al rango UV [0-1] para poder pintar.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c1_image" src="../assets/uvtiles-legacy.jpg" width="500px"/></div> |

### Configuración de importación

| ***Parámetro*** | ***Descripción*** |
| --- | --- |
| **Importar cámaras** | Si hay cámaras en el archivo de malla, se importarán al proyecto y se podrá acceder a ellas como ajustes preestablecidos para su visualización.  **Nota:** Substance 3D Painter no admite algunas cámaras en determinadas condiciones:<ul data-preserve-html="true"><li data-preserve-html="true">Cámaras físicas de 3DS Max.</li><li data-preserve-html="true">Cámaras ortográficas almacenadas en archivos Alembic (&#42;.abc).</li></ul> |
| **Desempaquetar automáticamente** | Si se habilita, se generarán las UV que faltan en la malla importada. El procesamiento puede cambiar en función de la configuración seleccionada mediante el botón **Opciones**.Para obtener más información, consulte la [documentación sobre el desajuste automático de UV](../features/automatic-uv-unwrapping.md). |

### Importar mapas con bake

Usa el botón <b>Agregar</b> para cargar archivos de textura como mapas de malla y asignarlos automáticamente en la configuración de [Conjunto de texturas](../interface/texture-set/texture-set-settings.md). Se debe seguir una convención de nomenclatura específica para que los mapas de malla se asignen automáticamente a sus conjuntos de texturas. Los mapas de malla también se pueden hornear directamente dentro de la aplicación; consulte la documentación de Horneado.

Convención de nomenclatura:<b> TextureSetName\_MeshMapName</b>

Ejemplo:<b> DefaultMaterial\_ambiente\_oclusión.png </b>

Lista de mapas de malla compatibles y sus nombres:

| *Mapa de malla* | *Convención de nombres de archivo* |
| --- | --- |
| **oclusión de ambiente** | ambiente\_oclusión |
| **Curvatura** | curvatura |
| **Normal** | normal\_base |
| **Normal del Espacio Mundial** | world\_space\_normals |
| **ID** | id |
| **Posición** | posición |
| **Thickness** | grosor |

### Tamaño físico

La configuración de tamaño físico le permite ajustar la forma en que Painter determina el tamaño físico de la malla en unidades del mundo real. Esto resulta útil para garantizar que los materiales se aplican a una escala realista.

* Utilice la escala de unidades interna del archivo de malla: La mayoría de los tipos de archivo incluyen información sobre el tamaño físico del objeto tal y como se exportó desde la aplicación de modelado 3D. Con esta opción seleccionada, Painter utilizará esta información del archivo importado.
* Escala de unidad personalizada: Sobrescribir la escala de unidades del archivo importado o, si no se incluye ninguna escala de unidades, utilizar el cuadro de entrada personalizado para ajustar el tamaño de una sola &quot;unidad&quot;.
* Cambiar la escala de la capa de relleno a Tamaño físico al asignar materiales: Si esta opción está activada, los materiales con información de tamaño físico pueden ajustar su escala para que coincida con el tamaño físico de la superficie a la que se aplican.

### Gestión de colores

![](../assets/newproj-cm.png)

Esta sección controla la configuración de gestión de color del proyecto. De forma predeterminada, se establece en Heredado (sRGB / flujo de trabajo lineal).

Consulta la documentación de [administración de color](../features/color-management/color-management.md) para obtener más información sobre cómo usar este flujo de trabajo y lo que está haciendo la configuración.
