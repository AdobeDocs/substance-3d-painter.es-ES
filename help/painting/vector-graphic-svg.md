---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/painting/vector-graphic-svg.html"
breadcrumb-title: ''
description: Aprenda a utilizar gráficos vectoriales (archivos de SVG y AI) en Substance 3D Painter para añadir ilustraciones vectoriales ampliables a las texturas.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gráfico vectorial (SVG)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---


# Gráfico vectorial (.svg y .ai)

![Imagen que muestra un archivo svg proyectado en una malla junto a una lista de parámetros](../assets/svg_overview.png)

Los archivos de gráfico vectorial (tanto <b>.svg</b> como Illustrator <b>.ai</b>) se pueden importar como imágenes normales dentro de Painter. Hay disponibles algunos ajustes para ajustar el aspecto del gráfico y hacer que se ajuste mejor al resto de la texturización.

* Para obtener más información sobre los archivos de SVG, [consulte esta página](https://www.adobe.com/creativecloud/file-types/image/vector/svg-file.html).
* Para obtener más información sobre los archivos AI, [consulte esta página](https://www.adobe.com/ie/creativecloud/file-types/image/vector/ai-file.html).

Los archivos de SVG y AI se convierten automáticamente en imágenes de píxeles cuando se usan dentro de la [Pila de capas](../interface/layer-stack/layer-stack.md) (según la configuración seleccionada). Este es un proceso no destructivo, cambiar la resolución o actualizar el archivo de origen actualizará el resultado final en consecuencia.

## Propiedades

Después de importar un archivo vectorial y cargarlo en las propiedades de una capa o herramienta, estará disponible un conjunto de parámetros:

| Sección | Configuración | Descripción |
| --- | --- | --- |
| <b>Mesa de trabajo</b> | <b>Mesa de trabajo</b> | Seleccione qué mesa de trabajo incluida en el archivo se utiliza.  **Nota:** Esta configuración solo está disponible con archivos de Illustrator (.ai). |
| <b>Resolución</b> | Resolución | Defina el tamaño con el que el archivo SVG se convertirá en una imagen de mapa de bits (píxeles) cuando se utilice para el texturizado dentro de la Pila de capas.   Valores posibles:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Automático</b>: la resolución viene determinada por la resolución del conjunto de texturas actual (cuando se utiliza en la capa/efecto de relleno) o de 512 píxeles cuando se utiliza en una herramienta de pincel.<br/> </li> <li data-preserve-html="true"><b>Activo</b>: la resolución viene determinada por el tamaño de píxel definido dentro del propio archivo de SVG.<br/> </li> <li data-preserve-html="true"><b>Personalizado</b>: la resolución viene determinada por la configuración de resolución que se encuentra justo debajo de la interfaz.</li> </ul>  <div><img alt="configuración de resolución svg" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-ad42696-column-7212622_image" src="../assets/svg_resolution_custom.png" title="configuración de resolución svg"/></div> |
|  |  |  |
| <b>Área de recorte</b> | Recortar a | Defina cómo las formas de SVG se limitarán al área procesada.   Valores posibles:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Límites de activos</b>: el área está definida por los límites definidos dentro del archivo de SVG.</li> <li data-preserve-html="true"><b>Personalizado</b>: el área se define mediante valores explícitos a través de la configuración de la interfaz que se muestra a continuación.<br/> </li> </ul> |
|  | Relación de aspecto cuadrada | Si el área de recorte está definida por <b>límites de recursos</b>, esta configuración garantiza que se conserve la proporción original, lo que evita estires incorrectas al procesar el SVG como una imagen cuadrada.   Esta configuración puede hacer que algunos elementos sean inesperadamente visibles. Para evitar este problema, desactive esta opción y ajuste manualmente la configuración de UV dentro de una capa o efecto de relleno. |
|  | Superior izquierda Inferior derecha | Si el área de recorte se establece en Área personalizada, estos ajustes permiten definir el área manualmente especificando las esquinas superior izquierda e inferior derecha. |
|  |  |  |
| <b>Ámbito</b> | Ámbito | Define qué elementos del archivo de SVG se incluyen antes de procesarlo.   El valor predeterminado es <b>Document</b>, lo que significa que se utiliza todo el contenido del archivo de SVG. Use el botón <b>Cambiar</b> para ajustar los elementos que se van a incluir. |

### Ventana Ámbito

Al editar el ámbito de un gráfico vectorial (consulte la configuración anterior) aparecerá una ventana con una lista de elementos que seleccionar para especificar lo que se debe incluir o excluir de la imagen final representada.

Utilice la casilla de verificación <b>Mostrar miniaturas</b> para mostrar una imagen para cada elemento.

![](../assets/v10_ai_thumbs.jpg)
