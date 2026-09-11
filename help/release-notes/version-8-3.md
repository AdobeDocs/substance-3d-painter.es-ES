---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/version-8-3.html"
breadcrumb-title: ''
description: Consulte las notas de la versión 8.3 de Substance 3D Painter para obtener más información sobre las nuevas funciones, mejoras y correcciones de errores.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Version 8.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versión 8.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2607'
ht-degree: 0%

---


# Versión 8.3

**Substance 3D Painter 8.3** presenta un nuevo modo de hacer un bake, USD la importación de archivos y la compatibilidad con el tamaño físico en el modo de Proyección de UV.

Fecha de publicación: *10 de enero de 2023*

## Función principal

### Nuevo modo de hacer un bake

![](../assets/banner-baking_1.jpg)

La antigua ventana para hornear se ha sustituido por un modo específico con varias funciones nuevas, en particular con visualización de ventanilla, como la visualización de la jaula y los errores de coincidencia.

* **Acceso y cambio entre modos**\
  El horneado es ahora un modo nuevo e independiente, además de los modos de pintura y representación ya existentes en la aplicación. Para llegar al modo de hacer un bake, solo tiene que usar el icono del pequeño croissant en la barra de herramientas contextual. El cambio entre los modos también se puede hacer de otra manera: mediante el menú modo o los métodos abreviados de teclado. Para volver a otro modo, solo tienes que usar el icono específico del modo (además, el botón **Hacer un bake mapas de malla** dentro de la [configuración del conjunto de texturas](../interface/texture-set/texture-set-settings.md) se puede seguir usando para entrar en el nuevo modo).

  ![](../assets/baking-mode-switch-menu.png)

  ![](../assets/baking-mode-switch-icon.png)

* **Nueva interfaz de modo**\
  La ventana de haga un bake tradicional se ha transformado en un modo con muelles específicos, en particular:

  * **La lista de conjuntos de texturas** se puede usar para definir qué partes del proyecto se harán un bake.
  * **Bakeres de mapa de malla** permite seleccionar entre la configuración común de hacer un bake y la configuración de baker. También es donde se puede especificar qué proceso de panadería se iniciará.
  * **Configuración de mapa de malla** es donde se encuentran todos los ajustes comunes y de baker y se pueden modificar, dependiendo de lo que se haya seleccionado en las dos ventanas anteriores.
  * **Haciendo un bake registro** reagrupa información diferente sobre el proceso de hacer un bake, en particular mensajes de error.
  * **Haciendo un bake visualización**: este panel se encuentra en la ventana gráfica y controla varias opciones relacionadas con la visualización de las mallas de poli altas y bajas.

  ![](../assets/baking-mode-overview.jpg){width="500px"}

* **Iniciar y cancelar el proceso de pandeo directamente desde la ventana gráfica**\
  El botón para iniciar o cancelar el proceso de hacer un bake ahora se encuentra en la parte inferior de la ventana gráfica. También se puede utilizar una pequeña flecha para especificar el modo de hacer un bake: en función de la selección de lista Conjunto de texturas o mediante el conjunto de texturas activo actualmente.

  ![](../assets/baking-button.png)

  ![](../assets/baking-button-cancel.png)

* **Mostrar malla de alta densidad en la ventana gráfica**\
  Al especificar una malla de alta polaridad en los ajustes de hace un bake, ahora también se cargará en la ventana gráfica (a menos que la configuración de visualización dedicada esté desactivada). Esto permite comprobar si la geometría de malla de poli alta y baja coincide bien.

  ![](../assets/low-vs-high.jpg){width="400px"}

* **Mostrar malla de la jaula en la ventana gráfica con áreas perdidas como error**\
  La malla de la jaula también se puede mostrar en la ventana gráfica. Si no se utiliza un fichero de malla dedicado, se mostrará una jaula implícita y reaccionará al parámetro Distancia frontal máxima. Al ajustar el tamaño de la jaula, cualquier parte de la malla de alta densidad que esté fuera de la jaula se mostrará de color rojo por defecto, lo que permite encontrar fácilmente la parte de la malla que se perderá por el proceso de hacer un bake.

  ![](../assets/cage-distance.gif)

* **Observe la malla mientras carga y hace un bake**\
  La carga de mallas y el hago un bake ya no congelan la aplicación, lo que significa que es posible interactuar con la ventana gráfica durante esas operaciones. Esto puede resultar útil para investigar el hago un bake en curso, identificar los problemas con antelación y cancelar el hago un bake, lo que permite ahorrar tiempo al final. Del mismo modo, se hará un bake primero el conjunto de texturas más visible en la ventana gráfica, lo que ayudará a comprobar los resultados en áreas específicas de antemano.

  ![](../assets/interaction-while-baking.gif)

* **Configuración de la ventana gráfica y del material neutro**\
  Para ayudar a centrarse en los resultados de hacer un bake y buscar problemas si los hay, el modo de hacer un bake no muestra texturas pintadas, sino que utiliza un material neutro. Los ajustes de este material neutro se pueden ajustar en el panel de visualización Hacer un bake dentro de la ventana gráfica.

  ![](../assets/neutral-material-demo.gif)

* **Mostrar bordes duros con costuras UV que faltan**\
  Una fuente de defectos al hacer un bake es la presencia de bordes duros que no tienen costuras UV. Esto puede dar lugar a líneas visibles y romper el smoothness de sombreado. Para ello, se ha añadido una configuración de visualización para resaltarlas tanto en 3D como en Vista 2D, ya que de lo contrario son muy fáciles de perder.

  ![](../assets/hard-edge-missing-seams.png){width="450px"}

  ![](../assets/hard-edge-missing-seams-2d.jpg){width="300px"}

* **Sincronizar y dessincronizar parámetros**\
  La nueva acción de sincronización permite especificar qué parte de los ajustes de Hace un bake se sincronizan en los conjuntos de texturas. De lo contrario, sería tedioso configurar varias veces de la misma manera. A veces es útil tener conjuntos de texturas con configuraciones dedicadas y es preferible mantenerlos sin sincronizar. Por ejemplo, mantener separados los ajustes comunes ahora permite utilizar una distancia frontal máxima, una resolución o una lista de mallas de alto contenido de poli que serían diferentes según el conjunto de texturas.

  ![](../assets/sync-icon-1.png){width="400px"}

  ![](../assets/sync-ao-settings.png){width="400px"}

* **Comprobador de coincidencia por nombre**\
  La pestaña **Coincidencia por nombre** en el **Registro de Hace un bake** puede ayudar a encontrar errores en el proceso de coincidencia antes de hacer un bake, lo que facilita notar mallas que no coinciden. Las mallas que coinciden se agrupan juntas, mientras que las demás se aíslan y se muestran en rojo.

  ![](../assets/matching-by-name-log.png){width="450px"}

>[!NOTE]
>
> Hay muchos más ajustes nuevos en este nuevo modo. Para obtener más información, consulte la [página de documentación dedicada](../baking/baking.md).

### Nueva importación y exportación de archivos USD

![](../assets/banner-usd.jpg)

Esta nueva versión agrega la compatibilidad con el formato de archivo [Universal Scene Description (USD)](https://graphics.pixar.com/usd/release/intro.html). Ahora es posible iniciar un proyecto de Painter, exportando mallas y texturas mediante un formato USD, lo que hace que el flujo de trabajo sea más coherente en todas las aplicaciones.

* **Importar USD archivo con variantes, aspectos y en un marco específico**\
  Se puede utilizar un formato de archivo USD al crear un proyecto o volver a importar una malla dentro de un proyecto. USD archivos pueden ser a menudo escenas complejas, por lo que también hay disponibles un selector de ámbito y de variante para importar solo un subconjunto del archivo.

  ![](../assets/usd-import-settings.png){width="400px"}

  ![](../assets/usd-scope-variants.png){width="400px"}

* **Exportar USD como un nuevo archivo o vinculado al USD original utilizado en el proyecto**\
  Cuando el texturizado esté listo, puedes usar la ventana **Archivo > Exportar texturas** para exportar tu archivo USD junto con tus archivos de textura. Simplemente habilite la configuración **Exportar USD recurso** para hacerlo. Esto generará varios archivos USD que se pueden integrar fácilmente en una canalización posteriormente. Si se ha utilizado un fichero que no es USD o un fichero de USD sin UV, se exportará un nuevo fichero de geometría de USD además de los mapas de textura y USD fichero de material.\
  Además, también es posible utilizar **Archivo > Exportar malla** para exportar la geometría del proyecto como un archivo USD.

  ![](../assets/usd-export-textures.png)

  ![](../assets/usd-export-mesh.png){width="400px"}

### Compatibilidad mejorada con el tamaño físico en modo UV

![](../assets/banner-physicalsize-1.jpg)

El soporte de materiales Substance con tamaños físicos incrustados se ha extendido a las proyecciones basadas en UV.

* **Tamaño físico en modo UV**\
  Ahora es posible establecer el modo Escala en Tamaño físico en lugar de Mosaico en la capa de relleno y efectos de relleno mediante el modo Proyección de UV. El tamaño del UV se calcula automáticamente en función del tamaño medio de los triángulos del desenvolvimiento UV.

  ![](../assets/physicalsize-uvmode.png){width="400px"}

* **Cambiar automáticamente al tamaño físico** Se ha agregado una nueva configuración de proyecto para establecer automáticamente la configuración de escala en tamaño físico al crear un material (al arrastrar y soltar un recurso para la ventana Activo, por ejemplo). Esto permite utilizar un tamaño coherente en todo el proyecto sin tener que cambiar la configuración manualmente cada vez que se crea una nueva capa de relleno. Para habilitarla en un proyecto existente, ve a **Editar > Configuración del proyecto** y habilita **Cambiar escala de capa de relleno a Tamaño físico al asignar materiales**. Esta configuración también se puede habilitar al crear un nuevo proyecto.

  ![](../assets/physicalsize-settings.png)

## Información de soporte de plataforma

Con esta versión, hemos aumentado la versión mínima compatible de Painter en Steam a Ubuntu 20.04.

## Tutoriales

Para descubrir y aprender sobre el nuevo modo de Hacer un bake, echa un vistazo a nuestro último tutorial:

## Notas de la versión

*(Lanzado: 10 de enero de 2023)*\
Resumen: **Versión principal con nuevo modo de hacer un bake, nueva importación y exportación de archivos USD y compatibilidad de tamaño físico para la Proyección de UV**

**Agregado:**

* [Modo de Hacer un bake] Nuevo modo de hacer un bake dedicado a hacer un bake el proceso
* [Modo de Hacer un bake] Definir el método abreviado para cambiar al modo de hacer un bake a F8
* [Modo de Haga un bake] Botón Añadir Inicio y Cancelar hacer un bake en la ventana gráfica
* [Modo de Hace un bake] Añadir selección de hace un bake en la lista Conjunto de texturas
* [Modo de Hace un bake] Añada una nueva ventana Bakeres de mapa de malla para seleccionar bakeres
* [Modo de Hace un bake] Añadir nueva ventana Ajustes de mapa de malla para editar los ajustes de hace un bake
* [Modo de Hace un bake] Añadir nueva ventana Hacer un bake registro para seguir el proceso de hace un bake
* [Modo de Hace un bake] Añadir parámetros de hace un bake y acciones de deshacer a la ventana de historial
* [Modo de Hace un bake] Añadir rutas de navegación en Ajustes de mapa de malla
* [Modo de Hace un bake] Añadir miniaturas de mapas de malla en la ventana Bakeres de mapas de malla
* [Modo de Haga un bake] Añadir menú de ajustes de visualización contraíbles en la ventana gráfica 3D
* [Modo de Hace un bake] Añadir ajuste de visualización para mostrar/ocultar la malla de alta densidad
* [Modo de Haga un bake] Añadir ajuste de visualización para mostrar/ocultar la malla de la jaula y la malla metálica
* [Modo de Hace un bake] Añadir ajuste de visualización para mostrar/ocultar la malla de baja densidad
* [Modo de Haga un bake] Añada ajustes de visualización para mostrar bordes duros sin costuras UV como errores
* [Modo de Hace un bake] Informar en la ventanilla sobre los errores de malla y hacer un bake si el registro de Hace un bake no está visible
* [Modo de Hace un bake] Añadir acción para sincronizar la configuración de baker en todos los conjuntos de texturas

  En la ventana Bakeres de mapa de malla, cada baker (así como los ajustes comunes) se pueden sincronizar en los conjuntos de texturas haciendo clic en el icono de enlace junto a su nombre. Esta acción abrirá una ventana que permite seleccionar qué conjuntos de texturas compartirán los mismos parámetros.
* [Modo de Hace un bake] Añadir acciones para copiar y pegar ajustes de baker

  En la ventana Mesh Map Bakers hay disponibles acciones para copiar y pegar cada configuración de panadero en los conjuntos de texturas, ya sea a través del menú dedicado en la parte superior de la ventana o el menú contextual del botón derecho.
* [Modo de cocción] Botón Añadir en el registro de cocción para saltar del error a la configuración correcta

  Cuando un panadero falla o una malla no se carga correctamente, aparece un mensaje de error en el registro de panadería. Un botón junto al mensaje permite cambiar los marcadores de mapa de malla y la ventana Ajustes de mapa de malla para mostrar los ajustes relacionados. Esto ayuda a aislar con mayor facilidad el origen de un problema para poder solucionarlo.
* [Modo de cocción] Añadir menús para gestionar conjuntos de texturas y selecciones de panadero

  En las ventanas &quot;Texture Set list&quot; y &quot;Mesh Map Bakers&quot; se ha añadido un pequeño menú de acción para ayudar a copiar e invertir las selecciones.
* [Modo de cocción] Dividir la lista de selección de panadero por conjunto de texturas
* [Modo de cocción] Dividir ajustes comunes por conjunto de texturas
* [Modo de cocción] Cargar mallas de alta polietileno y jaula sin congelar la interfaz
* [Modo de cocción] Utilice la barra de progreso de la ventanilla para mostrar la carga de la malla
* [Modo de cocción] Añadir estado de carga de malla en el registro de cocción
* [Modo de cocción] Permitir girar la malla en la ventanilla durante la cocción
* [Modo de cocción] Establecer el orden de cocción en función de la visibilidad actual de la ventana gráfica de la malla
* [Modo de cocción] Visualización de la jaula de cocción implícita en la ventana gráfica

  Si no se utiliza un fichero de malla de jaula personalizado, se generará una malla de jaula automática y se mostrará en la ventana gráfica. Su tamaño se basará en el parámetro Distancia frontal máxima de los ajustes comunes de horneado. La malla de la jaula se utiliza para indicar hasta dónde llegará la coincidencia entre el poli bajo y alto.
* [Modo de cocción] Mostrar la lista de nombres de malla coincidentes por nombre en el registro de cocción
* [Modo de cocción] Utilice material neutro para mostrar el modelo 3D en la ventana gráfica
* [Modo de cocción] Desactivar el cálculo del motor en modo de cocción
* [Modo de cocción] Mostrar una advertencia al salir de la aplicación mientras hay una cocción en curso
* [Bakers] Actualizar etiquetas de configuración de suavizado

  Los valores del ajuste de suavizado se han cambiado de nombre a &quot;Supersampling&quot; (Supermuestreo) y con un número multiplicador explícito para aclarar su comportamiento.
* [Baker] Actualice baker a la versión 2.5.7.
* [USD] Archivos de Universales Scene Description de importación y exportación (USD)
* [USD] Añada opciones de USD a la ventana Nuevo proyecto al seleccionar un archivo USD
* [USD] Añadir nueva ventana de selección Ámbito y Variantes

  Al importar un fichero USD, pulsando en el botón de cambio de la ventana Nuevo Proyecto o Configuración del Proyecto podrá seleccionar qué parte y variantes de un fichero USD desea importar.
* [USD] Opción Añadir niveles de subdivisión

  Al crear un nuevo proyecto con un archivo de malla USD que contiene subdivisiones, es posible seleccionar el nivel de subdivisiones mediante un regulador. El proyecto se creará con la malla subdividida. El nivel se puede modificar mediante la configuración del proyecto.
* [USD] Importar mallas de piel USD en un marco específico

  Al crear un nuevo proyecto con un archivo de malla USD que contiene animación, es posible seleccionar el fotograma mediante un regulador que refleje la secuencia de cronología incrustada. El marco se puede modificar mediante la configuración del proyecto.
* [USD][Exportar] Añadir una opción para exportar archivos USD

  Se ha añadido la nueva casilla de verificación Exportar USD a la ventana Exportar texturas. Cuando está activada, permite exportar archivos USD, así como mapas de textura, utilizando cualquier plantilla.
* [USD][Exportar] Añadir el formato de archivo USD a la malla de exportación
* [USD] Cambie el nombre del ajuste preestablecido de exportación existente &quot;Rugosidad del metal PBR en USD&quot; para que sea más explícito

  Se puede acceder a la plantilla de exportación en USD denominada anteriormente &quot;Rugosidad del metal PBR en USD&quot; a través de Exportar texturas > Plantilla de salida > USDz (Apple AR).
* [Auto Unwrap] Añadir orientación de bloqueo para el empaquetado

  Nueva opción para la configuración de desajuste automático que permite conservar la orientación de las Islas de UV existentes al utilizar la función de empaquetado. Se puede acceder a él desde Nuevo proyecto > Opciones de desajuste automático > Orientación de la Isla de UV.
* [Tamaño físico] Añada una configuración para utilizar automáticamente el Tamaño físico en el efecto de relleno/capa

  Se ha añadido una nueva opción para cambiar automáticamente a la escala de tamaño físico al utilizar un material con tamaño físico incorporado. Se puede activar por proyecto a través de Nuevo proyecto o a través de Editar > Configuración del proyecto > Tamaño físico > Cambiar la escala de la capa de relleno a Tamaño físico al asignar materiales.
* [Tamaño físico] Exponer tamaño físico para Proyección de UV

  La escala de tamaño físico ahora está disponible para las Proyecciones de UV: permite el cambio de tamaño automático para un material en función del tamaño físico de una malla. Se puede seleccionar a través de Escala > Tamaño físico en la ventana Propiedades de la capa de relleno o del efecto.
* [Scripting] [Python] Permitir consultar la versión de la aplicación
* [Scripting] [JavaScript] Actualización de la API para que coincida con los nuevos parámetros de procesamiento
* [Scripting] [Python] Módulo de horneado: editar parámetros de procesamiento
* [Scripting] [Python] Módulo de horneado: iniciar/cancelar el procesamiento
* [Scripting] [Python] Módulo de horneado: seleccionar método de curvatura
* [Scripting] [Python] Módulo de horneado: selección de panaderos/baldosas ultravioletas
* [Scripting] [Python] Módulo de horneado: sincronizar la configuración de panadero en todos los conjuntos de texturas
* [SVT] Habilitar la compatibilidad de hardware disperso en las GPU AMD

  La aceleración de hardware para el sistema de texturas virtuales dispersas ahora se puede activar con las GPU AMD. Este ajuste se activa automáticamente en las preferencias generales.
* [Proyección] Cambiar nombre de parámetros de proyección cilíndrica

  El parámetro &quot;Cylinder Cap Culling&quot; ha pasado a denominarse &quot;Backface Culling&quot; para representar mejor su acción. La información sobre herramientas asociada se ha ajustado en consecuencia.
* [Project] Guarde la versión de la aplicación en el proyecto y recuperarla mediante scripts

  Desde la versión 8.2, la versión de la aplicación se almacena ahora dentro del archivo spp al guardar.\
  Este número de versión se puede recuperar con la función last\_saved\_substance\_painter\_version() en el módulo de proyecto de la API de Python.\
  Para un proyecto realizado antes de la versión 8.2, el valor devuelto será nulo.
* [Importar] Mejora el tiempo de importación general de modelos 3D

  Mejoramos el tiempo general de importación de mallas. Por ejemplo, reducir el tiempo de espera al cargar mallas de alto contenido de polietileno para hornear. Esta optimización se aplica en particular a la carga de archivos OBJ.

**Corregido:**

* [Bloqueo] Cambio de canales en el filtro con una pila específica
* [Mac][M1] Bloqueo al crear una capa de relleno y salir de la pila de capas

  Este problema se puede solucionar actualizando a Mac OS 13 (Ventura).
* [Scripting] [Python] Bloqueo al utilizar ui.add\_dock\_widget() con un tipo incorrecto
* [Haciendo un bake] Mensaje de error incompleto en el registro cuando falla una hace un bake
* [Haciendo un bake] La memoria no se libera cuando finaliza la hace un bake
* [Motor] La caché de Textura no se actualiza al cambiar la visibilidad del efecto
* [Exportar] 2DView exporta un mapa aleatoriamente uniforme
* [Proyecto] Error de asignación de memoria al guardar el proyecto con malla grande
* [Ventana gráfica] El TAA provoca defectos al pintar en algunos casos

**Problemas conocidos:**

* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* [Pila de capas] El origen de entrada no se guarda por capa
* [Exportar] exportaciones de vista 2D mapa aleatoriamente uniforme
