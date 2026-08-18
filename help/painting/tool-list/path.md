---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/path.html"
breadcrumb-title: ''
description: Utilice la herramienta Trazado de Substance 3D Painter para crear y editar trazados para una pintura de textura y una colocación de trazos precisas.
helpx_creative_field: ""
helpx_description: Painting > Path tools list > Path tool
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Introducción a la herramienta Trazado
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---


# Introducción a la herramienta Trazado

![Imagen que muestra la herramienta de trazado usada en una zapatilla](../../assets/v90_banner_path.jpg)

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

<b>Audio</b>

Ajusta o añade audio a tu proyecto.


* Ajuste el volumen del vídeo de origen si tiene audio.
* Agregar, quitar o reemplazar un archivo de audio externo.
* Ajuste el volumen del archivo de audio externo.

</td>
<td style="border: 0;" valign="top">

![](../../assets/image_180.png)

</td>
</tr>
</table>

Las <b>herramientas de trazado</b> te permiten definir una curva con puntos en la superficie de la malla. Una vez creada la curva, las diferentes herramientas de trazado le permiten crear diferentes efectos a lo largo de la curva.

## Creación de un trazado

Los trazados se pueden crear en capas de pintura y efectos de pintura. Existen dos formas de acceder a la herramienta Trazado:

* <b>Mediante la interfaz</b>: vaya a la barra de herramientas de la herramienta en el lado izquierdo y haga clic en el tercer icono de la parte superior.
* <b>Mediante un método abreviado de teclado</b>: de forma predeterminada, la herramienta no tiene ninguna asignada. Esto se puede cambiar en el menú Ajustes editando el método abreviado &quot;Seleccionar la herramienta de pintura en el trazado&quot;.

Una vez seleccionada la herramienta, los puntos se pueden colocar pulsando en la superficie del modelo 3D dentro de la ventana gráfica 3D. Se necesitan al menos dos puntos (o vértices) para crear un trazado.

![Gif que muestra la selección de la herramienta de trazado y la creación de puntos](../../assets/path_create_points.gif)

La herramienta Trazado tiene diferentes modos, que pueden ser similares a las otras herramientas de pintura disponibles en la aplicación:

* Pintar a lo largo del trazado: Dibuje un trazo de pincel normal a lo largo de un trazado definido.
* [Ruta de lazo](ribbon-tool.md): Dibuja una imagen extendida o repetida a lo largo de un trazado.
* [Ruta rellena](filled-path.md): Rellene el interior de un trazado con un color uniforme.
* Borrar en el trazado: Dibuje un trazo que borre o elimine información a lo largo de un trazado definido.
* Difuminado a lo largo del trazado: Dibuje un trazo que difumine o desenfoque la información a lo largo de un trazado definido.

![Captura de pantalla de la barra de herramientas de la herramienta que muestra los diferentes modos de herramienta de ruta](../../assets/PathTools.png)

Por ejemplo, esta es la herramienta de ruta de acceso en modo <b>Difuminado</b> que afecta a otra información de pintura:

![Gif que muestra una herramienta de ruta en modo de difuminado](../../assets/v90_path_smudge.gif)

>[!NOTE]
>
> Las <b>herramientas de trazado</b> solo funcionan en el espacio 3D de la superficie de la geometría. Actualmente no se admite la creación de un trazado en espacio UV o como proyección de espacio de pantalla.

### Edición de un trazado

Los puntos de trazado (o vértices) se adhieren automáticamente a la superficie de la malla. Se pueden mover y ajustar en cualquier momento. Es posible añadir nuevos vértices a un trazado existente haciendo clic en cualquier punto de la línea. 

* Al pulsar <b>Escape </b> o <b>Enter </b>, se cerrará la edición de ruta de acceso.
* Una vez que se salga, al hacer clic en una superficie en blanco de la malla se iniciará un nuevo trazado.
* Al pasar el ratón por encima y hacer clic en un trazado existente, se seleccionará, lo que permite continuar o editar dicho trazado. Los trazados también se pueden volver a seleccionar a través del panel <b>Trazados</b> (véase a continuación).

![Gif que muestra la adición de nuevos puntos y el movimiento de puntos existentes en un trazado](../../assets/path_edit_move_points.gif)

Algunas propiedades son específicas de un trazado en su conjunto. Este es el caso de las opciones que se encuentran en la ventana <b>Propiedades </b>. Al igual que con un trazo normal (consulte la [documentación de la herramienta Pintura](paint-brush.md)), es posible definir las siguientes propiedades para un trazado:

* <b>Pincel</b>
* <b>Alpha</b>
* <b>Material</b>

La sección <b>pincel </b> contiene opciones adicionales que solo están disponibles con la herramienta Trazado:

| <b>Configuración</b> | <b>Descripción</b> |
| --- | --- |
| <b>profundidad de proyección</b> | Determina lo cerca que debe estar el trazado de la superficie de malla para que aparezcan las marcas de pincel. Para ver esta información visual directamente en la ventana gráfica, es posible habilitar <b>Normals</b> en la configuración de visualización de <b>Path </b> (ver a continuación). |
| <b>Eje superior</b> | Eje utilizado para orientar las marcas de pincel cuando <b>Seguir ruta</b> está desactivado.   En algún contexto, tiene más sentido tener todos los sellos alineados a lo largo de un eje/dirección global y no a lo largo del trazado. Por ejemplo, con remaches sobre una superficie metálica. |

Otras propiedades se definen por puntos (vértices) del trazado, como la presión. Para editar un punto específico, simplemente haga clic en él (o utilice la selección rectangular). A continuación, utilice la barra de herramientas contextual para editar los valores de puntos seleccionados.

![Gif que muestra la edición de presión por vértice](../../assets/path_point_pressure_example.gif)

### Control de tangentes

Puede haber ocasiones en las que un trazado suave no sea ideal, ya sea porque no sigue lo mejor de la superficie del modelo 3D o porque no se ajusta a un aspecto específico. Para resolver estos problemas, es posible modificar las tangentes de un vértice determinado. Las tangentes son las direcciones de un punto que controlan cómo se dobla el trazado.

Para cambiar entre tangentes suaves o lineales/rotas, simplemente haga doble clic en un vértice (o utilice el botón dedicado en la barra de herramientas contextual):

![Cuadrícula que muestra cómo controlar las tangentes en un trazado](../../assets/path_break_tangents.gif)

Para controlar de forma más precisa la orientación de las tangentes, utilice el botón Tangentes personalizadas de la barra de herramientas contextual para sustituirlas manualmente:

![Cuadrícula que muestra cómo controlar las tangentes en un trazado](../../assets/path_control_tangents.gif)

Usa el método abreviado de teclado <b>ALT</b> para romper las tangentes mientras te mueves si el punto aún no lo estaba.

Utilice el método abreviado de teclado <b>CTRL</b> para escalar ambas tangentes al mismo tiempo.

>[!NOTE]
>
> Los controles de tangente se definen a lo largo del plan y se alinean con la normal del punto dado del trazado. Esto significa que las tangentes no pueden doblarse en algunas direcciones.

### Barra de herramientas contextual

![Captura de pantalla de la barra de herramientas contextual en modo de ruta](../../assets/path_contextual_toolbar_overview.png)

La <b>barra de herramientas contextual</b> cuando la herramienta <b>Path</b> está seleccionada proporciona varias configuraciones que permiten controlar la ruta seleccionada actualmente:

| <b>Parámetro</b> | <b>Descripción</b> |
| --- | --- |
| <b>Mostrar u ocultar la interfaz de la ventana gráfica</b>  <div><img alt="Herramienta Trazado mostrar icono Ocultar" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-1k12728-column-xc227lz_image" src="../../assets/path_contextual_toolbar_showhide.png"/></div> | Si se activa, los trazados y los vértices superpuestos serán visibles en la ventana gráfica. |
| <b>Configuración de pantalla</b>  <div><img alt="Icono de configuración de visualización de trazado" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-uj427cc-column-xc227lz_image" src="../../assets/path_contextual_toolbar_display.png"/></div> | Controle el aspecto de los comentarios visuales de ruta en la ventana gráfica:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Tamaño de identificador</b>: controle el tamaño de los puntos del trazado.</li> <li data-preserve-html="true"><b>Ancho de ruta</b>: controlar el thickness de la línea de ruta de acceso.<br/> </li> <li data-preserve-html="true"><b>Color de ruta</b>: controlar el color de la línea de ruta de acceso.<br/> </li> <li data-preserve-html="true"><b>Color de ruta no seleccionado</b>: controlar el color de las rutas de acceso no activas.<br/> </li> <li data-preserve-html="true"><b>Normales</b>: Si está habilitado, muestre la dirección de proyección en cada punto de un trazado.<br/> </li> <li data-preserve-html="true"><b>Tangentes</b>: Si está habilitado, muestre la dirección de la curva de los puntos de control del trazado.<br/> </li> <li data-preserve-html="true"><b>Dirección de la ruta</b>: Si está activada, muestre una pequeña flecha al final del trazado para indicar la dirección de pintura. Esto resulta útil para saber cómo se orientarán los sellos dentro del trazo.</li> </ul>  <div><img alt="Captura de pantalla del panel de configuración de visualización de trayectorias" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-uj427cc-column-vo327hy_image" src="../../assets/path_contextual_toolbar_display_settings.png"/></div> |
| <b>Invertir la dirección de la ruta</b>  <div><img alt="Icono de dirección de ruta inversa" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-5xb27rp-column-xc227lz_image" src="../../assets/path_contextual_toolbar_direction.png"/></div> | Voltear la dirección del trazado actual. La dirección define la orientación general utilizada para pintar los sellos dentro del trazo. Invertir el trazado puede ayudar a reorientar el patrón dibujado. |
| <b>Alternar esquina / suave</b>  <div><img alt="Icono de alternar esquina suave" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-8wd27al-column-xc227lz_image" src="../../assets/path_contextual_toolbar_smoothcorner.png"/></div> | Romper o alinear la tangente de los vértices seleccionados actualmente, lo que permite cambiar entre una curva suave o lineal.  <div><img alt="Captura de pantalla de un trazado con un trazado suave y lineal " class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-8wd27al-column-vo327hy_image" src="../../assets/path_smooth_corner_demo.png"/></div>  **Nota:** El cambio entre el comportamiento de esquina/suavizado también se puede realizar haciendo doble clic en un punto directamente en el trazado. |
| <b>Tangentes personalizadas</b>  <div><img alt="Icono de la herramienta Trazado para tangentes personalizadas" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-r302zw8-column-xc227lz_image" src="../../assets/path_icon_custom_tangents.png"/></div> | Si está activado, permite controlar manualmente las tangentes de un punto determinado del trazado.  <div><img alt="Imagen que muestra tangentes de trazado personalizadas" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-r302zw8-column-vo327hy_image" src="../../assets/paht_cutom_tangents_demo.png"/></div> |
| <b>Abrir/cerrar ruta</b>  <div><img alt="Icono de abrir ruta de cierre" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-7ve27oq-column-xc227lz_image" src="../../assets/path_contextual_toolbar_close.png"/></div> | Abra o cierre la ruta actual. Para cerrar un trazado, primero debe seleccionarse uno de los dos puntos finales del trazado actual.  <div><img alt="Gif que muestra un trazado abierto y cerrado" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-7ve27oq-column-vo327hy_image" src="../../assets/v90_path_open_close.gif"/></div> |
| <b>Eliminar vértice</b>  <div><img alt="Icono de eliminar vértice de ruta" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-v0f273z-column-xc227lz_image" src="../../assets/path_contextual_toolbar_delete.png"/></div> | Elimina los vértices seleccionados actualmente en un trazado. |
| <b>Simetría</b>  <div><img alt="Icono de función de simetría" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-hkg27qa-column-xc227lz_image" src="../../assets/path_contextual_toolbar_symmetry.png"/></div> | Habilite o deshabilite la simetría para la ruta actual. Consulte la [documentación de simetría](../symmetry/symmetry.md) para obtener más información.  <div><img alt="Gif que muestra un trazado dibujado en simetría" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-hkg27qa-column-vo327hy_image" src="../../assets/v90_path_symmetry.gif"/></div> |
| <b>Ocultar/omitir geometría excluida</b>  <div><img alt="Icono de la función de exclusión de máscara de geometría" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-52h27be-column-xc227lz_image" src="../../assets/path_contextual_toolbar_exclude.png"/></div> | Si está activado, haga que el trazado actual se pinte en la geometría oculta. Consulte la [documentación de máscara de geometría](../../interface/layer-stack/geometry-mask.md) para obtener más información. |

### Panel Trazados

![Panel Ruta](../../assets/path_panel_visibility.png)

>[!NOTE]
>
> El panel se oculta cuando la herramienta actual no es la herramienta Trazado o si se selecciona una capa o carpeta de relleno.

Dentro de la ventana gráfica se encuentra el panel <b>Trazados</b>, en el que se muestran todos los trazados de la capa o efecto de pintura actualmente seleccionado. Proporciona una forma sencilla de seleccionar y administrar trazados.

Con este panel, es posible:

* Haga doble clic en una ruta para <b>cambiarle el nombre</b>.
* <b>Elimine</b> una ruta seleccionándola y presionando la tecla Supr.
* <b>Copiar</b>/<b>Pegar</b>/<b>Duplicar</b> una ruta con métodos abreviados de teclado dedicados.
* <b>Mostrar</b> u <b>ocultar</b> una ruta con el icono de ojo (que controla si la ruta se aplica a la creación de texturas).

Por comodidad, también es posible hacer clic con el botón derecho en un trazado para abrir el menú contextual que ofrece las mismas acciones:

![Menú contextual del panel Trazado](../../assets/path_panel_rightclick_menu_copy_properties.png)

El menú contextual también abre acciones para copiar las propiedades o la posición de un trazado en otro trazado. Esto permite compartir o sincronizar características fácilmente a través de diferentes rutas:

![Gif que muestra cómo copiar y pegar propiedades de ruta](../../assets/path_copy_paste_properties.gif)

![Gif que muestra cómo copiar y pegar posiciones de ruta](../../assets/path_copy_paste_vertices.gif)

>[!NOTE]
>
> Las propiedades de copia y pegado solo funcionan cuando los trazados se basan en la misma herramienta de pintura. Por ejemplo, no es posible compartir propiedades entre un trazado con ajustes de difuminado y otro con ajustes de pincel.

## Herramientas preestablecidas

![Captura de pantalla de la sección de ajustes preestablecidos del panel propiedades cuando se selecciona una herramienta de trazado](../../assets/path_presets.png){width="400px"}

Cuando se selecciona una herramienta de trazado, hay disponible una sección Ajustes preestablecidos en la parte superior del panel Propiedades. Desde aquí, puede acceder rápidamente a los ajustes preestablecidos de las diversas herramientas de trazado.

### Ajustes preestablecidos de ruta favorita

La opción Favoritos de la sección Ajustes preestablecidos solo incluye los ajustes preestablecidos que haya seleccionado para acceder a ellos con mayor rapidez. Para comenzar a agregar favoritos, seleccione Favoritos y, a continuación, &quot;Mostrar ajustes preestablecidos compatibles en recursos&quot; para obtener una lista completa de los ajustes preestablecidos de ruta disponibles.

Para marcar como favorito un ajuste preestablecido, haga clic con el botón derecho en el panel Activos o en la sección Ajustes preestablecidos del panel Propiedades y, a continuación, seleccione &quot;Añadir a favoritos&quot;. 

También puede eliminar los ajustes preestablecidos de la lista de favoritos. Haga clic con el botón derecho en un ajuste preestablecido Favoritos y, a continuación, seleccione &quot;Quitar de favoritos&quot;.

![Captura de pantalla de la sección de ajustes preestablecidos del panel propiedades cuando se selecciona una herramienta de trazado. La opción Favoritos está seleccionada y el botón &quot;Mostrar ajustes preestablecidos compatibles en Recursos&quot; está resaltado.](../../assets/ShowCompatiblePresets.png){width="400px"}

### Creación de ajustes preestablecidos de trazado

Al igual que otras herramientas, se pueden crear ajustes preestablecidos para restaurar rápidamente la configuración o los ajustes del pincel. Para ello, solo tienes que hacer clic con el botón derecho en la ventana <b>Propiedades</b> y elegir el ajuste preestablecido <b>Crear herramienta.</b> Este ajuste preestablecido recién creado cambiará automáticamente a la herramienta Ruta cuando se seleccione en la ventana <b>Activos</b>.
