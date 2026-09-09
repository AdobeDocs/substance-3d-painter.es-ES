---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/painting/tool-list/path.html'
breadcrumb-title: ''
description: Utilice la herramienta Trazado de Substance 3D Painter para crear y editar trazados con el fin de obtener una textura y una colocación de trazos precisas.
helpx_creative_field: ''
helpx_description: Painting > Path tools list > Path tool
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Introducción a la herramienta Trazado
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6fcf10add7086a0e2a070ee6046c0a261ef1ae34
workflow-type: tm+mt
source-wordcount: '1666'
ht-degree: 0%

---


# Introducción a la herramienta Trazado

![Imagen que muestra la herramienta de trazado usada en una zapatilla](../../assets/v90_banner_path.jpg)

Las **herramientas de trazado** te permiten definir una curva con puntos en la superficie de la malla. Una vez creada la curva, las diferentes herramientas de trazado le permiten crear diferentes efectos a lo largo de la curva.

## Creación de un trazado

Los trazados se pueden crear en capas de pintura y efectos de pintura. Existen dos formas de acceder a la herramienta Trazado:

* **Mediante la interfaz**: vaya a la barra de herramientas de la herramienta en el lado izquierdo y haga clic en el tercer icono de la parte superior.
* **Mediante un método abreviado**: de forma predeterminada, la herramienta no tiene ninguna asignada. Esto se puede cambiar en el menú Ajustes editando el método abreviado &quot;Seleccionar pintura en la herramienta de trazado&quot;.

Una vez seleccionada la herramienta, los puntos se pueden colocar pulsando en la superficie del modelo 3D dentro de la ventana gráfica 3D. Se necesitan al menos dos puntos (o vértices) para crear un trazado.

![Gif que muestra la selección de la herramienta de trazado y la creación de puntos](../../assets/path_create_points.gif)

La herramienta Trazado tiene diferentes modos, que pueden ser similares a las otras herramientas de pintura disponibles en la aplicación:

* Pintura a lo largo del trazado: Dibuje un trazo de pincel normal a lo largo de un trazado definido.
* [Ruta de lazo](ribbon-tool.md): Dibuja una imagen repetida o estirada a lo largo de un trazado.
* [Ruta rellena](filled-path.md): Rellenar el interior de un trazado con un color uniforme.
* Borrar en el trazado: Dibuje un trazo que borre o elimine información a lo largo de un trazado definido.
* Difuminado a lo largo del trazado: Dibuje un trazo que difumine o desenfoque la información a lo largo de un trazado definido.

![Captura de pantalla de la barra de herramientas de la herramienta que muestra los diferentes modos de herramienta de ruta](../../assets/PathTools.png)

Por ejemplo, esta es la herramienta de ruta de acceso en modo **Difuminado** que afecta a otra información de pintura:

![Gif que muestra una herramienta de ruta en modo de difuminado](../../assets/v90_path_smudge.gif)

>[!NOTE]
>
> Las **herramientas de trazado** solo funcionan en el espacio 3D de la superficie de la geometría. Actualmente no se admite la creación de un trazado en espacio UV o como proyección de espacio de pantalla.

### Edición de un trazado

Los puntos de trazado (o vértices) se adhieren automáticamente a la superficie de la malla. Se pueden mover y ajustar en cualquier momento. Es posible añadir nuevos vértices a un trazado existente haciendo clic en cualquier punto de la línea.

* Al pulsar **Escape** o **Enter**, se cerrará la edición de la ruta de acceso.
* Una vez que se salga, al hacer clic en una superficie en blanco de la malla se iniciará un nuevo trazado.
* Al pasar el ratón por encima y hacer clic en un trazado existente, se seleccionará, lo que permite continuar o editar dicho trazado. Los trazados también se pueden volver a seleccionar a través del panel **Trazados** (véase a continuación).

![Gif que muestra la adición de nuevos puntos y el movimiento de puntos existentes en un trazado](../../assets/path_edit_move_points.gif)

Algunas propiedades son específicas de un trazado en su conjunto. Este es el caso de las opciones que se encuentran en la ventana **Propiedades**. Al igual que con un trazo normal (consulte la [documentación de la herramienta Pintura](paint-brush.md)), es posible definir las siguientes propiedades para una ruta:

* **Pincel**
* **Alpha**
* **Material**

La sección **brush** contiene opciones adicionales que solo están disponibles con la herramienta Path:

| **Configuración** | **Descripción** |
| --- | --- |
| **profundidad de proyección** | Determina lo cerca que debe estar el trazado de la superficie de malla para que aparezcan las marcas de pincel. Para ver esta información visual directamente en la ventana gráfica, es posible habilitar **Normals** en la **configuración de visualización de rutas** (ver a continuación). |
| **Eje superior** | Eje utilizado para orientar las marcas de pincel cuando **Seguir ruta** está desactivado.   En algún contexto, tiene más sentido tener todos los sellos alineados a lo largo de un eje/dirección global y no a lo largo del trazado. Por ejemplo, con remaches sobre una superficie metálica. |

Otras propiedades se definen por puntos (vértices) del trazado, como la presión. Para editar un punto específico, simplemente haga clic en él (o utilice la selección rectangular). A continuación, utilice la barra de herramientas contextual para editar los valores de puntos seleccionados.

![Gif que muestra la edición de presión por vértice](../../assets/path_point_pressure_example.gif)

### Control de tangentes

Puede haber ocasiones en las que un trazado suave no sea ideal, ya sea porque no sigue lo mejor de la superficie del modelo 3D o porque no se ajusta a un aspecto específico. Para resolver estos problemas, es posible modificar las tangentes de un vértice determinado. Las tangentes son las direcciones de un punto que controlan cómo se dobla el trazado.

Para cambiar entre tangentes suaves o lineales/rotas, simplemente haga doble clic en un vértice (o utilice el botón dedicado en la barra de herramientas contextual):

![Cuadrícula que muestra cómo controlar las tangentes en un trazado](../../assets/path_break_tangents.gif)

Para controlar de forma más precisa la orientación de las tangentes, utilice el botón Tangentes personalizadas de la barra de herramientas contextual para sustituirlas manualmente:

![Cuadrícula que muestra cómo controlar las tangentes en un trazado](../../assets/path_control_tangents.gif)

Use el método abreviado **ALT** para romper las tangentes mientras se mueve si el punto no estaba ya.

Utilice el método abreviado de teclado **CTRL** para escalar ambas tangentes al mismo tiempo.

>[!NOTE]
>
> Los controles de tangente se definen a lo largo del plan y se alinean con la normal del punto dado del trazado. Esto significa que las tangentes no pueden doblarse en algunas direcciones.

### Barra de herramientas contextual

![Captura de pantalla de la barra de herramientas contextual en modo de ruta](../../assets/path_contextual_toolbar_overview.png)

La **barra de herramientas contextual** cuando la herramienta **Path** está seleccionada proporciona varias configuraciones que permiten controlar la ruta seleccionada actualmente:

<table>
  <tr>
    <th><strong>Parámetro</strong></th>
    <th><strong>Descripción</strong></th>
  </tr>
  <tr>
    <td><strong>Mostrar/ocultar interfaz de ventanilla</strong><br><img src="../../assets/path_contextual_toolbar_showhide.png" alt="Herramienta Trazado mostrar icono Ocultar"/></td>
    <td>Si se activa, los trazados y los vértices superpuestos serán visibles en la ventana gráfica.</td>
  </tr>
  <tr>
    <td><strong>Configuración de la pantalla</strong><br><img src="../../assets/path_contextual_toolbar_display.png" alt="Icono de configuración de visualización de trazado"/></td>
    <td>Controle el aspecto de los comentarios visuales de ruta en la ventana gráfica:<br><ul><li><strong>Tamaño de identificador</strong>: controle el tamaño de los puntos del trazado.</li><li><strong>Ancho de ruta</strong>: controlar el thickness de la línea de trazado.<br></li><li><strong>Color de ruta</strong>: controlar el color de la línea de trazado.<br></li><li><strong>Color de ruta no seleccionado</strong>: controlar el color de los trazados no activos.<br></li><li><strong>Normales</strong>: Si se activa, muestra la dirección de proyección en cada punto de un trazado.<br></li><li><strong>Tangentes</strong>: Si se activa, muestra la dirección de la curva de los puntos de control del trazado.<br></li><li><strong>Dirección de la ruta</strong>: Si está activada, muestre una pequeña flecha al final del trazado para indicar la dirección de pintura. Esto resulta útil para saber cómo se orientarán los sellos dentro del trazo.</li></ul><br><img src="../../assets/path_contextual_toolbar_display_settings.png" alt="Captura de pantalla del panel de configuración de visualización de trayectorias"/></td>
  </tr>
  <tr>
    <td><strong>Invertir dirección de ruta</strong><br><img src="../../assets/path_contextual_toolbar_direction.png" alt="Icono de dirección de ruta inversa"/></td>
    <td>Voltear la dirección del trazado actual. La dirección define la orientación general utilizada para crear pinturas de los sellos dentro del trazo. Invertir el trazado puede ayudar a reorientar el patrón dibujado.</td>
  </tr>
  <tr>
    <td><strong>Alternar esquina / suavizar</strong><br><img src="../../assets/path_contextual_toolbar_smoothcorner.png" alt="Icono de alternar esquina suave"/></td>
    <td>Rompe o alinea la tangente de los vértices seleccionados actualmente, lo que permite cambiar entre una curva suave o lineal.<br><img src="../../assets/path_smooth_corner_demo.png" alt="Captura de pantalla de un trazado con un trazado suave y lineal "/><br><strong>Nota:</strong> El cambio entre el comportamiento de esquina/suavizado también se puede realizar haciendo doble clic en un punto directamente en el trazado.</td>
  </tr>
  <tr>
    <td><strong>Tangentes personalizadas</strong><br><img src="../../assets/path_icon_custom_tangents.png" alt="Icono de la herramienta Trazado para tangentes personalizadas"/></td>
    <td>Si está activado, permite controlar manualmente las tangentes de un punto determinado del trazado.<br><img src="../../assets/paht_cutom_tangents_demo.png" alt="Imagen que muestra tangentes de trazado personalizadas"/></td>
  </tr>
  <tr>
    <td><strong>Abrir/cerrar trazado</strong><br><img src="../../assets/path_contextual_toolbar_close.png" alt="Icono de abrir ruta de cierre"/></td>
    <td>Abra o cierre la ruta actual. Para cerrar un trazado, primero debe seleccionarse uno de los dos puntos finales del trazado actual.<br><img src="../../assets/v90_path_open_close.gif" alt="Gif que muestra un trazado abierto y cerrado"/></td>
  </tr>
  <tr>
    <td><strong>Eliminar vértice</strong><br><img src="../../assets/path_contextual_toolbar_delete.png" alt="Icono de eliminar vértice de ruta"/></td>
    <td>Elimina los vértices seleccionados actualmente en un trazado.</td>
  </tr>
  <tr>
    <td><strong>Simetría</strong><br><img src="../../assets/path_contextual_toolbar_symmetry.png" alt="Icono de la función de simetría"/></td>
    <td>Habilite o deshabilite la simetría para la ruta actual. Consulte la <a href="../symmetry/symmetry.md">documentación de la simetría</a> para obtener más información.<br><img src="../../assets/v90_path_symmetry.gif" alt="Gif que muestra un trazado dibujado en simetría"/></td>
  </tr>
  <tr>
    <td><strong>Ocultar/ignorar geometría excluida</strong><br><img src="../../assets/path_contextual_toolbar_exclude.png" alt="Icono de la función de exclusión de máscara de geometría"/></td>
    <td>Si está activado, realice la pintura de la trayectoria actual a través de la geometría oculta. Consulte la <a href="../../interface/layer-stack/geometry-mask.md">documentación de máscara de geometría</a> para obtener más información.</td>
  </tr>
</table>

### Panel Trazados

![Panel Ruta](../../assets/path_panel_visibility.png)

>[!NOTE]
>
> El panel se oculta cuando la herramienta actual no es la herramienta Trazado o si se selecciona una capa o carpeta de relleno.

Dentro de la ventana gráfica se encuentra el panel **Trazados**, en el que se muestran todos los trazados de la capa o efecto de pintura actualmente seleccionado. Proporciona una forma sencilla de seleccionar y administrar trazados.

Con este panel, es posible:

* Haga doble clic en una ruta para **cambiarle el nombre**.
* **Elimine** una ruta seleccionándola y presionando la tecla Supr.
* **Copiar**/**Pegar**/**Duplicar** una ruta con métodos abreviados de teclado dedicados.
* **Mostrar** u **ocultar** una ruta con el icono de ojo (que controla si la ruta se aplica a la creación de texturas).

Por comodidad, también es posible hacer clic con el botón derecho en un trazado para abrir el menú contextual que ofrece las mismas acciones:

![Menú contextual del panel Trazado](../../assets/path_panel_rightclick_menu_copy_properties.png)

El menú contextual también abre acciones para copiar las propiedades o la posición de un trazado en otro trazado. Esto permite compartir o sincronizar características fácilmente a través de diferentes rutas:

![Gif muestra cómo copiar y pegar propiedades de ruta](../../assets/path_copy_paste_properties.gif)![Gif muestra cómo copiar y pegar posiciones de ruta](../../assets/path_copy_paste_vertices.gif)

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

Al igual que otras herramientas, se pueden crear ajustes preestablecidos para restaurar rápidamente la configuración o los ajustes del pincel. Para ello, solo tienes que hacer clic con el botón derecho en la ventana **Propiedades** y elegir el ajuste preestablecido **Crear herramienta.** Este ajuste preestablecido recién creado cambiará automáticamente a la herramienta Ruta cuando se seleccione en la ventana **Activos**.