---
title: Filtros
description: Aprenda a utilizar efectos de filtro en Substance 3D Painter para aplicar filtros de procesamiento de imágenes y ajustes de textura.
source-git-commit: 4b8afda243f2969b036efe14588f201177ee3139
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 3%
---

# Filtros

Los efectos de filtro son sustancias que transforman el contenido de una capa o máscara. Con el modo de fusión de Acceso directo, una capa puede modificar los resultados de la pila de capas; el uso de un filtro en una capa con el modo de fusión Acceso directo permite utilizar filtros para modificar la pila de capas en su conjunto.

## ¿Cómo puedo aplicar un filtro?

Según el tipo de filtro, se debe crear un efecto de filtro en el contenido o la máscara de una capa. Hay dos formas de aplicar un filtro:

* El enfoque manual requiere varios pasos para configurar el filtro, pero proporciona un control directo sobre cada paso del proceso.
* El método de arrastrar y soltar le permite añadir un filtro de forma rápida y define automáticamente el modo de fusión para que pase por todos los canales.

### Agregar manualmente un filtro

En el siguiente ejemplo, se aplica un filtro de desenfoque al contenido de una capa, pero se utiliza más comúnmente para aplicar filtros a máscaras :

**1. Agregar un efecto de filtro**

Para empezar, selecciona el contenido de una capa o la máscara de capa y haz clic en el **botón Efecto** (o haz clic con el botón derecho para abrir el menú contextual). Seleccione la opción &quot;**Agregar filtro**&quot; en la lista.

![](../../assets/filters/filter-add-manually.gif)

**2. Seleccione el filtro en la ventana de propiedades**

En el **panel Propiedades**, todavía no se ha seleccionado ningún filtro. Haz clic en el botón de selección Filtro para abrir el estante pequeño y selecciona el filtro deseado. Aquí elegimos el **filtro Desenfocar**.
![](../../assets/filters/filter-select.gif)

>[!NOTE]
>
> Al aplicar un filtro manualmente, recuerde que puede necesitar utilizar el modo de fusión de paso a través si desea que el filtro afecte al contenido de las capas que se encuentran debajo.

## Arrastrar y soltar un filtro desde el estante

Este método solo está diseñado para filtros que deben aplicarse a toda la pila de capas. Establecerá automáticamente todos los [modos de fusión](../../interface/layer-stack/blending-modes.md) del canal. No funciona para aplicar filtros a una máscara.

**1. Abra el área Filtros del estante**

En la estantería, haz clic en la sección &quot;Filtros&quot; de la izquierda.

![](../../assets/shelf-filters.gif)

**2. Arrastre y suelte el filtro**

Selecciona el filtro que quieres usar en la estantería. Arrástralo y suéltalo en tu pila de capas, asegurándote de que se coloca en la ubicación correcta (evita soltarlo en grupos no deseados, por ejemplo).

![](../../assets/filter-dragdrop.gif)

Tenga en cuenta, en el ejemplo anterior, que el filtro soltado ya tiene un modo de fusión de Accesos directos. Esto se aplica a todos los canales del documento.

## Añadir nuevos filtros a Painter

Si tienes nuevos filtros que añadir a Painter, puedes añadirlos tal y como lo harías con los recursos estándar. Solo tienes que arrastrar y soltar el archivo SBSAR en el **panel de Recursos** y podrás gestionar la importación de tus nuevos filtros.

## Crea tus propios filtros

Todos los filtros son Substance, que se pueden crear con Substance 3D Designer. Substance 3D Designer proporciona plantillas para Substance 3D Painter que le ayudarán a comenzar rápidamente.

Para obtener más información, consulte esta página : [Creando efectos personalizados](../../content/creating-custom-effects/creating-custom-effects.md)

## Filtros predeterminados en Painter

### Estándar

* [Desenfoque](filters/standard/blur.md)
* [Dirección de desenfoque](filters/standard/blur-directional.md)
* [Pendiente de desenfoque](filters/standard/blur-slope.md)
* [Ajustar](filters/standard/clamp.md)
* [Equilibrio de color](filters/standard/color-balance.md)
* [Corrección de color](filters/standard/color-correct.md)
* [Luminosidad de contraste](filters/standard/contrast-luminosity.md)
* [Sombra paralela](filters/standard/drop-shadow.md)
* [Color del área de relleno](filters/standard/fill-area-color.md)
* [Máscara de área de relleno](filters/standard/fill-area-mask.md)
* [FXAA (Suavizado)](filters/standard/fxaa-anti-aliasing.md)
* [Resplandor](filters/standard/glow.md)
* [Degradado](filters/standard/gradient.md)
* [Dinámica de degradado](filters/standard/gradient-dynamic.md)
* [Conversión de escala de grises](filters/standard/grayscale-conversion.md)
* [Paso alto](filters/standard/highpass.md)
* [Escaneo de histograma](filters/standard/histogram-scan.md)
* [Desplazamiento del histograma](filters/standard/histogram-shift.md)
* [HSL Perceptiva](filters/standard/hsl-perceptive.md)
* [Invertir](filters/standard/invert.md)
* [Reflejar](filters/standard/mirror.md)
* [Pixelar](filters/standard/pixelate.md)
* [Posterización](filters/standard/posterize.md)
* [Enfocar](filters/standard/sharpen.md)
* [Smoothstep](filters/standard/smoothstep.md)
* [Umbral](filters/standard/threshold.md)
* [Transformar](filters/standard/transform.md)
* [Deformar](filters/standard/warp.md)

### Acabados

* [Acabado mate lineal cepillado](filters/finishes/matfinish-brushed-linear.md)
* [Acabado mate galvanizado](filters/finishes/matfinish-galvanized.md)
* [MatFinish Grainy](filters/finishes/matfinish-grainy.md)
* [Acabado mate pulido](filters/finishes/matfinish-grinded.md)
* [Acabado mate martillado](filters/finishes/matfinish-hammered.md)
* [Círculos perforados de acabado mate](filters/finishes/matfinish-perforated-circles.md)
* [MatFinish recubierto en polvo](filters/finishes/matfinish-powder-coated.md)
* [MatFinish Raw](filters/finishes/matfinish-raw.md)
* [MatFinish Rough](filters/finishes/matfinish-rough.md)

### MatFX

* [Cómic de MatFX](filters/matfx/matfx-comic-book.md)
* [Edge Wear de detalles MatFX](filters/matfx/matfx-detail-edge-wear.md)
* [Daños en el borde MatFX](filters/matfx/matfx-edge-damages.md)
* [MatFX HBAO](filters/matfx/matfx-hbao.md)
* [Pintura al óleo MatFX](filters/matfx/matfx-oil-paint.md)
* [MatFX Peeling Pintura](filters/matfx/matfx-peeling-paint.md)
* [Meteorización del Óxido MatFX](filters/matfx/matfx-rust-weathering.md)
* [Línea de cierre MatFX](filters/matfx/matfx-shut-line.md)
* [MatFX Watercolor](filters/matfx/matfx-watercolor.md)
* [Gotas de agua MatFX](filters/matfx/matfx-water-drops.md)

### Iluminación

* [Entorno de iluminación generado](filters/lighting/baked-lighting-environment.md)
* [Iluminación hecha un bake Estilizada](filters/lighting/baked-lighting-stylized.md)

### Avanzadas

* [Kuwahara anisotrópico](filters/advanced/anisotropic-kuwahara.md)
* [Bisel](filters/advanced/bevel.md)
* [Suavizado de bisel](filters/advanced/bevel-smooth.md)
* [Coincidencia de color](filters/advanced/color-match.md)
* [Distancia direccional](filters/advanced/directional-distance.md)
* [Curva de degradado](filters/advanced/gradient-curve.md)
* [Ajuste de height](filters/advanced/height-adjustments.md)
* [Height a normal](filters/advanced/height-to-normal.md)
* [Contorno de máscara](filters/advanced/mask-outline.md)
* [Validación PBR](filters/advanced/pbr-validate.md)
* [Cuantificar](filters/advanced/quantize.md)
* [Estilización](filters/advanced/stylization.md)
* [Tri-Plano avanzado](filters/advanced/tri-planar-advanced-filter.md)
