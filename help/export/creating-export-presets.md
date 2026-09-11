---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/getting-started/export/creating-export-presets.html"
breadcrumb-title: ''
description: Aprenda a crear plantillas de salida personalizadas en Substance 3D Painter para definir sus propias configuraciones de exportación de texturas.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Creating Output templates
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Creación de Plantillas de salida
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---


# Crear Plantillas de salida

En esta página se explica cómo crear y modificar Plantillas de salida personalizadas. Las plantillas de salida controlan la denominación y la configuración de las texturas exportadas. La creación de una Plantilla de salida personalizada le permite configurar sus exportaciones para que se ajusten perfectamente a su flujo de trabajo.

La ficha de configuración de la ventana de exportación se divide en tres partes principales:

* <b>Lista de ajustes preestablecidos:</b> (izquierda) permite elegir qué plantilla editar o duplicar y cambiar el nombre de las plantillas existentes.
* <b>Lista de texturas de salida</b>: (centro) muestra el contenido de un ajuste preestablecido seleccionado y muestra la convención de nomenclatura y las opciones de empaquetado de canal.
* <b>Lista de canales</b> y <b>texturas convertidas</b>: (derecha) lista de canales y texturas que se pueden utilizar para componer el contenido de una textura exportada.

![](../assets/image2018-4-25-13-36-44.png){width="800px"}

>[!NOTE]
>
> Las plantillas de salida se guardan en el disco como <b>archivos individuales</b> y se pueden compartir con cualquier otro usuario de Substance 3D Painter.\
> Puedes encontrar los archivos locales de las plantillas personalizadas que hayas creado en la carpeta assets/export-presets de tus [archivos de Substance 3D Painter](../pipeline-and-integration/resource-management/shelf-and-assets-location.md).

>[!NOTE]
>
> Cuando se utiliza una plantilla para exportar texturas, el archivo de plantilla se incluye automáticamente en el archivo de proyecto en guardados posteriores.\
> Esto permite compartir o mover un proyecto a otro equipo mientras se mantienen las plantillas para exportar las texturas.\
> Solo se guarda en el proyecto el último ajuste preestablecido utilizado. Sin embargo, si Substance 3D Painter detecta un ajuste preestablecido con el mismo nombre, el ajuste preestablecido dentro del proyecto se marcará como &quot;Desactualizado&quot; en la lista.

## Creación de una plantilla

En la parte superior de la lista de ajustes preestablecidos, hay tres botones:

![](../assets/image2018-4-25-13-39-6.png)

* <b> Duplicado</b> : duplicar una plantilla existente.
* <b> Quitar</b> : eliminar cualquier plantilla seleccionada.
* <b> Crear</b> : cree una plantilla nueva y vacía.

También puede hacer doble clic en una plantilla o <b>hacer clic con el botón derecho > cambiar nombre</b> para cambiar el nombre de una plantilla.

## Creación de mapas de salida

Una vez seleccionada una plantilla, es posible añadir nuevos mapas de salida mediante los botones dedicados, que están disponibles en la parte superior de la sección central de la ventana.

![](../assets/output-buttons.png)

![](../assets/output-map.gif)

Una vez creado un mapa, es posible asignarle un nombre y, a continuación, arrastrar y soltar mapas de entrada en una de las ranuras de canal disponibles.\
Una vez colocado un mapa de entrada en la sección de mapas de salida, se abrirá un menú preguntando qué tipo de contenido se va a cargar en esa ranura.

Las opciones van desde <b>RGB</b> y <b>canales individuales</b> hasta <b>Alpha</b> y la conversión de la entrada en <b>escala de grises</b>.

>[!NOTE]
>
> Cada vez que se arrastra y suelta un mapa de entrada, se genera un color aleatorio. Esto proporciona una señal visual para los canales y el mapa de entrada correspondiente que se carga.\
> El botón también indica lo que se carga en la ranura:
> 
> * Color de fondo: indica qué asignaciones de <b>input</b> están cargadas.
> * Barra del RGB: Indica que se han cargado los canales <b>R</b>, <b>G</b> y <b>B</b> del mapa de entrada.
> * Barra roja: indica que el canal <b>red</b> del mapa de entrada está cargado.
> * Barra verde : indica que el canal <b>green</b> del mapa de entrada está cargado.
> * Barra azul: indica que el canal <b>blue</b> del mapa de entrada está cargado.
> * Barra gris: Indica que la asignación de entrada se carga como <b>escala de grises</b> (desde un RGB a una conversión de escala de grises o porque la entrada ya está en escala de grises).
> * Línea blanca/negra: indica que se ha cargado el canal <b>alfa</b> del mapa de entrada. En Substance 3D Painter, el alfa de una entrada corresponde al área total pintada.

## Asignación de nombres de salida

![](../assets/output-name.gif)

Algunos indicadores están disponibles para generar automáticamente el nombre de la textura durante el proceso de exportación.

* <b> $mesh</b> : nombre del archivo de malla cargado en el proyecto
* <b> $textureSet</b> : nombre del conjunto de texturas
* <b> /</b> (barra diagonal): separación de carpetas

<b> Ejemplo</b> : cymourai.fbx con un conjunto de texturas denominado &quot;MaterialBase&quot;

* <b>$mesh\_$textureSet\_BaseColor</b> generará <b>cymourai\_MaterialBase\_BaseColor.png.</b>
* <b>$mesh/$textureSet\_BaseColor</b> generará una carpeta denominada <b>cymourai</b> con una textura denominada <b>MaterialBase\_BaseColor.png</b> dentro de ella.

>[!NOTE]
>
> Las carpetas se convierten automáticamente como grupos en caso de que el formato de exportación esté establecido como formato de archivo **PSD** (Photoshop).

## Asignación de canales a mapas de salida

![](../assets/empty-channel.gif)

Es posible dejar algunos canales (del mapa de salida) totalmente vacíos. En este caso, se asignará un color predeterminado.

>[!NOTE]
>
> Si una ranura hace referencia a un canal que no está presente en el conjunto de texturas durante la exportación, también se generará un color predeterminado.\
> Este color cambia en función del canal que ofrezca el mejor valor neutro.\
>  **Ejemplo**: Si falta, el canal de height se generará con un valor de gris predeterminado.

Hay diferentes tipos de mapas:

* <b>Mapas de entrada</b>: canales directos que se pueden añadir en un conjunto de texturas. Mediante el panel de configuración TextureSet.
* <b> Mapas de malla</b>: Texturas presentes en las ranuras de mapa adicionales de un conjunto de texturas (texturas hechas un bake).
* <b> Mapas convertidos:</b> texturas virtuales, estas se generan durante la exportación en función de los canales presentes en el documento.
  * <b>OpenGL de normal/DirectX</b>: Produce una normal en el espacio dedicado combinando la normal de los mapas adicionales, el height y el canal normal.
  * <b>OA mixta</b>: Combine el mapa de Oclusión ambiental adicional con el canal de Oclusión ambiental.
  * <b>Difuso</b>: Color de Difuso generado a partir de los canales BaseColor y Metálico (las partes metálicas se sustituirán por un color negro).
  * <b>Specular</b>: Color de specular generado a partir de los canales BaseColor y Metallic.
  * <b>Brillo</b>: Inverso del canal de rugosidad.
  * <b>Unity4 Difuso</b>: Color de Difuso generado desde BaseColor para que coincida con los sombreadores Unity4.
  * <b>Brillo Unity4</b>: Brillo generado a partir del canal Rugosidad y Metálico para que coincida con los sombreadores Unity4.
  * <b>Reflejo</b>: Exportar un mapa donde el blanco indique un material dieléctrico y otros colores para materiales metálicos
  * <b>1/o</b>: 1 dividido por el valor ior, ior se genera a partir del mapa metálico : 1,4 para dieléctricos, 100 para metales (color negro)
  * <b>Brillo<sup>2</sup></b>: Versión cuadrada del canal de brillo (Brillo \* Brillo)
  * <b>f0</b>: Valor de reflectancia en fresnel 0 (0,04 para dieléctricos, 1,0 para metálicos)
