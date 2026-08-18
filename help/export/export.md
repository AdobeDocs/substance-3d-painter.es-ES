---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/getting-started/export.html"
breadcrumb-title: ''
description: Aprenda a exportar texturas de Substance 3D Painter en diversos formatos para utilizarlas en otras aplicaciones y motores de juegos.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exportar
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---


# Exportar

## Exportar texturas

Las texturas se exportan como una colección de mapas de bits. Painter ofrece mucha flexibilidad al exportar texturas gracias a las Plantillas de salida. Las plantillas de salida le permiten controlar aspectos como el nombre de los archivos exportados, cómo se empaquetan las texturas en los canales y el formato y la profundidad de bits de los archivos exportados. Si esto suena intimidante, no se preocupe, Painter incluye docenas de Plantillas de salida predeterminadas que se configuran para aplicaciones y casos de uso 3D de uso común.

Abre la <b>ventana de exportación</b> y comienza a exportar texturas con <b>Archivo > Exportar texturas</b>, o usa el método abreviado de teclado <b>CTRL + MAYÚS + E</b>. Utilice los siguientes vínculos para obtener más información sobre la exportación de texturas:

* [Ventana de exportación](../export/export-window/export-window.md)
* [Plantillas de salida](../export/export-presets/export-presets.md)
* [Modificación o creación de Plantillas de salida](creating-export-presets.md)

### Exportar la malla

Painter puede modificar la malla importada, por ejemplo, generando automáticamente UV. Si ha realizado cambios en la malla en Painter, puede exportar la malla con <b>Archivo > Exportar malla</b>.

Al exportar una malla, tendrá varias opciones:

* <b>Sin desplazamiento/teselación</b>: exporta la malla base sin modificar la geometría en función de los materiales.
  * <b>Aplicar triangulación</b>: Si la malla importada estaba compuesta por cuadrantes o polígonos, puede activar esta opción para exportar la versión triangulada de Painter de la malla. Esto puede ayudar a evitar errores basados en la triangulación visual en caso de que otras aplicaciones se triangulen de forma diferente.
* <b>Con desplazamiento/teselación</b>: Painter vuelve a sellar la malla, agregando más polígonos, y utiliza desplazamiento o height para cambiar la geometría de la superficie de la malla.
  * <b>Actualizar normales de vértice</b>: la modificación de la superficie de la malla puede dar lugar a normales incorrectas de vértices preexistentes. Al activar esta opción, Painter actualizará automáticamente las normales de vértice al valor correcto para la nueva superficie.

![](../assets/export-render.jpg){width="500px"}
