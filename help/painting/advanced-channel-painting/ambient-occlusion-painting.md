---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/ambient-occlusion-painting.html"
breadcrumb-title: ''
description: Aprende a pintar mapas de oclusión de ambiente directamente en Substance 3D Painter para añadir sombras y profundidades realistas a las texturas.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Ambient Occlusion Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pintura de Oclusión ambiental
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Pintura de Oclusión ambiental

El canal de oclusión ambiental permite pintar detalles en las sombras ambientales de un objeto. Se puede utilizar para añadir detalles del AO procedentes de materiales o simplemente para corregir errores de cocción manual cuando sea necesario.

>> 

En los gráficos de ordenador, la oclusión de ambiente es una técnica de sombreado y de procesamiento que se utiliza para calcular la exposición de cada punto de una escena a la luz de ambiente. El interior de un tubo suele estar más ocluido (y, por lo tanto, más oscuro) que las superficies exteriores expuestas, y cuanto más profundo sea el interior del tubo, más ocluida (y más oscura) será la iluminación. La oclusión ambiental se puede ver como un valor de accesibilidad que se calcula para cada punto de superficie.\
Fuente: &lt;https://en.wikipedia.org/wiki/Ambient_occlusion>

El **resultado** de este cálculo se almacena en un mapa de bits denominado &quot;Oclusión ambiente&quot;. Este mapa se puede hornear directamente en la aplicación, consulte: [Horneado](../../baking/baking.md).

## Pintar Oclusión ambiental

Para pintar detalles de oclusión personalizados, se requiere un canal de Oclusión ambiental. Se puede agregar a través de la [configuración del conjunto de texturas](../../interface/texture-set/texture-set-settings.md):

![](../../assets/add-ao-channel.png)

Una vez que el canal se ha añadido a un conjunto de texturas, se puede utilizar cualquier capa para pintar nueva información. Dado que el canal AO solo contiene información en escala de grises, se recomienda el modo de fusión **Normal** (pintar encima) y **Multiplicar** (combinar).

Para obtener más información sobre ellos y cómo cambiarlos por canal, consulte: [Modos de fusión](../../interface/layer-stack/blending-modes.md).

## Pintar sobre el mapa adicional de la Oclusión ambiental

En algunas situaciones, puede ser útil pintar sobre la Oclusión de ambiente al horno para ocultar detalles o incluso corregir problemas de horneado.

La configuración predeterminada de un proyecto en Substance 3D Painter combinará la Oclusión ambiental **channel** con el mapa de Oclusión ambiental de **mapas adicionales** . Esto significa que pintar sobre el mapa adicional al horno no es posible por defecto, los resultados de cada mapa (los mapas con bake y los canales) se multiplicarán juntos. Sin embargo, esto se puede cambiar con la siguiente configuración:

### 1 - Añadir un canal de Oclusión ambiental

Añadir un canal de oclusión de ambiente en el conjunto de texturas actual :\
![](../../assets/edit-ao-channel-optimized.gif)

Establezca su modo de mezcla en &quot;**replace**&quot; en lugar de &quot;**multiply**&quot; :\
![](../../assets/ao-mix-mode.gif)

### 2 - Configuración de una capa de relleno con la oclusión de ambiente horneada

Cree una nueva capa de relleno y coloque la oclusión de ambiente horneada dentro de la ranura &quot;oclusión de ambiente&quot;, a través del panel Propiedades. No olvide cambiar el segmentado predeterminado de la capa de relleno si aún no está establecida en 1.\
![](../../assets/ao-stack.png)

### 3 - Cambio del modo de fusión de la capa de relleno

De forma predeterminada, el modo de fusión del canal AO en cualquier capa nueva está establecido en &quot;**Multiply**&quot;. Como es preferible usar la capa de relleno como base, elegimos el modo de fusión &quot;normal&quot; ya que el mapa de bits no tiene ningún alfa, reemplazará todo lo que hay debajo (incluido el color predeterminado del sombreado).\
![](../../assets/ao-blend-mode.gif)

### 4 - Creación de una capa para pintar sobre el mapa de oclusión ambiente horneado

Cree una nueva capa (normal o de relleno) y cambie su modo de fusión a &quot;normal&quot; para el canal de AO. Una vez realizada esta configuración, cualquier cosa pintada en el canal AO se hará cargo del mapa de AO horneado que se encuentra en la capa inferior.\
![](../../assets/paint-over-ao-optimized.gif)
