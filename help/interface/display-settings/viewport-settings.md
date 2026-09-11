---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/display-settings/viewport-settings.html"
breadcrumb-title: ''
description: Aprenda a configurar los ajustes de la ventana gráfica en Substance 3D Painter para personalizar las opciones de visualización y la calidad de procesamiento.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Viewport settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configuración del área de visualización
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 2%

---


# Configuración del área de visualización

Esta sección de **Configuración de visualización** controla varias configuraciones relacionadas con la visualización de la ventana gráfica, como el filtrado de texturas y la malla metálica de malla.

## Filtrado de textura

![](../../assets/texture-filtering.png)

El Filtrado anisotrópico y el Sesgo MipMap permiten controlar la visualización de texturas en la ventana gráfica. Esta configuración no afecta a las texturas directamente y no se aplicará durante la exportación; simplemente perfeccionan el procesamiento en la ventana gráfica. El ajuste Sesgo de MipMap permite forzar el uso de texturas muy nítidas para píxeles que están muy lejos o en ángulos oblicuos, sin embargo, en algunos casos pueden crear patrones Moiré o vibraciones.

Los ajustes predeterminados son un compromiso de calidad y rendimiento y solo se deben cambiar cuando sea realmente necesario.

| *Configuración* | *Descripción* |
| --- | --- |
| **Filtrado Anisotrópico** | El filtrado anisotrópico mejora la calidad de la textura al verla en ángulos oblicuos. Los valores de alta calidad proporcionan un mejor filtrado, pero pueden provocar una pérdida de rendimiento. Esta configuración controla la cantidad de muestras por píxel (spp) que se utiliza para el filtrado:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Deshabilitado</strong> : Sin filtrado</li><li data-preserve-html="true"><strong>Bajo</strong> (2 spp)</li><li data-preserve-html="true"><strong>Medio</strong> (4spp) : Valor predeterminado</li><li data-preserve-html="true"><strong>Alta</strong> (8 spp)</li><li data-preserve-html="true"><strong>Muy alto</strong> (16 spp)</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/quality-anisotropic-filtering.jpg"/></div> |
| **sesgo MipMap** | Desplaza el Nivel de mapa MIP de detalle para mejorar la calidad de la textura. Los valores marcados pueden provocar la pérdida de resultados y texturas irregulares.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>0 - Suave</strong> (rendimiento ligero) : Valor predeterminado</li><li data-preserve-html="true"><strong>1 - Suave medio</strong></li><li data-preserve-html="true"><strong>2 - Agudo</strong></li><li data-preserve-html="true"><strong>3 - Muy nítido</strong> (Rendimiento intensivo)</li></ul>(De 0 a -3) |

## Encuadre de la cámara

![](../../assets/camera-frame.png)

Para obtener más información sobre la administración de cámaras, consulte : [Administración de cámaras](../viewport/camera-management.md)

## Visualización de herramienta

![](../../assets/viewport-tool.png)

| *Configuración* | *Descripción* |
| --- | --- |
| **Ocultar galería de símbolos al pintar** | Al utilizar una galería de símbolos (consulte las propiedades de la herramienta pintura), esta configuración permite ocultarla temporalmente al pintar en la malla. |
| **Opacidad de visualización de galería de símbolos** | Controla la visibilidad de la galería de símbolos sobre la representación de la ventana gráfica cuando no se pinta. |
| **Canal de vista previa de proyección** | Controla el canal del material que se muestra al utilizar la herramienta de proyección. |

## Malla metálica de malla

![](../../assets/viewport-mesh.png)

| *Configuración* | *Descripción* |
| --- | --- |
| **Mostrar malla metálica de malla** | Activar o desactivar la visualización de la malla metálica de malla en la ventana gráfica. |
| **Color de Malla metálica** | Controla el color utilizado para dibujar la malla metálica de malla. |
| **Opacidad de la Malla metálica** | Controla cuánto será visible la malla metálica cuando se dibuje sobre la malla. |

## Visualización de canal

![](../../assets/viewport-channel.png)

>[!NOTE]
>
> La configuración de visualización de canales solo está disponible cuando se usa el modo de vista **canal único**.

| *Configuración* | *Descripción* |
| --- | --- |
| **Mostrar vista individual sin iluminación (sin iluminación)** | Cuando se visualiza en modo de un solo canal, al habilitar este ajuste se eliminará la iluminación y se mostrará el canal como colores planos. Si está desactivada, se aplicará un sombreado al borde de la malla. |
| **Escalar HDR. valores** | Al ver en modo de canal único una textura **HDR.** (como el height), esta configuración escalará los valores totales. Esto resulta útil para ver valores que superen 1 o sean inferiores a -1. El resultado es igual a **Canal dividido por escala**.En el ejemplo siguiente, el canal de height tiene valores de hasta 3. Sin embargo, de forma predeterminada, no se pueden ver a menos que se cambie el valor de escala : <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-hdr.jpg"/></div> |
| **Usar color +/- para HDR. valores** | Esta configuración permite ver más fácilmente la textura de HDR. reemplazando los valores positivos por el primer color y los valores negativos por el segundo color. Los valores neutros (0) son negros.Ejemplo : <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/colored-hdr.jpg"/></div> |
| **Canales de color** | Modifique el modo de visualización de la ventanilla para que solo se visualice individualmente el componente R, G, B o Alpha del canal actual. Este ajuste no está disponible en el modo de visualización de material. Cuando se activa, el nombre del canal de color seleccionado se muestra en la ventana gráfica:  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c1_image" src="../../assets/color-channel.png"/></div>  Valores posibles:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>RGBA</strong> (predeterminado): en Canales de color, muestre todos los componentes con la transparencia.</li><li data-preserve-html="true"><strong>Escala de grises+Alpha</strong> (predeterminado): en el canal Escala de grises, muestre los valores de escala de grises con la transparencia.</li><li data-preserve-html="true"><strong>R</strong>: en los canales de color, solo se muestra el componente rojo.</li><li data-preserve-html="true"><strong>G</strong>: en los canales de color, solo se muestra el componente verde.</li><li data-preserve-html="true"><strong>B</strong>: en los canales de color, solo se muestra el componente azul.</li><li data-preserve-html="true"><strong>Alpha</strong>: en cualquier canal, solo muestra la transparencia de la textura.</li></ul> |

## Cuadrícula

![](../../assets/display-settings-grid.png)

La configuración de cuadrícula permite mostrar y controlar el dibujo de una cuadrícula 3D dentro de la ventana gráfica 3D.

Las divisiones de cuadrícula son automáticas en función del nivel de zoom y ángulo de la cámara actual. La unidad de cuadrícula actual se muestra en la parte inferior izquierda de la ventana gráfica.

| Configuración | Descripción |
| --- | --- |
| **Mostrar cuadrícula** | Si está activada, haga que la cuadrícula sea visible en la ventana gráfica 3D. |
| **Eje** | Defina a lo largo de qué eje está visible la cuadrícula en la ventana gráfica. El valor predeterminado es Y, ya que este es el eje superior de la aplicación. |
| **Color de cuadrícula** | Color de la cuadrícula cuando se dibuja en la ventana gráfica. |
| **Opacidad de cuadrícula** | Opacidad de la cuadrícula en la ventana gráfica. |
