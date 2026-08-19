---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/physical-size.html"
breadcrumb-title: ''
description: Aprende a configurar el tamaño físico en Substance 3D Painter para definir dimensiones del mundo real para aplicar una escala de textura precisa.
helpx_creative_field: ""
helpx_description: Painter > Features > Physical size
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tamaño físico
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 2%

---


# Tamaño físico

![](../assets/banner-physicalsize-2.png)

El tamaño físico es una propiedad dentro de los materiales Substance que define su tamaño real. Puede utilizarse para hacer coincidir con precisión el tamaño y aspecto de los materiales en superficies 3D. Painter utiliza centímetros como unidad interna predeterminada.

Para utilizar tamaño físico, aplique un material que tenga esta propiedad con un valor distinto de 0,0,0 y, a continuación, active el modo tamaño físico en la capa de relleno (o efecto) en Transformación UV > Escala.

Para obtener más información, consulte:

* <b>Parámetros de Tamaño físico</b> en [Proyecciones de relleno](../painting/fill-projections/fill-projections.md)
* Parámetros de <b>cuadrícula</b> en [configuración de ventana gráfica](../interface/display-settings/viewport-settings.md)
* <b>Desplazamiento basado en tamaño físico</b> en [configuración del sombreador](../interface/shader-settings/shader-settings.md)

>[!NOTE]
>
> * A partir de la versión 8.3 de Painter, tamaño físico está disponible para todos los tipos de proyecciones.
> * La mayoría de los formatos de archivo de malla especifican la unidad utilizada durante la creación de la malla; esta unidad se convertirá a centímetros automáticamente durante la importación.
> * Algunos formatos, como .obj, no tienen información de unidades, por lo que cuando se crea un proyecto mediante una malla .obj, se mide en centímetros de forma predeterminada sin ninguna conversión.
