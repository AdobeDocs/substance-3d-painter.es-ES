---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export/export-window/export-settings.html"
breadcrumb-title: ''
description: Aprenda a configurar los ajustes de exportación en Substance 3D Painter para controlar la resolución de textura, el formato y las opciones de salida.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Export window > Export settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ajustes de exportación
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 1%

---


# Ajustes de exportación

![](../../assets/image2023-1-30-13-22-30.png){width="500px"}

La <b>pestaña Configuración de exportación</b> de la <b>ventana texturas de exportación</b> le permite configurar la composición, el tamaño y la ubicación de las texturas exportadas.

## Configuración General y Conjuntos de texturas

![](../../assets/texture-set-list-1.png)

El primer elemento de la ventana es la lista de conjuntos de texturas de la izquierda. La sección Configuración global proporciona acceso a parámetros comunes en todos los conjuntos de texturas. Esto facilita el ajuste de un único conjunto de ajustes para aplicarlos a todos los conjuntos de texturas del proyecto. Los cambios realizados en la configuración individual del conjunto de texturas anularán la configuración global de dicho conjunto de texturas. Por ejemplo, si se establece la resolución en 2048 en la configuración global y en 1024 como una modificación para un conjunto de texturas específico, todos los conjuntos de texturas se exportarán con una resolución 2048, excepto el establecido en 1024.

La casilla de verificación junto a cada nombre de conjunto de texturas indica si se exportarán o no las texturas asociadas.

El menú desplegable es útil con proyectos que tienen un gran número de conjuntos de texturas, ya que te permite modificar rápidamente la selección con las acciones <b>Comprobar todo</b>, <b>Desmarcar todo</b> e <b>Invertir todo</b>.

## Parámetros generales de exportación

![](../../assets/image2023-1-30-13-23-7.png)

Esta sección contiene la configuración compartida de cada textura que se generará:

| Configuración | Descripción |
| --- | --- |
| <b>Directorio de salida</b> | Guardar ubicación para las texturas exportadas. |
| <b>Plantilla de salida</b> | Seleccione la plantilla de salida utilizada para nombrar y componer los canales en archivos de textura. Para obtener más información sobre las plantillas, consulte la lista [Plantillas de salida](../export-presets/export-presets.md). |
| <b>Tipo de archivo </b> | El formato de archivo y su profundidad de bits. Si se selecciona la opción <b>Basado en la plantilla de salida</b>, el formato de archivo se hereda del ajuste preestablecido de exportación (que permite determinar el formato y la profundidad de bits por textura en lugar de globalmente). La profundidad de bits disponible depende del tipo de archivo; consulte la siguiente tabla para obtener más información. |
| <b>Tamaño </b> | Resolución del archivo de textura exportado. Valores posibles:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Según el tamaño de cada conjunto de texturas</b></li> <li data-preserve-html="true"><b>128</b></li> <li data-preserve-html="true"><b>256</b></li> <li data-preserve-html="true"><b>512</b></li> <li data-preserve-html="true"><b>1024</b></li> <li data-preserve-html="true"><b>2048</b></li> <li data-preserve-html="true"><b>4096</b></li> <li data-preserve-html="true"><b>8192</b> (solo disponible con GPU que tengan más de 1,5 GB de Vram)</li> </ul> |
| <b>Relleno </b> | Cómo se rellena el área exterior de las Islas de UV dentro de la textura. Los valores posibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Sin relleno (paso a través)</b>: utilice el estado actual de la textura tal cual.</li> <li data-preserve-html="true"><b>Dilación infinita</b>: estire los bordes de las Islas de UV hasta que lleguen a los bordes vecinos o hasta el final de la textura.</li> <li data-preserve-html="true"><b>Dilación + transparente</b>: estirar bordes de Isla de UV a la distancia dada en píxeles, el resto es transparente.</li> <li data-preserve-html="true"><b>Dilación + color de fondo predeterminado</b>: estirar bordes de Isla de UV a la distancia dada en píxeles, el resto se rellena con el color predeterminado del canal del conjunto de texturas.</li> <li data-preserve-html="true"><b>Dilación + color de fondo predeterminado</b>: estirar bordes de Isla de UV a la distancia dada en píxeles, el resto se rellena con el color predeterminado del canal del conjunto de texturas.</li> <li data-preserve-html="true"><b>Dilación + difusión</b>: estire los bordes de la Isla de UV a la distancia dada en píxeles, el resto se rellena con una versión borrosa de la Isla de UV (basada en mapas mip).</li> </ul> |

>[!NOTE]
>
> El formato de archivo **psd** es un contenedor, lo que significa que los mapas de salida se recopilarán dentro de un solo archivo en el disco.

### Tramado

La exportación de texturas de 8 bits puede provocar bandas en los degradados. Esto se nota especialmente en los mapas normales y de Height. Hay dos formas de resolver este problema: usando mayor precisión o compensando con tramado.

Una precisión más alta (16 o 32 bits) es ideal, pero esto puede no ser compatible con todas las aplicaciones. Lo más notable es que los motores de juego a menudo se comprimen a 8 bits. El tramado introduce ruido que ayuda a mitigar los problemas de bandas mientras se siguen utilizando 8 bits de información.

![](../../assets/dither-1.jpg)

### Formatos de archivo de textura

A continuación se muestra una lista de todos los formatos de archivo de exportación compatibles con Painter:

| Nombre de formato | Extensión de formato | Profundidad de bits compatible |
| --- | --- | --- |
| **Mapa de bits** | bmp | 8, 8 + tramado |
| **OpenEXR** | exr | 16 (flotante), 32 (flotante) |
| **Formato Graphics Interchange** | gif | 8, 8 + tramado |
| **Radiance HDR.** | hdr | 32 (flotante) |
| **Icono** | ico | 8, 8 + tramado |
| **Jpeg 2000** | j2k | 8, 8 + tramado, 16 |
| **Gráficos De Red Jpeg** | jng | 8, 8 + tramado, 16 |
| **Jpeg 2000** | jp2 | 8, 8 + tramado, 16 |
| **Jpeg** | jpeg | 8, 8 + tramado |
| **Intervalo extendido del JPEG** | jpeg-xr | 8, 8 + tramado, 16, 32 (flotante) |
| **Mapa de bits portátil** | pbm | 8, 8 + tramado, 16 |
| **Mapa de Flotante portátiles** | pfm | 32 (flotante) |
| **Mapa gris portátil** | pgm | 8, 8 + tramado, 16 |
| **Gráficos de red portátiles** | png | 8, 8 + tramado, 16 |
| **Mapa de píxeles portátil** | ppm | 8, 8 + tramado, 16 |
| **Documento de Photoshop** | psd | 8, 8 + tramado, 16 |
| **Truevision TGA** | targa | 8, 8 + tramado |
| **Formato de archivo de imagen de etiqueta** | tiff | 8, 8 + tramado, 16, 32 (flotante) |
| **Formato de mapa de bits de protocolo de aplicaciones inalámbricas** | wbmp | 8, 8 + tramado |
| **WebP** | webp | 8, 8 + tramado |
| **X PixMap** | xpm | 8, 8 + tramado |

## Mapas de salida

Cuando se selecciona un conjunto de texturas específico, la sección Mapas de salida es visible para ese conjunto de texturas.

![](../../assets/export-output-maps.png)

En esta sección se enumeran todas las texturas que se generarán en función del ajuste preestablecido de exportación actual. Indica la plantilla de nombre de textura, el formato de archivo y la profundidad de bits, así como el espacio de color, si está habilitada la [administración de color](../../features/color-management/color-management.md).

Esta sección le permite deshabilitar la exportación de archivos específicos o invalidar el <b>formato de archivo</b> y la <b>profundidad de bits</b>.

![](../../assets/export-override.gif)

## Exportar activo de USD

Al marcar esta casilla, podrá exportar en USD formato. A diferencia del ajuste preestablecido USDz (Apple AR) disponible en <b>Plantillas de salida</b>, esta exportación tendrá en cuenta cualquier plantilla o parámetro que haya configurado para la exportación. Los siguientes archivos se exportan cuando se marca la casilla USD activo:

* Una carpeta con mapas de textura
* *.usda* que señala a la carpeta de asignaciones de textura.
* Un .usd opcional que ensambla materiales con el archivo de malla original. Se puede utilizar directamente en Omniverse para mostrar tu malla con materiales aplicados automáticamente.
* Un archivo .usd opcional, que incluye la malla utilizada en el proyecto. Solo se exporta si el archivo de malla original no es un USD o si se utilizó la función de desajuste automático de Painter para generar UV.
