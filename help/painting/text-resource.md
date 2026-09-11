---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/painting/text-resource.html"
breadcrumb-title: ''
description: Aprenda a usar recursos de texto en Substance 3D Painter para añadir texto y tipografía a sus flujos de trabajo de textura.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Recurso de texto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---


# Recurso de texto

![](../assets/v10_text_resource_banner-1.jpg)

El <b>recurso de texto</b> de se puede usar para escribir texto en texturas con el uso de <b>archivos de fuentes</b> específicos. Hay varios parámetros disponibles para ajustar el aspecto del texto final dibujado.

## Examinar fuentes

Para examinar los archivos de fuentes disponibles, simplemente haz clic en el filtro de fuentes (el botón <b>T</b>) en la [ventana Activos](../interface/assets/assets.md):

![](../assets/v10_text_assets.png)

Las fuentes también se pueden filtrar por rutas según su ubicación en el sistema:

![](../assets/v10_font_path.png)

Las ubicaciones de fuentes disponibles dependen del sistema operativo actual:

|  |  |
| --- | --- |
| Windows | <ul data-preserve-html="true"> <li data-preserve-html="true"><b>Sistema</b>: C:/Windows/Fonts</li> <li data-preserve-html="true"><b>Usuario</b>: C:/Users/username/Appdata/Local/Microsoft/Windows/Fonts</li> </ul> |
| MacOS | <ul data-preserve-html="true"> <li data-preserve-html="true"><b>Sistema</b>: /Sistema/Biblioteca/Fuentes</li> <li data-preserve-html="true"><b>Local</b>: /Biblioteca/Fonts</li> <li data-preserve-html="true"><b>Usuario</b>: /Usuarios/nombre_usuario/Biblioteca/Fonts</li> </ul> |
| Linux | <ul data-preserve-html="true"> <li data-preserve-html="true"><b>Sistema</b>: /usr/share/fonts/</li> <li data-preserve-html="true"><b>Local</b>: /usr/local/share/fonts/</li> <li data-preserve-html="true"><b>Usuario</b>: /home/username/.local/share/fonts/</li> </ul> |

### Importación de fuentes

Las fuentes se pueden importar manualmente o colocarse en una biblioteca de Painter existente, como cualquier recurso normal. Para ello, consulte la [documentación de importación](../content/importing-assets/import-drag-and-drop.md).

Painter admite los formatos de fuente <b>.ttf</b> y <b>.otf</b>.

>[!NOTE]
>
> Si un recurso no se carga o importa con el mensaje de error &quot;no se puede importar debido a la restricción de licencia de la fuente&quot;, significa que Painter no lo puede usar. Solo se puede usar la fuente marcada como <b>incrustable</b> en sus metadatos.

### Uso de una fuente como recurso de texto

Un recurso de textura funciona como otros recursos (imágenes o materiales de Substance, por ejemplo) y se puede utilizar en parámetros de pincel, proyecciones de relleno o entradas de imagen de Substance.

Para crear un recurso de texto, basta con añadir una fuente en una ranura de recurso. También es posible arrastrar y soltar una fuente en la ventana gráfica.

![](../assets/v10_text_drag_drop.gif)

### Parámetros de recursos de texto

Un recurso de texto tiene los siguientes parámetros básicos:

![](../assets/v10_text_params_base.png)

| <b>Parámetro</b> | <b>Descripción</b> |
| --- | --- |
| <b>Texto</b> | Texto que se va a representar.  **Nota:** El campo de texto de la interfaz usa una fuente genérica con una amplia gama de caracteres que pueden crear discrepancias entre lo que se escribió en el campo y lo que la fuente seleccionada puede representar en la textura. |
| <b>Tamaño de fuente</b> | Especifique el modo utilizado para calcular el tamaño de fuente. Los modos disponibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Automático</b>: el tamaño se calcula automáticamente a partir del contenido de texto y se ajusta a la textura.</li> <li data-preserve-html="true"><b>Personalizado</b>: el tamaño se puede controlar manualmente mediante la configuración dedicada.</li> </ul> |
| <b>Alineación</b> | Controlar la alineación vertical y horizontal. Utilice los botones para elegir el modo que desea utilizar. |
| <b>Color</b> | El color del texto procesado. Este ajuste puede ser de escala de grises si el recurso de texto se utiliza en una máscara o en un canal de escala de grises. |

También hay disponibles parámetros más avanzados:

![](../assets/v10_text_params_advanced.png)

| <b>Parámetro</b> | <b>Descripción</b> |
| --- | --- |
| <b>Interlineado</b> | Distancia entre líneas de texto (&quot;interlineado&quot;) en relación con el tamaño de fuente. |
| <b>Espaciado entre caracteres</b> | Cantidad de espacio entre caracteres adyacentes en relación con el tamaño de fuente. Puede ser negativo para restar espacio. |
| <b>Desplazamiento</b> | Desplazamiento horizontal y vertical del texto. Normalizado al tamaño de fuente. |
| <b>Relleno de fondo</b> | Color del fondo detrás del texto. |
| <b>Opacidad de fondo</b> | Cantidad de color de fondo visible. |
| <b>Resolución</b> | Especifique el modo utilizado para calcular el tamaño de la textura utilizada para representar el texto. Los modos disponibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Automático</b>: La resolución se calcula automáticamente.</li> <li data-preserve-html="true"><b>Personalizado</b>: La resolución se puede definir manualmente mediante la configuración dedicada.</li> </ul> |
