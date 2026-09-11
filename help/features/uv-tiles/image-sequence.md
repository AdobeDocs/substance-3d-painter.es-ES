---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/uv-tiles/image-sequence.html"
breadcrumb-title: ''
description: Aprenda a utilizar secuencias de imágenes con mosaicos UV en Substance 3D Painter para flujos de trabajo de textura animados.
helpx_creative_field: ""
helpx_description: Painter > Features > UV Tiles > Image Sequence
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Secuencia de imágenes
user-guide-description: ''
user-guide-title: ''
source-git-commit: 8b892d2d6c9d0f1a3b5d9d3ab9b180a7c2770a83
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Secuencia de imágenes

Las secuencias de imágenes son una colección de imágenes que se agrupan como un único recurso en la estantería. Las imágenes se agrupan en función de un patrón específico en sus nombres de archivo.

## Cómo importar imágenes como una secuencia

Al importar un archivo de imagen, si el nombre de archivo coincide con un patrón específico, se importará automáticamente como una secuencia. Si hay imágenes adicionales junto al archivo importado, también se tendrán en cuenta. Por lo tanto, no es necesario importar todos los archivos de una secuencia manualmente, basta con seleccionar el primer archivo.

Ejemplos de coincidencia de nombre de archivo:

Los siguientes nombres de archivo importarán correctamente una secuencia de imágenes porque pueden reconocer que la última parte del nombre de archivo hace referencia a un número de UDIM 1032:

* archivo\_22.1032.jpg
* archivo\_22-223.1032.jpg
* archivo\_22-223-1032.jpg
* archivo\_22-223\_1032.jpg

Los siguientes nombres de archivo no se importarán como una secuencia de imágenes porque no están estructurados correctamente:

* archivo\_22-2232032.jpg
* archivo\_22-223PM2032.jpg
* archivo\_22-223-0032.jpg
* file\_22-223\_Rec2020.jpg

La coincidencia de nombre de archivo se basa en la siguiente expresión regular:

```
 ^(.+?)[\.\-\_](?
```


## Cómo usar secuencias de imágenes

Las secuencias de imágenes se pueden cargar en cualquier ranura de recurso de la interfaz, como cualquier otro recurso. Sin embargo, en algunos casos pueden requerir ajustes adicionales para usarse correctamente.

En [Capas de relleno](../../painting/fill-projections/fill-projections.md) (y efectos de relleno), asegúrese de que el modo de proyección esté establecido en **Relleno (coincidencia por Mosaico de UV)** para garantizar que cada imagen de la secuencia esté asignada al [Mosaico de UV](uv-tiles.md) derecho en el conjunto de texturas.
