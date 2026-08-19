---
title: Versión 12.0
description: ''
helpx_description: "Substance 3D Painter"
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/release-notes/version-12-0.html"
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---


# Versión 12.0

<b>Substance 3D Painter 12.0</b> ofrece acoplamiento de texturas directamente en la pila de capas, un nuevo modo automático para la proyección de deformación, un conjunto renovado de efectos de procesamiento posterior y un flujo de trabajo mejorado de creación y configuración de proyectos.

Fecha de publicación: <b>9 de marzo de 2026</b>

>[!NOTE]
>
> En esta versión, se ha mejorado la compatibilidad de las <b>GPU integradas</b> con <b>memoria unificada/compartida</b>. Cabe esperar una mejor detección de la memoria de vídeo, lo que se traduciría en un mejor rendimiento y menos problemas gráficos.

## Funciones principales

### Nuevo acoplamiento de CAPAS

![](../assets/v12_banner_flatten.jpg)

Ahora hay disponible una nueva acción <b>Acoplar</b> en el menú contextual del botón derecho de la pila de capas. Se pueden combinar varias capas rápidamente agrupándolas (<b>Ctrl/Cmd + G</b>) y creando una copia acoplada (<b>Ctrl/Cmd + M</b>). El grupo de origen se deshabilita automáticamente, lo que deja la opción de eliminarlo o, alternativamente, guardarlo como <b>Material inteligente</b> para su posterior edición.

Los elementos acoplados de la pila de capas también se pueden exportar directamente al disco para iteraciones rápidas en otras aplicaciones. Los grupos, las capas o las máscaras se pueden exportar de forma individual o por lotes mediante el menú contextual de la pila de capas.

* <b>Acoplar texturas directamente en la pila de capas</b>\
  Cualquier grupo se puede acoplar pulsando <b>Ctrl/Cmd + M</b> o seleccionando la entrada <b>Acoplar grupo</b> en el menú contextual del botón derecho. Esto genera una copia combinada del contenido seleccionado mientras se deshabilita automáticamente el grupo de origen, manteniendo las capas originales intactas hasta que se tome la decisión de eliminarlas o restaurarlas.

  ![](../assets/v12_flatten_menu.jpg)
* <b>Acoplar y exportar texturas al disco</b>\
  Una acción de exportación dedicada en el menú que se muestra al hacer clic con el botón derecho copia el resultado acoplado de una capa, máscara o grupo y lo guarda directamente en el disco. Esto resulta útil para transferir contenido horneado a otras aplicaciones sin tener que pasar por la canalización de exportación de texturas completa.
* <b>Operaciones por lotes</b>\
  Es posible seleccionar varias capas, grupos o máscaras a la vez y acoplarlas o exportarlas individualmente en una sola operación, lo que hace más eficiente procesar grandes porciones de una pila de capas en un solo paso.

  ![](../assets/v12_flatten_batch.jpg)

>[!NOTE]
>
> Encontrará más información sobre el acoplado de capas en la [página de documentación dedicada](../interface/layer-stack/flatten-layers.md).

### Nuevo modo de deformación a geometría para proyecciones

![](../assets/v12_banner_warp_auto.jpg)

Las pegatinas ahora se pueden adaptar automáticamente a superficies complejas, lo que reduce la necesidad de ajustes manuales. El selector <b>Deformar en geometría</b> está disponible en la barra de herramientas contextual mientras la proyección de deformación está activa.

* <b>Nuevo parámetro en la barra de herramientas contextual</b>\
  Siempre que el modo de proyección Deformar esté activo, estará disponible un nuevo conmutador <b>Deformar en geometría</b> en la barra de herramientas contextual. Se puede desactivar en cualquier momento sin restablecer la configuración de proyección actual.

  ![](../assets/v12_warp_toolbar.png)
* <b>Ajuste automático a la superficie de malla</b>\
  Cuando está activada, la proyección de deformación sigue automáticamente la curvatura y la topología de la malla subyacente. Si arrastra la proyección por la superficie, se ajustará suavemente a la geometría, lo que reduce significativamente la cantidad de ajuste manual necesario al colocar pegatinas en formas complejas o curvas.

  ![](../assets/v12_warp_to_geometry.gif)
* <b>Conservación de deformaciones locales</b>\
  Al editar los vértices de la cuadrícula de proyección de deformación, la deformación en modo de geometría intentará conservar la deformación predefinida para garantizar que siempre se proyecta la misma forma.

  ![](../assets/v12_warp_to_geometry_deformed.gif)

>[!NOTE]
>
> Para obtener más información sobre la proyección de deformación, consulte la [página de documentación dedicada](../painting/fill-projections/warp-projection.md).

### Nuevos efectos de publicación

![](../assets/v12_banner_post_effects2.jpg)

Los procesamientos dentro de Painter ahora se pueden mejorar con un nuevo conjunto de efectos de posprocesamiento disponibles en la ventana <b>Configuración de visualización</b>. Ahora hay nuevas adiciones, como <b>Destello de lente</b> y <b>Película granulada</b>, además de <b>Profundidad de campo</b> y efectos de <b>Resplandor</b> mejorados, entre muchos otros.

A continuación se muestra un ejemplo de lo que puede lograr con los nuevos efectos:

![](../assets/v12_render_withpost.jpg)

* <b>Nuevos efectos de posprocesamiento</b>\
  Todos los efectos de procesamiento posterior se pueden habilitar y configurar individualmente desde la ventana <b>Configuración de visualización</b>. Los efectos se aplican en orden de pila y cada uno se puede activar o desactivar de forma independiente, lo que facilita la combinación y la experimentación con resultados diferentes.

  ![](../assets/v12_display_settings_post_effects.png)
* <b>Nueva lista de efectos:</b>

  * <b>Profundidad del campo</b>: Desenfoca objetos fuera del rango focal para simular el enfoque de la lente de la cámara.
  * <b>Bloom</b>: Añade un resplandor suave que emana de las áreas brillantes de la imagen.
  * <b>Destello</b>: Crea rayas de luz alrededor de las fuentes de luz.
  * <b>Destello de lente</b>: Simula los reflejos ópticos del objetivo cuando una luz brillante brilla en la cámara.
  * <b>Aberración lateral</b>: Simula el halo cromático en los bordes de la imagen causado por las imperfecciones de la lente.
  * <b>Viñeta</b>: Oscurece las esquinas y los bordes del fotograma para enfocar hacia el centro.
  * <b>Perfilar</b>: Aumenta el contraste de los bordes para que la imagen procesada parezca más nítida.
  * <b>Película granulada</b>: Superpone ruido sutil para replicar la textura de la película analógica.
  * <b>Asignación de tonos</b>: Reasigna los valores de luminancia HDR a un rango visible para obtener un aspecto más cinematográfico.
  * <b>Corrección de color</b>: Ajusta el contraste, la saturación, el brillo y la temperatura para ajustar el equilibrio de color general.

>[!NOTE]
>
> Para obtener más información sobre los nuevos efectos, consulta la [documentación dedicada](../features/post-processing/post-processing.md).

### Se ha mejorado el nuevo proyecto y la ventana de configuración

![](../assets/v12_banner_project_window.jpg)

La nueva ventana del proyecto y el cuadro de diálogo de configuración del proyecto se han rediseñado para facilitar la navegación. Los parámetros se han reordenado y agrupado para facilitar su lectura, y el flujo de trabajo de reimportación de mallas se ha mejorado para reducir los pasos repetitivos al iterar en un proyecto.

* <b>Ventana de nuevo proyecto mejorada</b>\
  Los parámetros de la nueva ventana de proyecto se han reorganizado y reordenado para que los ajustes más utilizados ocupen un lugar más destacado. El diseño general ahora es más fácil de analizar, lo que reduce el tiempo necesario para configurar un nuevo proyecto.
* <b>Nuevo flujo de trabajo para volver a importar mallas en la configuración del proyecto</b>\
  Una nueva casilla de verificación <b>Reimportar malla</b> en la configuración del proyecto permite volver a importar la malla del proyecto más fácilmente gracias a la ruta de archivo del archivo cargado anteriormente que ahora se guarda y se rellena previamente automáticamente.

  ![](../assets/v12_project_settings.png)

## Notas de la versión

## Versión 12

### 12.0.0

Fecha de publicación: <b>2026/03/09</b>\
Resumen: <b>Esta es una versión principal. Esta versión contiene las funciones de acoplar capas, deformar en geometría, nuevos efectos posteriores, mejoras en la nueva ventana de proyecto y otras mejoras.</b>

<b>Agregado</b>:

* [Acoplar capas] Acoplar capas dentro de la pila de capas
* [Acoplar capas] Exportar capas acopladas a un disco
* [Deformar en geometría] Añadir nueva función de deformación automática a las proyecciones de deformación
* [Efectos posteriores] Reemplace los efectos posteriores por la adición de otros nuevos
* [Post-effects] Actualizar el asignador de tonos
* [Post-effects] Añadir nuevo uso para recursos Post-effects
* [Contenido]&#x200B;[Efectos posteriores] Integrar activos de efectos posteriores predeterminados en la biblioteca
* [Nuevo proyecto] Mejora de la interfaz de usuario para la creación de proyectos
* [Nuevo proyecto] Cambios en la función de reimportación de mallas
* [Nuevo proyecto] Permitir la apertura de archivos \*.geo.usd
* [Configuración del proyecto] Mejorar la interfaz de usuario para la configuración del proyecto
* Actualizar la biblioteca USD a la versión 25.05
* Actualizar Substance Engine a la versión 9.3.4
* Aumentar controladores mínimos a 25.3.1/25.Q2 para las GPU AMD
* Actualizar Qt a 6.8.6
* [Scripting] Actualice la API de JavaScript a la versión 1.1.20
* Actualizar Python a 3.13

<b>Corregido:</b>

* [Bloqueo] Cambiar una salida de canal de material en una máscara puede bloquearse
* [Importar] Las texturas EXR se fuerzan en sRGB en lugar de lineales al importar archivos USD
* [UV Tiles] La secuencia de imágenes con una sola imagen también llena otros UV Tiles
* [Banca] El AO es diferente entre la CPU y la GPU
* [Gestión de color] [MacOS] Viewport BaseColor no coincide con el selector de color
* [USD] En algunos casos, los valores uniformes no se importan
