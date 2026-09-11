---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/release-notes/old-versions/version-7-3.html"
breadcrumb-title: ''
description: Consulte las notas de la versión 7.3 de Substance 3D Painter para obtener más información sobre las nuevas funciones, mejoras y correcciones de errores.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 7.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versión 7.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1822'
ht-degree: 0%

---


# Versión 7.3

**Substance 3D Painter 7.3** ofrece nuevas formas de texturizar las mallas con las nuevas proyecciones de deformación y cilindro para las capas de relleno.

Fecha de publicación: *13 de octubre de 2021*

## Funciones principales

### Nueva proyección de deformación

![](../../assets/proj-warp.jpg)

Esta versión presenta la nueva proyección de deformación 3D para capas de relleno y efectos de relleno. Esta proyección permite distorsionar una textura o una imagen con la ayuda de una cuadrícula de deformación y puntos controlables.

* **Configuración rápida mediante arrastrar y soltar** Elige un material, un alfa, una textura o un procedimiento de la biblioteca de activos, arrastra y suelta en la parte deseada de la malla (se requiere el método abreviado **ALT** para los materiales). Si el activo no es un material, aparece un mensaje emergente con información sobre el canal al que desea asignarlo.\
  Una vez creada la capa, verás que la nueva *proyección de deformación* se selecciona automáticamente. La capa tiene controles de modo de proyección 3D estándar, pero también un nuevo parámetro *Profundidad de proyección* que permite establecer la profundidad de la proyección de deformación (representada por flechas verdes como cola visual).\
  También puede seleccionar este modo de proyección manualmente en cualquier capa de relleno o efecto sin tener que arrastrar y soltar un recurso en la ventana gráfica.

  ![](../../assets/drop-viewport-warp.gif)

* **Colocación automática con la herramienta Superficie** Cuando se crea la nueva capa de deformación, verás que la herramienta Superficie se selecciona automáticamente. Esto le permite mover la imagen para que permanezca en la superficie de la malla en todo momento. Sin embargo, siempre puedes cambiar a cualquiera de los otros manipuladores y ajustar su traslación (método abreviado **W**), rotación (método abreviado **E**) o escala (método abreviado **R**). Para volver a la herramienta Superficie, use el método abreviado **MAYÚS + W**. Al cambiar al modo *Editar vértices*, la herramienta Superficie también es la selección predeterminada y ajusta el movimiento del vértice a la superficie de la malla. Sin embargo, puede reemplazar temporal y rápidamente la herramienta de superficie **manteniendo CTRL**, lo que le permite mover el punto seleccionado en cualquier dirección, no solo en la superficie.

* **Cuadrícula de deformación fácilmente editable** Una vez que se haya colocado la imagen en su totalidad, también es posible editar la cuadrícula de deformación para obtener una mayor precisión y flexibilidad. Para entrar en el modo de edición de cuadrícula, puedes usar el menú de deformación recién agregado o el método abreviado **MAYÚS + V**. Esto permitirá editar los vértices existentes de la cuadrícula.\
  Puede subdividir uniformemente la cuadrícula en su conjunto, pero tenga en cuenta que si previamente ha movido los vértices, se restablecerán a sus posiciones originales. La subdivisión de la cuadrícula se puede realizar mediante el nuevo menú de opciones de deformación.\
  Como alternativa, es posible añadir divisiones colocadas individualmente que permitan tener más detalles solo cuando sea necesario. Para añadir divisiones, seleccione cualquiera de las tres opciones del menú de deformación: transversal, horizontal o vertical. Cuando se selecciona una de ellas, al pasar el cursor sobre la proyección de deformación y hacer clic en cualquier punto dentro de ella, se agregará una nueva división. Esto no alterará la posición de los puntos existentes.

  ![](../../assets/warp-split.gif)
* **Ajuste automático de la orientación del vértice** De forma predeterminada, las tangentes de los vértices individuales se ajustan a la superficie de la malla, lo que significa que siempre estarán orientadas correctamente en relación con la malla, independientemente de dónde se arrastren. Esta opción de tangente automática se puede desactivar a través de un nuevo botón en la barra de herramientas contextual, en cuyo caso la orientación permanecerá fija en todo momento.

  ![](../../assets/warp-tangent-adjustment.gif)

Para obtener más información sobre la configuración y las propiedades de la proyección de deformación, consulte la [página de documentación dedicada](../../painting/fill-projections/warp-projection.md).

### Nueva proyección del cilindro

![](../../assets/cylinder-proj.jpg)

Esta versión añade un método de proyección cilíndrica para capas de relleno y efectos de relleno. La nueva proyección permite ajustar una imagen o textura alrededor de objetos como columnas, pilares o más formas orgánicas como los brazos de un personaje.

* **Ajustar una imagen alrededor de una malla**\
  Puede ajustar fácilmente una imagen alrededor de una superficie cilíndrica mediante una capa de relleno o un efecto de relleno y seleccionando *Proyección cilíndrica* en el menú desplegable Proyección. Si no es necesario repetir la imagen fuera del gizmo de proyección, debe seleccionar *Ninguno* para *Ajuste de UV* y *Recorte de forma* en *Recorte de forma* para asegurarse de que la imagen no se salga de los límites. A continuación, solo tiene que utilizar el manipulador para ajustar la proyección a la posición deseada.

* **Ajustar el ángulo de proyección**\
  Una vez que la imagen esté en su sitio, habrá disponible un nuevo ajuste de ángulo. Este ajuste se puede utilizar para ajustar si la imagen se proyecta en todo su contorno alrededor de la forma cilíndrica o se restringe a un ángulo determinado. No recorta la imagen, sino que reduce su anchura.

  ![](../../assets/cylindrical-angle.gif)

Para obtener más información, consulte la [página de documentación dedicada](../../painting/fill-projections/cylindrical-projection.md).

### Selector de color mejorado

![](../../assets/colorpicker-banner.jpg)

Esta versión incluye varias mejoras de calidad de vida en el selector de color.

* **Nuevo diseño de ventana**\
  La ventana del selector de color mejorada se ha rediseñado para adaptarse a un diseño más vertical, similar a la última versión de Sampler. Se divide en tres secciones: el campo de color principal, que incluye la selección actual y la última, el campo hexadecimal, el cuentagotas y el regulador de tono; la sección de reguladores manuales de RGB/HSV; y las muestras.\
  ![](../../assets/colorpicker.jpg)

* **Nuevos valores de RGB del 0 al 255**\
  Además de migrar las formas existentes de introducir el valor del color, el selector de color mejorado también permite trabajar con valores de RGB de 0 a 255. Esta opción está disponible cuando *Valores de punto flotante* está desactivada en el menú desplegable de la sección de reguladores.

  ![](../../assets/colorpicker-floatingpoints.jpg)
* **Guardando muestras de color**\
  Las muestras de color ahora se pueden guardar en Painter. Una vez seleccionado el color deseado, es posible pulsar el botón más en la sección Muestras del selector de color y el color se almacenará en todas las sesiones y proyectos. Una muestra se puede borrar haciendo clic derecho sobre ella, o alternativamente es posible eliminar todas las muestras de una vez a través del menú desplegable de esta sección. No hay límite en el número de muestras que se pueden guardar.

  ![](../../assets/colorpicker-swatches.gif)
* **La ventana del selector de color permanece abierta**\
  La ventana del selector de color ahora se puede mover y colocar en cualquier lugar, incluso en una pantalla diferente, y permanecerá abierta mientras no haya un cambio de contexto, lo que significa que cuando cambie entre capas de pintura mientras pinta texturas a mano, puede mantener abierta la ventana del selector de color para acceder más fácilmente.

  ![](../../assets/picker-persistent.gif)

* **Cuentagotas más accesible**\
  Ahora, el cuentagotas de selección de color se encuentra directamente junto al campo de color, pero también se puede encontrar en el selector de color. El cuentagotas más accesible conserva todas las funcionalidades anteriores: puede seguir haciendo clic y manteniendo pulsado para seleccionar un color en cualquier lugar de las pantallas. Este cuentagotas expuesto se puede encontrar junto a todos los campos de color en Painter, no solo en los canales de capa.

  ![](../../assets/eyedropper-5.jpg)

Para obtener más información, consulte la [página de documentación dedicada](../../interface/color-picker.md).

### Otras funciones y mejoras

* **Mejoras al arrastrar y soltar activos**\
  Con la introducción de la deformación, la función de pegatina en la que los activos se pueden arrastrar y soltar desde la biblioteca al puerto de visualización, mientras se mantiene la ALT, había sido objeto de algunas modificaciones. Ahora, cuando se crea una pegatina de esta forma, ya no se utiliza la proyección Planar, sino la proyección Deformar. La selección automática de la proyección de deformación debería mejorar la velocidad y la eficiencia de los ajustes de calcomanía en la malla.\
  Además, ahora es posible arrastrar y soltar no solo materiales, sino activos de tipo imagen en la ventana gráfica. Al seleccionar un alfa, una textura o un procedimiento, no es necesario utilizar el modificador ALT. Se puede soltar en la malla, lo que provocaría un menú con la opción de seleccionar si esta imagen se debe usar dentro de una máscara o en cualquiera de los canales de la capa.

  ![](../../assets/improved-decal.gif)

* **Mejora del complemento de guardado automático**\
  El guardado automático ya no se activará durante operaciones más largas o más pesadas, como la recarga, hace un bake o exportación de malla.

* **Mejoras de rendimiento**\
  Se realizaron tareas de mantenimiento y optimización para la manipulación de los reguladores y el rendimiento de la pintura.

* **Nuevas funciones en la API python**\
  La API de Python ha visto algunas adiciones recientes, que permiten volver a cargar mallas, actualizar recursos, así como establecer y consultar la resolución de los Mosaicos de UV a través de scripts.

* **Actualización del motor del Substance 8.3.0**\
  Junto con algunas correcciones y mejoras generales, esta actualización del motor de Substance ahora tiene en cuenta nuevos tipos de gráficos. También es posible comprobar la versión del archivo .sbsar, lo que debería mejorar el uso y la descarga de las versiones de Substance 3D Assets adecuadas.

* **Recibiendo Substance 3D Assets desde el escritorio de CC**\
  Ahora es posible acceder a Substance 3D Assets, como Materiales, Atlas y Calcomanías, desde la aplicación de escritorio de CC. Además, se pueden enviar directamente a la biblioteca de Painter.

## Notas de la versión

### 7.3.0

*(Publicado El 13 De Agosto De 2021)*\
Resumen : **Versión principal. Contiene una nueva proyección de deformación 3D, una nueva proyección cilíndrica, mejoras del selector de color, nuevas funciones en la API de Python y correcciones de errores**

**Agregado:**

* [Proyección] [Deformar] Exponer deformación 3D como un nuevo modo de proyección
* [Proyección] [Deformar] Permitir el modo de pegatina para Alpha, texturas y procedimientos con la función de arrastrar y soltar en la ventana gráfica
* [Proyección] [Deformar] Utilice la proyección de deformación con el método abreviado de pegatina (ALT)
* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Transformar deformación como completa o por vértices
* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Añadir puntos de cuadrícula con opciones de deformación dividida en sentido cruzado, horizontal o vertical
* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Menú específico para acciones de restablecimiento
* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Opción para ajustar automáticamente las tangentes al mover puntos
* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Menú específico para la edición de la cuadrícula (tamaño, restablecimiento, color y tamaño del control)
* [Proyección] [Deformar] Nuevo método abreviado de teclado para cambiar el modo de edición de deformación de vértices completos (MAYÚS+V)
* [Proyección] [Deformar] Haga clic en + Ctrl para cambiar entre la herramienta Superficie y otras herramientas
* [Proyección] [Cilíndrica] Exponer el modo de proyección cilíndrica
* [Proyección]&#x200B;[Barra de herramientas] Configuración del manipulador de grupos (tamaño, pasos de cuadrícula, pasos de ángulo)
* [Selector de color] Nueva interfaz de usuario del selector de color
* [Selector de color] Uso de valores sRGB en widgets de selector de color
* [Selector de color] Permitir guardar y eliminar muestras de color
* [Selector de color] Cuentagotas accesible desde las ranuras normales y de color
* [Selector de color] Permite editar colores dinámicos entre 0 y 255 valores
* [Selector de color] Hacer que el estado de HSV/RGB sea común en toda la aplicación
* [Selector de color] La ventana del selector de color es semipersistente
* [Selector de color] Al pulsar Esc se cierra la ventana del selector de color
* Mejora del rendimiento para la interacción de la interfaz de usuario y la pintura
* [Motor] Actualización a la nueva versión del motor de Substance (8.3.0)
* [Scripting] [Python] Permite volver a cargar la malla del proyecto actual
* [Scripting] [Python] Permitir la actualización de recursos en proyectos
* [Scripting] [Python] Permite establecer y consultar la resolución de los mosaicos UV
* [Interoperabilidad] No disponible para las ediciones Steam y Substance
* [Interoperabilidad] Recibir varios recursos de Bridge

**Corregido:**

* El selector de color no muestra el color correcto
* [Horneado] La lista de conjuntos de texturas no está ordenada correctamente
* [Importación FBX] No se tienen en cuenta las transformaciones de pivote de grupo 3ds Max
* [Substance Engine] Bloqueo al importar SBSAR dañado
* [MacOS] La opción de configuración de proyecto en diferentes idiomas no está presente
* El guardado automático puede congelar Painter durante procesos largos

**Problemas conocidos:**

* [Proyección] [Deformar] La opción Dividir permanece seleccionada después de realizar la división
* [Proyección] [Deformar] El giro no funciona cuando la transformación se establece en espacio de entorno
* [Proyección] [Deformación] Líneas de artefactos entre parches en algunos casos raros
* [Proyección] [UV] El punto de giro se restablece al voltear la proyección
* [Mac M1] Los Materiales inteligentes no se muestran correctamente
* [M1]&#x200B;[Regresión] Las capas de materiales no funcionan
