---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/uv-reprojection.html"
breadcrumb-title: ''
description: Aprenda a utilizar la reproyección UV en Substance 3D Painter para transferir texturas entre diferentes diseños UV.
helpx_creative_field: ""
helpx_description: Painter > Features > UV Reprojection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Reproyección UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Reproyección UV

La reproyección UV es un proceso automático que se produce cuando se cambia la resolución de la textura o se importa una nueva malla.\
Si carga una nueva malla en el documento (a través de la ventana [Configuración del proyecto](https://substance3d.adobe.com/display/draftpainter/project%20configuration) ), todas sus acciones se reproyectarán en esa nueva malla. No importa si la topología ha cambiado (siempre que sea similar) o si los UV han cambiado. Dado que la reproyección funciona recalculando todas las capas y trazos de pincel, puede tardar un poco (especialmente en resoluciones de alta textura).

Pintar en vista 2D

Dado que cada trazo realizado en el Vista 2D se realiza en el espacio UV, no hay forma de reproyectarlo correctamente en caso de que el UV de la malla cambie drásticamente después de una reimportación. La mejor forma de hacer que el proyecto sea reproyectado es utilizar el enmascaramiento mediante un mapa de ID y otro tipo de selección y pintura en lugar del Vista 3D.

## ¿Cómo funciona la reproyección?

Substance 3D Painter guarda sus datos en 3D en el espacio de entorno para que todo no sea destructivo. Esto significa que cuando se reimporta una malla, Substance 3D Painter intenta realizar una pintura donde estaba la malla antes de la reimportación, no tiene forma de saber dónde podrían haberse movido algunas piezas.

Además, cuando Substance 3D Painter importa una malla, calcula su cuadro delimitador para registrar el espacio y definir una escala relativa para las herramientas (pincel de pintura, partículas, etc.). Este cuadro delimitador tiene 1 unidad de ancho en cada eje. Cuando se importa una nueva malla, si se desmarca la opción &quot;conservar trazo&quot;, se vuelve a normalizar el cuadro delimitador a la nueva malla. Por lo tanto, si la malla cambia drásticamente de tamaño, los trazos pueden moverse. Sin embargo, si marca &quot;conservar trazos&quot;, escalamos el cuadro delimitador original al nuevo para volver a proyectar correctamente los trazos de pincel.

>[!WARNING]
>
> El cambio de las unidades de la malla 3D puede provocar que la reproyección UV no funcione; la malla antigua y la nueva, a pesar de que la topología no ha cambiado, se pueden interpretar como escalas muy diferentes. Lo ideal es evitar cambiar la configuración de la unidad, ya que puede ser difícil de arreglar.
