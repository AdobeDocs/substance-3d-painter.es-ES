---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/release-notes/all-changes.html'
breadcrumb-title: ''
description: Revisa todos los cambios y actualizaciones en las versiones de Substance 3D Painter para realizar un seguimiento de la evolución y las mejoras de las funciones a lo largo del tiempo.
helpx_creative_field: ''
helpx_description: Painter > Release notes > All Changes
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Todos los cambios
user-guide-description: ''
user-guide-title: ''
hold: false
source-git-commit: fc154cd38e23b0e598c15bfbfee8a263d5770592
workflow-type: tm+mt
source-wordcount: '34015'
ht-degree: 0%

---


# Todos los cambios

Esta página contiene notas de la versión de todas las versiones anteriores de Substance 3D Painter, ordenadas de la más reciente a la más antigua.

>[!NOTE]
>
> Para ver los problemas conocidos que pueden afectar a Painter, consulte la [página de documentación dedicada](known-issues.md).

## Versión 12

### 12.1.4

Fecha de publicación: **2026/09/04**

Resumen: **Versión secundaria**

**Corregido:**

- \[Bloqueo\] Bloqueo al importar o exportar archivos cuyo nombre de archivo contiene caracteres no ASCII

### 12.1.3

Fecha de publicación: **2026/08/26**

Resumen: **Versión secundaria**

**Agregado:**

* Actualizar el motor de Substance a la versión 9.4.6

**Corregido:**

* El selector [Escala de grises] permanece abierto después de cambiar la herramienta
* [Hacer un bake sesgo] La corrección de sesgo se interrumpe al pintar y deshacer
* La herramienta de proyección [Projection Tool] bloquea la interacción de la ventana gráfica
* [Trazo dinámico]: faltan parámetros de trazo dinámico en las propiedades del pincel
* La exportación a una red ya no funciona

### 12.1.2

Fecha de publicación: **2026/08/03**

Resumen: **Versión secundaria**

**Corregido:**

* \[Bloqueo\] Algunos Substance pueden provocar un bloqueo al procesarse
* \[Bloqueo\] Volver a importar la malla mientras está en modo de hacer un bake
* \[Bloqueo\] Si no se inicializa la visualización de gráficos, se puede producir un bloqueo
* \[Bloqueo\] La exportación de texturas puede bloquearse en algunos casos al actualizar el registro
* \[Crash\] Bloqueo en el modo de procesamiento en algunos casos al cargar o actualizar el mapa de entorno
* \[Horneado\] Si se vuelve a iniciar el horneado después de modificar el archivo de alta densidad, se puede producir un bloqueo
* \[Enviar a Photoshop\] No se puede exportar la máscara de capa
* \[Motor\] El resultado del punto de ancla no se procesa entre una máscara y un canal de color

### 12.1.1

Fecha de publicación: <b>2026/07/09</b>

Resumen: Versión secundaria

Añadido:

* [Horneado de sesgo] Exponer modo normal de base de sesgo: malla o por triángulo
* [Propiedades] Hacer que los colores uniformes siempre se restablezcan al valor predeterminado de su canal
* [OpenPBR] reagrupa los canales por categorías en la ventana Exportar texturas para crear plantillas de salida
* Actualizar el motor de Substance a la versión 9.4.5

Corregido:

* [Proyecto] Abrir y guardar algunos proyectos puede tardar más de lo habitual
* [Bloqueo] La recarga de varias mallas puede provocar un bloqueo
* [Bloqueo] Al eliminar un canal en el modo de vista de máscara, se produce un bloqueo
* [Bloqueo] Algunos Substance pueden producir un bloqueo al procesarse
* [Sesgar pintura] La herramienta seleccionada en el sesgo de pintura permanece seleccionada después de cambiar al modo de pintura
* [Configuración común de horneado] La configuración de la distancia de la jaula no actualiza la visualización de la malla metálica de la jaula y del sombreador
* El modo &quot;Vecino del espacio 3D&quot; del relleno UV [Engine] no funciona bien en triángulos finos
* El resultado del punto de anclaje [Engine] no se procesa entre una máscara y un canal de color

### 12.1.0

Fecha de publicación: <b>2026/06/23</b>

Resumen: <b>Esta actualización es una versión importante, contiene mejoras en los panaderos con el nuevo estado predeterminado de la interfaz de usuario para panificación, mapa de sesgo de pintura, reprocesamiento automático, nueva opción para el desempaquetado UV automático para mallas de superficie dura y OpenPBRs. Para obtener más detalles, vea las notas de la versión completas.</b>

<b>Agregado</b>:

* [Skew baking] Herramientas de pintura de sesgo
* [Skew Baking] Añada sombreador de previsualización de sesgo y elementos visuales de dirección de sesgo al pintar el mapa de sesgo
* [Skew Baking] Añadir protección de bordes, opción
* [Sesgar la cocción] Auto rehacer
* [Skew Baking] Interfaz de usuario de lista de mapas de malla de reprocesamiento
* [Sesgar horneado] Dividir mapa de malla / Configuración común de horneado + Mover ajustes comunes de la lista de mapas de malla solo en color o máscara
* [Sesgar horneado] Cambiar botones de la barra de herramientas de la ventana gráfica
* [Sesgar horneado] Mostrar alternancia de simetría para el pincel en la barra de herramientas superior
* [Skew Baking] Cambiar nombre de opciones en el menú de sincronización de lista de mapa de malla
* [Skew Baking] Cuadro de diálogo Actualizar sincronización y estado marcado
* [Sesgar horneado] Crear variante del selector de color de escala de grises
* [Sesgar horneado] Icono Actualizar modo de horneado
* [Auto Unwrap] opción Integrar superficie dura
* [OpenPBR] Añadir apoyo para el OpenPBR 1.1
* [OpenPBR] Hacer que OpenPBR sea el flujo de trabajo y el sombreado predeterminados
* [OpenPBR] Importar materiales y texturas de OpenPBR a través de USD
* [OpenPBR] Exportar materiales y texturas de OpenPBR a través de USD
* [OpenPBR] Actualice la ventana Exportar texturas para mostrar la convención de nomenclatura del OpenPBR
* [OpenPBR] Añadir documentación sobre los cambios en el OpenPBR de asistencia
* [OpenPBR] [Israel] Añádase un nuevo MDL para prestar apoyo al OpenPBR 1.1 de Israel
* Varias mejoras menores de las exportaciones en dólares
* [UI] Añada una advertencia en la ventana gráfica al intentar pintar en otro conjunto de texturas
* [Aplanar] Permite acoplar todas las capas con instancias en los conjuntos de texturas
* [Ajustes del conjunto de texturas] Permite seleccionar varios canales a la vez mediante una nueva ventana
* [Historial] Actualizar &quot;valor&quot; Deshacer texto de entrada para reflejar el nombre del parámetro
* [Pila de capas] Los efectos de relleno de las máscaras se establecen de forma predeterminada en blanco (1.0)
* [Substance] Añadir nueva entrada de mapa del motor &quot;mesh_hard_edges_triangle&quot;
* [Substance] Añadir nueva entrada de mapa del motor &quot;mesh_hard_edges&quot;
* [Sombreador] Evitar que las instancias del sombreador compartan los mismos nombres
* [Sombreador] Utilice el sombreador de la plantilla de proyecto al importar un archivo USD o GLTF
* Actualizar Adobe Color Engine a la versión 7.0
* Actualizar la versión mínima de MacOSX a 13.0 (Ventura)
* [Contenido] Nuevas plantillas de proyecto para el OpenPBR
* [Contenido] Actualizar proyectos de muestra para utilizar el nuevo sombreador de OpenPBR
* [Python] Amplía la API de máscara de geometría para permitir modos de inclusión y exclusión como en la interfaz de usuario

<b>Corregido</b>:

* [Bloqueo] [Ajustes de Mapas de Malla] Aplicación de ajustes a otros conjuntos de texturas
* [Bloqueo] Al hacer un bake la curvatura del mapa sin espacio mundial normal
* [Bloqueo][Hacer un bake] Hacer un bake con la jaula personalizada activada, pero sin bloqueos de archivo seleccionados
* [Bloqueo] Cancelación de hace un bake de AO
* [Auto-Cage] Carga infinita cuando la ruta del archivo de poli alto no es válida
* [Linux] [Windows] En ocasiones, el selector de color puede ser completamente negro o no aparecer
* [Herramienta Relleno poligonal] La herramienta no funciona con PBR
* [[Pintura] Al eliminar el canal de color base no se elimina el color pintado anteriormente
* [USD] No se detectan correctamente todas las Instancias del sombreador
* [Substance] Solo se tiene en cuenta el primer uso de un nodo de entrada/salida
* [Sombreador] La Oclusión ambiental se aplica dos veces con los conjuntos de texturas usando diferentes métodos de mezcla
* [Motor] Las texturas normales con un canal azul vacío (negro) pueden producir resultados de mezclas incorrectos
* [Importación GLTF] La fusión alfa está activada en todos los conjuntos de texturas
* [GLTF Export] La fusión alfa siempre está activada en la exportación
* [Exportar] La geometría de doble cara siempre está desactivada al importar un archivo GLTF
* [Javascript] La modificación de la configuración de los sombreadores no contribuye al historial de deshacer
* [Muestras] La dispersión subsuperficial no está activada en Configuración de visualización para Meet Mat

### 12.0.3

Fecha de publicación: **2026/05/05**

Resumen: **Versión secundaria**

**Agregado:**

* Actualizar bakeres a la versión 3.2.2
* Actualizar el motor de Substance a la versión 9.4.3
* \[Python\] Guardar un material inteligente en una ubicación específica

**Corregido:**

* \[Ubuntu\] Bloqueo al seleccionar material
* \[Mac\] Aparece una ventana emergente periódica para solicitar acceso a los datos de otras aplicaciones
* \[Hacer un bake\] Pueden aparecer artefactos en el mapa de curvatura
* \[Hacer un bake\] Hacer un bake es más lento en algunos casos
* \[Deformar en geometría\] En algunos casos, la opción Deformar en geometría se desactiva
* \[Mosaico de UV\] El alfa extraído del punto de anclaje es ignorado por otros mosaicos
* \[Python\]\[Mac\] Excepciones en la consola de Python con SSL
* \[Python\] bloqueo de Painter al salir con widgets Qt sobrantes

### 12.0.2

Fecha de publicación: **2026/04/07**

Resumen: **Versión secundaria**

**Agregado:**

* [Gestión de color] Añada nuevos OCIO para especificar el espacio de color predeterminado del selector de color
* [Python] Exponer la configuración de desajuste automático en la API de Python

**Corregido:**

* [Bloqueo] Si no hay suficiente espacio en disco, los proyectos se pueden bloquear o dañar
* [Bloqueo] [Cinta] El uso de la cinta puede producir bloqueos en algunos proyectos
* [Crash] [Baking] se bloquea cuando el archivo .assbin no se puede escribir en la carpeta
* [Importar] Las mallas OBJ de Stager pueden fallar en la creación del proyecto
* [Importar] A OBJ le falta cara en algunos casos
* [Importar] La malla USD sin material asignado puede bloquearse al importar
* [Ruta rellena] No se ve afectada por la simetría
* [Stencil] La previsualización tiene una resolución inferior a la del resultado pintado
* [UI] &#39;UV island&#39; sigue apareciendo en la información sobre herramientas de origen de color del mapa de ID
* [Display] Las sombras aparecen invertidas
* [Ventana gráfica] La transformación de proyección de deformación permanece después de cambiar al modo de deformación
* [Deformar] La cuadrícula desaparece cuando la escala se establece en 0 en el eje Z con la opción Deformar en geometría activada
* [Python] Error inesperado al agregar un canal con modificación de ámbito

### 12.0.1

Fecha de publicación: **2026/03/18**

Resumen: **Versión secundaria**

**Corregido:**

* \[Crash\]\[Freeze\] Exportar desde proyectos específicos

### 12.0.0

Fecha de publicación: <b>2026/03/09</b>
Resumen: <b>Esta es una versión importante. Esta versión contiene las funciones de acoplar capas, deformar en geometría, nuevos efectos posteriores, mejoras en la nueva ventana de proyecto y otras mejoras.</b>

<b>Agregado</b>:

* [Acoplar capas] Acoplar capas dentro de la pila de capas
* [Acoplar capas] Exportar capas acopladas a un disco
* [Deformar en geometría] Añadir nueva función de deformación automática a las proyecciones de deformación
* [Efectos posteriores] Reemplace los efectos posteriores por la adición de otros nuevos
* [Post-effects] Actualizar el asignador de tonos
* [Post-effects] Añadir nuevo uso para recursos Post-effects
* [Contenido][Efectos posteriores] Integrar activos de efectos posteriores predeterminados en la biblioteca
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

## Versión 11

### 11.1.3

Fecha de publicación: <b>2026/02/12</b>
Resumen: <b>Versión secundaria</b>

<b>Corregido</b>:

* [Pintar] La galería de símbolos y la simetría no funcionan en algunos casos
* [Ruta] No hay actualización al cambiar el regulador de opacidad del trazo de difuminado
* [Proyecto] No se puede pintar en alguna geometría
* [Cinta de opciones] La ruta instanciada desaparece al cambiar la resolución del conjunto de texturas
* [UI] El selector de color puede reducirse y desaparecer en algunos casos

### 11.1.2

Fecha de publicación: <b>2026/01/13</b>
Resumen: <b>Versión secundaria</b>

<b>Agregado</b>:

* [Horneado] Mejore el tiempo de horneado para el proyecto de azulejos UV con el ahorro asíncrono
* [Shaders] Mención en cambios de registro de cambios tras la migración de Vulkan
* Actualizar OpenEXR a la versión 3.4.4

<b>Corregido</b>:

* [Bloqueo] Bloqueo al iniciarse en la serie Nvidia GTX 10xx
* [Bloqueo] El uso del selector de color en diferentes conjuntos de texturas puede producir un bloqueo al salir de la aplicación
* [Rendimiento] Problema de rendimiento al pintar en un proyecto con muchas capas
* [Rendimiento] Retraso al pintar con el lápiz de Tablet PC gráfico
* [UI] Los ajustes de la cámara permanecen desactivados en el modo de procesamiento (Iray)
* [Cinta] En algunos casos, la ruta puede superponerse inesperadamente después de una esquina
* [Ribbon] Problema de rendimiento con mosaicos UV
* [Substance][UI] Las entradas de imagen desaparecen al contraerse
* [Substance] [IU] Los grupos anidados pueden permanecer aunque se muestren si los oculta
* [Banking][UI] No se puede establecer el radio de muestreo de curvatura más allá de 0,01
* [Horneado][IU] No se puede establecer la distancia máxima del oclusor más allá de 1
* [Horneado] El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y un horneado bajo como alto
* [Horneado] El mapa de ID no hornea los colores de los vértices de FBX en modo Bajo como Alto
* [Contenido] El filtro Paso alto genera colores atenuados en canales con gestión de color

### 11.1.1

Fecha de publicación: <b>2025/12/09</b>
Resumen: <b>Versión secundaria</b>

<b>Agregado</b>:

* [Rendimiento] Mejora el rendimiento de los mosaicos UV al calcular texturas parciales
* [Bakers] Actualización a la versión 3.15.4

<b>Corregido</b>:

* [Bloqueo] [MacOS] Al guardar un proyecto de una versión anterior, siempre se bloquea
* [Bloqueo] El cierre de un proyecto puede provocar a veces un bloqueo
* [Proyecto] Error &quot;los miembros no coinciden en el recuento&quot; al abrir el proyecto realizado en la versión anterior
* [Horneado] Las baldosas UV no se combinan con los resultados anteriores del horneado, si están presentes
* [Banca] El dispositivo se pierde incluso con el trazado de rayos desactivado en la serie Nvidia GTX 10XX
* [Horneando] El AO con normal tiene defectos en los bordes porque no hay relleno
* [Horneado] El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y &quot;coincidencia por nombre&quot; en
* [Baking] El mapa de ID es completamente negro si a alguna malla de alto contenido de poli le faltan colores de vértice
* [Cinta] La información sobre herramientas del modo de fusión Alpha menciona el modo de fusión de pantalla en lugar de Sobreexposición lineal
* [Path] Las tangentes crean bucles inesperados cuando el punto se acerca a los extremos del trazado
* [Herramienta] La previsualización de material no funciona cuando se utiliza la proyección en una máscara
* [Motor] Pintar trazos pequeños puede dar como resultado artefactos de bloque
* [Shader] Al deshacer la creación de la instancia del sombreado, no se elimina correctamente
* El modo de Alpha [Export] para la exportación GLTF siempre está establecido en MASK
* [Python] Error inesperado al editar la pila de capas fuera del bloque de modificación de ámbito

<b>Problemas conocidos</b>:

* [Ribbon] Problema de rendimiento con mosaicos UV
* [Cinta] En algunos casos, la ruta puede superponerse inesperadamente después de una esquina
* [Bloqueo] [Cinta] La creación de textos muy largos en la cinta de opciones puede bloquearse
* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.1.0

Fecha de publicación: <b>11/2025/18</b>
Resumen: <b>Esta actualización es una versión importante, contiene la nueva herramienta Cinta de opciones con contenido nuevo dedicado, soporte de simetría para capas de relleno, parámetro de tamaño físico para desplazamiento, rendimiento mejorado a través de los panaderos actualizados, soporte completo de Vulkan para Windows y Linux y otras mejoras.</b>

<b>Agregado</b>:

* Nueva herramienta de cinta
* [Herramienta] Agregar nueva herramienta Cinta para crear trazados sin problemas
* [Cinta de opciones] Añadir accesos directos preestablecidos de cinta en la ventana Propiedades
* [Cinta] Permite cambiar la opacidad de la Cinta por vértice en la ruta
* [Cinta de opciones] Permite cambiar el tamaño de la Cinta de opciones por vértice en la ruta
* [Cinta de opciones] Quitar el inicio o el final definido en un Substance cuando las rutas están cerradas
* [Cinta] Quitar vista previa de ruta/material en la ventana de propiedades de las herramientas Pintar/Borrador/Difuminar trazado
* [Cinta] Añadir modos de fusión para el canal alfa y algunos canales cuando se superponen automáticamente
* Simetría de relleno
* [Relleno] Compatibilidad añadida para la simetría en capas y efectos de relleno
* [Relleno] [IU] Visualización de los ajustes de simetría en la ventana de propiedades para la capa de relleno y los efectos
* [Fill] Interfaz de usuario de configuración de simetría de trabajo tanto en el menú Ventana como en la ventana de propiedades
* [Rellenar] Reorienta correctamente las texturas normales al proyectar en modo de deformación
* desplazamiento tamaño físico
* [Desplazamiento] Utilice tamaño físico como unidad de desplazamiento
* Mejora del rendimiento
* [Rendimiento] Mejora el procesamiento de trazos de pincel pequeños en triángulos grandes
* [Performance] Mejora el tiempo de compilación del sombreado
* [Rendimiento] Compatibilidad total con Vulkan para Windows y Linux
* [Rendimiento] Panaderos actualizados con procesamiento de GPU más rápido y compatibilidad con trazado de rayos AMD
* [UI] Reorganizar las propiedades de las herramientas en grupos y contraer algunas de forma predeterminada
* [Motor] Actualice Substance Engine a la versión 9.2.5.
* [Substance] Anulación de resolución de exposición para recursos de Substance en Herramientas y rellenos
* [Exportar] Actualizar el ajuste preestablecido de exportación de Mapas de malla para exportar texturas en escala de grises
* Python
* [Horneando] [Python] Indicar en el registro de cambios los cambios de ruptura después de la actualización de los panaderos
* [Python] Exposición de los ajustes de simetría de relleno en Python
* Contenido y nuevo contenido
* [Contenido] Añadir 75 nuevos ajustes preestablecidos de herramientas para la herramienta Cinta de opciones
* [Contenido] Actualizar el recurso del generador de degradados para que sea compatible con la cinta de opciones

<b>Corregido</b>:

* [Bloqueo] La carga de otro proyecto mientras el ajuste de ruta está activado puede bloquearse
* [Bloqueo] El clic derecho en el panel Trazado con información de otra sesión del portapapeles puede bloquearse
* [UI] La interfaz se desplaza hacia arriba en las propiedades de la herramienta al crear un trazado
* [UI] El cursor del ratón desaparece cuando la visualización de la ventanilla de trazado está oculta
* [Path] Copiar/pegar diferentes propiedades de herramienta en el panel Trazado genera propiedades inestables
* [Herramienta] Los ajustes preestablecidos de las herramientas Borrador y Difuminado no siempre actualizan la selección de canales
* [Herramienta] El valor pintado es gris, pero la interfaz de usuario se muestra blanca después de cargar el ajuste preestablecido de herramienta de color en la máscara
* [Herramienta] El ajuste preestablecido creado a partir de la máscara conserva los valores de canales cargados de otro ajuste preestablecido
* [Substance] No se tiene en cuenta la anulación del espacio de color normal definido en el gráfico
* [Contenido] El recurso de forma de pincel predeterminado utiliza un Substance obsoleto

<b>Problemas conocidos</b>:

* El historial de instancias del sombreador no se rastrea correctamente
* [Ribbon] Problema de rendimiento con mosaicos UV
* [Cinta] En algunos casos, la ruta puede superponerse inesperadamente después de una esquina
* [Cinta] Las tangentes crean bucles no deseados cuando el punto se mueve de cerca a los extremos del trazado
* [Bloqueo] [Cinta] La creación de textos muy largos en la cinta de opciones puede bloquearse
* [Herramienta] La previsualización de material no funciona cuando se utiliza la proyección en una máscara
* [Haciendo un bake] El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y &quot;coincidencia por nombre&quot; activado
* [Haciendo un bake] El AO con normal tiene defectos en los bordes debido a la falta de relleno
* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.0.3

Fecha de publicación: <b>2025/08/05</b>
Resumen: <b>Versión secundaria</b>

<b>Agregado</b>:

* [Substance 3D Assets] Adición de un punto de notificación al panel Activos 3D
* [VFX Platform 2025] Añadir la configuración de ACES 2.0 en los ajustes de gestión de color
* [VFX Platform 2025] Actualice OCIO a la versión 2.4.2
* Actualizar Iray a la versión 2024.10
* [Motor] Actualización a Substance Engine v.9.2.3
* [Nvidia] Aumente la versión mínima de controladores de Nvidia a 572.60 (Windows) y 570.169 (Linux).

<b>Corregido</b>:

* [Python] La modificación de ámbito no aparece en la ventana Historial

<b>Problemas conocidos</b>:

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.0.2

Fecha de publicación: <b>2025/06/10</b>
Resumen: <b>Versión secundaria</b>

<b>Agregado</b>:

* [Mac] Se añade una advertencia sobre una versión específica del sistema operativo que provoca artefactos
* [Actualización automática] Pequeñas mejoras de UX en el registro de errores de Activos
* [Auto-unwrap] Actualice a la versión 1.3.2 con mejoras de unión
* [USD][FBX] Añade compatibilidad con varios conjuntos UV con datos dispersos
* [Exportar] Las mallas exportadas como FBX no tienen sus conjuntos UV adicionales si los había en la importación

<b>Corregido</b>:

* [MacOS][Linux] Bloqueo al guardar en una unidad de red
* [Windows] [Tablet] Parpadeo al realizar una panorámica
* [SpaceMouse] Problema al trabajar con la herramienta Trazado
* [Jaula automática] No se puede hornear después de una recarga de malla
* [Actualización automática] La secuencia de imágenes no se vuelve a cargar cuando falta el primer mosaico
* [Path] La tangente personalizada puede afectar a otra tangente
* [Path] El trazado no aparece en el conjunto de texturas si el primer punto está en otro conjunto de texturas
* [UI] Algunos menús siempre se desactivan después de abrir un proyecto (por ejemplo: simetría)
* [Propiedades] No es posible utilizar ni cargar los ajustes preestablecidos de la herramienta Trazado relleno
* [USD] No se reconocen varios conjuntos UV en el sombreador personalizado al utilizar archivos USD
* [USD] Se reemplazan las cámaras con los mismos nombres
* [Exportar] Enviar a Photoshop genera un espacio de color incorrecto para los resultados de color y escala de grises
* [Exportar] Los canales en escala de grises con alfa se exportan como color en lugar de como escala de grises con formato PNG
* [Exportar] Al exportar un canal de escala de grises como PSD, el archivo resultante no es válido o está truncado
* [Contenido] El filtro de deformación en modo multidireccional no funciona
* [Python] No se puede asignar el error de lista al rastrear nodos de pila de capas

<b>Problemas conocidos</b>:

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.0.1

Fecha de publicación: <b>2025/04/10</b>
Resumen: <b>Versión secundaria</b>

Nota: La versión de <b>Linux CCD se retrasará hasta el 29 de abril</b>

<b>Agregado:</b>

* Actualizar a Qt 6.5.8
* [Substance] Añadir mensaje de registro para filtros cuando varias entradas de imagen comparten el mismo uso
* [Nvidia] Añadir advertencia sobre los controladores más recientes de Nvidia (572.47)

<b>Corregido:</b>

* [Bloqueo] Al arrastrar y soltar una barra lateral con un uso en ranuras de un solo canal
* [Bloqueo][Ruta] La opción Cambiar tipo de ruta no aparece atenuada al no hacer clic en una ruta específica
* [Rellenar trazado] No debe poder seleccionar material de Substance
* [Motor] Artefactos a lo largo de trazos de pincel
* [Motor] Los trazados se pueden romper con ajustes específicos
* Problema con el menú desplegable para el espacio de color del cuentagotas
* [Actualización automática] [Python] Mensaje de error incorrecto al utilizar ResourceID sin versión
* [Shader] Bloqueo al abrir algunos proyectos

<b>Problemas conocidos:</b>

* [SpaceMouse] Problema al trabajar con la herramienta Trazado
* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.0.0

Fecha de publicación: <b>2025/03/11</b>
Resumen: <b>Versión principal, nueva función de actualización automática, herramienta de ruta rellena y otras mejoras en la ruta, así como nuevos filtros y una generación experimental de jaula automática para hornear</b>

<b>Agregado</b>:

* Actualización automática
* [Actualización automática] Actualización automática de activos modificados en el panel Activos
* [Actualización automática] Actualización automática de activos modificados en todo el proyecto
* [Actualización automática] Mantener la actualización automática desactivada de forma predeterminada
* [Actualización automática] Hacer que la actualización sea opcional si los parámetros del recurso no coinciden (.sbsar, .glsl, .ai, .svg)
* [Actualización automática] Añadir variable de entorno para desactivar la función de actualización automática
* [Actualización automática] [SBSAR] Convertir la actualización en opcional si los parámetros del recurso no coinciden
* Trazado relleno
* [Trazado][Rellenar] Añadir una nueva herramienta para crear trazados rellenos
* Mejoras de ruta
* [Path] Crear un trazado que se ajusta a polígonos
* [Path] Permitir cambiar entre tipos de ruta
* [Ruta] Permite copiar y pegar datos de vértices de ruta entre contenido y máscara
* [Trazado] Permite restringir el ángulo al crear un nuevo punto
* [Ruta] Permite crear puntos de restricción en una línea
* [Path] Cierre la forma con un solo clic
* [Path] Visualización de la información de ruta
* [Path] Permita escalar y rotar los vértices del trazado
* [Path][UX] Facilita el acceso a las herramientas de transformación
* [Path] Añadir vista previa de ruta
* [Trazado] Desactivar la previsualización de trazado con Mayús + P
* [Path] Mejora de la edición de tangentes desde la vista lateral
* [Trazado] Permitir que el enfoque se centre en un trazado 3D
* [Path] Los vértices deben conservar el estado de selección al activar o desactivar la IU de nuevo
* [Ruta] Permitir eliminar la ruta con la barra espaciadora
* [Path] Mantenga abierta la lista de rutas si el usuario la expande
* [Ruta] [Pila de capas] Cambiar el nombre de los duplicados correctamente al copiar y pegar
* [Path] Mejoras en la interfaz de usuario y la información sobre herramientas
* Rendimiento
* [Rendimiento] Mejore el rendimiento de la ventanilla al utilizar un nivel de teselación alto
* [Rendimiento] Habilite solo el primer canal en las nuevas capas/efectos de relleno
* [Rendimiento] Paralelizar el cálculo de trazos de pincel
* Baking
* [Horneado] Añadir nueva opción de generación de jaulas totalmente automática para horneado con mallas de alto contenido de polietileno (Experimental)
* Contenido
* [Contenido] Añade 6 filtros nuevos: estilización, cuantificar, anisotrópico kuwahara, suavizado de bisel, distancia direccional, conversión de escala de grises
* [Contenido] Actualización de Noises y Grunges a la versión más reciente de Designer (con el nuevo 2D Voronoi)
* [Contenido] Añada 3 nuevos generadores de texturas (Aleatorio de azulejos, Triangle Grid, Generador de Scratches)
* [Contenido] Cambiar nombre de plantilla de Unreal Engine y exportar ajustes preestablecidos
* Python
* [Shelf] [Python] Guarda material inteligente o máscara inteligente en el disco desde Python
* [Python] Adición de la jaula automática de banca a la API de Python
* [Python] Permite editar nombres y descripciones de conjuntos de texturas y mosaicos UV
* [Python] Compartir la configuración de resolución en fuentes de fuentes y vectores
* [Actualización automática] [Python] Exponer las funcionalidades de actualización automática del proyecto en Python
* Varios
* [Exportar] Facilite el acceso a las opciones de Enviar a con un nuevo panel
* [Nvidia] Añadir advertencia sobre los controladores más recientes de Nvidia (572.16)
* El ajuste de ángulo debe verse afectado por la selección de espacio Objeto/Mundo
* [Lista de conjuntos de texturas] Permite añadir un nombre personalizado a los mosaicos UV y utilizarlos en la exportación
* Mac
* [Mac] Uso de Metal en lugar de OpenGL para el procesamiento de gráficos
* [Mac] Se retira la asistencia de Mac Intel

<b>Corregido</b>:

* [Bloqueo] Eliminar entrada de imagen
* No se puede añadir una alfombra inteligente mediante el botón de pila de capas
* [Python] No se pueden encontrar efectos en GroupLayerNode

<b>Problemas conocidos</b>:

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [MacOS Intel] Bloqueo al importar algunos ajustes preestablecidos
* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando
* [RedHat] Problemas con el selector de color

## Versión 10

### 10.1.2

Fecha de publicación: <b>2024/12/3</b>
Resumen: <b>versión secundaria, correcciones de errores</b>

<b>Corregido</b>:

* [Bloqueo] Eliminar entrada de imagen
* No se puede añadir una alfombra inteligente mediante el botón de pila de capas
* [Python] No se pueden encontrar efectos en GroupLayerNode

<b>Problemas conocidos</b>:

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [MacOS Intel] Bloqueo al importar algunos ajustes preestablecidos
* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando
* [RedHat] Problemas con el selector de color

### 10.1.1

Fecha de publicación: <b>2024/11/5</b>
Resumen: <b>versión secundaria, correcciones de errores</b>

<b>Agregado</b>:

* [Project] Mantenga abierto el proyecto actual hasta que se valide la selección de nuevo proyecto
* [Auto-unwrap] La densidad de texto permite dividir mejor las Islas de UV en UDIM
* [Banking] Corregir copia ambigua en el menú contextual de Mapas de malla
* [Deformar] Eliminación de la escala en la ventana gráfica para el eje Z (profundidad)
* [Importar/Exportar] Quitar la compatibilidad de los formatos de archivo de imagen no utilizados
* Actualizar Substance Engine a 9.1.4

<b>Corregido</b>:

* [Bloqueo] Después de reubicar el recurso en Recursos y guardar el proyecto
* [Bloqueo] Problemas con la biblioteca de aiserver
* [Bloqueo] El servidor de Illustrator se bloquea en algunos casos excepcionales
* [Bloqueo] Al salir de la aplicación en algunos casos excepcionales
* No se pueden enviar informes de bloqueo en algunos equipos
* [Horneado] El color del vértice no se lee correctamente
* [UI] La ubicación de las ventanas y las novedades al inicio se cambian
* [Assimp] Maya&#39;s StandardSurface no reconocida en el baking de ID
* [Python] La biblioteca SSL que falta genera un error
* [Python][Windows] Error al llamar a QColorConstants.Transparent
* [Python] Las miniaturas de capas creadas mediante Python no se actualizan hasta que se hace clic dentro de la pila de capas
* [Shader] Vínculo roto en el registro de cambios de API del sombreador
* [3D Assets] Usar la configuración del proxy del sistema operativo al acceder a 3D Assets

<b>Problemas conocidos</b>:

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [MacOS Intel] Bloqueo al importar algunos ajustes preestablecidos
* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* [Python] El widget que parece eliminado mediante el script sigue funcionando
* [RedHat] Problemas con el selector de color

### 10.1.0

Fecha de publicación: <b>2024/09/17</b>
Resumen: <b>Versión principal, nuevo contenido: Filtro de color/máscara de área de relleno, filtro de pegatinas de bordado y seis filtros de Substance genéricos, importación de USD con propiedades de materiales y sombreadores, mejora del rendimiento, compatibilidad con VFX Platform 2024 y migración a Linux RedHat</b>

<b>Agregado</b>:

* [Contenido] Añadir nuevo filtro de color/máscara de área de relleno
* [Contenido] Añadir nuevo filtro de pegatinas de bordado
* [Contenido] Añade 6 nuevos filtros de Substance genéricos (FXAA, pixelado, paso alto, posterizar, paso suave y umbral)
* [USD] Exportar capa USD con un material de ASM definido
* [USD] Importar USD con propiedades de materiales y sombreadores
* [Rendimiento] Habilitar miniaturas de pila de capas optimizadas de forma predeterminada
* [Rendimiento] Reducir el tiempo de apertura de archivos de proyecto y el consumo de memoria (descodificación de datos)
* Compatible con la plataforma VFX 2024
* [VFX Platform 2024] Actualización a Python 3.11
* [VFX Platform 2024] Actualización a OpenEXR 3.2
* [VFX Platform 2024] [USD] Actualización de OpenSubdiv 3.6.0
* [VFX Platform 2024] [Gestión de color] Actualización a OCIO 2.3.2
* [Linux] Migración a Linux RedHat
* [Linux] Actualice la versión principal del controlador Nvidia a 535.171.04
* [Importar] Añada una opción para voltear la asignación normal al importar una malla GLTF
* [UI] Usar el valor predeterminado del sistema operativo para la distancia de detección de eventos de arrastre
* [Substance Engine] Añada la función de tira de llamadas para eliminar los símbolos del ejecutable
* [Pantalla de bienvenida] Actualización al nuevo formato de pantalla de bienvenida
* Actualizar Substance Engine a la versión 9.1.3
* [Python] Mostrar vínculos a ejemplos en el menú de documentación de la pila de capas
* [JavaScript] Mover complementos de Javascript a la subcarpeta javascript/plugins

<b>Corregido</b>:

* [Illustrator] Bloqueo al exportar un azulejo UV con un gráfico .ai en casos específicos
* [Trazos dinámicos][Trazado] La opción aleatoria por trazo no funciona en un trazado
* [UI][Propiedades] El bloqueo está activado cuando el mosaico no es uniforme
* El archivo TXT de depuración se crea al hacer doble clic en el proyecto de Painter
* [USD][Exportar] Es posible que falten algunas texturas
* [ASM] El canal de color de dispersión ignora el metal
* [Contenido] El filtro de desenfoque no funciona en espacios de color &quot;operativos&quot;
* [Contenido] Height Ajustar filtro también modifica el alfa de la capa

<b>Problemas conocidos</b>:

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Win] [Bloqueo] [ACE] No se utiliza el espacio de color sRGB ICE para la transformación de la pantalla
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [MacOS Intel] Bloqueo al importar algunos ajustes preestablecidos
* [Bloqueo] Reubicar recurso y guardar proyecto
* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando
* [RedHat] Problemas con el selector de color

### 10.0.1

Fecha de publicación: <b>2024/06/11</b>
Resumen: <b>Versión secundaria, correcciones de errores</b>

<b>Agregado:</b>

* [Biblioteca] Convertir fuentes de Substance en archivos de fuentes normales
* [Illustrator] [SVG] Aplica un fondo gris claro a las miniaturas en la selección de ámbito
* [Python] Añadir función en origen de mapa de bits para enumerar los espacios de color disponibles

<b>Corregido</b>:

* [Pila de capas] La carpeta siempre se cierra al entrar o salir de otras carpetas
* [Guardar] El archivo de proyecto se pierde cuando se produce un error al guardar como copia o al guardar automáticamente en casos específicos
* [Importar] Los recursos con el mismo nombre pero extensiones diferentes se anulan
* [Propiedades] Faltan opciones de configuración al utilizar un punto de anclaje en las entradas de imagen
* [Illustrator] No es posible importar archivos de Illustrator después de un bloqueo del servidor sin reiniciar Painter
* [Python] El padre de la instancia no se puede establecer con el tipo &quot;properties&quot;
* [Python] Al configurar el poli alto como parámetro de horneado, no se carga el poli alto
* [Python] El mensaje de error para set\_color\_space() es demasiado genérico
* [Python] Las fuentes de referencia permiten crear ciclos

<b>Problemas conocidos</b>:

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Regresión][IU] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [MacOS Intel] Bloqueo al importar algunos ajustes preestablecidos
* [Illustrator] Bloqueo al exportar un azulejo UV con un gráfico .ai en casos específicos
* [Trazos dinámicos][Trazado] La opción aleatoria por trazo no funciona en un trazado

### 10.0.0

Fecha de publicación: <b>2024/05/16</b>
Resumen: <b>Versión principal, edición de la pila de capas con la API de Python, lectura de archivos nativos de Illustrator, integración de recursos 3D y nuevo recurso de texto</b>

<b>Agregado</b>:

* [Illustrator] Uso de archivos de Illustrator con mesas de trabajo en Painter
* [Illustrator] [SVG] Añadir vistas previas en la selección de ámbito
* [Substance 3D Assets] Busque, seleccione y descargue contenidos 3D directamente en Painter
* [Substance 3D Assets][UI] Nuevo panel
* [Substance 3D Assets] Mapas y materiales del entorno de apoyo
* [Substance 3D Assets] Permite volver a cargar, navegar y abrir la carpeta de ubicación en el nuevo panel Substance 3D Assets.
* [Substance 3D Assets] Adición de un gestor de descargas
* [Recurso de texto] Permitir el uso de fuentes incrustables
* [Recurso de texto] Permitir procesar una fuente/texto en una malla
* [Recurso de texto] Visualización de fuentes del usuario y otras rutas compartidas en el panel Activos con una nueva categoría
* [Recurso de texto][Propiedades] Añadir compatibilidad con propiedades de fuentes avanzadas
* [Recurso de texto] Permitir buscar/ver fuentes en miniestantes
* [Recurso de texto] Añadir mensaje/cuadro de diálogo de error al importar una fuente incompatible
* Miscelánea
* [Proyección de relleno] Mejora el comportamiento del manipulador Escala al utilizar valores pequeños
* [Manipuladores] Añadir nuevo modo preciso al pulsar el método abreviado de CTRL
* [Manipuladores] Mejorar la estabilidad del manipulador de superficies al traducir
* [Exportar] Añadir nombre de espacio de color en salidas SBSAR
* [Rendimiento] Mejora el tiempo de detección de activos en la biblioteca en el disco
* [Substance] Actualización al motor de Substance versión 9.1.2
* [Arrastrar y soltar] Alinear la rotación de pegatinas con la cámara al soltar en la ventana gráfica
* [Python] Edición de la pila de capas
* [Python] Permite seleccionar capa, efecto, máscara o máscara geográfica en la interfaz de usuario.
* [Python] Permitir obtener/definir modos de fusión de capas
* [Python] Permitir obtener o establecer la configuración de proyección de la capa de relleno
* [Python] Permitir consultar el color de material de Substance desde una capa de relleno
* [Python] Permite consultar y establecer colores y recursos uniformes en capas y efectos
* [Python] Permita crear y editar recursos de texto en la pila de capas
* [Python] Permite editar canales activos en capas y efectos
* [Python] Permitir que las acciones por lotes tengan una sola acción de deshacer/rehacer
* [Python] Permita cargar o editar parámetros de origen vectoriales
* [Python] Permite editar propiedades de color de capas y efectos con la gestión de color
* [Python] Permite consultar y crear capas con instancias
* [Python] Permitir la adición del efecto de selección de color
* [Python] Permite controlar la administración de color de la imagen de mapa de bits
* [Python] Permitir detener/anular la pausa del motor
* [Python] Permite navegar a nodos hermanos y principales
* [Python] Permitir la creación de un efecto de filtro/generador
* [Python] Permitir añadir un efecto de nivel
* [Python] Permitir la adición de una máscara inteligente en una capa
* [Python] Permitir crear o editar puntos de ancla
* [Python] Permitir obtener/Establecer máscara en capas
* [Python] Permitir la creación del efecto de máscara de comparación
* [Python] Permitir consultar y utilizar ajustes preestablecidos de recursos de Substance
* [Python] Permite enumerar los ajustes preestablecidos y sus valores mediante la función interna\_properties para los recursos del Substance
* [Python] Permite enumerar los ajustes preestablecidos de exportación predefinidos
* [Python] Se permite enumerar los ajustes preestablecidos de exportación disponibles en la biblioteca.
* [Python] Permite recuperar el contenido de los ajustes preestablecidos de exportación

<b>Corregido</b>:

* [Bloqueo] Deshaciendo &quot;Quitar instancia de sombreado&quot; con Ctrl-Z
* [Bloqueo] Crear una capa en una pila vacía si la última selección fue un efecto
* [SVG] Problema con el valor de área recortada personalizada
* [Auto-Unwrap] Si se vuelve a calcular solo el empaquetado sin ningún cambio en la orientación UV, se produce un bloqueo
* [Arrastrar y soltar] El retraso debido a los recursos externos se carga previamente varias veces
* [UI] Arrastrar y soltar la miniatura de un recurso puede ocultar un mensaje de advertencia en la pila de capas
* [Rendimiento] Los mosaicos UV enmascarados aún se calculan
* [USD] Resaltado incorrecto para la selección del ámbito
* [Recurso] La imagen de mapa de bits se daña después de pintar en el canal normal y guardar el proyecto
* [USD] Admite la solicitud de mallas de vértices con la mano izquierda
* [Substance] Restablecer los valores predeterminados volver siempre a cero para el widget de ángulo
* [Motor] Pintar con un SVG en una galería de símbolos no funciona
* [Motor] Los trazos normales del pincel de mapa se rompen después de deshacer una acción
* [Contenido] El filtro Gráfico a material tiene una fusión alfa y un espacio de color incorrectos
* [Contenido] Los modos de fusión del Tile Generator no funcionan
* [Contenido] El filtro de barrido de histograma produce bandas en algunos casos
* [Contenido] La iluminación al horno estilizada no tiene en cuenta el height pintado
* [Python] Error inesperado al recuperar información de capas instanciada después de cambiar el sombreador
* [Guardar] El archivo de proyecto se pierde cuando se produce un error en &quot;Guardar como&quot; en casos específicos

<b>Problemas conocidos</b>:

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Crash][Linux][AMD] Arrastre y colocación de recursos en la pila de capas del sistema operativo Wayland
* [Regresión][UI] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
* [Guardar] El archivo de proyecto de Spp se pierde cuando se produce un error en &quot;Guardar como copia&quot; en casos específicos
* [MacOS Intel] Bloqueo al importar algunos ajustes preestablecidos
* [Illustrator] No es posible importar archivos de Ai tras un bloqueo del servidor sin reiniciar Painter
* [Importar] Los recursos con el mismo nombre pero extensiones diferentes se anulan

## Versión 9

### 9.1.2

Fecha de publicación: <b>30/01/2024</b>
Resumen: <b>versión secundaria, correcciones de errores</b>

<b>Agregado</b>:

* [Rendimiento] Mejora el tiempo de creación de la primera capa de relleno en nuevos proyectos
* [Rendimiento] Reducir el tiempo de carga de mapas de entorno pesados
* [Substance] Permite guardar o cerrar proyectos incluso cuando se generan miniaturas

<b>Corregido</b>:

* La acción de guardar falla en proyectos de versiones anteriores cuando se modifica la ventana gráfica
* [Bloqueo] Reimportación de mallas al utilizar archivos AO y gestión de color personalizados
* [Rellenar la proyección] Al hacer clic en el manipulador Escala aparece el mensaje &quot;No se puede pintar&quot;
* [Pincel] Pintar con alineación UV provoca defectos
* [Pila de capas] El cambio de nombre de la capa es lento cuando la pila es muy larga
* [Pila de capas] Mensaje de error incorrecto al utilizar un filtro incompatible en la máscara
* [Pila de capas] La selección vuelve a la capa superior después de la eliminación
* [Exportar] La textura normal generada siempre se encuentra en el modo de relleno 3D Space Neighbor
* [Exportar] La textura alfa no se genera con el ajuste preestablecido de exportación de vista 2D
* [Exportar] La exportación SBSAR tiene usos incorrectos con mapas convertidos
* [Shader] El registro de cambios de API del sombreador no está actualizado con los últimos cambios de ASM

<b>Problemas conocidos</b>:

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Crash][Linux][AMD] Arrastre y colocación de recursos en la pila de capas del sistema operativo Wayland
* [Regresión][UI] El menú contextual es demasiado pequeño en pantallas HD
* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent

### 9.1.1

Fecha de publicación: <b>12/2023/05</b>
Resumen: <b>Versión secundaria, correcciones de errores y envío a la funcionalidad de After Effects</b>

<b>Agregado:</b>

* [Interop] Permitir el envío de una malla con textura a After Effects (Ae 24.1)

<b>Corregido:</b>

* [Relleno] La proyección del conjunto UV en UV no lee más de 2 conjuntos UV
* [Bloqueo] Uso del mapa de entorno de 16K
* [Bloqueo] Exr utilizado como entrada de imagen
* [Bloqueo] Copiar y pegar trazados en proyectos
* [QoL] Arrastrar y soltar un recurso de Alpha en modo de pegatina crea Proyección de UV en la máscara
* [Path] Al copiar vértices de trazado también se cambia el nombre de la ruta de destino al volver a abrir el proyecto
* [Linux] La selección de color se puede romper con varias pantallas
* [Auto Unwrap] Problema de interfaz de usuario para el control de densidad de texto
* Los comentarios de la interfaz de usuario de [Gestión de color] son razonables, pero el motor no
* [Gestión de color] Selección incorrecta del espacio de color en la máscara con anulación de datos de usuario

<b>Problemas conocidos:</b>

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Crash][Linux] con Linux Wayland en AMD al arrastrar y soltar el recurso en la pila de capas
* [Bloqueo] [Mac] Cambio del valor de filtrado anisotrópico en el sistema operativo Monterey
* [Regresión][UI] El menú contextual es demasiado pequeño en la pantalla HD
* [Python] Bloqueo al exportar USD activado por TextureStateEvent

### 9.1.0

Fecha de publicación: <b>2023/11/07</b>
Resumen: <b>Versión principal con compatibilidad con SVG y transparencia, así como mejoras en la herramienta de arrastrar y soltar y ruta</b>

<b>Agregado:</b>

* [SVG] Permitir la importación de archivos vectoriales (SVG)
* [SVG][IU] Añadir compatibilidad con propiedades específicas del SVG
* [SVG] Añada una opción para conservar fácilmente las proporciones originales de la imagen
* [SVG] Permitir el uso automático de alfa de SVG con transparencia
* [Interop] Permita el envío de una malla con textura a After Effects (Ae 24.1 beta).
* [Interop] Añadir configuración para Enviar a After Effects
* [QoL][Assets][UI] Activo de importación automática al arrastrar y soltar en la ranura de la IU
* [QoL] Permite arrastrar y soltar activos externos en la pila de capas
* [QoL] [Pila de capas] Arrastra y suelta texturas desde el panel de Recursos en la pila de capas
* [QoL] [Viewport] Permite arrastrar y soltar el generador, filtros en la malla
* [QoL][Viewport] Permite soltar recursos externos en la malla
* [QoL][Proyección] Añadir nuevo conjunto UV al modo de proyección Conjunto UV
* [QoL] Arrastrar y soltar máscaras inteligentes como nuevas capas en la ventana gráfica y la pila de capas
* [QoL] Añadir selector para generadores con varias salidas cuando se utiliza en la máscara
* [QoL] Permite arrastrar y soltar imágenes de un solo canal sobre un efecto de relleno
* [QoL] [Pila de capas] Utilice los modificadores CTRL/ALT con la función de arrastrar y soltar para especificar dónde y cómo crear efectos o capas
* [Path] Cambiar la visibilidad de los trazados individualmente en el panel de trazados
* [Path] Permite utilizar manipuladores de transformación para puntos de trazado
* [Path] Permite controlar manualmente las tangentes por vértice
* [Path] Copiar y pegar propiedades de ruta
* [Ruta] Introduzca un método abreviado vacío para el botón de tangente de rotura
* [Sombreador] Añadir compatibilidad con Opacidad y Translucidez en sombreador de ASM
* [Sombreador] Añadir compatibilidad para canal de Color de absorción con sombreador de ASM
* [Sombreador] Mejora de la información sobre parámetros de sombreador de ASM
* [Sombreador] Cambiar el color predeterminado del canal de Translucidez a negro
* [Configuración de pantalla] Habilitar Suavizado temporal de forma predeterminada
* [Configuración de visualización] Activar configuración de dispersión subsuperficial de forma predeterminada
* [Substance] Se ha añadido compatibilidad con la propiedad ColorSpace desde la entrada/salida del gráfico.
* [Substance] Actualice el motor del Substance a la versión 9.0.3.
* [UI] Hacer accesible el botón de la barra de herramientas contextual incluso si la ventana de la aplicación es pequeña
* [Auto Unwrap] Controle el número de Mosaicos de UV con la densidad de texto
* [Hacer un bake] Desactivar Trazado de rayos de GPU en GPU AMD de forma predeterminada
* [Rendimiento] Aplique compresión sin pérdida en imágenes de 16 bits para reducir el espacio del proyecto
* [Python] Permite manipular la cámara predeterminada en Vista 3D
* [Python] Exponer la capacidad de exportar mallas mediante scripts
* [Contenido][Muestras] Añadir nuevo proyecto de muestra &quot;French Restaurant Table&quot;
* [Contenido] Actualizar el logotipo de Substance alfa a una nueva versión
* [Contenido] Añade tres filtros de material enfocados en el SVG (pegatina personalizada, spray personalizado y gráfico en el material)

<b>Corregido:</b>

* [Bloqueo] Cambio del tamaño del manipulador cuando no se utiliza la herramienta simetría
* [Bloqueo] [Pila de capas] Crear capa cuando no hay nada seleccionado
* [Proyecto] Las asignaciones de malla se pueden dañar después de eliminar los recursos no utilizados
* [Proyecto] Daños en los recursos tras volver a importar o hacer un bake la imagen
* [Assets] Al volver a cargar un activo, se elimina de Favoritos
* [Importar] No se pueden importar recursos cuando &quot;No se encuentra ningún resultado&quot; en el panel de recursos
* [UI] La flecha de la barra de herramientas contextual no aparece en algunos casos
* [Substance] No se admite el botón en paralelo para valores booleanos
* [Nivel] Etiqueta de canal incorrecta cuando se utiliza en la máscara
* [Export][glTF] Los archivos glTF/GLB exportados desde Painter no tienen una unidad de tamaño físico
* [Contenido] La intensidad del filtro de desenfoque se fija en 16
* [Contenido] La entrada de imagen del filtro &quot;color de destino&quot; no está visible

<b>Problemas conocidos:</b>

* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* [Bloqueo] [Linux] con Linux Wayland en AMD al arrastrar y soltar el recurso en la Pila de capas
* [Bloqueo] [Mac] Cambio del valor de filtrado anisotrópico en el sistema operativo Monterey
* [Bloqueo] Exr utilizado como entrada de imagen
* [Bloqueo] Uso del mapa de entorno de 16K
* [Auto Unwrap] Problema de interfaz de usuario para el control de densidad de texto
* [Regresión][UI] El menú contextual es demasiado pequeño en la pantalla HD
* [Python] Exportación de Bloqueos USD activada por TextureStateEvent
* [QoL] Arrastrar y soltar un recurso de Alpha en modo de pegatina crea Proyección de UV en la máscara

### 9.0.1

Fecha de publicación: <b>2023/09/19</b>
Resumen: <b>Versión menor de corrección de errores con varias mejoras</b>

<b>Agregado:</b>

* [Importar] Establecer ubicación de importación predeterminada en la ventana de importación
* [Modo de cocción] Permite restablecer los parámetros a sus valores predeterminados
* [Baking] Establezca el procesamiento en resolución de pintura al crear un proyecto
* [Simetría] Desvincular el manipulador específico de simetría del método abreviado Q
* [Menú] Añada la opción &quot;mostrar registro&quot; en el menú de ayuda
* [Ventana gráfica] Mejorar la velocidad de procesamiento de sombras
* [Substance] Actualice el motor a la versión 9.0.1
* [Gestión de color] El archivo de configuración de OCIO puede tener cualquier tipo de extensión
* [Assets] El recurso de Sbsar con uso de &quot;pegatina&quot; debe configurarse automáticamente para deformar la proyección
* [Path] Muestra un mensaje al intentar interactuar con la herramienta Ruta mientras la IU y los Gizmos están ocultos

<b>Corregido:</b>

* [Bloqueo] Alt + Arrastrar en el panel Trazado
* [Importar recursos] Bloqueo aleatorio al quitar recursos para importar
* Bloqueo al importar un archivo GLB comprimido
* Problema al pintar en mallas que comparten UV
* Parpadeo de malla negro al volver a calcular o cargar la caché
* [Propiedades] El menú contextual para restablecer parámetros no aparece en los menús desplegables
* [Nivel] Reguladores de entrada bloqueados por nivel anterior
* [AMD] [Disperso] La opción SVT si se activa genera artefactos
* [Proyección][Deformación] Bloqueo al hacer doble clic en los vértices
* [Path] Interfaz de usuario y ruta de acceso visibles en el modo de procesamiento
* [AMD] Se pierde textura al jugar con la visibilidad
* Resolución [dispersa] demasiado baja al girar la malla

<b>Problemas conocidos:</b>

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción

### 9.0.0

Fecha de publicación: <b>2023/06/20</b>
Resumen: <b>Versión principal con Pintura a lo largo de la ruta que permite curvas 3D, nuevos materiales base y la limpieza de materiales heredados y nuevos ajustes preestablecidos para curvas 3D</b>

<b>Agregado:</b>

* [Path] Herramienta Agregar nueva Pintura a lo largo del trazado
* [Path] Agregar un método abreviado vacío para la herramienta de trazado
* [Path] Permite añadir nuevos puntos a un trazado existente
* [Path] Agregar método abreviado para salir de la creación de la ruta actual
* [Path] Permitir la edición de las propiedades de pincel de trazados
* [Trazado] Ajuste automático de tangentes al colocar un punto
* [Trazado] Calcular tangentes al mover un punto
* [Trazado] Ajuste los puntos recién creados a la superficie de una malla
* [Trazado] Permitir editar la presión por vértice
* [Trazado] Ajuste la presión del punto recién creado desde los puntos vecinos
* [Trazado] Permite convertir puntos en suavizado/esquina (salto de tangente)
* [Ruta] Permite mover un punto recién añadido inmediatamente
* [Path] Permite quitar puntos de un trazado existente
* [Path] Permite invertir la dirección de un trazado
* [Ruta] Permite seleccionar una ruta en la ventana gráfica
* [Trazado] Permitir la selección de puntos de trazado con selección de recuadro
* [Trazado] Introduzca métodos abreviados de CTRL-A para seleccionar todos los puntos de un trazado
* [Ruta] Permitir cerrar ruta
* [Path] Permite especificar el eje ascendente de la ruta en Propiedades
* [Path] Agregar un menú de control de vértices a la barra de herramientas contextual
* [Path] Introducción de los modos de pintura, borrado y difuminado en la herramienta de trazado
* [Path] Creación de comentarios visuales para rutas en la ventana gráfica
* [Ruta] Agregar un indicador visual de la dirección de la ruta
* [Ruta] Agregar thickness de línea a la configuración de visualización de ruta
* [Path] Permitir ocultar la interfaz de usuario de rutas
* [Path] Panel Añadir trazado para ver los trazados de la capa seleccionada actualmente
* [Path] Añadir comentarios visuales al pasar el puntero sobre un trazado en el panel Trazado
* [Path] Muestra el panel de trazado siempre que se selecciona la herramienta Trazado
* [Trazado] Permita cambiar el nombre, eliminar, copiar, cortar o duplicar el trazado en el panel Trazado
* [Path] Aparece un mensaje al intentar interactuar en la ventana gráfica 2D con la herramienta Ruta
* [Biblioteca] Integrar nuevo contenido (herramientas de ruta y materiales base)
* [Trazos dinámicos] Agregar propiedad de distancia para trazos dinámicos
* [Trazos dinámicos] Añadir propiedades de tamaño y espaciado a los trazos dinámicos
* [Trazos dinámicos] Agregar propiedad de inicio/centro/fin para trazos dinámicos
* [Python][USD] Exponer los parámetros de configuración del proyecto para el formato USD
* [Python][USD] Exponer parámetros de creación de proyectos para el formato USD
* [Export][USD] Añadir información de la ruta del proyecto dentro del archivo USD exportado
* [GLTF] Actualización de texturas en la biblioteca al volver a cargar un archivo GLTF
* [Sombreado] Reducir los defectos de costura de las Islas de UV con diferentes orientaciones
* [Motor] Actualice a la versión 9.0 del motor de Substance

<b>Corregido:</b>

* [Importar] Algunos GLB con texturas no obtienen texturas en Painter
* [AMD] Artefactos en los bordes para todos los rellenos de proyección 3D
* [Motor] Las texturas se rompen al alternar la visibilidad de la capa
* [Motor] Las texturas están vacías en algunos lugares al cambiar el modo de fusión
* [Motor] La textura/proyección está en modo de deformación vacío en algunos casos
* [Iray] La iteración se restablece en 0 al guardar el procesamiento
* [Log] Mensaje de error de USD al hacer Archivo > Nuevo

<b>Problemas conocidos:</b>

* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* [Pila de capas] El origen de entrada no se guarda por capa

## Versión 8

### 8.3.1

Fecha de publicación: <b>2023/04/27</b>

<b>Agregado:</b>

* [Modo de Hace un bake] Añada método abreviado (vacío) para mostrar u ocultar la visualización de la ventana gráfica
* [Modo de Haga un bake] Mostrar siempre la opción de baja resistencia al utilizar el botón &quot;Ocultar mallas de haga un bake&quot;
* [Modo de Hace un bake] Mostrar sufijo para hacer coincidir por nombre en función del conjunto de texturas actual
* [Importar] Añadir soporte para archivos binarios GLTF (glb)
* [Lista Conjunto de texturas] Añadir menú para seleccionar o crear instancias del sombreador
* [Lista de conjuntos de texturas] Permitir cambiar rápidamente el conjunto de texturas y la resolución de Mosaicos de UV
* [Tamaño físico] Mejora del comportamiento del manipulador al utilizar tamaño físico en Proyección de UV
* [UI] Volver a &quot;Guardar como&quot; en el menú Archivo principal
* [UI] Guardar selección de vista (solo 2D, solo 3D, ambos) en diseño de IU
* [USD] Mensaje de error menos impreciso al crear un proyecto con formas de USD no compatibles
* [Python] Añadir eventos de hace un bake para seguir el progreso de Hace un bake
* [Python] Permitir cancelar una hace un bake
* [Python] Exponer &quot;Según plantilla de salida&quot; para tipo de archivo y profundidad de bits en la exportación
* [Python] Exponer el tiempo de actualización para TextureStateEvent.Update

<b>Corregido:</b>

* [Bloqueo] bloqueo raro al cerrar un proyecto
* [Bloqueo] [Haciendo un bake] Activar la sincronización del mapa de malla con el Height o la curvatura en un proyecto específico
* [Bloqueo] [Scripting] Bloqueo al añadir un material después de crear la instancia del sombreador
* [Modo de Haga un bake] La intensidad de AO en material neutro no tiene efecto
* [Modo de cocción] Bloqueo al cambiar al modo de cocción antes de cargar el modelo
* [Modo de cocción] Mensaje de error que falta en la ficha Proceso de cocción
* [Modo de cocción] Los ajustes de material neutro no tienen efecto después de volver a importar una malla
* [Modo de panificación] El separador de ventanilla se guarda globalmente y no por modo
* [Modo de cocción] Problema de visualización: normal promedio no cambia la superficie de la jaula
* [Gestión de color] La opción Detección automática del espacio de color se desactiva cuando está presente OCIO env var
* [Contenido] El filtro Contorno de máscara tiene un artefacto con la entrada de height
* [Contenido] El regulador de intensidad del filtro de desenfoque de Pendiente se fija en 1.0
* [Interop] No se puede crear el proyecto con GLTF de Sampler
* [Pila de capas] El valor de mosaico de proyección no se actualiza correctamente con el manipulador
* [Linux] Desplazamiento entre el lápiz gráfico de la tableta y el cursor con HDPI superior al 100 %
* [Python] Bloqueo al volver a importar una malla después de crear un proyecto
* [Substance] Los ruidos 3D se rompen después de volver a importar una malla
* [UV Tiles] El desplazamiento para la Proyección de UV se fija en 1
* [Ventana gráfica] Los comentarios visuales de líneas rectas ya no son visibles
* [WhatsNew] Retorno de línea incorrecto en títulos de funciones

<b>Problemas conocidos:</b>

* [Importar] Algunos GLB con texturas no obtienen texturas en Painter

### 8.3.0

*(Lanzado: 10 de enero de 2023)*
Resumen: <b>Versión principal con nuevo modo de procesamiento, nueva importación y exportación de archivos en USD y compatibilidad de tamaño físico para la Proyección de UV</b>

<b>Agregado:</b>

* [Modo de cocción] Nuevo modo de cocción dedicado al proceso de cocción
* [Modo de cocción] Defina el método abreviado para cambiar al modo de cocción a F8
* [Modo de cocción] Botón Añadir inicio y Cancelar cocción en la ventana gráfica
* [Modo de cocción] Añadir selección de cocción en la lista Conjunto de texturas
* [Modo de cocción] Añadir nueva ventana Mesh Map Bakers para seleccionar panaderos
* [Modo de cocción] Añadir nueva ventana Ajustes de mapa de malla para editar los ajustes de horneado
* [Modo de cocción] Añadir nueva ventana de registro de cocción para seguir el proceso de cocción
* [Modo de procesamiento] Añadir parámetros de procesamiento y acciones de deshacer a la ventana de historial
* [Modo de cocción] Añadir rutas de navegación en Ajustes de mapa de malla
* [Modo de panificación] Añadir miniaturas de mapas de malla en la ventana Panificadores de mapas de malla
* [Modo de cocción] Añadir menú de ajustes de visualización contraíbles en la ventana gráfica 3D
* [Modo de cocción] Añada un ajuste de visualización para mostrar/ocultar la malla de alta densidad
* [Modo de cocción] Añadir ajuste de visualización para mostrar/ocultar la malla de la jaula y la malla metálica
* [Modo de cocción] Añada un ajuste de visualización para mostrar/ocultar la malla de baja densidad
* [Modo de cocción] Añada un ajuste de visualización para mostrar los bordes duros sin costuras UV como errores
* [Modo de cocción] Informar en la ventanilla sobre errores de malla y horneado si el registro de cocción no está visible
* [Modo de Hace un bake] Añadir acción para sincronizar la configuración de baker en todos los conjuntos de texturas

  En la ventana Mesh Map Bakers, cada panadero (así como los ajustes comunes) se pueden sincronizar en los conjuntos de texturas haciendo clic en el icono de enlace junto a su nombre. Esta acción abrirá una ventana que permite seleccionar qué conjuntos de texturas compartirán los mismos parámetros.

* [Modo de cocción] Añadir acciones para copiar y pegar ajustes de panadero

  En la ventana Mesh Map Bakers hay disponibles acciones para copiar y pegar cada configuración de panadero en los conjuntos de texturas, ya sea a través del menú dedicado en la parte superior de la ventana o el menú contextual del botón derecho.

* [Modo de cocción] Botón Añadir en el registro de cocción para saltar del error a la configuración correcta

  Cuando un panadero falla o una malla no se carga correctamente, aparece un mensaje de error en el registro de panadería. Un botón junto al mensaje permite cambiar los marcadores de mapa de malla y la ventana Ajustes de mapa de malla para mostrar los ajustes relacionados. Esto ayuda a aislar con mayor facilidad el origen de un problema para poder solucionarlo.

* [Modo de cocción] Añadir menús para gestionar conjuntos de texturas y selecciones de panadero

  En las ventanas &quot;Texture Set list&quot; y &quot;Mesh Map Bakers&quot; se ha añadido un pequeño menú de acción para ayudar a copiar e invertir las selecciones.

* [Modo de cocción] Dividir la lista de selección de panadero por conjunto de texturas
* [Modo de cocción] Dividir ajustes comunes por conjunto de texturas
* [Modo de Haga un bake] Cargar mallas de alta poly y jaula sin congelar la interfaz
* [Modo de Hace un bake] Utilice la barra de progreso de la ventanilla para mostrar la carga de malla
* [Modo de Hace un bake] Añadir estado de carga de malla en Hacer un bake registro
* [Modo de Haga un bake] Permitir girar la malla en la ventana gráfica durante la hace un bake
* [Modo de Hace un bake] Establecer el orden de hace un bake en función de la visibilidad actual de la ventana gráfica de la malla
* [Modo de Haga un bake] Visualización de la jaula de haga un bake implícita en la ventana gráfica

  Si no se utiliza un fichero de malla de jaula personalizado, se generará una malla de jaula automática y se mostrará en la ventana gráfica. Su tamaño se basará en el parámetro Distancia frontal máxima de los ajustes comunes que se hacen un bake. La malla de la jaula se utiliza para indicar hasta dónde llegará la coincidencia entre el poli bajo y alto.

* [Modo de Hace un bake] Mostrar la lista de nombres de malla coincidentes para Coincidencia por nombre en Registro de Hace un bake
* [Modo de Haga un bake] Utilice material neutro para mostrar el modelo 3D en la ventana gráfica
* [Modo de Hace un bake] Desactivar el cálculo del motor mientras se está en modo de hace un bake
* [Modo de Haga un bake] Mostrar una advertencia al salir de la aplicación mientras hay un haga un bake en curso
* [Bakeres] Actualizar etiquetas de configuración de suavizado

  Los valores del ajuste de suavizado se han cambiado de nombre a &quot;Supersampling&quot; (Supermuestreo) y con un número multiplicador explícito para aclarar su comportamiento.

* [Baker] Actualice baker a la versión 2.5.7.
* [USD] Importar y exportar archivos de Universal Scene Description (USD)
* [USD] Agregar USD opciones a la ventana Nuevo proyecto al seleccionar un archivo de USD
* [USD] Ventana de selección Agregar nuevo ámbito y variantes

  Al importar un fichero de USD, pulsar en el botón de cambio de la ventana Nuevo proyecto o Configuración del proyecto permite seleccionar qué parte y variantes de un fichero de USD se van a importar.

* [USD] Opción Añadir niveles de subdivisión

  Al crear un nuevo proyecto con un archivo de malla de USD que contiene subdivisiones, es posible seleccionar el nivel de subdivisiones mediante un regulador. El proyecto se creará con la malla subdividida. El nivel se puede modificar mediante la configuración del proyecto.

* [USD] Importación USD mallas desolladas en marcos específicos

  Al crear un nuevo proyecto con un archivo de malla de USD que contiene animación, es posible seleccionar el marco mediante un regulador que refleje la secuencia de cronología incrustada. El marco se puede modificar mediante la configuración del proyecto.

* [USD][Exportar] Añadir una opción para exportar archivos USD

  Nueva casilla de verificación Exportar USD añadida a la ventana Exportar texturas. Cuando está activada, permite exportar archivos USD, así como mapas de textura, utilizando cualquier plantilla.

* [USD][Exportar] Agregar USD formato de archivo a la exportación de malla
* [USD] Cambie el nombre del ajuste preestablecido de exportación existente &quot;USD PBR Metal Roughness&quot; para que sea más explícito

  Se puede acceder a la plantilla de exportación de USD conocida anteriormente como &quot;Rugosidad del metal de USD PBR&quot; a través de texturas de exportación > Plantilla de salida > USDz (Apple AR).

* [Auto Unwrap] Añadir orientación de bloqueo para el empaquetado

  Nueva opción para la configuración de desajuste automático que permite conservar la orientación de las Islas de UV existentes al utilizar la función de empaquetado. Se puede acceder a él desde Nuevo proyecto > Opciones de Desenvolvimiento automático > Orientación de la Isla de UV.

* [Tamaño físico] Añada una configuración para utilizar automáticamente el Tamaño físico en el efecto de relleno/capa

  Se ha añadido una nueva opción para cambiar automáticamente a la escala de tamaño físico al utilizar un material con tamaño físico incorporado. Se puede activar por proyecto a través de Nuevo proyecto o a través de Editar > Configuración del proyecto > Tamaño físico > Cambiar la escala de la capa de relleno a Tamaño físico al asignar materiales.

* [Tamaño físico] Exponer tamaño físico para Proyección de UV

  La escala de tamaño físico ahora está disponible para las Proyecciones de UV: permite el cambio de tamaño automático para un material en función del tamaño físico de una malla. Se puede seleccionar a través de Escala > Tamaño físico en la ventana Propiedades de la capa de relleno o del efecto.

* [Scripting] [Python] Permitir consultar la versión de la aplicación
* [Scripting] [JavaScript] Actualizar la API para que coincida con los nuevos parámetros de hace un bake
* [Scripting] [Python] Haciendo un bake módulo: editar hacer un bake parámetros
* [Scripting] [Python] Haciendo un bake módulo: iniciar/cancelar hacer un bake
* [Scripting] [Python] Haciendo un bake módulo: seleccionar método de curvatura
* [Scripting] [Python] Haciendo un bake módulo: selección de bakeres/mosaicos uv
* [Scripting] [Python] Haciendo un bake módulo: sincronizar la configuración del baker en todos los conjuntos de texturas
* [SVT] Habilitar la compatibilidad de hardware disperso en las GPU AMD

  La aceleración de hardware para el sistema de texturas virtuales dispersas ahora se puede activar con las GPU AMD. Este ajuste se activa automáticamente en las preferencias generales.

* [Proyección] Cambiar nombre de parámetros de proyección cilíndrica

  El parámetro &quot;Cylinder Cap Culling&quot; ha pasado a denominarse &quot;Backface Culling&quot; para representar mejor su acción. La información sobre herramientas asociada se ha ajustado en consecuencia.

* [Project] Guarde la versión de la aplicación en el proyecto y recuperarla mediante scripts

  Desde la versión 8.2, la versión de la aplicación se almacena ahora dentro del archivo spp al guardar.
  Este número de versión se puede recuperar con la función last\_saved\_substance\_painter\_version() en el módulo de proyecto de la API de Python.
  Para un proyecto realizado antes de la versión 8.2, el valor devuelto será nulo.

* [Importar] Mejora el tiempo de importación general de modelos 3D

  Mejoramos el tiempo general de importación de mallas. Por ejemplo, reducir el tiempo de espera al cargar mallas de alta densidad para hacer un bake. Esta optimización se aplica en particular a la carga de archivos OBJ.

<b>Corregido:</b>

* [Bloqueo] Cambio de canales en el filtro con una pila específica
* bloqueo [Mac] [M1] al crear una capa de relleno y salir de la pila de capas

  Este problema se puede solucionar actualizando a Mac OS 13 (Ventura).

* [Scripting] [Python] Bloqueo al utilizar ui.add\_dock\_widget() con un tipo incorrecto
* [Haciendo un bake] Mensaje de error incompleto en el registro cuando falla una hace un bake
* [Haciendo un bake] La memoria no se libera cuando finaliza la hace un bake
* [Motor] La caché de Textura no se actualiza al cambiar la visibilidad del efecto
* [Exportar] exportaciones de vista 2D mapa aleatoriamente uniforme
* [Proyecto] Error de asignación de memoria al guardar el proyecto con malla grande
* [Ventana gráfica] El TAA provoca defectos al pintar en algunos casos

<b>Problemas conocidos:</b>

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Pila de capas] El origen de entrada no se guarda por capa

### 8.2.0

*(Lanzado: 6 de octubre de 2022)*
Resumen: **Versión principal con nuevos paneles de incorporación (nuevo panel de bienvenida y nuevo panel), exportación a SBSAR, efectos para carpetas, varias mejoras para la calidad de vida y correcciones de errores.**

**Agregado:**

* [Onboarding] Panel de incorporación para dar la bienvenida a nuevos usuarios

  Se ha añadido una nueva pantalla de bienvenida cuando los nuevos usuarios de CC abren Painter por primera vez.

* [Incorporación] Panel Novedades para mejorar la detección de nuevas funciones

  Se ha añadido una nueva pantalla Novedades que muestra las principales funciones nuevas. Se muestra automáticamente la primera vez que se abre Painter después de una actualización importante, y se puede volver a acceder a él a través de Ayuda > Novedades.

* [Onboarding] Cambiar el nombre de la versión antigua Bienvenido a la &quot;pantalla de inicio&quot;

  Se ha cambiado el nombre de la pantalla de bienvenida para evitar confusiones con la nueva pantalla de bienvenida.

* [UI] Resolver problemas de escalado de pantallas de alta resolución

  Se ha mejorado la adaptación de la interfaz de usuario de Painter en pantallas de alta definición con escala de visualización personalizada.

* [UI] Evite los mensajes de error persistentes en la IU

  Los mensajes de error de proyectos anteriores ahora se eliminan de la barra de estado inferior.

* [UI] Menú para guardar repeticiones

  Las opciones de guardado adicionales ahora se agrupan en un submenú y se cambia el nombre de algunas de ellas por coherencia.

* [IU] Guardar y exportar/compartir diseños de IU

  En el menú Ventana hay nuevas acciones para guardar el diseño de interfaz de usuario en archivos y volver a cargarlos. Los diseños de pintura y procesamiento se guardan por separado.
  Se han añadido varias funciones a &quot;substance\_painter.ui&quot; para guardar, restablecer y cargar diseños de interfaz de usuario también.

* Añadir acciones de copiar/pegar para los modos de fusión/opacidad de una capa

  Se ha añadido una nueva entrada &quot;Opciones de fusión&quot; en el menú contextual de las capas. Permite copiar y pegar el modo de fusión y la opacidad de todos los canales de una capa a otra.

* Aplicar el modo de fusión/opacidad a todos los canales de una capa

  Se ha añadido una funcionalidad de clic con el botón derecho al modo de fusión y la opacidad de las capas, lo que permite aplicar la configuración en la que se ha hecho clic a todos los canales.

* Volver a cargar la malla con un método abreviado de teclado (CTRL+MAYÚS+R)

  Se ha añadido un método abreviado editable para volver a cargar el archivo de malla con los últimos ajustes disponibles. También se puede acceder a través de Editar > Reimportar malla.

* Restablecer los parámetros del Substance a sus valores predeterminados

  Se ha añadido un nuevo botón en Propiedades en la parte inferior de los recursos .sbsar que permite restablecer el recurso a sus valores predeterminados.

* Restablecer el pincel de pintura a sus valores predeterminados

  Se ha añadido un nuevo menú a la sección Pincel en Propiedades que permite restablecer el pincel básico predeterminado.

* Haga clic con el botón derecho para restablecer los parámetros individuales del Substance a sus valores predeterminados

  Se ha añadido la posibilidad de restablecer parámetros individuales dentro de un recurso .sbsar haciendo clic con el botón derecho.

* [Panel Activos] Los activos favoritos del &quot;Pin&quot; aparecen en la parte superior del panel Activos

  Se ha añadido una nueva opción de clic con el botón derecho en los recursos de la biblioteca que permite pin como favoritos en la parte superior del panel. También puede ver todos sus activos favoritos a través de Búsquedas guardadas.

* [Panel Activos] Eliminar, volver a cargar y cambiar el nombre de los activos

  Se han añadido opciones de menú contextual para eliminar, volver a cargar y cambiar el nombre de los activos en la biblioteca del usuario. Se eliminan directamente de la ubicación de su biblioteca en el disco y se vuelven a cargar desde la ubicación original. Los activos que forman parte de un paquete como .abr o .sbsar no se pueden editar individualmente.

* [Selección de color] Añadir modos de fusión al efecto Selección de color
* [Pila de capas] Añadir modo de fusión y opacidad en los filtros
* [Pila de capas] Permitir valores de mosaico mayores que 128 para capas/efectos de relleno
* [Pila de capas] Tapones cilíndricos para proyección cilíndrica en capa de relleno/efecto

  La proyección cilíndrica en Propiedades de capa de relleno ahora tiene la opción de eliminar tapas de cilindro.

* [Log] Mostrar un mensaje de error si los elementos de malla están en espacio negativo al intentar crear un proyecto de Mosaico de UV

  Se ha añadido un mensaje de error más claro al no crear un proyecto de Mosaico de UV porque las partes UV se encuentran en espacios negativos.

* [Project] Indica la versión en el mensaje de error &quot;Datos demasiado recientes&quot; al abrir un proyecto

  Al abrir un proyecto que es demasiado reciente para la aplicación, el mensaje de error indicará ahora la versión del proyecto para que sea más fácil identificar la versión correcta de la aplicación.

* [Ventana gráfica] Permite iluminar la malla desde abajo

  Se ha añadido un nuevo parámetro Alineación del entorno en Configuración de la pantalla > Cámara > Configuración del entorno para alinear la iluminación del mapa de entorno con la cámara cuando se establece en &quot;Local&quot;.

* [Ventana gráfica] Ver R, G, B y Alpha en la ventana gráfica (modo de visualización individual)

  En Configuración de visualización > Configuración de ventana gráfica > Visualización de canal , hay un nuevo ajuste de Canales de color que solo permite mostrar el componente R, G, B o Alpha de un canal en el modo de visualización única.

* [Shader] Permite definir canales de usuario como RGBA en sombreadores de capas de material

  Al definir la configuración de canales del conjunto de texturas dentro de un sombreado para la capa de material, ahora es posible especificar el formato del canal que se va a desviar del valor predeterminado. Esto permite en particular solicitar canales de usuario de color en lugar de solo escala de grises.

* [Exportar] Permitir exportar texturas como SBSAR

  Al exportar texturas a través de la ventana Archivo > Exportar Texturas, se puede elegir el formato de archivo SBSAR (Archivo de Substance) para reagruparlas. El contenido de la SBSAR depende de la plantilla de salida utilizada.
  El formato de archivo SBSAR también se puede establecer en los ajustes preestablecidos de exportación. Cuando se utiliza una configuración híbrida (SBSAR + otro formato), las texturas que tienen como destino un SBSAR se agrupan mientras que el resto se exporta junto a ellas.

* [Exportar] Opción de exposición de 16 bits para EXR formato de archivo

  Al exportar archivos de textura de EXR, ahora es posible elegir 16f bit (medio Flotante) o 32f bit (Flotante) en la ventana Exportar Texturas (tanto para ajustes de exportación como para ajustes preestablecidos de exportación). Los proyectos antiguos y los ajustes preestablecidos de exportación antiguos se establecerán de forma predeterminada en 16f bit para reflejar el comportamiento antiguo.

* [Python] Añadir evento para saber cuándo se modifican los conjuntos de texturas

  El nuevo &quot;substance\_painter.event.TextureStateEvent&quot; permite saber cuándo se ha modificado un conjunto de texturas debido a un trazo de pintura, un nuevo canal añadido o un canal eliminado.

* [Python] Permitir obtener y establecer recursos de mapa de malla en los ajustes de Conjunto de texturas

  Se han añadido nuevas funciones en el módulo &quot;substance\_painter.project&quot; para obtener y definir recursos de mapas de malla. Estas funciones se pueden utilizar para actualizar los mapas de malla a los que hace referencia la configuración de Conjunto de texturas.

* [Plugins] Opción Eliminar para obtener otros plugins de JS

  Se ha eliminado la opción para obtener los complementos de JavaScript, ya que se alojaban en el sitio web obsoleto Compartir .

* [Contenido] Añadir nueva plantilla Roblox y exportar ajuste preestablecido

  Se han añadido una nueva plantilla de proyecto &quot;Material Variant&quot; y &quot;Surface Appearance&quot; de Roblox y un ajuste preestablecido de exportación para facilitar la exportación de texturas PBR a Roblox. Se puede acceder a la plantilla desde la ventana Archivo > Nuevo proyecto.

* Actualizar Substance Engine a la última versión (8.6.3)
* [Steam] Compilación optimizada para chipset Apple Silicon (Apple M1 / M2)

**Corregido:**

* Bloqueo al utilizar 16k exr
* [Bloqueo] Ctrl Z Después de eliminar una instancia de sombreado
* [Iray] El valor de IoR está bloqueado en 1 para algunos sombreadores
* [Win] [Horneando] No se pueden cargar algunos elementos de alta poli
* [Gestión de color] Nombre de espacio de color incorrecto en la IU con filtros
* [Python] Los objetos de recursos devueltos por la función de importación no tienen un tipo

  Al importar un paquete de Substance en Python, la función devolvía el paquete en lugar de sus gráficos. El módulo de recursos ahora proporciona funciones y parámetros para recuperar los gráficos de un paquete de Substance.

**Problemas conocidos:**

* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
* [Pila de capas] El origen de entrada no se guarda por capa
* [Pintura] El suavizado temporal provoca defectos al pintar en algunos casos
* [Exportar] La vista 2D exporta un mapa aleatoriamente uniforme

### 8.1.3

*(Lanzado: 25 de agosto de 2022)*
Resumen: **Versión secundaria de corrección de errores**

**Agregado:**

* Actualizar a Iray SDK 1.6

**Corregido:**

* [Shader] Bloqueo con el sombreador antiguo defectuoso
* [Material Layering] Los materiales pueden desaparecer al reabrir un proyecto

**Problemas conocidos:**

* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* [Pila de capas] El origen de entrada no se guarda por capa
* [Bloqueo] Ctrl Z Después de eliminar una instancia del sombreador
* [Iray] El IoR está bloqueado a 1 para algunos sombreadores

### 8.1.2

*(Lanzado: 19 de julio de 2022)*
Resumen: **Versión secundaria de corrección de errores**

**Agregado:**

* [Auto Unwrap] Nueva opción &quot;Optimizar para mallas orgánicas&quot; para seleccionar el algoritmo de segmentación
* [Tamaño físico] Opciones de unidad de exposición en Nueva configuración de proyecto y proyecto
* [Gestión de color] Usar la pantalla del monitor de forma predeterminada al utilizar ACE
* [Gestión de color] [Python] Tenga en cuenta ACE archivo de ajustes preestablecidos env-var al crear el proyecto
* [Gestión de color] Restablecer la configuración de Gestión de color en la ventana Nuevo proyecto cuando cambie la configuración
* [Gestión de color] Desactivar el acceso a la configuración de OCIO cuando está presente env-var
* [Gestión de color] Actualice de forma segura ACE configuración cuando ya no exista un parámetro
* Actualizar Substance Engine a la versión 8.6.0
* [Exportar] Añada un nuevo ajuste preestablecido de exportación GLTF compatible con Desplazamiento
* [Scripting] [Python] Recuperar información de recursos (incluidos metadatos personalizados)
* [Scripting] [Python] Añadir función a la lista de consulta de nombres de malla por conjunto de texturas
* [Contenido] Añade una nueva plantilla de Blender y exporta un ajuste preestablecido

**Corregido:**

* [MacOS] Bloqueo al iniciar Iray en algunos casos
* [Miniaturas] Las miniaturas de los estantes no se cargan correctamente
* Se omiten varios canales UV
* [Auto Unwrap] Cálculo innecesario al dividir islas largas
* [Auto Unwrap] Opción para evitar las islas alargadas no tomada en cuenta
* [Auto Unwrap] Pérdida de datos adicionales (colores de vértice) al reempaquetar UV
* [UI] Barra de desplazamiento horizontal en la ventana de propiedades cuando está activada la gestión de color
* [Gestión de color] Faltan configuraciones de OCIO substance\_3d\_painter\_standard\_srgb rol
* [Generator] Uso incorrecto de datos de usuario &quot;deshabilitado&quot;
* [Gestión de color] No se debe hacer clic en el menú desplegable Espacio de color no compatible
* [Gestión de color][Sombreador] La anulación de sRGB definida ya no funciona
* [Generator] Uso incorrecto de los datos de usuario &quot;desactivar&quot;
* [Pila de capas] Vistas previas rotas en proyectos de Mosaico de UV
* [Sombreador] La documentación de la API no está completamente actualizada con Normales dobladas
* [Export][Interoperability] No se puede enviar a Stager con caracteres especiales
* [Contenido] Algunas miniaturas de ajustes preestablecidos de pincel están vacías o son demasiado oscuras

**Problemas conocidos:**

* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* [Pila de capas] Las fuentes de entrada no se guardan por capa
* [Bloqueo] Ctrl Z Después de eliminar una instancia del sombreador
* [Iray] El valor de IoR está bloqueado en 1 para algunos sombreadores
* [Sombreador] Bloqueo con sombreador defectuoso

### 8.1.1

*(Lanzado: 28 de junio de 2022)*
Resumen: **Revisión de versión secundaria**

**Agregado:**

* [Pila de capas] Pulsar Alt en la máscara ya no anula la selección de efectos

**Corregido:**

* [Bloqueo] Abrir un proyecto antiguo guardado en modo de vista en solitario
* [Bloqueo] Eliminar un generador en propiedades
* [Ajustes del conjunto de texturas] Se interrumpe la mezcla de normal/Oclusión ambiental y el height con los métodos normales
* [Exportar] La exportación de texturas mediante relleno de difusión genera mapas negros

**Problemas conocidos:**

* [MacOS] Bloqueo al lanzar Iray en Monterey
* [Vista previa en miniatura] Las miniaturas simplificadas no se actualizan cuando se utiliza un anclaje
* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción

### 8.1.0

*(Lanzado: 7 de junio de 2022)*
Resumen: **Versión principal compatible con ICC, escalado de materiales basado en datos de tamaño físico, nuevos bakeres, mejoras en el cuentagotas de color y una amplia gama de contenido adicional**

**Agregado:**

* [Gestión de color] Añadir compatibilidad para perfiles ICC con Adobe Color Engine (ACE)
* [Gestión de color] Añada compatibilidad con &quot;RGB de Adobe 98&quot; como espacio de color de trabajo para ICC
* [Gestión de color] Permitir la configuración de ACE/ICC mediante un archivo de configuración
* [Gestión de color] Permitir la entrada de valores de color lineal en el Selector de color con el modo Heredado
* [Gestión de color] Permite especificar el perfil de color utilizado para seleccionar el color fuera de la interfaz de usuario
* [Gestión de color] Recordar el último valor de visualización elegido en la ventana gráfica
* [Gestión de color] [Substance] Hacer que los generadores/filtros funcionen correctamente con la gestión de color
* [Gestión de color][Substance] Añadir nuevas palabras clave de anulación de espacio de color $working y $standardsrgb
* [Tamaño físico] [Motor] Extraer información de tamaño físico de la malla
* [Tamaño físico] [Motor] Cálculo del Tamaño físico
* [Tamaño físico] Opciones de exposición para utilizar tamaño físico en la interfaz de usuario
* [Tamaño físico] Añadir ayudantes visuales en la ventana gráfica
* [Haciendo un bake] Añadir baker de Height
* [Haciendo un bake] baker Agregar Normales dobladas
* [Hacer un bake] Añadir baker de opacidad
* [Cuentagotas] Nueva previsualización del cuentagotas de color junto al ratón y gestión del color
* [Cuentagotas] El panel del selector de color vuelve a aparecer en su última posición cuando se vuelve a abrir
* [Cuentagotas] Un nuevo icono para el Selector de material
* [Cuentagotas] Color para administrar la vista previa del canal del selector de color
* [Cuentagotas] Añada la funcionalidad de hacer clic para seleccionar al cuentagotas
* [Cuentagotas] El selector de material ya no activa los canales no activos
* [Cuentagotas] Permitir el uso del cuentagotas con un método abreviado
* [Cuentagotas] El cuentagotas selecciona el canal correspondiente, cuando corresponde
* [Cuentagotas] Al entrar en el modo del selector de color se desactivan todos los métodos abreviados
* [Cuentagotas] Eliminación de la selección automática del campo hexadecimal
* [Cuentagotas] No cerrar el panel al utilizar el selector de material
* [Cuentagotas] Nuevo estado deshabilitado cuando el canal no está disponible para seleccionar
* [Export] Añadir atributo de tangente a la exportación glTF
* Actualizar Substance Engine a v8.4
* Actualizar Auto Unwrap a 0.9.0
* Actualizar a Qt 5.15.8
* Actualizar a Python 3.9
* [Sombreado] Añadir compatibilidad con el sombreado de normales dobladas
* [MacOS] Compatibilidad con SpaceMouse de conexión 3D
* [Python] Documentar la versión de Python utilizada en la API
* [Contenido] Añade 6 nuevos sonidos 3D con 105 ajustes preestablecidos
* [Contenido] 20 nuevos mapas de suciedad y 2 patrones de pliegues de tela
* [Contenido] Actualizar el ajuste preestablecido &quot;Mapas de malla&quot; para utilizar nuevos bakeres
* [Contenido] La Pendiente de desenfoque y el filtro de deformación dependen de la resolución del conjunto de texturas
* [Contenido] Actualizar proyectos de muestra para utilizar los 3 nuevos panaderos

**Corregido:**

* [glTF] No se puede abrir glTF con un carácter especial
* [Motor] Artefactos con anisotropía y SVT desactivados
* [MacOS] [M1] Los materiales inteligentes no se muestran correctamente
* [Procesamiento de malla] No se pueden importar mallas desde Modeler
* [UI] Barra de desplazamiento horizontal en la ventana de nuevo proyecto con la gestión de color habilitada
* [Gestión de color] Falta el valor del espacio de trabajo en el selector de color con algunas configuraciones de OCIO
* [Gestión de color] La previsualización del pincel en la ventana gráfica no tiene gestión de color
* [SpaceMouse] La tabla dinámica no se actualiza inmediatamente con el cambio de enfoque y, a veces, se sale del modelo
* [Export][USD] Los archivos USD exportados tienen una estructura incorrecta
* [USD] Problema de Oclusión ambiental al exportar
* [Contenido] Actualice la malla de la miniatura para que coincida con el proyecto de ejemplo Previsualizar esfera

**Problemas conocidos:**

* La exportación de texturas mediante relleno de difusión produce mapas negros
* La mezcla de Oclusión normal/ambiental no funciona
* [MacOS] Bloqueo al iniciar Iray en algunos casos excepcionales
* [Vista previa en miniatura] Las miniaturas simplificadas no se actualizan cuando se utiliza un delimitador
* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción

## Versión 7

### 7.4.3

*(Lanzado: 11 de abril de 2022)*
Resumen: **Corrección de error compatible con SpaceMouse de conexión 3D en la ventana gráfica 2D**

**Agregado:**

* [SpaceMouse] Compatibilidad con SpaceMouse de conexión 3D en la ventana gráfica 2D

**Corregido:**

* [Selector de color] No se puede escribir en campos hexadecimales
* [Gestión de color] Los recursos utilizados en el modo de proyección no se administran por color en la superposición
* [Gestión de color] No se notifican errores en el registro
* [SpaceMouse] Quitar mensaje de error genérico si el usuario no tiene un SpaceMouse
* [SpaceMouse] Al cargar un proyecto, el punto de giro siempre está oculto
* [Panaderos] El ajuste &quot;Normal promedio&quot; no tiene efecto en los proyectos de azulejo UV
* [Mosaico UV] Las superposiciones de mosaicos uv inactivos desaparecen al volver a cargar mallas con diferentes mosaicos
* [Scripting] [Python] La secuencia de comandos remota no funciona
* [Scripting] [Python] No se pueden consultar varios canales desde la API y se produce un error.
* [Scripting][Python] Bloqueo al utilizar el evento ProjectEditionEntered
* [Scripting][Python] Bloqueo al llamar a get\_active\_stack()

**Problemas conocidos:**

* Conexión 3D con SpaceMouse no compatible en MacOS
* [UI] Barra de desplazamiento horizontal con administración de color que aparece en algunos casos en la ventana de nuevo proyecto
* [Mac M1] Los materiales inteligentes no se muestran correctamente

### 7.4.2

*(Lanzado: 8 de marzo de 2022)*
Resumen: **Corrección de error compatible con SpaceMouse de conexión 3D y mejoras en la administración de color (OCIO)**

**Agregado:**

* [SpaceMouse] [Windows] Compatibilidad con la conexión 3D de SpaceMouse en el área de visualización 3D para la navegación
* [SpaceMouse] [Windows] Métodos abreviados/teclas básicos para los modelos Pro y Enterprise SpaceMouse en la ventana gráfica 3D
* [SpaceMouse] [Windows] Icono de centro de rotación dedicado en la ventana gráfica 3D
* [Gestión de color] Utilice las funciones de la configuración de OCIO para cambiar la configuración predeterminada
* [Gestión de color] Gestión de color de la ventana de propiedades para widgets de color
* [Gestión de color] Gestión de color de la ventana de propiedades para la previsualización de materiales
* [Gestión de color] Gestión de color de muestras en el selector de color
* [Gestión de color] Añadir un ajuste para definir el espacio de color sRGB estándar
* [Gestión de color] Añadir el espacio de color sRGB estándar desde la configuración de OCIO en el selector de color Lista de selectores de visualización
* [Gestión de color] Mejoras en el menú de anulación del espacio de color
* [Gestión de color] Permita anular el espacio de color del mapa de entorno en Ajustes de visualización.
* [Gestión de color] Dibujo de degradados del selector de color en función de la visualización actual
* [Gestión de color] Fijar valores HDR de forma predeterminada en el editor de color
* [Gestión de color] Usar passthrough (sin espacio de color) para filtros en modo heredado
* [Gestión de color] Limitar la visualización de degradados en el editor de color para que coincidan con el rango [0-1]
* [Gestión de color] Ocultar el selector de visualización en el selector de color en el modo Heredado
* [Administración de color] Convertir el campo hexadecimal del selector de color siempre en espacio de color sRGB
* [Gestión de color] Desactivar el menú desplegable de visualización del selector de color para canales de datos
* [Optimización] La cuadrícula de deformación vuelve a calcular únicamente los mosaicos UV cubiertos
* [Exportar] Permite exportar proyectos de azulejo UV para Sketchfab, USD y glTF
* [Scripting][Python] Permitir el cambio de la función de asignación de tonos

**Corregido:**

* [Sketchfab] Al actualizar el modelo existente, se crea un nuevo modelo
* [Sketchfab] Bloqueo al buscar un modelo actualizado anteriormente
* Bloqueo al exportar a USD
* Bloqueo al crear una nueva instancia de sombreado en Máscara de geometría o cuando la geometría está oculta
* [Ventana Importar recurso] Bloqueo al cambiar el tipo de recursos importados
* Los mapas de malla normales se invierten cuando se utilizan en la pila de capas
* [Substance] No se tiene en cuenta el modo de fusión de datos de usuarios
* [Gestión de color] Los mapas de bits con espacio de color en el nombre de archivo se importan como secuencias de mosaico UV
* [Gestión de color] Las salidas con gestión de color del gráfico del Substance están en un espacio de color incorrecto
* [Gestión de color] La herramienta Relleno poligonal muestra un color incorrecto
* [Gestión de color] El asignador de tonos ACES se aplica a los canales en modo solo
* [Gestión de color] La previsualización de la iluminación de la esfera de la herramienta no está gestionada por color
* [Administración de color] [Exportar] Los mapas convertidos aplican una conversión incorrecta
* [Scripting][Python][Gestión de color] Los proyectos creados con plantillas y variables de entorno OCIO están en modo heredado
* [Scripting] [Python] No se puede utilizar la función de evaluación de JavaScript al inicio
* [Oferta de Adobe 3D] No se puede iniciar Painter si se utiliza la configuración regional con idiomas no admitidos de forma predeterminada

**Problemas conocidos:**

* Conexión 3D con SpaceMouse no compatible en MacOS
* [UI] Barra de desplazamiento horizontal con administración de color que aparece en algunos casos en la ventana de nuevo proyecto
* [Panaderos] El ajuste &quot;Normal promedio&quot; no tiene efecto en los proyectos de azulejo UV
* [Mac M1] Los materiales inteligentes no se muestran correctamente
* [Gestión de color] Los recursos utilizados en el modo de proyección no se administran por color en la superposición
* [Selector de color] No se puede escribir en campos hexadecimales

### 7.4.1

*(Lanzado: 14 de diciembre de 2021)*
Resumen: **Corrección de error con mejoras en la administración de color**

**Agregado:**

* [Gestión de color] Usar función de datos en nombres de archivo exportados
* [Gestión de color] Expanda la sección Gestión de color de forma predeterminada cuando OCIO está seleccionado en las nuevas ventanas de configuración de proyecto y proyecto
* [Gestión de color] Añadir ACES a un asignador en modo heredado
* [Gestión de color] Ajustar los valores de configuración predeterminados
* [Gestión de color][Exportar] Rellenar $colorSpace en nombres de archivo para canales de datos
* [Exportar] Exportar proyecto de azulejo UV a Stager
* [Interoperabilidad] No disponible para las ediciones Steam y Substance
* [Interoperabilidad] Permitir el envío de un proyecto de mosaico UV a Stager

**Corregido:**

* [MacOS] [Bloqueo] Painter no se inicia con Catalina
* [Administración de color] [Bloqueo] Bloqueo aleatorio al reproducir con administración de color/tipo de datos en el canal de usuario
* [Gestión de color] Recursos utilizados como escala de grises en la máscara visualización del espacio de color nuevo menú
* [Gestión de color] El canal del usuario es más oscuro en la ventana gráfica en el modo heredado + vista en solitario
* [Gestión de color] El mapa Env siempre es lineal cuando se utiliza en iRay
* [Gestión de color] El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
* [Gestión de color] El selector de color se interrumpe en el interior de un Substance en modo heredado
* [Gestión de color] Al cambiar entre vistas de canal solo en la ventana gráfica, no se muestra con el espacio de color correcto al utilizar el menú desplegable
* [Gestión de color] La exportación aplica la conversión incorrecta en canales de usuario con gestión de color en modo heredado
* Los trazos realizados en la máscara de vista solo no se muestran al volver a la vista de material
* [Exportar] Los mapas convertidos no se exportan como canales con gestión de color
* [Conjunto de texturas] Falta la información sobre herramientas con el nombre original en los canales de usuario con nombre cambiado
* [Steam] Faltan archivos al comprobar su integridad con Steam

**Problemas conocidos:**

* [Mac M1] Los materiales inteligentes no se muestran correctamente

### 7.4.0

*(Lanzado: de noviembre de 2021)*
Resumen: **Versión principal. Introducción de la primera versión de la administración de color, desacoplar vista 2D o 3D, nueva opción de desempaquetado UV automático para evitar islas alargadas, llamar a funciones de JavaScript desde la API de Python y nuevo contenido**

**Agregado:**

* [Gestión de color] Compatibilidad con la gestión de color OpenColorIO versión 2
* [Gestión de color] Añadir ajustes de gestión de color a los ajustes del proyecto
* [Gestión de color] Ventana de advertencia sobre los cambios de configuración de la gestión de color al abrir un proyecto
* [Gestión de color] Mostrar un mensaje de error si se selecciona un archivo de configuración de OCIO no válido
* [Gestión de color] Permite anular la configuración con la variable de entorno OCIO
* [Gestión de color] Varias configuraciones OCIO integradas de forma predeterminada en la aplicación
* [Gestión de color] Extraer nombre de espacio de color del nombre de archivo de mapa de bits importado
* [Gestión de color] Permita anular el espacio de color con un espacio de color desde la configuración de la ventana Propiedades
* [Gestión de color] Añadir opciones de gestión de color en Configuración del conjunto de texturas
* [Gestión de color][Ventana] Permitir la gestión de color de vistas 2D y 3D por separado
* [Gestión de color] Cargar y convertir mapa de entorno en el espacio de color de trabajo
* [Gestión de color] Ajuste el selector de color y el editor con el espacio de color actual
* [Gestión de color] Permite seleccionar el espacio de color de transformación de visualización en la ventana gráfica con un nuevo menú desplegable.
* [Gestión de color] Aplicación de la transformación de visualización con resultados de procesamiento de Iray
* [Gestión de color] Exportar texturas con diferentes espacios de color
* [Gestión de color] [Python] Aplicación de la configuración de gestión de color de la variable de entorno (OCIO) a proyectos nuevos
* [Ventana gráfica] Permite desacoplar la ventana gráfica 2D o 3D
* [Auto Unwrap] Nueva opción para evitar islas alargadas
* [Scripting Python] Llamar a funciones de JavaScript desde la API de Python
* [Nueva ventana de proyecto] Hacer que la sección de mapas importados sea contraíble
* [Proyección][Deformar] Permite ocultar las normales como una opción en los ajustes de Deformación
* [Contenido] 11 nuevos mapas de suciedades
* [Contenido] 8 nuevos ajustes preestablecidos de herramientas (cremallera, cordón de apriete, brillo)
* [Contenido] 8 materiales nuevos (cicatriz, bolsillo, ...)
* [Contenido] 1 generador nuevo (inflar encogimiento)

**Problemas conocidos:**

* [Mac M1] Los materiales inteligentes no se muestran correctamente
* [Administración de color] [Bloqueo] Bloqueo aleatorio al reproducir con administración de color/tipo de datos en el canal de usuario
* [Gestión de color] El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
* [Gestión de color] [Iray] Guardar el renderizado en EXR o TIFF mientras la Gestión de color está activada en la ventana gráfica siempre se guarda en lineal
* [Administración de color] Los recursos utilizados como escala de grises en la máscara muestran un menú de espacio de color incorrecto
* [Gestión de color] [Iray] El mapa Env siempre es lineal cuando se usa en Iray
* [Gestión de color] [Exportar] Los mapas convertidos no se exportan como canales con gestión de color
* [Gestión de color] [Exportar] La exportación ignora si el canal del usuario tiene gestión de color o no está en modo heredado

### 7.3.1

*(Lanzado: de noviembre de 2021)*
Resumen: **Corrección de error**

**Agregado:**

* [Proyección] La escala solo debería funcionar en el espacio de objetos

**Corregido:**

* [Mac M1] Las capas de materiales no funcionan
* [Mac M1] [Proyección] La deformación no funciona
* Los detalles del micro no se muestran correctamente
* [Proyección] [Bloqueo] Cambio al modo de deformación con una capa creada con una versión anterior
* [Proyección] [Deformar] El giro no funciona cuando la transformación se establece en espacio de entorno
* [Proyección] [Deformar] La opción Dividir permanece seleccionada después de realizar la división
* [Proyección] [UV] El punto de giro se restablece al voltear la proyección
* [Filter] El entorno de Bake Lighting cambia al volver a cargar o cambiar un parámetro
* [Interoperabilidad] No disponible para las ediciones Steam y Substance
* [Interoperabilidad] El botón &quot;Examinar recursos 3D en el mercado&quot; siempre debe abrir el CCD en la pestaña 3D de Stock y Mercado

**Problemas conocidos:**

* [Mac M1] Los materiales inteligentes no se muestran correctamente

### 7.3.0

*(Lanzado: 13 de octubre de 2021)*
Resumen: **Versión principal. Contiene una nueva proyección de deformación 3D, una nueva proyección cilíndrica, mejoras del selector de color, nuevas funciones en la API de Python y correcciones de errores**

**Agregado:**

* [Proyección] [Deformar] Exponer deformación 3D como un nuevo modo de proyección
* [Proyección] [Deformar] Permitir el modo de pegatina para Alpha, texturas y procedimientos con la función de arrastrar y soltar en la ventana gráfica
* [Proyección] [Deformar] Utilice la proyección de deformación con el método abreviado de pegatina (ALT)
* [Proyección][Deformar][Barra de herramientas] Transformar deformación como completa o por vértices
* [Proyección][Deformar][Barra de herramientas] Añadir puntos de cuadrícula con opciones de deformación dividida en sentido cruzado, horizontal o vertical
* [Proyección][Deformar][Barra de herramientas] Menú específico para acciones de restablecimiento
* [Proyección][Deformar][Barra de herramientas] Opción para ajustar automáticamente las tangentes al mover puntos
* [Proyección][Deformar][Barra de herramientas] Menú específico para la edición de la cuadrícula (tamaño, restablecimiento, color y tamaño del control)
* [Proyección] [Deformar] Nuevo método abreviado de teclado para cambiar el modo de edición de deformación de vértices completos (MAYÚS+V)
* [Proyección] [Deformar] Al pulsar+Ctrl se puede cambiar entre la herramienta Superficie y otras herramientas
* [Proyección] [Cilíndrica] Exponer el modo de proyección cilíndrica
* [Proyección][Barra de herramientas] Configuración del manipulador de grupos (tamaño, pasos de cuadrícula, pasos de ángulo)
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
* [Mac M1] Los materiales inteligentes no se muestran correctamente
* [M1][Regresión] Las capas de materiales no funcionan

### 7.2.3

*(Lanzado: 24 de agosto de 2021)*
Resumen: **Versión secundaria, corrección de errores**

**Agregado:**

* [Bibliotecas] Agregar una forma de excluir archivos no deseados del rastreo

**Corregido:**

* [Windows] Problemas de suspensión y varias pantallas
* [MacOS] [Bloqueo] Cambio del sombreado al utilizar efectos
* [Ventana gráfica] El modo de previsualización completa ya no muestra el cursor del pincel sin alfa
* [UI] El widget de ángulo gira en la dirección equivocada
* [Pila de capas] Muchas subcarpetas crean bloqueos muy largos
* [Iray] Diferentes puntos de vista en Iray y OpenGL: Visible si no funciona
* [Iray] El índice de refracción no se tiene en cuenta y no aparece en las propiedades de mdl
* [JavaScript] ShowExportDialog() nunca devuelve true
* No se puede leer mtl desde Adobe Stock

### 7.2.2

*(Lanzado: 27 de julio de 2021)*
Resumen: **Versión secundaria, corrección de errores**

**Agregado:**

* Actualizar la versión de requisitos de controlador AMD

**Corregido:**

* [Mac M1] Detección de memoria incorrecta
* [Exportar] Los trazados muy largos no se muestran correctamente

**Problemas conocidos:**

* [Contenido] Sombreadores obsoletos de las muestras

### 7.2.1

*(Lanzado: 2 de julio de 2021)*
Resumen: **Versión secundaria, revisión**

**Agregado:**

* [Interop] Añada información sobre herramientas para indicar que el envío de proyectos de UV Tile a Stager aún no es compatible
* [Plugin][UI] Actualización del icono de Livelink

**Corregido:**

* [Nvidia] La versión del controlador que comienza por 30 se considera obsoleta
* [Bibliotecas] El estado del panel Activos no se guarda a menos que esté abierto un proyecto
* [Bibliotecas] La nueva búsqueda guardada conserva la palabra clave de la antigua búsqueda guardada
* [Bakers] [UVTiles] Los mapas de ID por meshID también tienen en cuenta los mosaicos UV
* [Exportar] Los archivos gLTF no importan el color del vértice
* [Iray] Faltan algunas sugerencias
* [Interop] Enviar a Stager no siempre está desactivado cuando Stager no se detecta
* [Resource Updater] No se puede actualizar el fabricante de pinceles de Photoshop
* [Contenido] Generador de desgaste de borde de fibra de vidrio roto

### 7.2.0

*(Lanzado: 23 de junio de 2021)*
Resumen: **Versión principal, proporciona una actualización del panel de activos, un nuevo sombreado con acceso a nuevos canales y parámetros, una actualización general de la interfaz de usuario, algunas mejoras de rendimiento muy solicitadas, compatibilidad de idioma ampliada y mucho más.**

**Agregado:**

* [Bibliotecas] Nuevo panel Activos para sustituir el estante
* [Bibliotecas][IU] Nuevo diseño del panel Activos
* [Bibliotecas][IU] Cambiar la orientación y la interfaz de usuario predeterminadas del panel Activos
* [Bibliotecas][IU] Introducir una opción de vista de lista en la biblioteca
* [Bibliotecas] [IU] Nueva navegación de rutas de navegación en el panel Activos
* [Bibliotecas][UI] Seleccione &quot;Todas las bibliotecas&quot; al seleccionar una búsqueda guardada
* [Bibliotecas] [IU] Seleccione &quot;Todas las bibliotecas&quot; cuando se anule la selección de todas las carpetas
* [Bibliotecas][IU] Nueva etiqueta para pinceles de partículas
* [Bibliotecas] [IU] Se ha sustituido &quot;estantería&quot; por &quot;Todas las bibliotecas&quot; en la aplicación.
* [Bibliotecas][IU] Permitir ocultar carpetas vacías
* [Bibliotecas][UI] La biblioteca de usuario predeterminada debe estar visible aunque esté vacía.
* [Bibliotecas][IU] Nuevo método de filtrado mediante iconos de tipos de activos
* [Bibliotecas] Método abreviado de teclado &quot;CTRL&quot; para seleccionar varios tipos de recursos
* [Bibliotecas] Nueva variable de entorno para controlar el presupuesto de memoria de previsualización de activos
* [Bibliotecas][Contenido] Nuevos mapas de entorno
* [Bibliotecas][Contenido][IU] desplazamiento de procesamiento en los materiales predeterminados
* [Bibliotecas][Contenido] Establezca el sombreado de Adobe Standard Material (ASM) como predeterminado para la generación de vistas previas
* [Bibliotecas][Contenido][ASM] Nuevas plantillas de proyecto para el nuevo sombreador de ASM
* [Bibliotecas][Miniatura] Usar nuevo mapa de entorno de Studio 6
* [Bibliotecas][Miniatura] Lea la miniatura del recurso en lugar de generarla
* [Bibliotecas][Miniatura] Añadir desplazamiento a la generación de miniaturas
* [Ajustes del conjunto de texturas]
* [Ajustes del conjunto de texturas][IU] Exponer el nuevo height al método de conversión normal
* [Ajustes del conjunto de texturas] [IU] Reorganización de la IU de los canales
* [Ajustes del conjunto de texturas] El límite de canales de usuario se eleva a 16 canales
* [Ajustes del conjunto de texturas] [IU] Indica qué canales son compatibles con el sombreado seleccionado actualmente
* [Shader][ASM] Nuevo sombreador de Adobe Standard Material
* [Shader] [ASM] Se ha agregado compatibilidad con Anisotropía, capa transparente, dispersión subsuperficial, Specular edge color y brillo
* [Shader][ASM] Cambiar los valores de color de los canales predeterminados
* [Shader][ASM][Export] Plantilla de exportación actualizada de Adobe Dimension a Adobe Substance 3D Stager
* [Shader] [ASM] Se han añadido etiquetas y sugerencias de herramientas para los parámetros de sombreado y MDL
* [Shader][ASM] Haga visible el color de la Dispersión en la vista 2D aunque no se admita SSS
* [Shader][ASM][Iray] Se admite el sombreado de ASM en Iray con el nuevo MDL.
* [Shader][ASM][Iray] Dispersión subsuperficial actualizada en brillo y revestimiento de especificaciones PBR heredadas
* [Shader][ASM][Content] Se ha cambiado el tipo de SSS predeterminado para las muestras.
* [Shader][ASM] Se ha añadido documentación para la API de ASM
* [Shader][ASM] Optimizar sombreadores para ignorar los canales no utilizados
* [Shader] Exponer nuevos canales de conjunto de texturas
* [Shader] Dispersión subsuperficial mejorada
* [Shader] Se han ocultado nuevos parámetros de sombreado para algunos sombreadores.
* [Shader] Visible si para parámetros de sombreado
* [Rendimiento]
* [Bibliotecas] Mejoras en el tiempo de carga y el rendimiento de cálculo de la vista previa de recursos
* [Motor] Mejoras en el rendimiento de pintura
* [Auto Unwrap]
* [Auto Unwrap] Mejoras en el rendimiento del Empaquetado
* [Auto Unwrap] Auto unwrap compatible con el flujo de trabajo de UV Tile
* [Auto-Unwrap] Nueva opción para colocar las coordenadas UV según la orientación de la malla
* [Otros]
* [Configuración] Se ha cambiado la dirección de zoom predeterminada
* [UI] Actualización general de la IU
* [UI] Repaso del menú Ayuda
* [UI] Reemplazar el icono de inversión
* [UI][Complemento] Icono Reemplazar para el vínculo de dcc del complemento
* [UI][AMD] Mensaje emergente y versión mínima requerida de actualización
* [Pila de capas] Crear una nueva capa dentro de la carpeta vacía seleccionada
* Actualizar documentación de Python
* [Marca]
* [Branding][UI] Se ha actualizado el nombre de la aplicación a Adobe Substance 3D Painter.
* [Marca][IU] Se ha actualizado la versión independiente a &#39;Edición de Substance&#39;
* [Marca][IU] Se ha actualizado el nombre del ejecutable de la aplicación, la ruta de instalación, el paquete y los iconos
* [Branding][UI] Se ha cambiado el nombre de la biblioteca y la ruta predeterminadas
* [Branding][UI] Acerca de la ventana
* [Branding][UI] Pantalla de bienvenida actualizada
* [Marca][IU] Se ha eliminado el número de versión anual
* [Localización] Nuevas traducciones en alemán, francés y chino simplificado
* [Interoperabilidad] No disponible para las ediciones Steam y Substance
* Interoperabilidad con el ecosistema de Adobe: Designer, Sampler, Stager y Bridge
* [Interoperabilidad] [IU] Recibir y actualizar recursos de Designer
* [Interoperabilidad] [IU] Recibir recursos de Sampler
* [Interoperabilidad][IU] Enviar el recurso a Stager
* [Interoperabilidad][IU] Mostrar en Adobe Bridge
* [Interoperabilidad][IU] Permitir el acceso rápido a Adobe 3D Assets
* [Interoperabilidad] Nuevas etiquetas de uso de sbsar
* [Interoperabilidad] Gestionar tipos de activos recibidos
* [Interoperabilidad] Los recursos recibidos de Adobe Substance 3D Designer o Adobe Substance 3D Sampler se almacenan en la biblioteca predeterminada elegida por el usuario
* [Interoperabilidad][UI] Nuevo icono en la barra de herramientas de la izquierda para enviar a Stager o Photoshop

**Corregido:**

* [Tablet] Bajo rendimiento al pintar con presión
* [Tablet] Problema en tabletas con controles deslizantes
* [Bloqueo] El nombre no coincide entre la lista de conjuntos de texturas y el exportador
* [Bloqueo] [Bibliotecas] Haga doble clic en una subbiblioteca
* [Bibliotecas] Problema al rastrear directorios de bibliotecas
* [Bibliotecas] La línea de comandos de generación de vista previa forzada no funciona del modo esperado
* [Bibliotecas][Contenido] El filtro Entorno de luz horneada está en negro de forma predeterminada
* [Linux][MacOS][Export Mesh] No se puede importar glTF creado en Linux/MacOS
* [Linux] Arrastrar y soltar un archivo en el panel Activos puede provocar un bloqueo
* [Auto-Unwrap] Auto-Unwrap está disponible incluso si no se ha seleccionado una malla para recargar
* Comportamiento incorrecto de las partículas con la gravedad
* [Pila de capas] El histograma de niveles solo puede utilizar Luminancia con algunos canales
* [Máscara de geometría] El menú contextual de una carpeta al editar la máscara de geometría no funciona
* [Proyección] Costura con proyección esférica y filtrado bilineal
* [UV Tiles] Exportar máscara a archivo solo exporta el mosaico 0, 0
* [Exportar malla] La exportación de malla FBX está vacía
* [Iray] El mapa normal no se tiene en cuenta en los nuevos proyectos al procesar
* [Guardar] Guardar problemas en unidades compartidas
* [Horneado] Al volver a hornear una malla con parámetros modificados, se muestra una advertencia
* [Horneado] [Regresión] Resultado incorrecto cuando el cuadro delimitador global de mallas de poli altas no incluye el origen de la escena
* [Python] Las bibliotecas de usuarios personalizados no se tienen en cuenta

**Problemas conocidos:**

* [Bibliotecas] Las búsquedas guardadas no se guardan si no hay ningún proyecto abierto
* [NVIDIA] Mensaje para el controlador obsoleto incluso si el controlador está actualizado

### 7.1.1 (2021.1.1)

*(Lanzado: de marzo de 2021)*
Resumen: **Versión secundaria, corrección de errores con posibilidad de introducir valores hexadecimales en el selector de color**

**Agregado:**

* [Log] Advertencia a los usuarios sobre los controladores de GPU AMD incompatibles
* [Selector de color] Permita escribir valores hexadecimales

**Corregido:**

* [Baker] Disminución del rendimiento
* [Máscara de geometría] Pulsar Alt en el nombre de la malla puede provocar un bloqueo
* [Motor] La pintura no actualiza toda la vista cuando es necesario
* [Pila de capas] La selección se bloquea tras cambiar el sombreado
* [MacOS] [Selector de color] El color es ligeramente diferente del que se ha seleccionado
* [Export] El uso del formato de archivo de PSD no genera un archivo por Mosaico de UV
* [Scripting][Javascript] alg.mapexport.getPathsExportDocumentMaps() no devuelve todos los valores
* [Scripting] [Python] Los complementos deshabilitados se vuelven a habilitar al volver a abrir Painter

### 7.1.0 (2021.1.0)

*(Lanzado: de enero de 2021)*
Resumen: **Versión principal, nueva máscara de geometría que permite seleccionar y pintar partes de la geometría, copiar y pegar efectos en la pila de capas, mejorar el flujo de trabajo del azulejo UV, actualizar Iray, Bakers, Substance Engine y nuevo contenido**

**Agregado:**

* Nueva máscara de geometría y pinte las partes seleccionadas de la geometría
* [Máscara de geometría] Permite pintar las partes seleccionadas de la geometría por nombres de malla
* [Geometry Mask] Selección rectangular en ambas ventanas gráficas
* [Máscara de geometría] Permite ocultar/ignorar la geometría excluida en cualquier capa
* [Máscara de geometría][Propiedades] Selección rápida de casillas de verificación al hacer clic y arrastrar
* [Geometry Mask][Properties][UI] Include/Exclude all con un menú desplegable en la ventana Propiedades
* [Máscara de geometría][Propiedades] Permite seleccionar rápidamente un elemento de una lista con ALT+CLIC IZQUIERDO
* [Máscara de geometría][Propiedades] Superposición en las ventanas gráficas al pasar el cursor por los nombres/Mosaicos de UV de malla en la ventana Propiedades
* [Máscara de geometría] [Pila de capas] Añadir opciones de Copiar/Pegar a la máscara de geometría
* [Máscara de geometría] Nuevo icono para el botón Ocultar/ignorar geometría excluida
* [Máscara de geometría] Nueva información sobre herramientas para Ocultar/ignorar geometría excluida
* [Máscara de geometría] Método abreviado de teclado ALT + H para activar o desactivar el botón &quot;Ocultar geometría excluida&quot;.
* [UV Tiles] [Layer Stack] Nueva miniatura de vista previa de la esfera de capa de relleno para UV Tiles y modo simplificado
* [Mosaicos de UV][Pila de capas] Permite salir fácilmente de la máscara de Mosaico de UV
* [Mosaicos UV][Lista de conjuntos de texturas] Permite proporcionar una descripción por mosaico UV
* [UV Tiles][Texture Set Settings][UI] Dos nuevos títulos de sección en el menú desplegable para cambiar la resolución del azulejo UV
* [Mosaicos de UV] [Ventana gráfica] Salir de la máscara de Mosaico de UV al arrastrar un material a la ventana gráfica
* [Pila de capas] Añadir opciones de Copiar/Pegar para efectos
* [Pila de capas] Permite copiar y pegar efectos de un conjunto de texturas a otro
* [Pila de capas] Permitir selección múltiple de efectos
* [Pila de capas] Añadir opciones de copiar y pegar como métodos abreviados de efectos de capa
* [Pila de capas] Cambiar automáticamente entre máscara y contenido al arrastrar efectos a otra capa
* [Pila de capas] Crea automáticamente una máscara al pegar una máscara de otra capa
* [Pila de capas] Añada acciones de mover efectos dentro del menú contextual del botón derecho de los efectos
* [Pila de capas] Permite arrastrar y soltar efectos de una capa a otra
* [Pila de capas] Al arrastrar elementos a una carpeta, se colocan en la parte superior de la carpeta
* Actualizar Iray a la versión 2020.1.0
* [Bakers] Actualice Bakers a la versión 2.5.4
* [Bakeres] Mostrar Mosaicos de UV individuales en la ventana de progreso de hacer un bake
* [Bakers][UI] Permite hornear rápidamente el conjunto de texturas actual con un nuevo botón
* [Panaderos] Permite al usuario seleccionar rápidamente uno de los panaderos con ALT+CLIC IZQUIERDO
* Actualizar Substance Engine a la versión 8.0.8
* [Substance Engine] Compatibilidad con el color predeterminado en los nuevos archivos .sbsar
* [Auto Unwrap] Mejora del rendimiento
* [Exportar] Añada comentarios visuales para indicar qué resolución del azulejo UV difiere de la predeterminada del proyecto
* [Exportar] Añada el factor de tamaño de escena al archivo json de sombreado exportado
* [Idioma] Añadir traducción al japonés
* [UI] Ventana Actualización Acerca de con control de versiones de dependencias internas
* [Scripting][Python] Permita administrar recursos de Shelf
* [Scripting] [Python] Permite saber cuándo un proyecto está listo para su procesamiento y exportación
* [Scripting] [Python] Permite saber cuándo un Shelf ha terminado de rastrear recursos en el disco
* [Scripting] [Python] Permite consultar la lista de mosaicos UV por conjuntos de texturas
* [Scripts] [Python] Permite asignar una vista previa personalizada a los recursos de la estantería
* [Scripting] [Python] Permita administrar estantes personalizados
* [Scripting] [Python] Agregue un índice de método en cada submódulo de la documentación
* [Scripting] [Python] Nuevo estilo para la documentación
* [Scripting] [Python] Mejora de los recursos y de la documentación de la estantería
* [Contenido] Tres nuevos ajustes preestablecidos de herramientas para realizar puntos de sutura
* [Estante] Quitar temporalmente &quot;Exportar a Substance share&quot; al realizar la transición a la nueva plataforma de Substance share

**Corregido:**

* Bloqueo al utilizar monitores con diferentes resoluciones
* Bloqueo en Substance Engine con algunos proyectos raros
* La actualización de la ventana gráfica falla con Ocultar/Ignorar geometría excluida al cambiar de capa
* [Vista 2D] Puede que falte la ventana 2D en algunos proyectos
* [Horneado] &quot;Coincidir por nombre de malla&quot; ignora partes del objeto
* [Pila de capas] Al hacer clic en un efecto de capa se abre la carpeta
* [Máscara de geometría] El azulejo UV se sigue contando en la máscara, incluso al volver a importar la malla sin ella
* [Máscara de geometría] El menú contextual de la ventana gráfica no proporciona las herramientas correctas
* [Motor] Grandes retrasos en proyectos concretos
* [Scripting] Alta latencia con solicitudes remotas de POST JSON en Windows
* [Linux] La cantidad de Vram no se detecta correctamente con GPU integradas específicas
* [Auto Unwrap] Bloqueos o desempaquetado prolongado en algunos proyectos

## Versión 6

### 6.2.2 (2020.2.2)

*(Lanzado: de septiembre de 2020)*
Resumen: **Versión secundaria, corrección de errores con algunas funciones en la API de Python**

**Agregado:**

* [Rendimiento] No calcular todos los Mosaicos de UV al utilizar la selección de ID de color
* [Bakeres][IU] Visualización de descripciones de conjuntos de texturas
* [Bakeres] Permitir guardar la configuración de hacer un bake
* [Bakeres] Añada las opciones contraer todo/expandir todo a la pestaña Selección
* [Lista de conjuntos de texturas] Ocultar descripción cuando está vacía
* [Mosaicos de UV][Lista de conjuntos de texturas] Al hacer clic en el Mosaico de UV, se expande o se contrae la lista.
* [Export][UI] Permite cambiar el tamaño horizontal del panel Lista de conjuntos de texturas
* [Exportar] [IU] Texto de información sobre herramientas coherente para el flujo de trabajo de Mosaicos de UV y Conjunto de texturas con texturas no seleccionadas
* [Scripting] [Python] Permitir el uso de ajustes preestablecidos de exportación para exportar texturas
* [Scripting] [Python] Añadir un registro de cambios en la documentación
* [Scripting] [Python] Permite consultar todos los canales disponibles en una pila determinada
* [Scripting] [Python] Mejoras en la IU de la consola

**Corregido:**

* [AMD] Detección incorrecta de la versión obsoleta del controlador
* Bloqueo al volver a importar una malla con un diseño de Mosaicos de UV diferente en algunos casos
* Bloqueo al utilizar partículas con UDIM en mallas muy pesadas
* [UV Tiles] Bloqueo al exportar una malla con información de desplazamiento en algunos casos
* [Exportar] [Bloqueo] Exportar una vista 2D en formato psd puede producir un bloqueo
* Importar imágenes como secuencias al crear un proyecto no funciona
* Motor atascado en un bucle infinito
* [Acceso directo] La cámara gira siempre en modo de ajuste al cambiar los métodos abreviados de modo de ajuste
* Las mallas siempre se desenvuelven automáticamente cuando se vuelven a importar aunque la opción esté desactivada
* [Lista de conjuntos de texturas] En ocasiones, el campo de texto Descripción no está totalmente visible durante la edición
* [Lista de conjuntos de texturas] El menú desplegable para ocultar/mostrar conjuntos de texturas no está completamente visible
* [Lista de conjuntos de texturas] Al hacer clic en el icono del ojo no se debe introducir el nombre &quot;Editar conjunto de texturas&quot;
* [Ajustes del conjunto de texturas] Al quitar un canal, también se elimina el canal siguiente
* [Exportar] Incluir todo y Restablecer todo no tiene en cuenta los mosaicos UV
* [Panaderos] Durante el proceso de cocción aparecen panaderos no seleccionados
* La actualización de la resolución no se tiene en cuenta para los mapas con bake utilizados como entrada
* [Mosaicos UV] [Ventana gráfica] La ventana gráfica 3D se bloquea al añadir material inteligente tras una carpeta con la máscara de mosaico UV seleccionada
* [Mosaicos UV] [Ventana gráfica] La Malla metálica sigue siendo visible para los mosaicos ocultos con el modo de pintar
* [Exportar] [Sketchfab] Problemas con el tipo de suscripción &quot;más&quot;
* [Sketchfab] La casilla &quot;Este recurso es privado&quot; no se muestra después de cambiar de cuenta
* [Exportar] [Contenido] Los ajustes preestablecidos de pincel &quot;ondulante&quot; pueden provocar problemas de rendimiento
* [Plugin Photoshop] Mensaje en el registro: no compatible con el flujo de trabajo de azulejo UV
* [Scripting][Python] PYTHONPATH env var impide que se inicie la aplicación
* [Scripting] [Python] Error tipográfico en la documentación de Python

### 6.2.1 (2020.2.1)

*(Lanzado: 29 de julio de 2020)*
Resumen: **Versión secundaria, revisión**

**Agregado:**

* Añada la variable de entorno &quot;SUBSTANCE\_PAINTER\_VRAM\_BUDGET&quot; para anular la cantidad de GPU VRam
* [Mosaicos UV][Rendimiento] No calcule todos los mosaicos UV al utilizar la herramienta Relleno poligonal

**Corregido:**

* [Iray] Guardar renderizado devuelve un error que genera una imagen en negro
* [Linux] Bloqueo después de la pantalla de bienvenida en CentOS 7.3
* [Linux] La cantidad de Vram no se detecta correctamente con configuraciones específicas
* [Bloqueo] Apertura de un proyecto con el nombre de un conjunto de texturas duplicado
* [Motor] Problema de invalidación de caché al modificar una máscara
* [Lista de conjuntos de texturas] Efecto de fuente incorrecto al desactivar Conjunto de texturas

**Problemas conocidos:**

* [Texture Set List] No se puede ocultar la descripción
* [Lista de conjuntos de texturas] Problemas de IU
* [Iray] El procesamiento de PSD no se abre
* [Plugin Photoshop] No compatible con el flujo de trabajo de mosaicos UV

### 6.2.0 (2020.2.0)

*(Lanzado: 23 de julio de 2020)*
Resumen: **Versión principal con nuevo flujo de trabajo de mosaicos UV, pintura en mosaicos UV y mejora del rendimiento**

**Agregado:**

* Mosaicos UV (UDIM)
* [UV Tiles] Pintura en mosaicos UV
* [Mosaicos UV] Permite elegir entre el flujo de trabajo nuevo y el heredado para los mosaicos UV
* [UV Tiles] Importar secuencias de imágenes UDIM/UV Tile como recurso
* [UV Tiles] Añadir una lista de UV Tiles por conjunto de texturas en la ventana Lista de conjuntos de texturas
* [Mosaicos UV] Permite editar la resolución de varios mosaicos UV a la vez en Ajustes de conjunto de texturas
* [Mosaicos de UV][vista 2D] Mostrar Mosaicos de UV como una cuadrícula
* [Mosaicos UV][Vista 2D] Botón Nueva ventana para mostrar u ocultar la información de los mosaicos UV
* [UV Tiles] Cambiar la herramienta de pintura a un solo canal de forma predeterminada para proyectos de UV Tile
* [UV Tiles] Botón Nuevo en la barra de herramientas contextual para ignorar los mosaicos UV enmascarados mientras se pinta
* [Mosaicos de UV][Pila de capas] Nuevos iconos de pila de capas para mejorar el rendimiento
* [Mosaicos de UV] [Pila de capas] Mejora de los iconos de Pintura y relleno en la barra de herramientas
* [Máscara de Mosaico de UV][vista 2D] Permite incluir o excluir varios Mosaicos de UV a la vez (clic izquierdo, CTRL+clic izquierdo)
* [Máscara de Mosaico de UV] Nueva máscara de Mosaico de UV para incluir, excluir azulejos por capa con un nuevo icono
* [Máscara de Mosaico de UV] [Pila de capas] Mostrar el número de Mosaicos de UV en el icono de máscara de Mosaicos de UV cuando no se incluyen todos
* [Máscara de Mosaico de UV] [2D/Vista 3D] Añade el efecto de pasar por encima para visualizar los Mosaicos de UV bajo el cursor
* [Mosaicos de UV][Bakeres] Permite seleccionar y hacer un bake Mosaicos de UV específicos
* [Mosaicos de UV][Bakeres] Añadir opciones de selección para conjuntos de texturas/Mosaicos de UV
* [Mosaicos de UV] [Bakeres] Haga clic con el botón derecho en la opción de menú para seleccionar Mosaicos de UV dentro de un conjunto de texturas
* [Mosaicos UV] [Panaderos] Permite una selección rápida en el Conjunto de texturas/Mosaicos UV arrastrando
* [Mosaicos de UV] [Bakeres] Reemplace los botones &quot;Todo&quot; y &quot;Ninguno&quot; en Mapas de malla por opciones de selección más explícitas
* [Mosaicos de UV][Bakeres] Mostrar el número de texturas que se van a hacer un bake
* [Mosaicos de UV][Exportar] Permitir la selección y exportación de Mosaicos de UV específicos
* [UV Tiles][Export] Permite una selección rápida de UV Tiles arrastrando
* [UV Tiles][Exportar] Añadir opciones de menú desplegable para UV Tiles
* [Mosaicos de UV] [Exportar] Hacer que algunos ajustes preestablecidos de exportación no estén disponibles si no funcionan con Mosaicos de UV (Adobe Dimension, Sketchfab, glTF, USD)
* [Mosaicos de UV][Contenido] Actualice los ajustes preestablecidos de exportación para utilizar la nueva etiqueta $udim
* [Mosaicos de UV] Mejora de los informes de errores al importar mallas con Islas de UV superpuestas
* [Mosaicos de UV] Mosaicos de UV compatibles en Irak
* [UV Tiles][Scripting] Añadir documentación de exportación de UV Tile a Python doc
* Rendimiento
* [Rendimiento] Botón nuevo en la barra de herramientas contextual para pausar el cálculo del motor al trabajar (MAYÚS+ESC)
* [Rendimiento] Apertura más rápida de proyectos al retrasar el cálculo de la caché del conjunto de texturas
* [Rendimiento] No espere a que se carguen los mapas de malla al abrir el proyecto
* [Rendimiento][Vista 2D/3D] No calcular el canal de máscara en la ventana gráfica cuando no se utiliza
* [Rendimiento] No bloquee la aplicación al cargar los mapas de malla mostrados en las ventanas gráficas
* [Rendimiento] Mejora la velocidad de guardado incremental al guardar un proyecto
* [Rendimiento][Bakeres] Cambie la configuración de dilatación predeterminada para ahorrar tiempo y mejorar el tamaño del proyecto
* [Rendimiento] [Panaderos] Cambie a escala de grises en Panaderos específicos para ahorrar tiempo y mejorar el tamaño del proyecto
* [Rendimiento][Exportar] Mejorar el rendimiento del motor para exportar texturas más rápido
* [Rendimiento] [Exportar] Mejore la capacidad de respuesta al abrir el cuadro de diálogo de exportación con muchos conjuntos de texturas
* [Rendimiento][Exportar] Mejorar el rendimiento al cambiar a la ficha &quot;Lista de exportaciones&quot;
* [Rendimiento][Iray] Reducir el tiempo de inicio de Iray
* Otro
* [Bakers] Añadir opciones de selección para conjuntos de texturas
* Mover la administración de instancias del sombreador a la configuración del conjunto de texturas
* [Vista 2D/3D] Añada un mensaje en la parte inferior de la ventana gráfica para indicar qué tipo de máscara se ha editado
* [Pila de capas] Nueva opción en la configuración para cambiar entre las miniaturas nuevas y heredadas
* [Pila de capas] Añada comentarios visuales para indicar el estado de carga de las miniaturas
* [Proj] Nuevo modo de proyección &quot;Fill (Match Per UV-Tile)&quot; para cargar secuencias de imágenes
* [Proj] Cambie el modo de proyección de capas de relleno a &quot;Rellenar (coincidencia por mosaico UV)&quot; en casos específicos
* [Contenido] Optimización de los ajustes preestablecidos de pincel de carboncillo para mejorar el rendimiento
* Actualizar Iray a la versión 2020.0.0
* [Exportar] Desactive la ficha Lista de exportaciones si no hay nada seleccionado
* Desempaquetado automático
* [Auto Unwrap] Mejora la tasa de éxito del proceso de desajuste automático
* [Auto Unwrap] Parametrización mejorada para aumentar la velocidad y la estabilidad

**Corregido:**

* [Alembic] Las facetas se omiten al importar archivos
* [Alembic] Tiempo de carga infinito con archivos específicos
* [Import] Se importa una secuencia de imágenes de UDIM incorrecta cuando solo difiere la extensión del archivo
* [Bloqueo] Al intentar abrir un proyecto bloqueado por otro proceso, se produce un bloqueo
* [Proyección] Artefactos en malla duplicada al utilizar proyección triplanar
* [Exportar] El canal de Emisivo no se exporta con USD formato
* [Contenido] El Material inteligente &quot;Carboncillo&quot; contiene trazos de pintura

**Problemas conocidos:**

* [Texture Set List] No se puede ocultar la descripción
* [Lista de conjuntos de texturas] Problemas de IU

### 6.1.3 (2020.1.3)

*(Lanzado: 16 de junio de 2020)*
Resumen: **Corrección de error**

**Agregado:**

* [Exportar] Añadir ajustes de desplazamiento en el archivo json de parámetros de Sombreador

**Corregido:**

* bloqueo [Bloqueo] [Motor] al intentar borrar y sustituir canales existentes
* [Bloqueo] Cambio de sombreador después de pintar una máscara en capas de material
* [Bloqueo] [Motor] Bloqueos con algunos proyectos pesados
* [Bakeres] La coincidencia por nombre no funciona con OBJ exportados desde zBrush
* Las Texturas [Desplazamiento] [SVT] no se muestran al abrir el proyecto cuando el desplazamiento está activado
* [Exportar] Algunas texturas se exportan en gris uniforme
* [Exportar] Los conjuntos de texturas desactivados no se deben exportar para los ajustes preestablecidos de exportación de Dimension y Sketchfab
* [Scripting][JavaScript] Bloqueo al utilizar la API JavaScript para acceder a la configuración de exportación en el evento onProjectOpened
* No se llama a [Scripting][Javascript] onExportFinished() después de una exportación

### 6.1.2 (2020.1.2)

*(Lanzado: 28 de mayo de 2020)*
Resumen: **Corrección de error con la actualización de Substance Engine y Bakers**

**Agregado:**

* [Baker] Actualice a la versión más reciente
* [Panaderos] Nuevo método de muestreo en Oclusión ambiental, curvatura, panaderos de Thickness
* Actualizar a la versión más reciente de Substance Engine
* [Scripting][Python] Permite la creación de ResourceID para los recursos del proyecto
* [Scripting][Python] Permitir consultar información del canal
* [Scripting] [Python] Adición de funciones de ejecución en seco y devolución de llamada para simular la exportación de texturas

**Corregido:**

* [Panaderos] Normales incorrectas en el Panadero de Normales Espaciales Mundiales usando un mapa Normal tangente en casos específicos
* [Bakeres] Error al hacer un bake la Oclusión ambiental con Optix cuando no hay poli alta
* [Trazos dinámicos] Retraso al cargar un conjunto de texturas específico
* [Export] No se deben exportar los conjuntos de texturas desactivados para USD, glTF
* [Scripting] [JavaScript] No se puede editar la nueva configuración del panadero de curvatura
* [Scripting][JavaScript] alg.texturesets.addChannel() no devuelve un error en algunos casos
* [Scripting] [JavaScript] Error tipográfico en la documentación de la API de Javascript para setProjectExportOptions()
* [Scripting] [JavaScript] Exporta siempre todos los conjuntos de texturas
* [Scripting][Python] sys.ejecutable devuelve una ruta de acceso a python.exe en lugar de Substance Painter
* La caché de textura no es compatible en los sistemas operativos Mac y Windows/Linux
* [Livelink UE4] Solo se usa el último material para todos los conjuntos de texturas en una malla combinada

**Problemas conocidos:**

* [Export][Dimension][Skecthfab] No se deben exportar los conjuntos de texturas desactivados
* [Bloqueo] Cambiar el sombreador después de haber pintado una máscara en capas de material

### 6.1.1 (2020.1.1)

*(Lanzado: 5 de mayo de 2020)*
Resumen: **Revisión**

**Agregado:**

* [Export] Comentarios visuales de estado anulado en TextureSet

**Corregido:**

* [Exportar] El tamaño de la ventana del Exportador es demasiado grande en un monitor con resolución especial y no se puede cambiar de tamaño
* [Exportar] Las opciones no se guardan después de la exportación
* [Exportar] Bloqueo o no se puede exportar con el ajuste preestablecido exportar &quot;desde caché&quot;
* [Exportar] Al cancelar la exportación, se genera un mapa vacío adicional inesperado
* [Exportar] Corregir ajustes preestablecidos de exportación virtual
* [Python] PYTHONPATH env var no se tiene en cuenta
* [Python] [Exportar] Si se cancela la exportación mediante Python, se devuelve un error de excepción
* [Python][Export] export\_project\_texturas resultado incorrecto con formato de archivo psd
* [Bakeres] Bloqueo en Linux con Trazado de rayos de GPU

**Problemas conocidos:**

* [JavaScript] No se puede editar la nueva configuración del baker de curvatura
* [JavaScript] [Exportar] Exporta siempre todos los conjuntos de texturas
* [Export][USD] No se deben exportar los conjuntos de texturas desactivados
* [Bloqueo] Cambiar el sombreador después de haber pintado una máscara en capas de material

### 6.1.0 (2020.1.0)

*(Lanzado: 22 de abril de 2020)*
Resumen: **Versión principal con nueva textura y exportador de malla (con desplazamiento y teselación), desempaquetado UV actualizado con más controles, nuevos bakeres, nueva API python de scripts, mejor experiencia de usuario para la proyección de pegatinas y nuevo contenido**

**Agregado:**

* Nueva textura y exportador de malla
* [Exportar] Nueva interfaz de exportador
* [Exportar] [ficha Exportar] Permite seleccionar qué canales de mapas se exportan por conjunto de texturas
* [Exportar] [ficha Exportar] Permite modificar el tamaño del conjunto de texturas para todos los conjuntos de texturas en una sola acción
* [Exportar] [ficha Exportar] Permite crear una plantilla diferente por conjunto de texturas (excepto para USD, glTF, Sketchfab y Dimension)
* [Exportar] [Ficha Exportar] Activación y desactivación rápidas de mapas y conjuntos de texturas
* [Exportar] [Ficha Exportar] La resolución de exportación 8192x8192 ya no es experimental
* [Exportar] [ficha Exportar] Permite modificar el formato de archivo y la profundidad de bits por mapa
* [Exportar] [ficha Exportar] Permite restablecer los valores de los parámetros predeterminados
* [Exportar] [ficha Exportar] Permite guardar la configuración sin exportar
* [Exportar] [ficha Plantillas de salida] Cambie el nombre de la ficha &quot;Configuración&quot; a la ficha &quot;Plantillas de salida&quot;
* [Exportar] [ficha Plantillas de salida] Permite definir el formato de archivo y la profundidad de bits por mapa preestablecido
* [Exportar] [ficha Lista de exportaciones] Nueva ficha de vista previa para resumir y ver el proceso de exportación
* [Import/Export Mesh] Optimización del rendimiento del tiempo de importación/exportación
* [Exportar malla] Exportar malla en FBX
* [Exportar malla] Exportar malla con desplazamiento y teselación
* [Exportar malla] [IU] Nuevos ajustes para volver a calcular el vértice normal, aplicar triangulación
* [Exportar malla] Exportar topología de malla original con nuevas UV generadas por el desajuste automático
* Se ha actualizado el desajuste automático de UV con más controles
* [Desempaquetado UV][UI] Añadir configuración para activar el desempaquetado UV automático en la ventana de nuevo proyecto
* [Desempaquetado UV][UI] Nuevas opciones para controlar los pasos de desempaquetado (costuras, desempaquetado, empaquetado)
* [UV Unwrapping][UI] Permitir la conservación de las costuras de desenvolvimiento existentes/desenvolvimiento/empaquetado
* [Desajuste UV][UI] Nuevas opciones para volver a calcular completamente los pasos de desajuste
* [Desajuste UV][UI] Nueva opción para controlar el tamaño del margen (ninguno, pequeño, mediano y grande)
* Nuevos Bakeres
* [Bakeres] Reemplazar la curvatura antigua por la nueva curvatura de la malla
* [Bakeres] Opción Añadir coincidencia por nombre para ignorar la cara posterior en el baker &quot;Oclusión ambiental&quot;
* [Bakeres] Opción Añadir plano de tierra en el baker &quot;Oclusión ambiental&quot;
* Nueva API de Python de scripts (3.7.6)
* [Python][UI] Nuevo menú de scripts para Python
* [Python][UI] Nueva documentación de Python en el menú Ayuda
* [Python] Exponer módulos de Python de Substance Painter: substance\_painter, alg, display, project.setting, project, texturesets, ui
* [Python] Exponer nuevo módulo Python &quot;substance\_painter&quot;
* [Python] Exponer nuevo submódulo de Python: alg, display, log, project, resource, texturesets, ui
* [Python] Listener para cambios de proyecto
* [Python] Nuevos ejemplos en la documentación de Python
* [JavaScript] [IU] Menú de complementos reemplazado por JavaScript
* [Ventana gráfica] Permite crear una proyección de pegatinas &quot;arrastrando/soltando + ALT&quot; de un recurso desde la estantería
* Nuevo contenido
* [Contenido] 5 nuevos materiales de pegatina de Substance Source
* [Contenido] Añadir nuevas plantillas de proyecto y ajustes preestablecidos de exportación para el procesador Maxwell
* [Contenido] Añadir plantilla de proyecto para la exportación de Keyshot 9
* [Contenido] Actualice el ajuste preestablecido de exportación de Keyshot 9 para admitir desplazamientos y emisiones
* [Contenido] [Exportador] Actualización de todos los ajustes preestablecidos de exportación para que coincidan con las últimas versiones de motores de juegos y procesadores
* [Contenido] [Exportador] Actualice los archivos de ajustes preestablecidos de exportación para utilizar el nuevo formato y la nueva configuración de tramado
* [Contenido] Nuevas plantillas y sombreadores para admitir material de VRay (VRayMtl)
* [Pila de capas] Permita la eliminación de efectos de capa mediante el icono de la papelera o el método abreviado de teclado Eliminar
* Eliminar el Substance Source de plugins (utilizar el iniciador con la funcionalidad &quot;enviar a&quot;)
* [Windows] No se muestra ninguna advertencia de TDR en las GPU de gama alta

**Corregido:**

* Problemas de traducción en el cuadro de diálogo Nuevo archivo de proyecto
* [Bakers] La configuración &quot;Guardar archivo de escena preprocesado&quot; ya no funciona
* [Proyección plana] La proyección no funciona en mallas con UV repetidos
* [Decal] Diferencia de comportamiento en el canal normal al utilizar distintos modos de proyección de la capa de relleno
* [Difuminado] [Clonar] El artefacto puede aparecer al pintar en una máscara
* [Motor] Bloqueo con contenido de capa específico
* [Motor] Bloqueo aleatorio al pintar en algunos casos
* [Punto de anclaje] La referencia a una máscara vacía siempre devuelve blanco
* [Exportar] Capa no tenida en cuenta en algunas configuraciones de pila concretas
* [Exportar malla] No se puede exportar con una ruta que contenga caracteres especiales
* [Export Mesh] No se pueden leer archivos glTF al exportar desde Linux o MacOS
* [Importar malla] La reimportación de DAE, PLY o glTF no funciona según lo previsto

**Problemas conocidos:**

* [Scripting] [JavaScript] No se puede editar la nueva configuración del panadero de curvatura
* [Bakers] Bloqueo en Linux con Trazado de rayos de GPU
* [Export][USD] No se deben exportar los conjuntos de texturas desactivados
* [Bloqueo] Cambiar sombreado después de pintar una máscara en capas de material

## Versión 5

### 5.3.3 (2019.3.3)

*(Lanzado: 6 de febrero de 2020)*
Resumen: **Corrección de error con actualización a Iray 2019.3**

**Agregado:**

* Actualización a Irak 2019.3
* [Log] Indicar bios obsoletos para la CPU Ryzen que conduce a un bloqueo durante el procesamiento
* [ABR] Extraer alfa de ABR al estante

**Corregido:**

* [Baker] La cocción falla si la malla High-poly no tiene UV
* [Linux] Los métodos abreviados de ratón personalizados no se guardan
* [Pincel] El contorno desaparece con algunas formas alfa
* [Tablet] Detección incorrecta al mover los reguladores
* [Accesos directos] No se puede configurar ningún acceso directo con &quot;Ctrl+Alt+Clic del ratón&quot;
* [Estante] No se ve información sobre herramientas de recursos al utilizar una tableta con lápiz
* [Vista 2D] [Exportar] El ajuste preestablecido de vista 2D no tiene en cuenta la información normal
* Bloqueo al pintar en alineación UV con determinados pinceles
* Pintar bajo un filtro crea artefactos en el trazo en curso
* [Ventana gráfica] Caché de textura incorrecta en la ventana gráfica después de volver a importar una malla
* [Bloqueo] Error al guardar después de exportar a Photoshop
* [Bloqueo] Escribir símbolos especiales en el prefijo al importar recursos
* [Bloqueo] Haga clic en la referencia en Propiedades de punto de anclaje
* [Puntos de anclaje] El canal no se actualiza cuando hay un filtro entre el punto de anclaje y la referencia
* El vínculo de la URL de Iray en el menú Ayuda no funciona

**Problemas conocidos:**

* [Desempaquetado de UV] El procesamiento de mallas de alto contenido de polietileno puede tardar mucho tiempo
* [Desempaquetado UV] Se combinan vértices en las mismas coordenadas exactas
* La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* [Desempaquetado UV] Relación de textil no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* [Desempaquetado UV] Relación de textura no uniforme entre conjuntos de texturas
* [Desempaquetado UV] La Isla de UV generada puede ser muy alargada y, en algunos casos, no cabe en el espacio UV
* [Desempaquetado de UV] Las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no pueden desenvolverse con UV

### 5.3.2 (2019.3.2)

*(Lanzado: de enero de 2020)*
Resumen: **Corrección de error**

**Corregido:**

* Al abrir un proyecto guardado en el modo de canal solo, no se muestra la malla
* La ventana gráfica no siempre se actualiza al pintar en una capa con la herramienta de clonación

**Problemas conocidos:**

* [Bakers] Bloqueo relacionado con subprocesos múltiples en CPU Ryzen
* [Desempaquetado de UV] El procesamiento de mallas de alto contenido de polietileno puede tardar mucho tiempo
* [Desempaquetado UV] Se combinan vértices en las mismas coordenadas exactas
* La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* [Desempaquetado UV] Relación de textil no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* [Desempaquetado UV] Relación de textura no uniforme entre conjuntos de texturas
* [Desempaquetado UV] La Isla de UV generada puede ser muy alargada y, en algunos casos, no cabe en el espacio UV
* [Desempaquetado de UV] Las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no pueden desenvolverse con UV

### 5.3.1 (2019.3.1)

*(Lanzado: de diciembre de 2019)*
Resumen: **Revisión**

**Corregido:**

* Bloqueo al trabajar en mallas con Proyecciones de UV específicas
* [ABR] Bloqueo al cambiar entre ajustes preestablecidos de Photoshop
* [Linux] No se puede iniciar Substance Painter en CentOS 7.4 debido a un problema de dependencia libGLX
* [Bakers] Bloqueo al realizar el procesamiento después de utilizar Archivo > Limpiar
* [Panaderos] El cuadro de diálogo Progreso de panificación se bloquea después de cancelar
* [Panaderos] La cocción de mallas después de exportar texturas no funciona
* [Panaderos] El uso de resultados de &quot;Coincidir por nombre&quot; con mapas de malla negros
* [Panaderos] No se tiene en cuenta la jaula
* [Shelf] La importación de archivos de PSD genera imágenes rotas
* [Muestra] El proyecto de muestra &quot;Mat&quot; tiene cámaras rotas y un ajuste preestablecido de exportación incorrecto

**Problemas conocidos:**

* [Bakers] Bloqueo relacionado con subprocesos múltiples en CPU Ryzen
* [Desempaquetado de UV] El procesamiento de mallas de alto contenido de polietileno puede tardar mucho tiempo
* [Desempaquetado UV] Se combinan vértices en las mismas coordenadas exactas
* La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* [Desempaquetado UV] Relación de textil no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* [Desempaquetado UV] Relación de textura no uniforme entre conjuntos de texturas
* [Desempaquetado UV] La Isla de UV generada puede ser muy alargada y, en algunos casos, no cabe en el espacio UV
* [Desempaquetado de UV] Las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no pueden desenvolverse con UV

### 5.3.0 (2019.3.0)

*(Lanzado: 17 de diciembre de 2019)*
Resumen: **Versión principal con mejora de la experiencia del usuario al pintar a mano, uso de tabletas, desempaquetado automático de UV en versión beta (0.3.0) y nuevo contenido diverso para pintar a mano**

**Agregado:**

* Integrar la versión 0.3.0 del desempaquetado automático de UV en Substance Painter
* [Desempaquetado de UV] Desempaquetado automático de UV en el Substance Painter cuando no hay UV o UV parciales
* [Desempaquetado UV] Una configuración global para activarla y desactivarla
* [Desempaquetado UV] Versión registrada en el archivo de registro
* [Desempaquetado UV][IU] Indicar el progreso del desempaquetado UV
* [UI] Nuevos ajustes en la barra de herramientas contextual para seleccionar la vista previa del pincel: Vista previa completa, contorno de pincel y forma de cruz
* [Herramienta] Nuevo modo de fusión avanzado en la sección alfa: Aclarar (máxima) además de Normal
* [Pila de capas] Opción de corrección de gamma por capa para alfa o máscara (menú del botón derecho)
* [Pila de capas] [IU] Se añade el icono &quot;i&quot; cuando se corrige gamma en una capa alfa
* [Tablet] [Herramienta] Exponer presión mínima para tamaño y flujo
* [Tablet][UI] Nueva configuración en la barra de herramientas contextual para seleccionar la presión de curva: lineal, fácil de entrar, fácil de salir
* [Tablet][UX] Pulse Ctrl+Alt y haga clic para desplazarse
* Importar ajustes preestablecidos de pincel de Photoshop (formato ABR)
* [ABR] Compatibilidad con parámetros de forma
* [ABR] Compatibilidad con parámetros de dinámica de forma
* [ABR] Parámetros de transferencia de soporte
* [ABR] Compatibilidad con parámetros de dispersión
* [ABR][Trazos dinámicos] Compatibilidad con redondez y volteo
* [ABR][Estante] Se muestra la estructura de carpetas del pincel en el Editor de filtros.
* [ABR][Estante] Añadir icono de Photoshop en miniaturas
* [ABR][Shelf] Añadir una lista de parámetros no admitidos en la miniatura detallada de ABR
* [Herramienta][Trazos dinámicos] Nuevo ajuste de trazo dinámico para controlar cuántas semillas aleatorias se van a generar
* [Herramienta][IU] Añadir nuevos ajustes de distribución y eje para la variación de dispersión
* [Método abreviado] Pulse Ctrl+Mayús+B para abrir la ventana que Hace un bake
* [UI][Menu] Añadir entrada en el menú &quot;Editar&quot; para abrir la ventana Hornear
* [UI][Configuración] Mejora de la alineación de la lista de métodos abreviados
* [UI] Reemplazar los controles de presión (tamaño y flujo) por botones de activación/desactivación
* [Ventana gráfica] Permite enfocar la ventana gráfica 2D y 3D por separado
* Actualización a QT 5.12.5
* [UI] Indicar el progreso de carga de malla
* [Substance] Añade compatibilidad con rangos suaves y no sujetos con reguladores
* [Substance] Aumentar la precisión de los parámetros del Substance hasta 6 decimales
* [Substance] Tenga en cuenta el paso definido por un parámetro
* [Substance] Optimizar la generación de trazos dinámicos con compatibilidad con condiciones en los datos de usuario
* [Substance] Permite designar una salida de gráfico como una máscara para todos los canales a través de los datos de usuario.
* [Contenido] Actualizar proyecto de muestra &quot;Mat&quot; con topología compatible con desplazamientos, nuevo mapa de ID y nuevas cámaras
* [Content] Integra 3 filtros nuevos (MatFx): Cómic, Acuarela, Pintura al óleo (inspirado en el trabajo de Cubukcu emrecano)
* [Contenido] Integrar 102 ajustes preestablecidos de pinceles de Photoshop de los paquetes de Kyle T. Webster
* [Contenido] Integrar 18 nuevos ajustes preestablecidos de pincel: Flecha de rodillo de pintura, texto de advertencia de rodillo de pintura, carboncillo fino y más
* [Contenido] Integrar 9 nuevos alfa: Rodillo de Pintura del creador de pinceles, Photoshop del creador de pinceles, patrones de pinceles y mucho más
* [Contenido] Integra 2 nuevos ajustes preestablecidos de herramientas: Gouache denso y Gouache descolorido
* [Content] Integrar 1 nuevo generador: Comprobador UV (Islas de UV de realce y costuras)
* [Contenido] Integrar 2 nuevos ajustes preestablecidos de exportación: Keyshot 9+ y Spark AR Studio
* [Contenido] Integra 1 nueva plantilla de proyecto : Spark AR Studio (Facebook)

**Corregido:**

* [Tablet] Al deshacer trazos de lápiz (Ctrl+Z) se produce un retraso mayor que al deshacer trazos del ratón
* [Tablet] La presión inicial y final no se tiene en cuenta al dibujar una línea recta
* [Tablet] El primer sello se dibuja dos veces cuando se usa una línea recta
* [Tablet] Mejorar la compatibilidad con los métodos abreviados de la tableta Huion
* [Tablet] Mejorar la compatibilidad con los botones del lápiz Huion
* [Tablet] Desplazamiento entre la vista previa del pincel y el sello dibujado
* [Tablet] Los métodos abreviados para modificar pinceles con lápiz suelen dar lugar a un rendimiento bajo en casos excepcionales
* [Tablet] Retraso al pintar en una capa específica
* En raras ocasiones, pueden producirse texturas borrosas al cambiar la ventana gráfica
* [UI][Substance] No siempre se muestran las entradas de imagen
* Limpiar no elimina los ajustes preestablecidos del estante que se hayan importado en un proyecto
* [Herramienta] [Trazo dinámico] Problema de rendimiento al ajustar el recuento cíclico de sello
* Problemas de actualización al pintar en modo de ventanilla 3D/2D en casos excepcionales
* Pintar un trazo muy largo puede provocar un congelamiento
* [Herramienta] Problema de rendimiento al pintar con trazos dinámicos específicos
* [UI] La barra de herramientas contextual sigue mostrando las propiedades del pincel al seleccionar una carpeta
* Los valores del eje de simetría no se restablecen
* La importación de texturas EXR con valores de coma flotante es totalmente negra
* Pulsar Alt+clic en un canal para aislar no funciona para el filtro y el generador
* [Exportar] El proyecto específico se bloquea durante la exportación
* [Substance] Valor predeterminado incorrecto en el menú desplegable si el parámetro está oculto por Visible If
* [Sombreador] Los canales definidos mediante Material Layering no se ordenan de la misma forma en la interfaz de usuario
* [Shelf] Los metadatos de ajustes preestablecidos no se guardan en el disco

**Problemas conocidos:**

* [Desempaquetado de UV] El procesamiento de mallas de alto contenido de polietileno puede tardar mucho tiempo
* [Desempaquetado UV] Se combinan vértices en las mismas coordenadas exactas
* La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* [Desempaquetado UV] Relación de textil no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* [Desempaquetado UV] Relación de textura no uniforme entre conjuntos de texturas
* [Desempaquetado UV] La Isla de UV generada puede ser muy alargada y, en algunos casos, no cabe en el espacio UV
* [Desempaquetado de UV] Las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no pueden desenvolverse con UV
* El ejemplo de reunión tiene algunos problemas con cámaras importadas

### 5.2.3 (2019.2.3)

*(Lanzado: 23 de octubre de 2019)*
Resumen: **Versión de corrección de errores**

**Agregado:**

* [Lista de conjuntos de texturas] Botón Añadir para activar o desactivar rápidamente el modo de enfoque
* [Log] Añadir número de versión de Windows 10 en el archivo de registro
* Actualizar a la versión más reciente de Substance Engine
* [MacOS] Notarizó el software para seguir los nuevos requisitos de distribución de MacOS Catalina

**Corregido:**

* [Plugin] El complemento de origen no funciona
* [MacOS] [Sombreador] Mac OS 10.14.5 y AMD: la colocación de los materiales en capas no funciona como se pretende

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.2 (2019.2.2)

*(Lanzado: 20 de septiembre de 2019*
Resumen: **Versión de corrección de errores**

**Corregido:**

* La importación de recursos mediante secuencias de comandos puede provocar un bloqueo
* [Plugin] Descargar material de la fuente puede llevar a un bloqueo

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.1 (2019.2.1)

*(Lanzado: 17 de septiembre de 2019*
Resumen: **Versión de corrección de errores**

**Corregido:**

* [Mac][USD] Los archivos USDZ exportados de MacOS no se pueden abrir
* [Conjunto de texturas] No es posible aislar un conjunto de texturas con el modificador ALT
* [Shelf] Los ajustes preestablecidos, Materiales inteligentes y Máscaras inteligentes siempre se modifican al salir de la aplicación
* [Pila de capas] No se puede seleccionar el efecto después de eliminar otro efecto
* Parpadeo al utilizar un regulador dentro del panel de propiedades de la herramienta
* Bloqueo al exportar ajustes preestablecidos a la estantería
* Bloqueo al exportar un ajuste preestablecido con espacio insuficiente
* Bloqueo al crear un ajuste preestablecido con espacio insuficiente

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.0 (2019.2.0)

*(Lanzado: 25 de julio de 2019)*
Resumen: **Versión principal con actualizaciones de los bakeres en términos de rendimiento y un nuevo modo de previsualización + nuevo contenido**

**Agregado:**

* [Bakeres] Se ha agregado compatibilidad para Trazado de rayos de GPU con DXR y OptiX (Oclusión ambiental, Thickness)
* [Baker] Optimizaciones y aceleraciones para el Trazado de rayos de la CPU
* [Bakeres][Modo Vis][IU] Nuevo modo de visualización de hace un bake en la ventana gráfica
* [Bakeres][Preferencias][IU] Nueva opción de hacer un bake para activar y desactivar el Trazado de rayos de GPU
* [Bakeres][IU] Repaso del cuadro de diálogo de la barra de progreso
* [Bakeres] Mejora de los mensajes de advertencia y error
* [Bakeres] Permitir una cancelación más receptiva del proceso de hacer un bake
* [Baker] Vuelva a abrir la ventana hacer un bake después de hacer clic en Cancelar
* [Proj][UX] Mejora de la usabilidad del manipulador de rotación
* [Configuración] Opción para mejorar el rendimiento reduciendo la resolución de la ventana gráfica para las pantallas HDPI
* [Scripting] Cambiar la resolución del conjunto de texturas
* [Scripting] Obtener conjunto de texturas seleccionado
* [Scripting] Permite que el usuario seleccione un conjunto de texturas
* [Scripting] Función para saber cuándo se ha cambiado la selección del conjunto de texturas
* [Estante] Se han añadido 40 materiales inteligentes nuevos
* [Estante] Se han añadido 20 máscaras inteligentes nuevas

**Corregido:**

* [Pila de capas] Bloqueo de la interfaz de usuario al seleccionar varias capas
* [Pila de capas] Agrupar muchas capas bloquea la interfaz de usuario más tiempo del habitual
* [Pila de capas] En algunos casos, se pueden seleccionar simultáneamente una capa y un efecto
* Los gráficos de Substance utilizados dentro de las herramientas de pintura no se generan con la resolución adecuada
* [Baker] El botón &quot;Hacer un bake todos los conjuntos de texturas&quot; no se desactiva si no se ha seleccionado ningún baker
* [MacOS] Desactivar el mensaje de advertencia sobre la teselación
* La herramienta Proyección no tiene previsualización cuando se utiliza con una máscara
* Bloqueos y proyectos dañados al intentar ahorrar con espacio en disco insuficiente
* [Shelf] Bloqueo al importar un recurso en el disco a través de la estantería con espacio insuficiente
* [Shelf] Bloqueo al restaurar el ajuste preestablecido de sesión
* [Estante] Al importar un ajuste preestablecido con un nombre que termina en un espacio, se crea un bloqueo
* [Shelf] Importar un recurso con un prefijo que termina con un espacio vacío conduce a un bloqueo

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.1.3 (2019.1.3)

*(Lanzado: 1 de julio de 2019)*
Resumen: **Corrección de error con 2 nuevas características**

**Agregado:**

* Permite especificar el presupuesto de VRam con una línea de comandos (p. ej. —vram-budget 4096)
* [QML] Exponer las propiedades wrapMode y elide de los botones y casillas de verificación QML

**Corregido:**

* &quot;Seguir ruta&quot; no funciona todo el tiempo
* La asignación de canales no funciona con SBSAR utilizado en ranuras de un solo canal
* [Pila de capas] Bajo rendimiento al desplazarse con capas ocultas
* bloqueo [TextureSet] al hacer clic entre máscaras
* [SVT] El Desplazamiento no se muestra correctamente y parpadea en algunos casos
* [Alembic] Bloqueo con malla usando normales de punto en lugar de normales de vértice
* [Alembic][Log] Informar de un error en Log si no se admite el archivo Alembic durante la importación

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Los bloqueos raros al importar algunos archivos Alembic

### 5.1.2 (2019.1.2)

*(Lanzado: 21 de mayo de 2019*
Resumen: **Revisión**

**Corregido:**

* Bloqueo al seleccionar dos recursos con una entrada de imagen

### 5.1.1 (2019.1.1)

*(Lanzado: 20 de mayo de 2019*
Resumen: **Revisión**

**Agregado:**

* Actualización a la versión más reciente de Substance Engine con la última versión de Substance Designer 2019.1

**Corregido:**

* [Substance] Visible Si no se tiene en cuenta para las imágenes de entrada
* [SVT] [Motor] El cambio de la resolución del conjunto de texturas provoca bloqueos en algunos casos
* [Motor] En algunos casos aparecen texturas negras aleatorias
* [Pila de capas] [IU] Al alternar una máscara con MAYÚS, se pueden seleccionar varias capas al mismo tiempo
* [Pila de capas] La opacidad no afecta al efecto Pintura con el modo de fusión PassThrough
* [Pila de capas] La entrada de Height a filtro normal no se actualiza correctamente con el trazo del pincel del borrador
* [LayersStack] Bloqueo al deshacer el soltar una máscara inteligente
* Malla metálica parpadeando con sombras y anti-aliasing temporal activado
* [Desplazamiento] Retraso en AMD con algunas mallas pesadas
* [Windows] Bloqueo al abrir algunos proyectos mediante el explorador de archivos
* [Histograma] Bloqueo al eliminar la máscara con el punto de anclaje en algunos casos
* Bloqueo en la generación de vistas previas en algunos casos excepcionales
* [Bloqueo] No se puede volver a abrir un proyecto con demasiadas herramientas de clonación y difuminado
* No se muestra ninguna malla en el modo de material después de guardarla en algunos casos
* [Scripting] alg.mapexport.documentStructure() devuelve valores incorrectos para las carpetas

**Problemas conocidos:**

* Al hacer doble clic en el nombre del conjunto de texturas, se seleccionará antes de entrar en el modo de cambio de nombre

### 5.1.0 (2019.1.0)

*(Lanzado: 23 de abril de 2019)*
Resumen: **Trazo dinámico con contenido nuevo dedicado, Desplazamiento y teselación en tiempo real e Iray, efecto Máscara de comparación, simetría radial, Plano y Proyección esférica**

**Agregado:**

* [Herramienta] Trazo dinámico: Variación Substance junto a un trazo de pincel
* [Trazo dinámico] Exponer nuevo parámetro de índice de sello con opciones
* [Trazo dinámico] Tenga en cuenta el parámetro $time
* [Trazo dinámico] Generar un nuevo parámetro $randomseed por trazo y por sello
* [Trazo dinámico] Iniciar un índice de trazo dinámico a partir de un número aleatorio
* [Trazo dinámico] [Estante] Ayuda para buscar un recurso de trazo dinámico con un icono nuevo dedicado
* Desplazamiento y teselación en la ventana gráfica en tiempo real
* Desplazamiento y teselado en Iray
* [Configuración de sombreado][IU] Nueva ficha para controlar el desplazamiento y la teselación
* [Pila de capas] Nuevo efecto CompararMáscara: generar una máscara comparando dos canales
* [Pila de capas][IU] Nueva entrada en el menú contextual &quot;Añadir máscara con combinación de heightes&quot; para insertar un efecto Comparar máscara
* [Simetría] Nuevo modo de simetría: pintura radial
* [Configuración de simetría] Expanda las secciones &quot;Configuración&quot; y &quot;Pantalla&quot;
* [Ajustes de simetría] [IU] Vista previa para pintura radial
* Exponga dos nuevos modos de proyección: planar y esférico
* [Proj] Nuevo modo de recorte de forma para todas las proyecciones
* [Proj] Modo plano con nuevo manipulador: Herramienta Superficie
* [Proj][Acceso directo] Método abreviado MAYÚS+W para la herramienta Superficie
* [Proj] Enmascaramiento de proyección plana con selección de profundidad y sacrificio de la cara posterior
* [Manipulador] Mejora del manipulador de rotación en los tres ejes para triplanar
* [Herramienta] [Experiencia de usuario] Al pulsar Alt y hacer clic en un canal, se selecciona ese canal (lo activa o desactiva todos los demás).
* [Motor] Actualizar a la versión más reciente de Substance Engine
* [Conjunto de texturas] Selección múltiple y resolución de cambios
* [Conjunto de texturas] Activación y desactivación rápidas de los conjuntos de texturas
* [Conjunto de texturas] Combina solo y todas las opciones en un nuevo menú
* [Conjunto de texturas] [Pila de capas] Nuevo icono para activación y desactivación
* [Pila de capas][UX] Inserta efectos por encima de los que ya están seleccionados
* [Pila de capas][IU] Reprocesamiento de la vista de la pila de capas
* [Pila de capas] El modo de fusión para capas con instancias ahora está en modo Pass Through de forma predeterminada
* [Exportar] Opción para activar y desactivar el tramado
* [Plugin] Compatibilidad con el modificador de precisión para reguladores (MAYÚS)
* [Plugin][UI] Nuevo icono para autoguardar
* [Scripting] Enumera el contenido de una carpeta
* [Scripting] Permitir la eliminación de archivos
* [Scripting] Lea toda la información de la pila, incluidos los recursos utilizados
* [Contenido][Trazo dinámico] Nuevas herramientas y ajustes preestablecidos de pincel
* [Content][Dynamic stroke] Dos nuevos degradados de procedimiento: Tono de degradado y Generador de degradado
* [Contenido] 11 nuevos filtros: Pintura descascarillada MatFx, gotas de agua MatFx y más
* [Contenido] 7 nuevos generadores: Stitcher automático, UV Random Color, UV Texel Density y más
* [Contenido] 93 alfas nuevas: nuevos textos, flechas y otras formas
* [Contenido] 2 nuevos procedimientos: Tono de degradado, Generador de degradados y mucho más
* [Contenido] 21 nuevos ajustes preestablecidos de herramienta y pincel para Trazos dinámicos : Guijarros, Huellas, Spray y más
* [Contenido] 2 HDR nuevos: Canopus Ground y Autumn Forest
* [Contenido] Actualizar el contenido con la selección aleatoria de semillas en el estante
* [Contenido] Nuevo icono con parámetro de semilla aleatoria expuesto en la estantería

**Corregido:**

* [Pila de capas] La pila de capas se sigue arrastrando para siempre
* [Mac] La opción &quot;Mostrar en Finder&quot; puede provocar la congelación
* [Scripting] La configuración guardada mediante la interfaz de usuario personalizada se pierde si se mueve el archivo de sombreado
* El número de versión de la API [Scripting] es incorrecto y no está actualizado
* [Efecto] El contenido del histograma no se muestra correctamente
* [Efecto] El efecto del histograma no se actualiza en algunos casos
* [Estante] Los puntos no se alinean correctamente en el material &quot;Pirámide de tela plástica&quot;

**Problemas conocidos:**

* Al hacer doble clic en el nombre del conjunto de texturas, se seleccionará antes de entrar en el modo de cambio de nombre
* [Pila de capas] [IU] Al alternar una máscara con MAYÚS, se pueden seleccionar varias capas al mismo tiempo

## Versión 4

### 4.3.3 (2018.3.3)

*(Lanzado: 7 de marzo de 2019)*
Resumen: **corrección de errores**

**Agregado:**

* [Contenido] Integrar nueva plantilla de proyecto: &quot;PBR - Mezcla Alpha de rugosidad metálica&quot;
* El orden de búsqueda de la biblioteca dinámica de Linux ha cambiado para priorizar las bibliotecas en el directorio de instalación antes de lo que está instalado en el sistema

**Corregido:**

* La malla desaparece a veces de la ventana gráfica 3D (presione F para restablecer la cámara)
* Actualizar el cargador de Substance Painter de Sketchfab con los nuevos tipos de licencia de Sketchfab
* [Import][glTF] Modulación incorrecta de la textura de entrada definida en los archivos glTF
* [Import][glTF] El plano de tierra se muestra incorrectamente con la importación de glTF en algunos casos
* [Export][USD] La opacidad no funciona en Arkit
* [Export][USD] La exportación de USDz se bloquea en algunos casos
* [Export][USD] Exportar a USD sin guardar provoca un bloqueo
* [Export][USD] Modo de mosaico incorrecto para texturas, modo de subdivisión para mallas y tipos de salida para sombreadores
* [Export][USD] Exportaciones dispersas de solo algunos conjuntos de texturas con toda la geometría
* [Instancia] Bloqueo al intentar eliminar una capa de instancia rota
* [Regresión][Exportar] Algunos mapas no exportados en la profundidad de bits elegida
* [Linux] Problema con library libtbb.so.2

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.3.2 (2018.3.2)

*(Lanzado: 24 de enero de 2019)*
Resumen: **Revisión con nuevas características (exportación USDZ y filtrado de texturas en la ventana gráfica)**

**Agregado:**

* [Exportar] Permitir exportación a USDZ
* [Ventana gráfica] Permite controlar la calidad de la textura en los Ajustes de visualización
* [Viewport] Se ha añadido el ajuste de sesgo mip en la configuración de visualización
* [Ventana gráfica] Se ha añadido un filtrado anisotrópico en la configuración de visualización
* [complementos] Actualizar los complementos oficiales para usar el estilo de Substance Painter 2018
* [Licencia] Instalar la licencia de forma predeterminada en una carpeta de usuario

**Corregido:**

* Bloqueo vinculado a la descompresión
* Añadir TAA en material solo
* Ruido con sombra, TAA y sombreador de prueba alfa con tramado
* Eliminar el tramado de specular para todos los sombreadores PBR clásicos
* Bloqueo en la configuración del sombreado en algunos casos
* La activación de la dispersión no está sincronizada entre los procesamientos de OpenGL e Iray
* Las herramientas de difuminado y clonación ya no funcionan en mallas específicas
* Algunos conjuntos de texturas no pueden aparecer en el procesamiento de Iray
* Los conjuntos de texturas renombrados no se guardan después de cerrar el proyecto
* Artefactos de malla metálica al arrastrar y soltar materiales en mapas de ID
* [Scripting] La creación de la ruta de archivo no se fuerza al guardar un proyecto
* [Scripting] La devolución de llamada &quot;onProjectAboutToSave()&quot; ya no funciona
* Vínculos de foro rotos en la ventana de informe de errores

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.3.1 (2018.3.1)

*(Lanzado: 6 de diciembre de 2018)*
Resumen: **Revisión**

**Agregado:**

* [Simetría] [Ventana gráfica] El dibujo de la Simetría en la Vista 2D ha vuelto y ahora se ha corregido una previsualización del pincel clónico

**Corregido:**

* [Exportar] La exportación de vista 2D genera una textura negra en algunos casos
* [Iray] La información normal se vuelve incorrecta en Iray después de crear instancias de una capa de material
* Los conjuntos de texturas no cuadradas pueden provocar bloqueos en algunos casos
* [Deshacer] Varias teclas Ctrl+Z pueden provocar el bloqueo en algunos casos de forma aleatoria
* [QML] AlgScrollView puede crear una advertencia en el registro en algunos casos (bucles de enlace)

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows
* El suavizado y las sombras cuando están activos juntos pueden dar resultados inesperados

### 4.3.0 (2018.3.0)

*(Lanzado: 20 de noviembre de 2018)*
Resumen: <b>Actualizaciones de la ventana gráfica, exportación adecuada de la vista 2D, nuevos ayudantes de interfaz de usuario, una herramienta de simetría mejorada, nuevo contenido y un gran aumento en el rendimiento</b>

<b>Agregado:</b>

* [Suavizado] [Ventana gráfica] Nuevo filtrado de suavizado temporal para la ventana gráfica 3D (mediante Configuración de visualización)
* [Exportar] Exporte el contenido de la ventana gráfica 2D como una única textura
* [Exportar] [Tramado] Exponer tramado en la exportación
* [Pila de capas] Colores en capas y carpetas
* [Pila de capas] Activación y desactivación rápidas de varias capas y efectos
* [Pila de capas] Navegación más sencilla por los modos de fusión con las teclas hacia arriba y el desplazamiento del ratón
* [Proj][UI] Manipulador de rotación adicional en los tres ejes para triplanar
* [Proj][Atajos] : y + para cambiar el tamaño del manipulador de Proyección de UV
* [Shader] Controle los parámetros de capa revestida con canales en el sombreador recubierto de PBR
* [Substance] Expone nuevas entradas de textura basadas en malla para filtros y generadores
* [Simetría][Ventana gráfica][IU] Controlar el desplazamiento de simetría con manipuladores
* [Simetría][Barra de herramientas contextual][IU] Nuevo panel de simetría con opciones
* [Simetría] Nuevo modo de intersección de línea de simetría
* [Simetría] Nuevo cursor de clonación de simetría
* [Simetría] [Métodos abreviados] Q para ocultar y -, + para cambiar el tamaño y cambiar para ajustar
* [Log] Mejore los mensajes de error cuando no se pueden exportar texturas
* [Scripting] Permite cambiar o actualizar los recursos en Configuración de visualización
* [Scripting] Permite crear o quitar canales en conjuntos de texturas
* [Contenido][Shaders] Añadir compatibilidad para la anisotropía con un sombreado específico (pbr-metal-rough-anisotropía-angle)
* [Contenido] Actualización de la esfera de previsualización con anisotropía y ángulo modificado
* [Contenido] Se ha actualizado el obturador de matFx
* [Contenido] Nueva digitalización de caras sin problemas Texturing.XYZ
* [Contenido] Nuevos procedimientos anisotrópicos
* [Content] Nuevo filtro: entorno de iluminación generado
* [Contenido] Nuevo mapa de entorno: studio automotive neutral
* [Contenido] Nueva plantilla de proyecto: PBR - ángulo de Anisotropía de rugosidad metálica (con canales de anisotropía)
* [Contenido] Nueva plantilla de proyecto: PBR - Rugosidad metálica Recubierta
* [SVT][Motor] Texturas virtuales dispersas (SVT)
* [SVT][Preferencias][IU] Opción de aceleración de compatibilidad de hardware SVT
* [SVT][Log] Información adicional para la función de texturas virtuales dispersas (p. ej., disco de tamaño)
* [SVT][UI] Ventana de mensaje al inicio si el tamaño del disco es demasiado bajo para la caché
* [SVT][Preferencias][IU] Ubicación de caché global del Substance Painter
* [SVT] Nueva variable de entorno para especificar la ruta de acceso de la caché del Substance Painter
* [SVT] Nueva variable de entorno para activar la aceleración de compatibilidad de hardware SVT
* [SVT] Detectar compatibilidad dispersa por hardware
* [SVT][Hardware disperso] Aumentar la versión mínima del controlador para la GPU Nvidia
* [SVT][Shader][Viewport][UI] Advertencia al usuario si hay artefactos con texturas virtuales dispersas al abrir el proyecto

<b>Corregido:</b>

* [Selector de color] Cursor de pintura que aparece al intentar seleccionar un color
* Bloqueo al seleccionar o anular la selección de capas en un orden específico puede producir un bloqueo
* Bloqueo al pegar como instancia una capa con una máscara
* [Canal de usuario][Regresión] Bloqueo al cambiar el nombre del canal de usuario
* [Canal de usuario] Vista previa de pincel atenuado
* [Alembic] Solo un conjunto de texturas de varios materiales tras la importación
* [Motor] La textura exportada difiere de la ventana gráfica para los sellos de pincel
* [Motor] La inversión con un efecto de nivel no afecta por completo a una textura
* El selector de material está aplicando un trazo de pincel al seleccionar
* Cambiar la resolución a 128x128px provoca un bloqueo
* Los vínculos de mapa de malla no se actualizan correctamente al rehornear o crear instancias de capas
* [Substance] UserData ColorSpace no funciona en la malla Hecha un bake Normal solicitada como entrada
* No coincide la asociación MDL al utilizar varias instancias de sombreado
* [Simetría] [Capa de relleno] Plano de Simetría y su manipulador activo en Capa de relleno
* [Ventana gráfica] El punto de tabla dinámica para la traducción no siempre se actualiza después de hacer clic
* [UI] Se han corregido los iconos y la eliminación de marcadores de posición para los monitores HDPI

<b>Problemas conocidos:</b>

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows
* El suavizado y las sombras cuando están activos juntos pueden dar resultados inesperados

### 4.2.3 (2018.2.3)

*(Lanzado: 25 de septiembre de 2018)*

**Corregido:**

* [vista 2D] La vista 2D se rompe con algunas mallas al crear un nuevo proyecto
* [Bloqueo] El cambio de la Proyección de UV a la proyección triplana conduce a un bloqueo
* [RayCollider] Varios bloqueos debido a &quot;RayCollider&quot;
* [Herramienta] Al cambiar las capas, se pierden las propiedades de pincel modificadas
* La configuración del pincel se restablece al cambiar al borrador

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.2.2 (2018.2.2)

*(Lanzado: 11 de septiembre de 2018)*
Resumen: **Revisión con actualización de contenido, nuevas funcionalidades de secuencias de comandos y poder deshabilitar la actualización automática**

**Agregado:**

* [Contenido][Estante] Añadir un ajuste preestablecido de Estante de piel
* [Contenido] [estante] Conversión de 19 normales de piel en materiales para dispersión subsuperficial
* [Scripting] Crear una plantilla de proyecto a partir de un proyecto abierto
* [Scripts] Obtener o establecer la configuración de exportación de un proyecto abierto
* [Actualizaciones] Puede desactivar la ventana emergente de actualización automática de la variable de entorno y configuración
* [Actualizaciones] No se muestra hasta la próxima versión en la ventana emergente de mantenimiento obsoleta

**Corregido:**

* [Cámara] Zoom incorrecto al cambiar de ortográfico a Perspectiva
* [Display] Algunos mapas se muestran en línea en lugar de sRGB
* [Ventanas] El enfoque de malla no se comporta correctamente
* [vista 2D] El proyecto con la cámara rota ha desaparecido UV
* [SSS] [Información sobre herramienta] aparece información sobre herramientas de dispersión subsuperficial en el registro
* Algunos proyectos no se pueden abrir en 2018.2 y el mensaje de error no puede guardar un paquete de substance nulo
* [Máscara] El color de la herramienta de Pintura se puede bloquear en algunos casos al trabajar en una máscara
* [Material] Mapas que no aparecen en situaciones específicas
* [Proj][Tools] Manipulador activo con un generador
* [Substance] Faltan grupos de parámetros de Substance
* [Scripting] Nombre de software incorrecto en la documentación
* [UDIM] No hay información en el registro acerca de los proyectiles de UV en múltiples mosaicos de UV

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.2.1 (2018.2.1)

*(Lanzado: 03 de agosto de 2018)*

**Corregido:**

* Faltan parámetros de sombreador de dispersión subsuperficial en los proyectos de actualización

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.2.0 (2018.2.0)

*(Lanzado: 2 de agosto de 2018)*
Resumen: **Versión de verano, compatibilidad con dispersión subsuperficial, mejoras en la proyección y el relleno, importación y selección de cámaras, compatibilidad con Alembic y glTF, arrastrar y soltar en mapa de ID, compatibilidad de formato de Substance mejorada y nuevo contenido**

**Agregado:**

* [SSS][Viewport][Iray] Dispersión subsuperficial genérica
* [SSS] Sincronización de MDL y parámetros de dispersión subsuperficial
* [SSS] Se ha añadido un nuevo canal de escala de grises denominado Dispersión
* [SSS][Configuración del sombreador] Parámetro de tipo de dispersión para dispersión subsuperficial (piel o translúcido)
* [SSS][Configuración de sombreado] Parámetro de escala de dispersión para dispersión subsuperficial
* [SSS][Configuración de sombreado] Parámetro de color de dispersión para dispersión subsuperficial
* [SSS][Configuración de pantalla] Dispersión Recuento de muestras para dispersión subsuperficial
* [Shader] [Iray] Integrar MDL de dispersión subsuperficial para Iray
* [Shader] Actualización del sombreado mediante el actualizador de recursos
* [Shader] Actualizar la API y la documentación del registro de cambios
* [Tool Properties][Proj] Nuevos parámetros para la proyección triplanar
* [Ventana gráfica][Proyecto] Controle las propiedades de la capa de relleno en la vista 3D directamente con los manipuladores (proyección triplanar)
* [Atajos][Proj] Nuevos atajos Q, W, E, R, T para manipuladores de proyección triplanar
* [Viewport][Proj] Controle las propiedades de la capa de relleno en la vista 2D directamente con los manipuladores (Proyección de UV)
* [Atajos][Proj] Nuevo atajo Q para manipuladores de Proyección de UV
* [Barra de herramientas contextual][Proj] Controlar manipuladores de proyección triplanar
* [Barra De Herramientas Contextual][Proj] Controlar Manipuladores De Proyección de UV
* [Propiedades de la herramienta] Desactivar el mosaico de texturas con las herramientas Proyección y Galería de símbolos
* [Galería de símbolos] Usar imágenes no cuadradas con la herramienta o galería de símbolos Proyección
* [Stencil] Permitir el control del modo de mosaico en la ventana Propiedades
* [Stencil] El zoom no está centrado en una galería de símbolos que no sea de mosaico
* [Cámaras] Importar cámaras de Maya, Max, Blender, Modo, DAE
* [Cámaras] [Ventana gráfica] Seleccione y controle las cámaras importadas en la ventana gráfica
* [Cámaras] [Israel] Seleccione y controle las cámaras importadas en Irán
* [Cámaras][IU][Nuevo proyecto][Configuración del proyecto] Importar cámaras está marcado de forma predeterminada
* [Cámaras] [Accesos directos] Añadir accesos directos para cambiar de cámara
* [Cámaras][Ventana gráfica] Añadir fotograma en la ventana gráfica
* [Cámaras] [Configuración de la ventana gráfica] Control de la opacidad de los fotogramas
* [Cámaras][Configuración de la cámara] distancia focal máxima de 500 mm
* [Cámaras][Configuración de la cámara] Relación de exposición
* [Cámaras][Configuración de la cámara] Añadir una opción de bloqueo
* [Cámaras][Configuración de la cámara] Añadir una opción de restauración
* [Cámaras][Configuración de la cámara] Añadir el atributo de distancia de enfoque
* [glTF] Importación de un archivo glTF
* [glTF] Importar mapa de oclusión ambiental
* [Alembic] Importar Alembic 1 fotograma con geometría estática
* [Estante] Arrastre y suelte materiales directamente en la malla mediante mapas de ID con un modificador (CTRL/Comando)
* [Pila de capas] Creación automática de máscaras de ID con arrastrar y soltar materiales en la malla con mapas de ID
* [Pila de capas] Desplazamiento automático de capas con arrastrar y soltar por la pila de capas
* [UI][Propiedades de la herramienta] Exponer el ajuste preestablecido de Substance
* [UI][menú Ayuda] Mejora del menú Ayuda
* [UI][Nuevo proyecto][Configuración del proyecto] Reorganización de la ventana
* [UI][Nuevo proyecto][Configuración del proyecto] Reemplazar término de malla por archivo
* [UI][Substance] Visualización de atributos de Substance en IU
* [Métodos abreviados] F4 cambia entre la vista 2D y 3D
* [Accesos directos] Nuevos métodos abreviados para activar o desactivar la galería de símbolos N y la máscara rápida U
* [Substance integration] Tenga en cuenta las sentencias &#39;visible if&#39; en los parámetros del Substance
* [Ventana gráfica] Las sombras no se ven forzadas a computarse después de mover la cámara
* [Contenido] Actualizar MeetMat con cámaras importadas
* [Contenido] Añadir una muestra con la dispersión subsuperficial activada - JadeToad
* [Contenido] Añade una nueva plantilla de proyecto PBR con la dispersión subsuperficial activada
* [Contenido] Se han actualizado los ajustes preestablecidos de exportación para añadir un nuevo canal de dispersión
* [Content][Shelf] Se ha añadido compatibilidad de dispersión subsuperficial para: pbr-metal-rough, pbr-metal-rough-alpha-test, recubierto de pbr, pbr-spec-gloss
* [Contenido] [Estante] Se ha añadido un canal de dispersión a 5 materiales inteligentes (mármoles y máscaras)
* [Contenido][Estante] 1 nuevo material de jade
* [Contenido][Estante] 1 nuevo material de cera

**Corregido:**

* [CMD] Diferentes resultados usando la misma línea de comandos con diferentes versiones
* [TDR] Si se configura TdrLevel, no hay errores en el registro
* [Baker] El mapa de Oclusión ambiental está volteado
* [Mapa de ID] Bloqueo al seleccionar fuera del rango 0-1
* [Iray] Bloqueo al cambiar conjuntos de texturas y volver al modo de Pintura
* [Ventana gráfica] Sincronizar áreas de colocación entre ventanas gráficas para arrastrar y soltar
* [Motor] Artefacto de moiré al aplicar mosaico a capas de relleno o pintar pinceles pequeños
* [Licencia] Comprobación de versión de software errónea del servicio de licencias
* [Licencia] Cambiar la forma de gestionar la autenticación
* [API] Llame al evento de API de scripts onNewProjectCreated incluso al crear con una plantilla
* [Sombreador] El sombreador compilado no se carga de la memoria caché cuando el archivo de sombreador no se compila
* [Shelf] Al exportar el archivo HDR. de la estantería, se generará un archivo con valores de sujeción
* [Exportar] EXR exportar abrazaderas RGB valores de color entre 0 y 1
* [Contenido] Ruido Procedimiento 3D Perlin Noise Fractal se pixeló

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.1.3 (2018.1.3)

*(Lanzado: 28 de junio de 2018)*

**Agregado:**

* [Preferencias] Propuesta de guardar el proyecto cuando se reinicie Painter

**Corregido:**

* [Plugin] El Substance Source de búsqueda no funciona
* [Materiales inteligentes] La importación de Materiales inteligentes provoca un bloqueo en algunos casos
* [Materiales inteligentes] Al eliminar Materiales inteligentes, en algunos casos se produce un bloqueo
* [Guardar] Guardar conduce a un bloqueo en algunos casos raros
* [Estante] Invertir no funciona en las Celdas 2 y 3
* [Estante] Error tipográfico en algunos Alpha
* [Estante] Algunos materiales de Substance no se procesan correctamente

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.2 (2018.1.2)

*(Lanzado: 12 de junio de 2018)*
Resumen: **Mejora en la velocidad de Hace un bake, Sistema de guardado mejorado, Reguladores actualizados, Plugin API actualizado, Traducción al chino, Relleno mejorado ahora Opcional**

**Agregado:**

* [Bakeres] Mejora del rendimiento con la nueva versión de baker
* Cuadro de diálogo Forzar visualización con GPU no compatible
* [Guardar] Exponer nueva funcionalidad de proyecto compacto (modo de guardado completo/compacto)
* [Guardar] Informar al usuario en caso de error de guardado
* [Limpiar] A continuación, guarde en modo completo/compacto
* [Reguladores] Mejora de la precisión de las barras y los reguladores de color/escala de grises
* [Reguladores] Adición de controles de flecha arriba/abajo
* [Reguladores] Misma zona de detección para los reguladores de barras de color y escala de grises
* [Plugin] Autoguardar siempre en modo incremental
* [Plugin] Opción para cambiar los complementos al nuevo estilo de interfaz
* [Idioma] Añadir traducción al chino
* [Padding] Opción para cambiar entre el relleno UV y el relleno contiguo de espacio 3D por conjunto de texturas en Ajustes de conjunto de texturas
* [Script] Exponer modo de guardado: completo/compacto o incremental
* [Script] Actualizar documentación de scripts/QML
* [Log] Indicar modo de guardado en log (completo/compacto o incremental)

**Corregido:**

* [Herramienta] La ranura de canal se transforma en una ranura de material en rellenos de un solo canal
* Bloqueo al cargar una malla (FBX) con algunas caras no asignadas por un material
* Bloqueo en Irán con NVIDIA GRID 5.2 en máquina virtual
* Bloqueo al deshacer la eliminación de un ajuste preestablecido de material
* Bloqueo al cargar algunos proyectos
* [Línea de comandos] Nueva línea de comandos para mallas de UDIM divididas por audio
* [Barra de herramientas] Reducción de la barra de herramientas
* [Instanciación] No se pueden crear instancias de mapas de bits en varios conjuntos de texturas
* [Ventana gráfica] La actualización no se completa al pintar en malla con UV en mosaico
* [Iray] El Mapa de normales se aplica dos veces a los dieléctricos
* [Shelf] Errores tipográficos en algunos parámetros del Substance (alfas, procedimientos y matfx)
* [Shelf] Error tipográfico para el mapa de bits &quot;Solo personal autorizado&quot;
* [Script] La función alg.shaders.materials() ya no funciona

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.1 (2018.1.1)

*(Lanzado: 3 de abril de 2018)*

**Corregido:**

* [Tablet] Problema al cambiar las opciones de interacción predeterminadas
* [Bakers] Bloqueo con la biblioteca de Assimp
* [Bakers] Regresión en el rendimiento con mapa A.O.
* [Iray] La Distorsión de lente no se aplica al canal del Alpha
* [Controladores] Actualización de los requisitos mínimos de controladores
* [3Dview] Las normales no se generan correctamente en mallas UDIM sin información de normales
* [Intel] Bloqueo con Substance Painter 2018.1.0
* [Intel][Viewport] Problema con relleno (defectos negros)

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.0 (2018.1.0)

*(Lanzado: 15 de marzo de 2018)*

**Agregado:**

* Nuevo estilo general (iconos, color, comportamiento)
* Nuevo diseño predeterminado
* [Tablet] Mejora de la experiencia del usuario al pintar
* [Menú principal] Ordenar primero los elementos nativos de las vistas y barras de herramientas
* [Menú principal] Sección Mover acciones rápidas de máscara en la ventana gráfica
* [Menú principal] Sección Mover las acciones del botón derecho al área de visualización
* [Menú principal] Cambiar el nombre del menú &quot;Ver&quot; por &quot;Ventana&quot;
* [Menú rápido] Nuevas propiedades de la herramienta haciendo clic con el botón derecho en la ventana gráfica
* [Widget de Dock] Nueva barra de herramientas de Dock para reducir/recuperar rápidamente
* [Configuración de la pantalla] Ventana de configuración de la cámara y del visor combinada
* [Pila de capas] Menú contextual del botón derecho
* [Pila de capas] Arrastra y suelta para mover cualquier efecto dentro de la misma capa
* [Barra de herramientas] Reorganización de la barra de herramientas y nueva barra de herramientas contextual
* [Barra de herramientas Herramientas] Dividir la herramienta Clonar en dos herramientas independientes
* [Herramientas, propiedades] Valor de escala de grises de fondo más claro en la previsualización
* [Herramientas propiedades] Organización en fichas (rellenar y herramientas)
* [Herramienta] El resultado de la pintura coincide con la galería de símbolos
* [Ventana gráfica] Nuevo cursor para la capa de relleno
* [Ventana gráfica] Navegación y pintura más fluidas (velocidad de marco más alta)
* [Ventana gráfica] Cuadro combinado de selección de material/canal/mapa en la ventana gráfica
* [Ventana gráfica] Reducción del parpadeo durante la rotación (sombra activada)
* [Shelf] Mostrar materiales de forma predeterminada al abrir Painter
* [Estante] Mejora del tiempo de carga de texturas y materiales Substance (2 a 6 veces más rápido)
* [Estante] Reorganizar las carpetas de materiales para que se ajusten a la estructura del Substance Source
* [Estante] Arrastre y suelte los materiales directamente en la malla en la ventana gráfica
* [Shelf] Nuevos ruidos 3D (Perlin, Perlin Fractal, Simplex y Worley)
* [Estante] Nuevo generador de máscaras de 3D linear gradient usando la posición de malla
* [Estante] Ruidos básicos actualizados para admitir la expansión no cuadrada
* [Estante] Se ha añadido una nueva plantilla y un ajuste preestablecido de exportación para Lens Studio (aplicación Snap)
* [Estante] Materiales inteligentes y Máscaras inteligentes actualizados para utilizar la última versión del Editor de máscaras (detalles micro)
* [Estante] Nuevo proyecto de muestra &quot;TilingMaterial&quot; para crear materiales de mosaico sin costuras
* [Estante] Nuevos ajustes preestablecidos de pincel (caligrafía, mojado, sombreado, etc.)
* [Reguladores] Nuevos reguladores y estilo y comportamiento de las barras de escala de grises y de color
* [Bakeres] Permite el uso del cuadro delimitador de escena completo para calcular el mapa de posición
* [Sombreador] Quitar el parámetro de fuerza de height de los parámetros de sombreador predeterminados
* [Motor] Motor del Substance actualizado
* [Motor] No hay discontinuidades o menos en los fragmentos UV
* [Complementos] Importa materiales descargados de Substance Source con mayor rapidez
* [Plugins] Actualice todos los plugins para que coincidan con el nuevo estilo general
* [Preferencias] La vista previa del color de fondo cambia automáticamente
* [Limpio] Menor riesgo de corrupción de proyectos
* [Abrir] Mejora del tiempo de apertura del proyecto
* [Nuevo proyecto] Nuevo proyecto: mejora del tiempo de actualización de la malla
* [Guardar] Ahorro de tiempo del proyecto
* [Log] Tipo de licencia registrado en el registro
* [TextureSet] Cambie el nombre del botón &quot;Hacer un bake Texturas&quot; por &quot;Hacer un bake mapas de malla&quot;
* Cambie el nombre de &quot;Mapas adicionales&quot; por &quot;Mapas de malla&quot;

**Corregido:**

* [Viewport] Mal rendimiento con mallas que contienen muchos subobjetos
* [Herramientas > Propiedades] Canal desactivado al arrastrar y soltar una imagen en la ranura de material
* [Herramientas, propiedades] La vista previa del pincel se rompe con las herramientas de difuminado y clonado
* [Conjunto de texturas] El orden de los canales es incorrecto al utilizar plantillas
* [Shelf] Falta icono para el generador de conversión de escala de grises
* [Estante] El número de círculo de Sign alfa está roto (falta fuente)
* Detección incorrecta de GPU integradas al iniciarse
* [Bloqueo] Arrastrar y colocar un recurso importado cuyo nombre tenga el carácter #
* [Motor] Problema de detección de Vram en la GPU integrada
* [Motor] Se han solucionado numerosos bloqueos en Substance Engine Linker
* [Motor] Artefactos cuadrados al cambiar la resolución
* [Efectos de posprocesamiento] El cambio de tamaño de la interfaz es lento cuando los efectos de posprocesamiento están activados
* [Bakeres] La unidad de escena no se respeta correctamente para los valores de distancia de rayos
* [Bakeres] El AO de la distancia del Mesh Occluder se fija en 1 independientemente del valor de entrada
* [Bakeres] La coincidencia por nombre ignora algunas mallas con nombres específicos
* [Bakeres] El color de la configuración de Polygroup de malla e ID de submalla siempre devuelve una imagen en negro
* [Bakeres] La Hace un bake de ID falla con mallas de FBX binarias de Blender
* [Sombreador] Ruido en el vista 2D con dota-2 y non-pbr-spec-gloss
* [Linux] Sólo se utiliza un subproceso de CPU al hacer un bake
* [MacOS] Bloqueo con el cursor del pincel moviéndose por la ventana gráfica

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* El proceso posterior de distorsión no se tiene en cuenta al exportar en IRay (alfa)

## Versión 3

### 3.4.2 (2017.4.2)

*(Lanzado: 24 de enero de 2018)*

**Agregado:**

* [Exportar] Obtenga el estado de una exportación con el progreso del paso
* [Exportar] Permitir cancelar una exportación
* [Exportar] Exportar texturas a Sketchfab sin perder calidad de mapa de normales
* [Export] Exportación en formato binario glTF (glb)
* [Exportar] Permitir cambiar el tamaño de las columnas en la ficha de configuración de la ventana de exportación
* [Sombreador] Agregar un registro de cambios para la API del sombreador
* [Scripting] Agregar funciones de devolución de llamada Antes y Después al exportar texturas
* [Israel] Actualización a SDK 2017.1 (compatibilidad con las GPU Volta)

**Corregido:**

* Bloqueo al salir de la aplicación antes de mostrar la ventana principal
* [MAC] Bloqueo al cargar mapas en escala de grises con IRA
* [MAC] VRAM detección no es correcta con el nuevo sistema operativo High Sierra
* [Complemento] La descarga de recursos de Substance Source ya no funciona
* [Scripting] Detección de versión mínima de plugin incorrecta
* [Exportar] Error al guardar el ajuste preestablecido de exportación después de exportar texturas
* [Instancing] Problema en generadores instanciados en un TextureSet sin Mapas Adicionales
* [Ventana gráfica] El tramado no funciona con una resolución superior a 4k
* [Ventana gráfica] La visualización de material de vista 2D está cubierta de ruido
* [Estante] Mejorar el tiempo de carga para los ajustes preestablecidos de estante
* [Motor] Fusión incorrecta al pintar en la selección de color

### 3.4.1 (2017.4.1)

*(Lanzado: 15 de diciembre de 2017)*

**Agregado:**

* [Scripting] Exportar malla mediante la API de scripting
* [Importar] Desactivar la importación de formatos de archivo de malla no compatibles (permitir solo obj, fbx, dae, ply)
* [Log] Indique con mayor precisión el problema de TDR en el archivo de registro

**Corregido:**

* Bloqueo si la aplicación se cierra antes de que finalice el rastreo de recursos
* Bloqueo al abrir proyectos con la herramienta Dedo/Clonar
* Bloqueo al utilizar rehacer después de deshacer un cambio de sombreado en la configuración del visor
* [Motor] Las texturas difieren entre Painter 2017.2 y 2017.4
* [Ventana gráfica] Al seleccionar un mapa de ID de una instancia, se muestra un color incorrecto
* bloqueo [Export] al exportar una textura normal o de oclusión no válida
* [Exportar] Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6
* [Plugin] El plugin de Photoshop ignora la selección de canales y siempre exporta todo
* [Capas] Los anclajes se rompen al copiar o pegar entre conjuntos de texturas
* [Capas] Algunas referencias de anclaje no se pueden restaurar si se rompen
* [Sombreador] el parámetro de rugosidad secundaria con revestimiento de pbr está roto
* [Steam] La ventana emergente del comprobador de versiones no debería estar visible al iniciarse

**Problemas conocidos:**

* [AMD] Se bloquea al intentar pintar en una malla. Se puede solucionar con una actualización del controlador de la GPU.

### 3.4.0 (2017.4.0)

*(Lanzado: 23 de noviembre de 2017)*

**Agregado:**

* [Instanciación] Permite crear instancias de parámetros en capas
* [Instancing] Permite saltar entre una capa de origen y una instancia
* [Instanciación] Añadir una acción &quot;Crear instancias en conjuntos de texturas&quot;
* [Instanciación] Indicar en la pila de capas instancias de reentrada (ciclos)
* [Instanciación] Elimina instancias cuando se elimina un origen
* [Instanciación] No permitir referencias de delimitador desde fuera de una carpeta con instancias
* [UI] Mueva la pila Deshacer a su propia ventana llamada &quot;Historial&quot;
* [Plugin] Integrar el plugin Live-Link de DCC
* [Motor] Mejore el rendimiento de la pintura con pintura dispersa
* [Exportar] Añadir opciones de borrador y reexportación al exportador de Sketchfab
* [Shelf] Añadir control &quot;flip&quot; para las sustancias de fuentes
* [Estante] Añadir 20 nuevos materiales de procedimientos
* [Shelf] Añadir 40 nuevos mapas grunges (basados en mapa de bits y de procedimiento)
* [Ventana gráfica] Activar colisiones de previsualización de pincel en otros conjuntos de texturas visibles
* Requisitos mínimos de actualización de controladores de GPU AMD

**Corregido:**

* Bloqueo al calcular Substance con resoluciones demasiado grandes
* Bloqueo al pintar con partículas
* [Ventana gráfica] Reflejo de specular incorrecto en la vista 2D con mallas específicas
* [UI] Aparecen algunas acciones no deseadas en la ventana Historial

**Problemas conocidos:**

* [Capas] Algunas referencias de anclaje no se pueden restaurar si se rompen
* Bloqueo al utilizar rehacer después de deshacer un cambio de sombreado en la configuración del visor

### 3.3.3 (2017.3.3)

*(Lanzado: 01 de diciembre de 2017)*

**Corregido:**

* [Steam] La ventana emergente del comprobador de versiones no debería estar visible al iniciarse
* [Exportar] Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6

### 3.3.2 (2017.3.2)

*(Lanzado: 20 de noviembre de 2017)*

**Agregado:**

* [UI] Mejora el diálogo de la nueva versión y añade el registro de cambios
* [IU] Indique si el mantenimiento ha caducado en el cuadro de diálogo Nueva versión
* [Licencia] Actualizar el sistema de licencias para gestionar las fechas de mantenimiento
* [Exportar] Cambiar el nombre de Adobe Standard Material a Adobe Dimension

**Corregido:**

* [Mac] La pintura genera cuadrados negros y corrupciones de texturas
* [Motor] La caché puede desaparecer en ocasiones en la ventana gráfica
* [Motor] Aparecen artefactos de bloqueo cuando se activa la compresión de memoria
* [Horneado] Mensajes de error extraños al hornear mallas específicas
* [Export] PSD no se han escrito correctamente y Photoshop no los reconoce correctamente
* [Capas] No debería ser posible copiar y pegar capas en varios proyectos
* [Substance] El espacio de color UserData para la entrada Normal se invierte en algunos casos
* [Estante] Micro-normal en generadores genera curvatura invertida
* [Estante] El filtro HSL también afecta al canal alfa
* [Linux] La instalación en Centos falla debido a la falta de dependencias
* El instalador no elimina todos los recursos de la instalación anterior en ciertos casos

### 3.3.1 (2017.3.1)

*(Lanzado: 26 de octubre de 2017)*

**Agregado:**

* [Exportar] Permita exportar la malla desde un proyecto
* [Estante] Quitar &quot;Sub-Shelf&quot; de los títulos de las pestañas
* Guardar la configuración posterior al proceso en plantillas
* Haz que el mensaje TDR sea más comprensible
* Mejorar la ventana Configuración para informar de errores

**Corregido:**

* Bloqueo al eliminar varios subestantes
* Bloqueo al cambiar de un nivel a otro durante un cálculo del motor
* [Mac] Bloqueo en la GPU Intel durante los cálculos del motor
* [Mac] [Ventana gráfica] Se producen errores de rendimiento cuando el tramado está activado
* [Mac] MacOS 10.13 se reconoce como &quot;Versión desconocida&quot; en el archivo de registro.
* [Baker] Hornear con una jaula ya no funciona
* [Capas] El método abreviado de teclado Ctrl+C (acción de copiar) ya no funciona
* [Capas] Al pegar capas, no se actualiza la interfaz de usuario con las referencias del anclaje
* [Anclaje] Duplicar o Copiar/Pegar capa con referencias rompe vínculos
* [Exportar] La exportación en 8K puede bloquearse o interbloquear la aplicación en algunos casos
* [Exportar] Varios problemas en el formato de archivo glTF generado
* [Importar] Volver a importar una malla con el mismo nombre de archivo ya no funciona
* [Plugin] La ventana de guardado automático siempre aparece encima de todo
* [UI] Bucle infinito al pulsar &quot;Escape&quot; en el cuadro de diálogo TDR
* [UI] Restaurar IU muestra una segunda barra de título en la ventana de la estantería

### 3.3.0 (2017.3.0)

*(Lanzado: 28 de septiembre de 2017)*

**Agregado:**

* [Exportar] Permitir la exportación de mallas y texturas para el proyecto de Adobe Felix
* [Export] Permitir la exportación al formato de archivo glTF
* [Motor] Optimizar el tamaño de las texturas en VRAM mediante la compresión de bloques
* [Ventana gráfica] Puede arrastrar y soltar una malla o un proyecto en la ventana gráfica
* [UI] Mejora el mensaje de advertencia sobre TDR
* [UI] El registro solo se debe mostrar si se solicita
* [UI] Permitir borrar el contenido de la ventana de registro
* [UI] Mostrar advertencias y errores en la barra de estado
* [UI] Mostrar pestañas en la parte superior como en los navegadores web
* [UI] Mejorar el contexto y los mensajes &quot;no pintables&quot;
* [IU] Añada una acción &quot;guardar como copia&quot; en el menú Archivo
* [Capa] Establecer el ajuste de mosaico predeterminado en 1 de forma predeterminada
* [Shelf] Filtro de degradado mejorado para admitir 10 colores dinámicos
* [Estante] Agregue un espacio en la consulta predeterminada de la miniestantería
* [Estante] Agregue una acción &quot;Abrir en el explorador&quot; para los recursos locales en el estante
* [Estante] Añadir plantilla y sombreador para Adobe Material Standard (Proyecto Felix)
* [Estante] Aumentar el mosaico máximo a 128 en sombreadores de capas de material
* [Estante] Se ha añadido curvatura sobel para microdetalles de generadores de máscara
* [Plugin] Añadir complemento de guardado automático con intervalo de tiempo personalizable
* [Scripting] Añadir una función &quot;Guardar como copia&quot;

**Corregido:**

* [UI] El diseño se interrumpe al iniciarse por primera vez
* El PSD [Export] generado en la exportación tiene errores de formato
* [Exportar] EXR siempre exporta el mapa de height de 8 bits
* [Exportar] Bloqueo al exportar mapas adicionales dañados
* [Importar] En algunos casos, los bordes duros no se conservan en mallas de polietileno bajas
* [Importar] Mensajes de error mejorados al importar mallas con problemas
* [Baker] Error al Hacer un bake la asignación de ID. si la opción Coincidir por nombre está activada
* [Ventana gráfica] El espacio tangente no se sincroniza con los bakeres
* [Efecto] Al retroceder una capa no se restaura la referencia de un anclaje
* [Efecto] Problema de actualización al crear un vínculo entre dos máscaras con anclajes
* [Efecto] No se deben enumerar los anclajes de máscaras encima de la máscara
* [Efecto] La opción Extraer Alpha de Anclajes no funciona
* [Motor] La máscara se invierte a sí misma tras el primer trazo del pincel
* [Motor] Bloqueo al cambiar el conjunto de texturas en un proyecto específico
* [Shelf] Bloqueo al eliminar un ajuste preestablecido de un proyecto
* [Shelf] Error en el filtro avanzado Tri-Plano
* [Estante] La escala de ruido de MG Mask Builder AO no funciona correctamente
* [Estante] MG Mask Builder tiene parámetros de curvatura invertidos
* [Estante] Los alfa importados generan una previsualización de esfera de material en lugar de una plana

### 3.2.0 (2017.2.0)

*(Lanzado: 27 de julio de 2017)*

**Agregado:**

* Puntos de anclaje: sistema de referencia de capas y máscaras
* [Layers] Capacidad de renombrar efectos de relleno y Pintura
* [Plugin] Complemento de Substance Source actualizado
* [Scripting] Permitir consultar la resolución del conjunto de texturas
* [Scripting] Permite obtener el estado del motor de pintura
* [Performance] Mejoras en la carga de proyectos y en las optimizaciones de estampado de pinceles

**Corregido:**

* [Herramienta] Problemas de rendimiento al ajustar parámetros de material
* [Motor] Trazos de pincel que desaparecen al cambiar la resolución (4K>2K)
* [Vista 3D] El espacio tangente no se sincroniza con los panaderos
* [Estante] La ruta de los estantes en los documentos de usuario no se crea automáticamente
* [Shelf] Hacer ajustes preestablecidos compatibles con versiones anteriores después de una actualización
* [Shader] El sombreado que no sea PBR ya no funciona
* [Bakers] Error de procesamiento de asignación de ID con la opción Coincidir por nombre activada
* [Ejemplo] Los nombres de los conjuntos de texturas del proyecto de muestra Meet Mat son incorrectos
* Guardar un proyecto antes de crear una plantilla devuelve errores de permisos de escritura

### 3.1.0 (2017.1.0)

*(Lanzado: 20 de junio de 2017)*

**Agregado:**

* [Plugin] Nuevo plugin de Substance Source (permite descargar recursos en el estante)
* [Estante] 4 Fuentes Nuevas (Japonés + Chino Simplificado, Typewriter, Segmento)
* [Estante] 230 nuevos Alpha (Mezcla de patrones, pinceles y digitalizaciones de huellas digitales)
* [Estante] 50 Nuevos Procedurales (Patrones de tela de ropa medieval y contemporánea)
* [Estantería] 2 Nuevos mapas ambientales (Mondarrain y Villa Nova Street)
* [Estante] 9 filtros nuevos (Edge Wear de detalle MatFx, abrazadera, HBAO, etc.)
* [Estante] Se ha mejorado el mapa de entorno de panorama predeterminado
* [Shelf] Nuevos ajustes preestablecidos de exportación de Arnold 5
* [Scripting] Permite importar recursos en la estantería

**Problemas conocidos:**

* [Exportar] La edición de un ajuste preestablecido de exportación es muy lenta

## Versión 2

### 2.6.2

*(Lanzado: 20 de octubre de 2017)*

<b>Agregado:</b>

* [Conjunto de texturas] Permitir la eliminación de conjuntos de texturas deshabilitados
* [Estante] Permite que varios usuarios escriban dentro de la misma carpeta de estante
* [Scripting] Poder recargar la carpeta de plugins
* [Scripting] Añada una versión mínima de API necesaria en los metadatos del plugin para garantizar la compatibilidad
* [IRay] Mejoras en el cuadro de diálogo Exportar imagen

<b>Corregido:</b>

* [Motor] Problema de desaparición de trazos al cambiar la resolución (4K>2K)
* [Bakers] Error de procesamiento de asignación de ID con la opción Coincidir por nombre activada
* [Bakers] Los mensajes de error no son lo suficientemente explícitos
* [Vista 3D] El espacio tangente no se sincroniza con los panaderos
* [Herramienta] Artefactos negros al utilizar la herramienta de difuminado
* [Shader] El sombreado que no sea PBR ya no funciona
* [Shader] &quot;pbr-coat&quot; está roto
* [Shader] La rugosidad del revestimiento del sombreador &quot;recubierto de pbr&quot; ya no tiene impacto
* [Shader] El sombreador de brillo de especificaciones no coincide con Iray y SD
* [Shelf] Bloqueo al cargar dos archivos con el mismo nombre pero diferentes extensiones
* [Estante] Ya no se pueden editar los ajustes preestablecidos en los estantes
* [Estante] No se puede establecer una vista previa personalizada para los recursos importados en el estante
* Los recursos cargados desde la caché pierden sus usos
* Guardar un proyecto antes de crear una plantilla devuelve errores de permisos de escritura
* Guardado de proyecto incorrecto si el nombre de archivo contiene dos puntos
* Importación de archivos con varios puntos (.) en el nombre de archivo causa problemas

### 2.6.1

*(Lanzado: 12 de mayo de 2017)*

**Agregado:**

* [TextureSet] No permitir la reasignación de materiales de malla a nada

**Corregido:**

* Bloqueo al cambiar de TextureSet después de reemplazar mapa con bake
* Bloqueo al hacer &quot;Deshacer y Rehacer&quot; después de cambiar el modo de fusión de la capa
* Bloqueo o congelación al utilizar el efecto &quot;selección de color&quot; con mapa de ID grande
* [Exportar] Los conjuntos de texturas cuyo nombre se ha cambiado no se ordenan alfabéticamente en la ventana de exportación
* [TextureSet] Restablecer el nombre predeterminado no comprueba la unicidad
* [TextureSet] El conjunto de texturas renombrado se desactiva después de volver a abrir el proyecto
* [Shelf] Falta contenido de plantillas predeterminadas
* [Estante] Las texturas no cuadradas se muestran como cuadradas
* [Sombreador] Cuando se desactiva un conjunto de texturas, se destruye el sombreador asociado
* [Scripting] alg.haga un bake.setTextureSetBakingParameters() ya no funciona
* [Scripting] Tutorial de error tipográfico en websocket
* [Scripting] Varios problemas en AlgWidgets
* [Log] Detección incorrecta de memoria virtual disponible en algunos casos

### 2.6.0

*(Lanzado: 27 de abril de 2017)*

**Agregado:**

* Agregar nuevo proyecto de muestra &quot;Meet Mat&quot;
* [Plugin] Nuevo plugin &quot;Resources Updater&quot;
* [TextureSet] Permite cambiar el nombre de los conjuntos de texturas y añadir una descripción a ellos
* [TextureSet] Permitir reasignar materiales
* [TextureSet] Añadir un botón de configuración en la ventana de lista de conjuntos de texturas
* [TextureSet] Mostrar conjuntos de texturas &quot;desactivados&quot; en la parte inferior de la lista
* [Substance] Utilice mapas adicionales con la resolución actual del conjunto de texturas para mejorar el rendimiento
* [Scripting] Permite actualizar un recurso utilizado en un proyecto (material, generador, etc.)
* [Scripting] Agregar una forma de agregar o quitar un estante
* [Scripting] Permitir consultar información de recursos en proyectos
* [Scripting] Permite recuperar una lista de shelfs disponibles
* [Scripting] Tutorial para mejorar la miniatura de AlgWidget
* [Exportar] Desactivar/Activar profundidad de bits según la compatibilidad con el formato de archivo
* [Log] Añadir nombre de plugin para imprimir en la consola
* [Log] Quitar error sobre conjuntos de texturas ocultos
* Actualizar la pantalla de bienvenida con nuevos iconos y texto para los ejemplos

**Corregido:**

* Bloqueo al actualizar una malla en proyectos específicos
* [Ventana gráfica] El color interior del plano de Simetría ya no es visible
* [Ventana gráfica] Algunos efectos posteriores al proceso se activan al utilizar la vista en solitario
* [Shaders] La fusión &quot;over\_premult&quot; no funciona correctamente
* [Shaders] Advertencia sobre la prueba alfa con el sombreador predeterminado
* [Shelf] Análisis incorrecto de etiquetas de Substance
* [Shelf] El intemperismo del Óxido MatFX no funciona correctamente
* [Shelf] HSL filtro está activado de forma predeterminada en canales incorrectos
* [Estante] El enfoque está activado de forma predeterminada en el canal Height/Normal
* [Exportar] Los ajustes preestablecidos de exportación no utilizan un mapa de normales OpenGL
* [Herramienta] Problemas de imprecisión al crear artefactos con la herramienta clonar/difuminar

### 2.5.3

*(Lanzado: 15 de marzo de 2017)*

**Corregido:**

* [Baker] Bloqueo al hacer un bake con mallas específicas

**Problemas conocidos:**

* [Mac] Las partículas pueden dañar la textura en algunos casos

### 2.5.2

*(Lanzado: 14 de marzo de 2017)*

**Corregido:**

* [Herramienta] Las tabletas Wacom no funcionan en Linux
* [Herramienta] Artefactos negros al utilizar la herramienta de difuminado
* [Baker] Se produce un error al Hacer un bake si se utiliza la coincidencia por nombre con una jaula
* [Bakeres] Oclusión ambiental rota al hacer un bake solo con Mapa de normales
* [Shelf] Los filtros genéricos no manejan alfa correctamente (contraste/luminosidad, paso alto, etc.)
* [Ventana gráfica] Problema de rendimiento al cargar un proyecto con sombras activadas
* [Ventana gráfica] Problema de tramado en Vista 3D en MacOS
* [Ventana gráfica] Las previsualizaciones de objetos se muestran incorrectamente cuando el perfil de color está activado
* [Iray] Bloqueo al volver a cambiar el proyecto a OpenGL si Iray no se inicializa
* El Brillo [IRay] se omite al procesar el sombreador SpecGloss/mdl
* [Sombreador] El sombreador Spec/Gloss no coincide con Iray y SD
* [Sombreador] La conversión de sRGB difiere de la conversión de LUT lineal a sRGB
* [Sombreador] Procesamiento incorrecto al cargar el proyecto con sombreadores obsoletos
* [Sombreador] Los sombreadores &quot;recubiertos de pbr&quot; ya no funcionan
* [Exportar] Algunos canales aún se exportan aunque no estén presentes en el conjunto de texturas
* [Capas] El modo de fusión &quot;mapa de normales de detalle inverso&quot; no funciona en canales en escala de grises
* [UI] Problema en &quot;Ventana de selección de color&quot; con monitor HDPI y zoom de visualización al 150 %

**Problemas conocidos:**

* [Mac] Las partículas pueden dañar la textura en algunos casos

### 2.5.1

*(Lanzado: 27 de febrero de 2017)*

**Corregido:**

* [Mac] La entrada de la tableta Wacom se rompe en 3D y Vista 2D
* [Bakeres] La coincidencia por nombre ya no funciona
* [Bakeres] El ajuste &quot;Normales medias&quot; ya no funciona
* [Iray] Procesamiento incorrecto con falta de mapa de normales hecho un bake
* [Iray] Los perfiles de color se comportan de forma diferente en comparación con el procesador OpenGL
* [Iray] Al exportar el procesamiento como mapa de bits, no se incluye la corrección del perfil de color
* [Substance] Los Filtros de material ya no funcionan
* [Herramienta] La opacidad del trazo no se almacena en los ajustes preestablecidos del pincel
* [Herramienta] La alineación UV del pincel del Clonar ya no funciona
* [Exportar] El canal de Desplazamiento debe estar centrado en 0,5 al exportar en entero
* [Plantilla] La ruta absoluta se almacena en Plantillas
* [TextureSet] La textura del canal se mantiene después de quitar el canal

**Problemas conocidos:**

* [Linux] Las entradas de tabletas Wacom no funcionan en 3D ni en Vista 2D
* [Mac] Las partículas pueden dañar la textura en algunos casos
* [Exportar] En casos muy raros, pueden aparecer rectángulos negros en las GPU AMD

### 2.5.0

*(Lanzado: 21 de febrero de 2017)*

**Agregado:**

* Compatibilidad añadida para las GPU AMD Radeon Pro y AMD FirePro
* [Herramienta] Compatibilidad añadida con la opacidad del trazo
* [Herramienta] Agregue un modificador que permita continuar con el último trazo de pincel
* [Iray] Actualización compatible con las GPU Pascal
* [Ventana gráfica] Compatibilidad añadida con perfiles de color (LUT)
* [Substance] Integrar nueva estructura (motor SD6)
* [UI] Aumentar la lista de tamaño de &quot;archivo reciente&quot; en el menú Archivo
* [Importar] Utilice la categoría de sustancias para rellenar el prefijo en el cuadro de diálogo de importación
* [Bakeres] Permitir hacer un bake texturas 8K
* [Panaderos] Permitir que se horneen resoluciones no cuadradas
* [Panaderos] Mejorar el consumo de memoria al hornear mallas pesadas de alto contenido de polietileno
* [Estante] Bloquear estantes (y proyectos) para prohibir la edición simultánea y evitar daños
* [Shelf] Lea la categoría y las palabras clave de las sustancias para usarlas para filtrar
* [Shelf] Permite excluir recursos del resultado de una consulta de búsqueda
* [Shelf] Cálculo del tiempo de las miniaturas mejorado
* [Estante] Permitir la incrustación de ajustes preestablecidos en proyectos
* [Estante] Permita contraer o expandir rápidamente la vista de árbol con MAYÚS
* [Estante] Permite guardar miniaturas cuando los recursos son de solo lectura (caché local)
* [Estante] Nuevo contenido : nuevos filtros (transformar, reflejar, triplanar, etc.)
* [Estante] Nuevo contenido : nuevos perfiles de LUT (clásicos y artísticos, como Film Noir, Vintage, etc.)
* [Estante] Nuevo contenido : 10 nuevos Substance de fuentes para generar rápidamente textos personalizados
* [Estante] Nuevas plantillas : Unity 5 y Unreal Engine 4
* [Estante] Se ha mejorado el filtro de HSL para que sea más fácil de usar por los artistas
* [Sombreador] Se ha agregado la compatibilidad con el canal de specular level en sombreadores PBR
* [Shader] Añadir compatibilidad con el tramado en el sombreador de prueba de Alpha
* [Sombreador] Añadir compatibilidad para la asignación de oclusión de paralaje en sombreadores PBR
* [Sombreador] Permite definir una interfaz de usuario personalizada para los parámetros de sombreador.
* [MatLayering] Creación de un nuevo canal de máscara para el flujo de trabajo de capas de materiales
* [Scripting] Permita escribir metadatos en un proyecto de SP
* [Scripting] Permitir la exportación con un ajuste preestablecido de exportación específico
* [Scripting] Permite recuperar parámetros de sombreado como JSON
* [Scripting] Agregar compatibilidad para conexiones WebSocket
* [Scripting] Añadir la posibilidad de cargar instancias del sombreador
* [Scripting] Añadir la posibilidad de crear un nuevo proyecto
* [Scripting] Permite recuperar la URL de la malla importada en un proyecto
* [Scripting] Permitir hagas un bake no cuadrados
* [Scripting] Informar de errores al configurar datos mediante la API de scripts
* [Substance] Añadir etiqueta de datos de usuario para especificar el formato de mapa de normales

**Corregido:**

* Bloqueo al elegir color con substancias
* Bloqueo al cargar una imagen que no es RGBA32f como mapa de entorno
* Bloqueo relacionado con la pintura en GPU AMD
* [Mesh] OBJ importación no reconoce materiales sin el archivo mtl
* [Mesh] La generación del nombre del conjunto de texturas del UDIM puede ser incorrecta en algunas mallas
* [UI] Botón Deshacer/Rehacer en la configuración del visor para robar el foco y detener el desplazamiento del ratón
* [UI] Algunas etiquetas se recortan incorrectamente en alta resolución
* [Capa] El modo de sustitución del efecto pintura se comporta de forma incorrecta en Máscara
* El modo de fusión de Restar [Layer] se comporta de forma incorrecta con alfa
* [Herramienta] El tamaño del pincel se vuelve enorme en vista 2D al pintar en bordes UV
* [Herramienta] La línea recta ajustada tiene un comportamiento errático con alta PPP
* [Herramienta] La resolución de la galería de símbolos a veces es incorrecta
* [Bakeres] Los valores de &quot;Distancia máxima del oclusor&quot; se fijan si &quot;relativo al cuadro delimitador&quot; está &quot;Desactivado&quot;
* [Sombreador] Las definiciones de canal de pilas y parámetros automáticos no coinciden
* [Vista 3D] Visualización incoherente del canal normal según la configuración del proyecto
* [Ventana gráfica] Algunos mapas de normales tienen valores sujetos que aparecen como artefactos
* [Ventana gráfica] Los efectos posteriores siempre están desactivados de forma predeterminada
* [Exportar] El ajuste de mezcla normal es incorrecto si falta un canal normal
* [Exportar] Generación de textura incorrecta en algunos casos en GPU AMD
* [Exportar] Los parámetros de Sombreador no se exportan correctamente si se encuentran dentro de un grupo
* [Exportar] Al editar un ajuste preestablecido de exportación en una estantería personalizada, se genera un error de registro
* [Shelf] El filtrado de vista de árbol no coincide exactamente con el nombre de la carpeta
* [Estante] Es difícil cambiar el nombre de un ajuste preestablecido de estante
* [Estante] El recurso de Sombreador importado en la Estantería no se conserva después de reiniciar
* [Estante] Contenido : Falta el ajuste preestablecido de la herramienta Soldadura
* [Estante] Contenido : El Tile Generator no funciona correctamente
* [Estante] Contenido : Se ha corregido una máscara incorrecta en el material inteligente sucio del neumático de goma
* [Estante] Contenido : Se ha corregido un nombre de grupo incorrecto en el material de la bolsa de cuero
* [Iray] La mitad de las mallas están desaparecidas en Irak
* [Linux] Bloqueo al arrastrar un recurso sobre la vista 3D
* [Mac] Las preferencias se restablecen en cada inicio en Sierra

**Problemas conocidos:**

* [Exportar] En casos muy raros, pueden aparecer rectángulos negros en las GPU AMD
* [Iray] Los perfiles de color pueden comportarse de formas extrañas a veces

### 2.4.1

*(Lanzado: 28 de octubre de 2016)*

**Corregido:**

* Bloqueo al crear un proyecto con una plantilla
* Bloqueo al cerrar el cuadro de diálogo de exportación durante una exportación
* [Mac] Errores al guardar el proyecto (error al guardar el ajuste preestablecido de exportación)
* [Shelf] Al crear un nuevo ajuste preestablecido, este se mostrará dos veces
* [Estante] Los ajustes preestablecidos no se pueden cargar en modo de solo lectura sin derechos de administrador

### 2.4.0

*(Lanzado: 27 de octubre de 2016)*

**Agregado:**

* [Shelf] Nueva interfaz para examinar los recursos (vista de árbol, filtros, etc.)
* [Estante] Permitir guardar una búsqueda como ajuste preestablecido
* [Estante] Permite crear una nueva ventana a partir de un ajuste preestablecido
* [Shelf] Nueva interfaz para importar recursos
* [Shelf] No copiar la bandeja algorítmica predeterminada en la carpeta Documentos
* [Shelf] Nuevos ajustes preestablecidos de partículas : Circuito eléctrico, Líneas eléctricas, Rococó, Venas pequeñas
* [Estante] Se han mejorado los ajustes preestablecidos de partículas antiguas para que sean más fáciles de usar (como &quot;Lluvia&quot;).
* [Shelf] Añadir nueva información en el menú contextual de recursos
* [Viewport] Mejora del rendimiento al cargar mapas de entorno
* [Viewport] Añada compatibilidad con mapas de entorno que no sean potencia de dos

**Corregido:**

* Bloqueo al quitar una máscara
* Bloqueo al pintar después de guardar un ajuste preestablecido
* Bloqueo con el desenfoque de entorno en algunas GPU
* Bloqueo al asignar un recurso incorrecto con el estante mini
* [Estante] Limpiar y guardar las etiquetas y los metadatos de eliminación de los recursos del proyecto
* [Estante] al importar un ajuste preestablecido, sus recursos se mostrarán en el estante
* [Exportar] El mapa normal generado a partir del canal de height tiene una intensidad baja
* [Exportar] Normal desde malla no siempre está presente en el mapa normal final
* [Exportar] La dilación con transparencia puede resultar en ocasiones sin transparencia
* [Scripting] &quot;alg.plugin\_root\_directory&quot; puede devolver una ruta de red truncada
* El botón Bloquear [TextureSet] se activa al volver a abrir proyectos no cuadrados

### 2.3.1

*(Lanzado: 07 de octubre de 2016)*

**Agregado:**

* [Plugin] [Photoshop] Permite especificar qué material/pila/canales se van a exportar
* [Scripting] Los nombres de función tienen algunas incoherencias

**Corregido:**

* [Export] El Alpha se puede descartar en los ajustes preestablecidos de exportación personalizados
* [Exportar] El Alpha obtiene una conversión de gamma incorrecta en canales sRGB
* [Exportar] Los documentos no cuadrados se exportan como cuadrados
* [Exportar] No es posible exportar mapas adicionales si falta uno
* [Iray] Algunos parámetros (como Intensidad de emisión) no tienen efecto
* [NVIDIA] Bloqueo al iniciar con NVIDIA Quadro K2200/GTX 750/760
* [AMD] Conjunto incorrecto de colores para miniaturas y vistas previas
* [AMD] Bloqueos y error del controlador al abrir archivos nuevos y abiertos
* [Log] Falta &quot;software-version&quot; en el archivo de registro

### 2.3.0

*(Lanzado: 15 de septiembre de 2016)*

**Agregado:**

* [Plugin] Nuevo plugin &quot;Exportar a Photoshop&quot; (exportar pila de capas completa)
* [Exportar] Permite especificar la anchura del relleno (en píxeles o infinito)
* [Exportar] Permite definir el tipo de fondo fuera de las UV
* [Estante] Nuevo sombreador de capas de material para mezclar 10 materiales
* [Estante] Nuevo sombreador de arcilla para ver los detalles con el height/canal normal
* [Estante] Nuevo filtro de iluminación horneada con entrada de entorno
* [Shelf] Se han actualizado algunos generadores de máscaras para añadir transformaciones no cuadradas
* [Ventana gráfica] Añadir mapa normal compuesto (normal+height+hornear) al modo solo
* [Scripting] Permitir la exportación de mapas adicionales
* [Scripting] Permitir consultar mapas adicionales disponibles por conjunto de texturas
* [Scripting] Permitir recuperar el formato de canal
* [Scripting] Añadir ejemplos en la documentación bancaria
* [Scripting] Permite consultar la visibilidad de una capa
* [Scripting] Permite consultar el modo de fusión y la opacidad de la capa
* [Scripting] Permite exportar mapas convertidos (mapas normales finales, archivos AO mixtos, etc.)
* [Substance] Lectura y conexión de usos personalizados
* [Métodos abreviados] Añadir tecla modificadora (MAYÚS) para retroceder en el modo solo cíclico
* [Exportar] Se ha actualizado el ajuste preestablecido de exportación predeterminado para desactivar alfa.
* [UI] Las miniaturas ahora solo se calculan si el motor está disponible
* [UI] Mostrar una mención cuando las miniaturas se están calculando

**Corregido:**

* Bloqueo en algunos proyectos antiguos al abrirlos
* Bloqueo con la caché de canales de textura dañada
* Bloqueo al mezclar más de 4 materiales con el flujo de trabajo de capas de material
* [UI] Los métodos abreviados de herramientas no funcionan si la barra de herramientas está oculta
* [UI] La barra de herramientas de Iray se etiqueta &quot;Sin título&quot; en el menú Ver
* [UI] Las barras de herramientas de los complementos se denominan &quot;Sin inclinación&quot; en el menú Ver
* [Baker] Al pulsar Intro al editar una configuración de horneado, se inicia el proceso de horneado.
* [Baker] Rangos incorrectos para algunos parámetros
* [Importar] Imposible importar mallas OBJ debido a números muy grandes
* [Importar] Algunos archivos OBJ se importan con demasiados subobjetos
* [Exportar] el fondo del canal se rellena con negro en lugar del color predeterminado en la exportación
* [Herramienta] Las partículas no funcionan correctamente si FOV es demasiado bajo
* [Herramienta] El color de previsualización del pincel es incorrecto con las máscaras en las subpilas
* [Ventana gráfica] Cuando el pincel se desplaza a áreas vacías en la vista 2D, se vuelve gigantesco
* [Ventana gráfica] Vista previa del pincel en blanco al pintar texturas normales
* [Scripting] Documentación incorrecta: &quot;ao&quot; en lugar de &quot;ambientocclusion&quot;
* [Scripting] El proceso iniciado con subprocess() se cierra al cerrar Painter
* [Estante] El filtro de iluminación al horno utiliza una entrada de AO incorrecta
* [MacOS] Se ha eliminado el proyecto Fire Hydrant (incompatible).
* El proyecto predeterminado se abre al cargar un archivo \*.spt (en lugar de \*.spp)

**Problemas conocidos:**

* [Plugin] Debido a Photoshop, el height y el canal normal no se pueden traducir tal cual

### 2.2.0

*(Lanzado: 22 de julio de 2016)*

**Agregado:**

* [Estante] Mejorar el sistema de búsqueda y las consultas
* [Estante] Añadir campo de búsqueda para miniestantes
* [Sombreado] Permite definir la precisión de paso de los reguladores
* [Shader] Añadir un botón Deshacer/Rehacer para parámetros de sombreado
* [Shader] La recarga de un sombreado no debe restablecer sus parámetros
* [MatLayering] Añadir compatibilidad para Controles dinámicos de capas de materiales y subpilas
* [MatLayering] Permita importar el archivo json para configurar los ajustes del sombreador
* [MatLayering] Desbloquear límite de muestras de textura (cambiar a texturas sin enlace)
* [Scripting] Permite establecer la configuración de los panaderos e iniciar su cálculo.
* [Substance] Usar &quot;uso&quot; para conexiones de entrada/salida además de identificadores
* [Herramienta] Permite seleccionar el canal de previsualización en la ventana gráfica de la herramienta Proyección

**Corregido:**

* Bloqueo durante el lanzamiento si las sustancias se encuentran en una carpeta incorrecta
* El informe de bloqueo a veces no funciona debido a un archivo de registro incorrecto
* [Iray] Los efectos posteriores no se actualizan cuando Iray está en pausa
* [Iray] El método abreviado de enfoque automático ya no funciona
* [Iray] El comportamiento del regulador de apertura cambia en función del tamaño del activo
* [Capas] El primer canal de materiales no está activado de forma predeterminada si todos están desactivados
* [Shader] No se imprimen errores si un &quot;param auto&quot; es incorrecto

**Problemas conocidos:**

* [Mac] El límite de muestras de textura está bloqueado en 16 (problema del controlador de la GPU)

### 2.1.1

*(Lanzado: 01 de julio de 2016)*

**Agregado:**

* [Licencia] Cambiar la ubicación del archivo de licencia
* [Ventana gráfica] Añada un método abreviado &quot;B&quot; para desplazarse entre mapas adicionales
* [Importar] Permitir importar FBX 2016/2017 correctamente
* [Herramienta] Quitar fichas cuando se utiliza la máscara rápida
* [Iray] Añadir información de dimensiones de escena
* [Iray] Permita aumentar el número máximo de muestras y el tiempo de procesamiento
* [UI] Actualizar el resultado inmediatamente al utilizar el botón +/- en los reguladores
* [UI] Mayor precisión de los reguladores de escala de grises
* [Exportar] No exportar un canal alfa para texturas que solo sean RGB
* [Exportar] Actualizar ajuste preestablecido de exportación de Dota 2
* [Estante] Nuevo patrón de &quot;Azulejos hexagonales&quot;
* [Estante] Nueva herramienta &quot;Soldadura&quot;
* [Estante] Filtros de acabado actualizados para proporcionar controles de dirección

**Corregido:**

* [Export] Imposible exportar archivos de PSD en 8 bits
* [Exportar] La exportación en 8K no está disponible en algunas configuraciones de hardware
* [Exportar] La ventana de Sketchfab se recorta
* [Exportar] Mapa de rugosidad incorrecto en el ajuste preestablecido de exportación de especificaciones/brillo
* [UI] Escribir en los reguladores de escala de grises ya no funciona
* [UI] Imposible colocar filtros en las entradas de sustancias (como Generadores)
* [UI] Algunos reguladores tienen comportamientos extraños
* [UI] El paso DeltaTime +/- para partículas es demasiado grande
* [Iray] Algunos proyectos bloquean la aplicación al cambiar a Iray
* [Iray] Bloqueo al detectar hardware
* [Herramienta] El color de previsualización del pincel es incorrecto en el modo Máscara
* [Herramienta] El selector de materiales se puede utilizar con herramientas incompatibles
* [Herramienta] La previsualización de proyección no cambia al flujo de trabajo Difusión con especificación/brillo
* [Estante] Al cambiar el sombreado predeterminado, se rompen las previsualizaciones de máscaras inteligentes/máscaras inteligentes
* [Estante] Algunos materiales inteligentes tienen nombres incorrectos
* [Shelf] Las formas alfa adicionales están dañadas y no se cargan
* [Viewport] Al cambiar al modo &quot;Mapa adicional&quot;, se muestra primero &quot;otro&quot;
* [Ventana gráfica] La ventana gráfica vuelve a cambiar a &quot;otro&quot; cuando no existe ningún mapa adicional
* [Crash][Linux] El informe de fallos no funciona en Ubuntu (Steam)
* [Crash][Linux] Los vínculos de URL web no funcionan en Ubuntu (Steam)
* [Bloqueo] [Windows] Quitar &quot;Crashwatcher&quot; cuando Substance Painter ya no se ejecuta
* [Bloqueo] [Mac] El sistema de informes de fallos no funciona correctamente
* [Bloqueo] Importar una malla mientras se importa una malla provoca un bloqueo
* El método abreviado de selección de conjunto de texturas se restablece en nada después de reiniciar

### 2.1.0

*(Lanzado: 02 de junio de 2016)*

**Agregado:**

* [UDIM] Importación de mosaicos UDIM de una malla como conjuntos de texturas
* [Linux] Se ha agregado la compatibilidad con CentOS 6.6 y Ubuntu 12.4
* [Exportar] Añadir resolución 8K (experimental)
* [Exportar] Permite elegir la profundidad de bits durante la exportación
* [Baker] Permita hornear varios conjuntos de texturas a la vez
* Compatibilidad con monitores de alta resolución (escala de PPP alta)
* [Scripts] Establecer resolución y relleno personalizados por textura al exportar
* [Ventana gráfica] Permite cambiar entre el conjunto de texturas haciendo clic en la malla (mediante Ctrl+Alt+Clic)
* [Ventana gráfica] Vaya a donde se encuentra el cursor del ratón al hacer zoom con la rueda del ratón
* [UI] Actualizar la visualización predeterminada del color de fondo y el mapa de entorno
* [UI] Añadir información sobre herramientas con nombres originales para los canales de usuario
* [UI] Cambiar el color de fondo de los canales a los que no se puede cambiar el nombre
* [Herramienta] Quitar fichas cuando se utiliza la máscara rápida
* [Sombreador] Permite definir grupos para parámetros de sombreador y materiales/máscaras
* [Motor] Optimización del estampado de tamaño pequeño
* [Stencil] Añada &quot;W&quot; como método abreviado para cambiar temporalmente la máscara
* [Estante] Añada un botón de cruz para borrar el campo de búsqueda
* [Estante] Cargar el Alpha con un solo clic
* [Shelf] Nuevo ajuste preestablecido de exportación : UDIM Vray, Arnold UDIM, Especificación/Brillo de Metal/Rugoso
* [Shelf] Nuevos alfa : formas geométricas, vetas y signos
* Agregar nombre y versión en las propiedades del ejecutable de Substance Painter

**Corregido:**

* [Substance] Imposible utilizar el canal normal y el mapa adicional al mismo tiempo
* [Iray] La refracción de MDL y el ajuste de absorción no funcionan
* [Iray] No se conserva la escala de escenas original
* [Estante] El Specular/plantilla de Brillo usa un sombreador incorrecto
* [Exportar] El ajuste preestablecido de exportación predeterminado no exporta algunos mapas (como AO)
* [Ventana gráfica] El punto de tabla dinámica no se actualiza al hacer clic fuera de las coordenadas UV en la vista 2D
* [UI] Los valores del regulador se redondean
* [UI] A veces, al editar los valores de los reguladores, hay un espacio libre muy pequeño
* [Nuevo proyecto] La lista desplegable de plantillas no se ha actualizado correctamente (de 1.x a 2.x)
* [Scripts] Se ha corregido el comportamiento de &quot;pasar cursor&quot; en los botones personalizados
* [Mac] Al deshacer un proyecto vacío, se bloquea la cámara

**Problemas conocidos:**

* El informe de bloqueo no está disponible en Ubuntu
* Es posible que algunos botones de URL no funcionen. Consulta nuestras preguntas frecuentes para obtener una solución alternativa

### 2.0.5

*(Lanzado: 29 de abril de 2016)*

**Agregado:**

* [Estante] Se ha añadido o actualizado una plantilla que no es de pbr, sombreador y ajuste preestablecido de exportación
* [Estante] Se ha actualizado el ajuste preestablecido de exportación UE4 para incluir la Oclusión ambiental

**Corregido:**

* Bloqueo al abrir y guardar algunos proyectos con recursos dañados
* [Ventana gráfica] La Malla metálica aparece rota en la Vista 2D
* [Shelf] Rendimiento mejorado de algunos mapas de entorno de estudio
* [Shelf] Algunos mapas de entorno de estudio están duplicados
* [Estante] Falta &quot;Material de iluminación Hecho un bake&quot;
* [Shelf] Falta el generador de conversión de escala de grises

### 2.0.4

*(Lanzado: 26 de abril de 2016)*

**Agregado:**

* Mejora de los choques de malla y optimiza la representación de mallas metálicas
* Mejorar el rendimiento y la gestión de la memoria con grandes proyectos
* Mejorar la precisión y el paso del regulador
* [UI] El motor de actualización solo se actualiza al validar un control deslizante (no al introducir un valor).
* [UI] Mover Iray cambiar a un botón dedicado en la barra de herramientas principal (y cambiar su método abreviado)
* [Herramienta] Agregar configuración para el comportamiento de ubicación de origen de la herramienta de clonación
* [Sombreador] Permitir la lectura de colores de vértices de malla en sombreadores personalizados
* [Scripting] Permite recuperar la lista de conjuntos de texturas, canales y capas
* [Scripting] Añadir funciones auxiliares (url a ruta, obtener ruta de exportación del proyecto)
* [Mac] Detectar la versión &quot;El Capitan&quot; de Mac Os en el archivo de registro

**Corregido:**

* Bloqueo después de la segunda exportación a Substance share
* Bloqueo al copiar una capa entre conjuntos de texturas con datos de Máscara rápida.
* Algunos proyectos tienen un actualizador muy largo que consume mucha memoria
* [Herramienta] Bloqueo al seleccionar un ajuste preestablecido de objeto con la herramienta de clonar/difuminar
* [Baker] La carga de archivos de FBX tarda demasiado en ejecutarse en mallas pesadas
* [Viewport] Mapa de entorno Estirado en algunos equipos
* [Ventana gráfica] Conversión de gamma incorrecta del alfa del pincel
* [Export] Alpha se almacena como transparencia en lugar de como canal independiente con archivos Tiff.
* [Exportar] El canal normal siempre se exporta como OpenGL
* [Iray] Faltan nombres de reguladores para la configuración de Iray
* [Iray] El procesamiento se realiza con una resolución incorrecta en Retina/High DPI
* [Iray] Bloqueo al cambiar el tamaño de la interfaz en modo Iray
* [Israel] Gran ralentización del rendimiento al renderizar en algunas resoluciones bajas
* [Iray] La pausa no funciona (Iray sigue computando en segundo plano)
* El canal normal a veces tiene defectos de cuadrados negros
* El canal normal se invierte mediante filtros de escala de grises
* El canal normal no se fusiona correctamente si la pila tiene alfa
* El proyecto se edita en el disco al abrir un proyecto aunque no se haya guardado todavía
* La reimportación de una malla en algunos proyectos produce un rendimiento de GPU muy malo
* La orientación del pincel no es correcta al no tocar una malla
* Falta el logotipo de substance share en la pantalla de bienvenida

### 2.0.2

*(Lanzado: 25 de marzo de 2016)*

**Agregado:**

* [Iray] Actualizar la plantilla y el sombreador Spec/Gloss para que sean compatibles con Iray
* [Exportar] Exportar capturas de pantalla a ArtStation
* [Scripting] Ejecución de soporte desde el directorio de plugins
* [Scripting] Permitir &quot;Guardar como&quot;
* [UI] Permita hacer doble clic en un regulador para editar su valor
* Mover muestra de Vela al Substance share
* Nuevo proyecto de muestra : Previsualización de esfera
* Advertencia a los usuarios sobre el conflicto de extensión de shell

**Corregido:**

* El instalador anula la instalación de Substance Painter 1.x
* [UI] El diseño de la lista de canales se rompe con los filtros
* [UI] No se muestran los parámetros de Sombreador
* [UI] Cambiar el tamaño de la ventana de capa recorta incorrectamente el contenido
* [Herramienta] El canal de opacidad no siempre se usa correctamente
* [Herramienta] El difuminado/Clonar no funciona con la Simetría
* [Herramienta] La opacidad de la vista previa del pincel es incorrecta en algunos canales
* [Iray] Bloqueo al utilizar Iray cuando todavía no se ha creado
* [Iray] No se pueden cargar datos de configuración de iris del proyecto
* [Iray] Iray no se ocupa de la modificación de la configuración después de haber sido pausado
* [Estante] Importar un material al estante no funciona
* La galería de símbolos no funciona con el canal Normal
* Bloqueo al pintar en algunos proyectos
* Bloqueo al pintar con partículas en algunos proyectos
* Bloqueo con el Procesador de píxeles durante algunos cálculos

### 2.0.0

*(Lanzado: 16 de marzo de 2016)*

**Agregado:**

* Método abreviado a Substance Almacén en la barra de herramientas principal
* Procesador Iray con modo de visualización y exportación de capturas de pantalla
* Compatibilidad con la creación y el uso de &quot;máscaras inteligentes&quot;
* Compatibilidad con el flujo de trabajo de PBR de Specular y glosinas (con el nuevo canal difuso)
* Encadenamiento de Substance (enchufe de sustancias en las entradas de imagen de sustancias)
* Compatibilidad de scripts con complementos personalizados
* Mejorar la conversión de Height a Normal utilizando un filtro Sobel
* Cambiar resolución de previsualización de proyección/galería de símbolos a 2K
* Agregar canal normal de forma predeterminada para proyectos nuevos
* Leer la etiqueta de datos de usuario del nodo de salida para activar o desactivar canales de una sustancia de forma predeterminada
* Exponer fusión Normal/AO en ajustes de TextureSet
* [Herramienta] Nueva herramienta de difuminado para fusionar y difundir colores
* [Herramienta] Nueva herramienta de Clonar para copiar parte de las texturas
* [Herramienta] Permite seleccionar canales para las herramientas Dedo, Clonar y Borrador
* [Capa] Añadir nombre de Substance para el nombre del efecto Rellenar
* [Layer] Permite exportar la máscara al portapapeles
* [Ventana gráfica] Cambiar entre el modo de perspectiva y el modo ortográfico
* [Ventana gráfica] Permitir el control del campo de visión en modo de Perspectiva
* [Ventana gráfica] Permite definir la Profundidad de la distancia del campo con CTRL+clic central
* [Ventana gráfica] Permite arrastrar y soltar mapas de entorno en la Vista 3D.
* [Ventana gráfica] Se han mejorado los comentarios cuando el motor realiza cálculos potentes.
* [Export] Permite exportar parámetros de sombreador en un archivo json
* [UI] Interfaz de actualización con nuevos iconos, colores y diseño
* [UI] Añadir nombres de recursos a los miniestantes
* [UI] Contraer &quot;asignación de canales&quot; de forma predeterminada
* [Sombreado] Seleccione un color personalizado para los parámetros de textura del sombreado
* [Estante] Pregunte dónde importar archivos al arrastrar y soltar recursos
* [Estante] Nueva esfera de previsualización para generadores y materiales inteligentes
* [Estante] Añadir sombreador de brillo de Specular
* [Estante] Nuevas formas de superficie dura
* [Estante] Nuevas texturas y formas de Alpha
* [Estante] Nuevas texturas de piel
* [Estante] Nuevos materiales basados en escaneo y materiales inteligentes
* [Estante] Nuevos materiales inteligentes y soporte de especificaciones/brillo de los antiguos
* [Estante] Nuevos filtros de acabado para la simulación de superficies metálicas
* [Estante] Nuevo generador de máscara potente &quot;Editor de máscara&quot;
* [Estante] Materiales antiguos retrabajados y limpiados
* Nuevo proyecto de muestra &quot;Vela&quot;

**Corregido:**

* [Ajustes] El proyecto anula la velocidad de zoom y la rotación de la cámara
* [Ventana gráfica] Un problema de precisión en la textura normal predeterminada genera reflejos incorrectos
* [Ventana gráfica] La viñeta está activada de forma predeterminada
* [Ventana gráfica] Aparecen artefactos en los bordes del mapa de entorno (GPU Nvidia)
* [Ventana gráfica] La miniatura en modo de proyección/galería de símbolos es muy larga de cargar
* [Baker] Almacenar texturas horneadas en enteros de 16 bits en lugar de 32 bits
* [Capa] Las sustancias obsoletas se muestran incorrectamente en la pila
* El color predeterminado y la profundidad de bits de algunos canales son incorrectos (p. ej.: Specular, Brillo)
* Se ha corregido el comportamiento del borrador para deshabilitar la fusión en modo de paso a través

**Problemas conocidos:**

* La simetría no funciona con las herramientas Dedo y Clonar
* Falta la exportación de ArtStation

## Versión 1

### 1.7.3

*(Lanzado: 1 de marzo de 2016)*

**Agregado:**

* [Exportar] Añadir una opción para desactivar el relleno
* [Estante] Compatibilidad con la jerarquía de subestantes dentro de una carpeta de estante

**Corregido:**

* Bloqueo al guardar sobre un archivo de solo lectura anterior
* Bloqueo al abrir un segundo proyecto
* Bloqueo al cargar algunas miniaturas (estanterías, capas o información sobre herramientas)
* La desactivación de &quot;Conservar posiciones de trazos en la malla&quot; no funciona
* [Exportar] El aumento de escala de los mapas de bits se realiza con el filtrado más cercano
* [Shelf] El descubrimiento de recursos es muy lento
* [Shelf] Los filtros de desenfoque no son compatibles con 16 bits
* [Herramienta] La simetría no funciona si se carga un ajuste preestablecido antiguo de la herramienta
* El cuadro de diálogo Color del canal de Specular no convierte el espacio de color

### 1.7.2

*(Lanzado: 13 de enero de 2016)*

**Agregado:**

* [Capas] Permite especificar el segmentado predeterminado para las capas de relleno

**Corregido:**

* [Exportar] La exportación de Sketchfab ya no funciona
* [Layer] El filtrado bilineal se aplica incluso en Relleno sin ninguna transformación
* [Herramienta] Rendimiento deficiente al utilizar Substance con entradas de imagen en modo de proyección
* [Herramienta] El selector de material está roto

### 1.7.1

*(Lanzado: 18 de diciembre de 2015)*

**Corregido:**

* Bloqueo al cambiar el conjunto de texturas
* Reproducciones lentas al pintar

### 1.7.0

*(Lanzado: 17 de diciembre de 2015)*

**Agregado:**

* [Interpretaciones] Calcula el contenido de las capas y sus miniaturas al mismo tiempo
* [Exportar] Guarde la ruta de exportación como relativa cuando esté al lado del proyecto
* [Capas] Se ha añadido un nuevo modo de fusión : restar y agregar/sub
* [Layers] Nuevo filtrado HQ bilineal para capas de relleno
* [Sombreador] Establezca un sombreador predeterminado para la generación de miniaturas en las preferencias.
* [Sombreador] Permite especificar un sombreador por conjunto de texturas
* [Sombreador] Dejar tomar muestras de las texturas de la estantería
* [Herramienta] Nuevo comportamiento de pincel &quot;Ajustar&quot; para pintar
* [Herramienta] Mejora del filtrado y reducción del suavizado al pintar
* [Herramienta] Calidad de pintura de subpíxeles mejorada
* [Herramienta] Se ha eliminado la visualización &quot;básica&quot; de la configuración del pincel y se ha mejorado el icono de apertura/cierre del marco.
* [Menú] Añadir iconos de efectos en el menú contextual
* Creación de plantillas desde Proyectos
* [Estante] Nuevas plantillas : PBR, Dota 2
* [Shelf] Nuevo ajuste preestablecido de exportación : Dota 2
* [Shelf] Nuevos sombreadores : Dota 2, pintura de coches PBR, revestimiento PBR, terciopelo PBR
* [Estante] Material nuevo : Óxido de acero y desgaste, iluminación estilizada
* [Shelf] Nuevos filtros : Difuminado direccional, iluminación estilizada
* [Estante] Nuevo pincel : disco duro por defecto suave y duro por defecto con un nuevo alfa para un mejor control de la dureza
* [Estante] Nuevos generadores : Distancia y luz 3D
* [Estante] Pinceles actualizados con proyección de ceñido y sacrificio de caras posteriores (activado de forma predeterminada)
* [Shelf] Se ha actualizado Ruido blanco con la versión de procesador de píxeles para agilizar el cálculo

**Corregido:**

* [Pantalla de bienvenida] Vínculo de Tutorials para enviar a vídeos antiguos
* [Canales] Si se indica &quot;no&quot; para rellenar la creación de capas con AO, se sigue creando la capa.
* [Canales] Los nombres de canales de UserX no se propagan en la interfaz
* [Ventana gráfica] La entrada de máscara está vacía en la lista de canales solo
* [Compartir] Al exportar un alfa a Compartir desde SP, se crea un archivo .image ilegible
* [Licencia] Solucionar problemas de activación para nombres de usuario que no tengan caracteres ASCII
* El cuadro de diálogo de parámetros de color de [Shader] desaparece al seleccionar un color
* [Shelf] Las miniaturas no se descargan de la memoria cuando no se utilizan
* [Estante] Filtro de degradado fijo
* [Herramienta] La Simetría no funciona con la galería de símbolos o la proyección
* [Herramienta] Nombre incorrecto al crear un nuevo ajuste preestablecido de pincel
* La opción Conservar trazo permanece desactivada incluso al volver a importar una malla
* Restablecimiento del controlador (TDR) al calcular partículas con un tamaño grande.

### 1.6.1

*(Lanzado: 09 de noviembre de 2015)*

**Corregido:**

* Bloqueo al abrir el proyecto si la vista 2D está visible
* Bloqueo al crear un nuevo ajuste preestablecido de exportación si el estante actual no existe
* [Herramienta] El icono del selector de material puede permanecer visible
* [Herramienta] El selector de material oculta el cursor del ratón al pintar al mismo tiempo
* [Shelf] Los metadatos se escriben en el disco después de cada salida

### 1.6.0

*(Lanzado: 29 de octubre de 2015)*

**Agregado:**

* Compatibilidad oficial con Windows 10
* [Substance] Contraer grupos de parámetros de sustancia de forma predeterminada
* [Substance] Añadir nueva estructura (Mejorar el rendimiento de los Procesadores de píxeles)
* [Ventana gráfica] Permite desactivar la visualización del plano de simetría en modo de simetría.
* [Ventana gráfica] Mejora del procesamiento y el rendimiento de las sombras
* [Ventana gráfica] Pausar cálculo de sombras al pintar
* [Viewport] Mejora del rendimiento de representación de mallas metálicas
* [Motor] Mejore la administración de la memoria Vram para reducir su espacio
* [Motor] Mejore la actualización de la textura en las GPU AMD para obtener un mejor rendimiento
* [Motor] Desactive la configuración de optimización de subprocesos en las GPU NVIDIA para obtener un mejor rendimiento
* [Effect] Añade una etiqueta para solicitar la entrada de imagen &quot;acolchada&quot;
* [Layer] Aumenta la precisión del Desplazamiento de UV/escala en el relleno
* [Capa] Haga que el regulador de escala sea exponencial en el relleno
* [Capa] Permite arrastrar y soltar materiales directamente en la pila de capas.
* [Capa] Permite arrastrar y soltar filtros directamente en la pila de capas
* [Capa] Ajuste el color del pincel de máscara al color de máscara recién creado
* [Sombreador] Exposición de varias texturas
* [Sombreador] Expone la función de asignación de gamma y tono para permitir funciones personalizadas
* [Bakeres] Cambiar la configuración predeterminada del baker de posición para el uso TriPlanar
* [Herramienta] Cambie el nombre &quot;Geometry Decal&quot; por &quot;Polygon Fill&quot;
* [Shelf] Actualice los generadores para que sean compatibles con TriPlanar : MG Desgaste del borde del metal, MG Constructor de la máscara, MG Fibra de vidrio, MG Dirt
* [Estante] Actualizar los materiales con nuevos ajustes y eliminar los materiales no utilizados
* [Estante] 22 nuevos materiales inteligentes (plástico, hierro, tela, acero y más)
* [Estante] Actualiza los filtros Enfocar, Desenfocar y Deformar con entrada de imagen acolchada para evitar costuras
* [Estante] Mejorar la configuración de deformación para facilitar el uso
* [Estante] 2 Nuevos ruidos procedimentales : Ruido de Perlin 3D y ruido de Worley 3D

**Corregido:**

* [Motor] La detección de la cantidad de Vram para la GPU dedicada es incorrecta en Mac
* [Motor] Las texturas se convierten en versiones más oscuras en la ventana gráfica
* [Motor] Rendimiento deficiente al pintar debajo de varias capas
* [Motor] Las capas calculadas al abrir el proyecto difieren de la versión almacenada en caché
* [Substance] Resultados incorrectos en 4K en Mac
* Los parámetros de [Substance] están en el orden incorrecto
* [Shader] Los sombreadores de tono y pixelado son totalmente negros
* [Shader] Los parámetros desaparecen después de cambiar env-map
* [Shelf] Bloqueo al colocar archivos PNG en la carpeta del generador
* [Estante] Las miniaturas se generan con poca rugosidad
* [Herramienta] Bloqueo al utilizar un mapa de bits en el pincel alfa en Windows
* [Exportar] El ajuste preestablecido de exportación de mapa adicional ahora exporta un mapa del RGB para Posición

### 1.5.7

*(Lanzado: 24 de septiembre de 2015)*

**Corregido:**

* El informe de bloqueos ya no funciona

### 1.5.6

*(Lanzado: 21 de septiembre de 2015)*

**Agregado:**

* [Shelf] Mejora la calidad de la representación de miniaturas (usa texturas de 1K)

**Corregido:**

* [Compartir] Imposible firmar con otra cuenta
* [Estante] Las miniaturas pesan demasiado en el disco
* [Estante] Los Materiales inteligentes son muy lentos de cargar
* [Windows] Solucionar problemas de instalación del servicio de licencias
* [Canales] El mapa de Transmisivo se crea como G8 de forma predeterminada

### 1.5.5

*(Lanzado: 15 de septiembre de 2015)*

**Agregado:**

* [Estante] Exportar recursos al Substance share
* [Estante] Añadir nueva vista previa de esfera para materiales
* [Estante] Utilice el mapa de env &quot;Patio acristalado&quot; para generar miniaturas
* [Estante] Aumenta la resolución del tamaño de la miniatura a 512x512 píxeles
* [Vista 3D] Exponer el valor de rotación del entorno
* [Windows] Firme la aplicación

**Corregido:**

* [Bakeres] Resultados incorrectos al hacer un bake mapas al mismo tiempo
* [Vista 3D] El mapa de env se muestra cuando no hay ningún proyecto abierto.
* [Capas] Los Generadores de máscaras no funcionan en el contenido de las capas
* [Layers] Puede realizar la pintura en capas ocultas
* [Shelf] Dirt\_5 y Dirt\_6 son idénticos
* [Estante] Algunos generadores de máscaras están pixelados o son de baja calidad
* [Herramienta] Rotación de gizmo incorrecta en determinados ángulos.
* [Herramienta] Si hay demasiados canales, los botones de canal se recortan
* [Herramienta] El método abreviado de inversión de máscara para Máscara rápida no funciona
* [Export] Sketchfab: el botón de cancelación no se ha tenido en cuenta correctamente
* [Licencia] Error de activación cuando no se puede copiar la licencia
* El limitador de velocidad de fotogramas ya no funciona en la IU

### 1.5.0

*(Lanzado: 20 de agosto de 2015)*

<b>Agregado:</b>

* [Sombreador] Añadir número de línea en Sombreador compilando mensajes de error
* [Shelf] Mejora la calidad de las vistas previas en miniaturas
* [Shelf] Automatiza la generación de miniaturas para Materiales inteligentes
* [Herramienta] Método abreviado para controlar el ajuste de dureza en la sustancia
* [Herramienta] Usar el widget de escala de grises para la calcomanía geométrica sobre una máscara
* [Herramienta] Método abreviado para invertir el color de la pintura mientras se pinta en un mapa en escala de grises
* [Ventana gráfica] Permite mostrar la malla metálica y cambiar su color
* [Ventana gráfica] Desenfocar el fondo del entorno
* [Controles] Añadir rotación a los métodos abreviados de pincel del ratón
* [Exportar] Exportar a Sketchfab
* [Exportar] Creación de ajustes preestablecidos de exportación para procesadores
* [Exportar] Añadir reflejo de mapa convertido, F0 y 1/IOR
* [UI] Pantalla Añadir bienvenida
* [UI] Actualizar diseño predeterminado
* [UI] Añade información sobre herramientas que faltan y cambia el nombre de alguna entrada del menú
* [Layers] Exportar la máscara seleccionada actualmente como mapa de bits
* [Capas] Añade la acción &quot;invertir máscara&quot; en el menú contextual

<b>Corregido:</b>

* [Proyecto] Si los pivotes de mallas son diferentes en el FBX, las mallas se explotan al importar
* [Substance] Los Substance utilizados en las herramientas de proyección están bloqueados en 256\*256
* [Capas] Bloqueo al utilizar la máscara transparente
* [Exportar] Conversión de gamma incorrecta en texturas muy oscuras
* [Exportar] El mapa de posición solo se puede utilizar en los ajustes preestablecidos de exportación como mapa de escala de grises
* [Herramienta] El color de inicio de la calcomanía geométrica es negro cuando se utiliza en una máscara
* [Herramienta] El método abreviado de rotación no funciona si no hay dureza en el alfa

### 1.4.2

*(Lanzado: 15 de julio de 2015)*

**Corregido:**

* [Herramienta] Bloqueo al utilizar la pegatina geométrica con la máscara rápida
* La actualización de un proyecto de la versión 1.4.0 a la 1.4.1 consume toda la memoria del equipo
* Importación incorrecta del formato de proyecto antiguo
* Los estantes personalizados analizan toda la jerarquía y duplican activos en todas partes

### 1.4.1

*(Lanzado: 23 de junio de 2015)*

**Agregado:**

* [Ventana gráfica] Permite acoplar paneles en paralelo
* [Efecto] Agregue un fondo y una regla para el efecto de nivel
* [Efecto] Añada un efecto de pintura que permita trabajar sobre otro efecto

**Corregido:**

* [Shelf] La generación de miniaturas se interrumpe si no hay ningún proyecto abierto
* [Estante] La previsualización de ajustes preestablecidos de material no se genera
* [Estante] Las previsualizaciones de material se generan en una malla con normales invertidas
* [Shelf] Las miniaturas siempre se vuelven a calcular debido a una función hash incorrecta
* [Estante] Hacer clic en un material de Substance no conecta mapas adicionales
* [Herramienta] Valor incorrecto muestreado con el selector de material
* [Herramienta] Selector de color seleccionar color de cursor de ventanilla
* [Vista 2D] Velocidad de fotogramas/rendimiento muy baja
* [Export] Bloqueo al abrir la ventana de exportación con ajustes preestablecidos de exportación demasiado recientes.
* [Exportar] El canal de Height al mapa normal se convierte en el espacio incorrecto
* [Mac] El color base de los efectos de Substance se muestra como lineal
* [Mac] El widget de líneas rectas se dibuja incorrectamente en Retina
* Las líneas rectas pueden permanecer activadas incluso con el método abreviado suelto.
* Las líneas rectas del guizmo desaparecen después de rotar el mapa de entorno
* Las salidas de oclusión ambiental de substancias no se conectan automáticamente al canal AO
* Solucionar el problema de copia de licencia en Windows con un carácter especial en el nombre de usuario

### 1.4.0

*(Lanzado: 10 de junio de 2015)*

**Agregado:**

* [Exportar] Añada asignaciones adicionales en la lista de los mapas de entrada disponibles
* [Estante] Usar materiales sbsar como ajustes preestablecidos de materiales
* [Estante] Permitir el uso de rutas de biblioteca personalizadas
* [Estante] Cambiar el tamaño mínimo
* [Estante] Nuevo contenido : 20 nuevos materiales inteligentes
* [Estante] Nuevo contenido : nueva sustancia de procedimiento (tejido, malla)
* [Shelf] Filtro de desenfoque actualizado
* Dibujo de líneas rectas mediante una tecla modificadora
* Adición de un canal de Oclusión ambiental y modificación del comportamiento AO/Normal en la pila de capas
* Leer el color predeterminado de la entrada de imagen definida en los datos de usuario del Substance
* Permitir la exportación del registro desde el menú de ayuda

**Corregido:**

* [Baker] [Mac] Bloqueo con Normal desde el panadero de mallas
* [Baker] Bloqueo si no hay UV en el archivo de jaula
* [Baker] La coincidencia por nombres no funciona con los OBJ exportados desde zBrush
* [Baker] El horneado con una jaula sobrescribe el horneado si se usan varios conjuntos de texturas y UV superpuestos
* [Baker] Los archivos OBJ específicos producen texturas negras
* [Shelf] No se pueden leer recursos si se establece como de solo lectura
* [Estante] Los archivos de recursos se escriben en Painter si se han utilizado en el proyecto.
* [Estante] Las sustancias de recarga también actualizan la capa
* [Export] Tiff exporta imágenes de 32 bits que Photoshop o los motores de juegos no pueden leer correctamente
* [Exportar] El ajuste preestablecido de canales predeterminados siempre se exporta como RGB
* [Material] La asignación de color base a los canales de Difuso anula la asignación de materiales
* [Vista 3D] Iluminación incorrecta con mapas de entorno específicos
* [Herramienta] No se puede rotar un pincel a un ángulo específico
* La ventana gráfica se enfoca al pasar el cursor por encima mientras se escribe en un campo de texto
* Bloqueo con ajustes preestablecidos demasiado recientes para la versión actual del estante
* Bloqueo después de reemplazar la malla
* Bloqueo al volver a cargar una sustancia con un número diferente de entradas
* FBX mallas de la importación de Cinema4D con nombres de material incorrectos

### 1.3.5

*(Lanzado: 29 de mayo de 2015)*

**Agregado:**

* [Licencia] Problema de activación cuando ya hay un archivo de licencia
* [Mac] Bloqueo al cargar archivos FBX específicos
* [Mac][Vista 3D] Reflejo incorrecto para la GPU integrada
* [Vista 3D] La fuente de la Máscara rápida está rota
* [Vista 3D] El selector de materiales hace que la ventana gráfica sea totalmente negra
* Bloqueo después de abrir proyectos creados en 1.3.3
* La previsualización de material está vacía al utilizar sombreadores con alfa
* La pintura deja de funcionar en mallas específicas
* Las prestaciones disminuyen mucho con mallas OBJ específicas
* Los canales de usuario no se asignan al utilizar efectos
* Las carpetas temporales no se limpian al inicio

**Corregido:**

* Mejoras de tiempo de cálculo en el proyecto extremadamente largo de carga
* Cambie la ventana &quot;Solución de problemas de GPU&quot; para que sea más comprensible
* [Capas] Guarde el estado del bloqueo de proporción para las capas de relleno y active esta opción de forma predeterminada
* [Bakers] La coincidencia por nombre ahora usa el sufijo como separador

### 1.3.4

*(Lanzado: 27 de abril de 2015)*

**Agregado:**

* [Mac] Bloqueo con Mac OS X Yosemite (10.10)
* [Mac] No es posible salir del modo de pantalla completa
* [Panaderos] La opción Coincidencia de horneado por nombre no funciona
* [Panaderos] El espacio tangente de la tinta utilizado en SP no funciona con UE4
* [Panaderos] El panadero de ID no puede hornear colores de ID de material
* [Vista 2D] La Malla metálica no aparece al utilizar la herramienta Calcomanía geométrica
* [Herramienta] El canal alfa del pincel se muestra como verificador en lugar de como transparencia con los materiales
* [Herramienta] Bloqueo con la pegatina geométrica
* [Capas] La ranura de material se contrae de forma predeterminada en la capa de relleno
* [Export] Bloqueo al exportar a un tamaño superior a la resolución del conjunto de texturas
* El canal de specular no se reconoce en los filtros.
* Limpiar y guardar no quita correctamente los recursos del archivo spp
* No almacenar la transformación de bajo contenido de poli en el archivo de asignación de alto contenido de poli
* El archivo FBX se importa con demasiados conjuntos de texturas

**Corregido:**

* Efectos: La abrazadera de niveles debe estar activada de forma predeterminada para imitar los niveles &quot;clásicos&quot;
* Capas: Cambio del nivel mínimo y máximo en la acción Rellenar
* Capas: Guardar y restaurar el estado de la pila
* Panaderos: AO Baker tener en cuenta el mapa normal si no se especifica ningún HP
* Panaderos: Se ha añadido información sobre herramientas e información adicional en la ventana de panadería
* Crear un archivo de copia de seguridad al guardar un proyecto

### 1.3.3

*(Lanzado: 01 de abril de 2015)*

**Agregado:**

* Añadir la versión de software y el nombre del proyecto en la barra de título
* Corregir nombres de conjuntos de texturas y nombres de materiales inteligentes
* Actualizar el motor del Substance a V5
* [Shelf] Añadir nuevos mapas de entorno : Corsica beach, studio 05, Tornoco studio y más
* [Shelf] Actualizar MG Mask Builder con nuevos parámetros
* [Shelf] Actualizar y calibrar mapas de entorno antiguos

**Corregido:**

* Bloqueo al abrir la ventana de exportación
* No es posible arrastrar y soltar en el widget de interfaz de usuario cuando no está acoplado
* &quot;Buscar actualizaciones&quot; no funciona
* [Capas] No seleccionar la máscara al pulsar ALT + clic en ella
* [Herramienta] El triplano no funciona con el canal Normal
* [Vista 3D] La iluminación difusa del mapa env es incorrecta
* [Vista 3D] El cálculo de la exposición es diferente de Designer
* [Vista 3D] Las sombras no deben ser visibles en superficies 100 % metálicas
* [Vista 3D] La malla con UV reflejados ha volteado la tangente/los binomales
* [Vista 3D] Las sombras producen resultados incorrectos en determinadas mallas
* [Bakers] Quitar la carpeta &quot;.alg\_meta&quot; creada por los archivos de asignación
* [Bakers] Bloqueo al realizar el procesamiento si Painter vuelve a calcular un TextureSet al mismo tiempo
* [Mac] Error de IU de White Box al iniciar la aplicación

### 1.3.2

*(Lanzado: 6 de marzo de 2015)*

**Corregido:**

* [Vista 3D] No es posible volver a cargar un mapa de env guardado con el proyecto

### 1.3.1

*(Lanzado: 5 de marzo de 2015)*

**Agregado:**

* [Bakers] Añada una versión en caché de mallas de alto contenido de poli para acelerar el cálculo
* [Bakers] Añada un icono de advertencia si no se carga ninguna malla de alta densidad
* [Bakers] Si no se carga ninguna malla de alta densidad, use la malla del proyecto en su lugar

**Corregido:**

* [Bakers] Al pulsar &quot;Intro&quot; al editar el valor de un regulador se cierra la ventana
* [Panaderos] Si se activa o desactiva un panadero, también se activará el botón
* [Panaderos] Imposible de hornear si usas el botón &quot;all/none&quot;
* [Panaderos] La ordenación de los botones del panadero no está en el orden correcto
* [Panaderos] Se omite la casilla de verificación y todos los panaderos siempre se procesan
* [Panaderos] Progreso de la barra de progreso fijo

### 1.3.0

*(Lanzado: 4 de marzo de 2015)*

**Agregado:**

* [Panaderos] [Vista 3D] Usar cálculo de espacio tangente Mikkt si no se encuentran tangentes/binormales
* [Panaderos] Se han añadido nuevos panaderos : Normal, ID, Oclusión, Curvatura, Thickness, Posición
* [Efectos] La pila de efectos ahora se invierte y se muestra de arriba abajo (como capas)
* [Efectos] Añadir nuevos iconos en la pila de efectos
* [Efectos] Añadir modo de fusión entre acciones de relleno en la pila de efectos
* [Efectos] Cambiar nombre de efectos (efecto de sustancia = filtro, etc.)
* Añadir un archivo &quot;lock&quot; durante el proceso de guardado
* [Effects] Acción Añadir relleno en la pila de efectos
* Se ha añadido un nuevo recurso : Materiales inteligentes
* [Capas] Permite reordenar los efectos de capa
* [Herramienta] Agregar proyección triplana
* [Vista 3D] Añadir compatibilidad con sombras
* [Vista 3D] Posibilidad de establecer los estados necesarios de OpenGL en sombreadores personalizados
* [Vista 3D] Compatibilidad con alfa mediante nuevos sombreadores
* [Vista 3D] Ahora los sombreadores tienen versiones y se guardan por completo en un proyecto
* [Vista 3D] Avisar al usuario si el sombreador ya no se compila

**Corregido:**

* [Capas] Se corrige el soltar debajo de una carpeta contraída
* [Estante] Corrección del filtrado de contenido en miniestantes
* [Shelf] Cambiar el nombre de las categorías y reorganizar las pestañas

### 1.2.1

*(Lanzado: 12 de febrero de 2015)*

**Agregado:**

* Los archivos \*.spp ahora se pueden abrir haciendo doble clic en el explorador
* [Exportar] Nueva etiqueta &quot;$project&quot; para los ajustes preestablecidos de exportación
* [Exportar] Añadir lista de mapas (con nomenclatura) debajo de cada conjunto de texturas
* [Exportar] Añada un botón Todo/Ninguno para seleccionar los conjuntos de texturas
* [Exportar] Los mapas vacíos se descartan durante la exportación

**Corregido:**

* [Exportar] Los ajustes preestablecidos de Unity5 tienen mapas invertidos
* [Exportar] Si se añade una barra diagonal en un nombre de ajuste preestablecido, se creará una carpeta dañada
* El canal de Height [Export] exportado en formatos de 32 bits no está correctamente sujeto
* [Exportar] La lista de conjuntos de texturas no se ordena como en el proyecto
* [Herramienta] El sacrificio de la cara posterior ya no funciona
* Guardar no funciona con caracteres especiales en el trazado

### 1.2.0

*(Lanzado: 28 de enero de 2015)*

**Agregado:**

* Nuevo canal Normal que permite pintar los datos normales del mapa y combinar los resultados
* [Exportar] Nueva ventana de exportación con la capacidad de crear empaquetados personalizados y definir nombres personalizados
* El formato del archivo de proyecto ahora es un único archivo en lugar de carpetas
* [Export] Admite diferentes formatos normales (DirectX, OpenGL)
* [Exportar] Crear un archivo de bloqueo temporal durante la exportación
* [Capas] Mayús + clic izquierdo del ratón se puede utilizar para alternar una máscara
* [Parámetros] Expone el espacio de color en la parte inferior de una entrada de imagen
* [Shelf] Efecto &quot;MG Mask Builder&quot; ahora tiene nuevos ajustes
* [Vista 3D] El mapa de Oclusión ambiental ahora oculta la contribución difusa, no el specular

**Corregido:**

* El material de proyección o la previsualización de la galería de símbolos no se muestran correctamente en la ventana gráfica
* [Vista 3D] La información sobre el método abreviado no se muestra al utilizar el método abreviado &quot;S&quot; (galería de símbolos)
* [Shelf] El efecto &quot;MatFx Skin Scale&quot; tiene ahora mejores prestaciones en baja resolución
* [Exportar] Las texturas de la exportación solo se aumentan al especificar un tamaño de documento más grande

### 1.1.2

*(Lanzado: 15 de enero de 2015)*

**Agregado:**

* Añadido: Nuevos ajustes de Traducir, Rotar y Escalar en la capa de Relleno
* Filtrado mejorado para capas de pinceles y de relleno
* La versión de prueba ya está totalmente disponible (se puede exportar), pero tiene un tiempo limitado.

**Corregido:**

* Imposible importar mallas OBJ con muy pequeñas precisiones
* Problema al activar una licencia en Windows 7 y 8
* Bloqueo durante la operación Guardar como de un proyecto
* Bloqueo al eliminar el último canal de un conjunto de texturas
* Bloqueo al eliminar una capa en un contexto específico

### 1.1.1

*(Lanzado: 25 de diciembre de 2014)*

**Agregado:**

* [Capa] Seleccione la capa superior al abrir un proyecto o cambiar el conjunto de texturas
* Se ha mejorado la velocidad de &quot;Guardar&quot; y &quot;Guardar como&quot; con el nuevo algoritmo de compresión
* Mostrar un error al abrir un proyecto demasiado reciente para Painter

**Corregido:**

* [Herramienta] La pegatina geométrica produce corrupciones de memoria
* [Pincel] No es posible introducir manualmente valores flotantes por debajo de 1 para el tamaño de pincel.
* [Capa] Al crear un efecto de selección de color, no se añade a la pila de capas
* [Capa] Al mover el ratón sobre las capas, Painter se mueve por la barra de tareas
* [Layer] Añadir un mapa de bits como máscara puede producir un bloqueo
* La interfaz gráfica de usuario para el modo solo con el canal de Height es incorrecta
* &quot;Guardar proyecto&quot; puede dar error y dañar un proyecto
* Bloqueo al abrir un proyecto después de cargar otro con un sombreador obsoleto

### 1.1.0

*(Lanzado: 16 de diciembre de 2014)*

**Agregado:**

* [Effect] Nuevo creador de máscaras de ID de material
* Nueva línea punteada blanca/negra para el gizmo del pincel
* Nuevo parámetro de seguimiento de ángulo
* Nuevo parámetro de sacrificio de la cara posterior
* Nuevo parámetro de ratón perezoso
* [Layers] Soporte para múltiples selecciones y administración
* [Capas] Copie y pegue de un conjunto de texturas entre sí
* [Exportar] Formato de PSD de Adobe Photoshop
* [Estante] Nueva herramienta : piel, puntadas metálicas y cremallera
* [Estante] Nuevo pincel : molde, lápiz, línea afilada y puntada
* [Shelf] Nuevo alfa : Ruido gaussiano, línea afilada, molde, pluma, salpicadura, puntada, cremallera
* Se han mejorado las prestaciones de pintura actualizando solo partes de las texturas necesarias

**Corregido:**

* [Estante] Imposible cargar una sustancia con un gráfico que tenga etiquetas idénticas
* El modo de fusión Pasar por [capas] no funciona con máscaras
* [Esténcil] La escala se rompe en la Vista 2D
* Problemas y bloqueo en el sistema operativo Mac Yosemite

### 1.0.2

*(Lanzado: 09 de noviembre de 2014)*

**Agregado:**

* Rendimiento mejorado en la previsualización de materiales con sustancias
* Se han mejorado las prestaciones con la vista previa del trazo de pincel al actualizar el documento
* Rendimiento mejorado en la ventana gráfica con una velocidad de actualización más baja para el área no operativa
* [Efectos de posprocesamiento] Se ha mejorado la interfaz de usuario para administrar la configuración
* [Efectos de posprocesamiento] Restablecer los valores predeterminados
* Operaciones de capas y efectos de Substance en el menú contextual
* Apoyo a los insumos/productos premultiplicados en sustancias

**Corregido:**

* [Vista 3D] Los parámetros de sombreador personalizados están separados por un espacio grande
* [Exportar] Falta la conversión sRGB para el ajuste preestablecido Unity4
* Posible Bloqueo al cargar mallas fbx
* Bloqueo a veces al cargar mallas obj simples
* La barra de cálculo permanece bloqueada al 100% al cargarse
* Volver a cargar una sustancia la coloca en todas las categorías
* Interruptor DirectX/OpenGL roto

### 1.0.1

*(Lanzado: 27 de octubre de 2014)*

**Agregado:**

* [Herramienta] Uso mejorado de parámetros de material
* Nuevo método abreviado para el sitio web uservoice en el menú Ayuda
* Varias mejoras de rendimiento en el motor

**Corregido:**

* Los valores de los parámetros están limitados a 2 decimales para Partículas
* El Substance cargado desde la caché no se muestra en la interfaz de usuario como obsoleto
* Bloqueo al cargar una malla desde una URL de red
* Painter ahora se reconoce como firmado en Mac OS X

### 1.0.0

*(Lanzado: 15 de octubre de 2014)*

**Agregado:**

* Compatibilidad con Sombreador personalizado
* Compatibilidad con resolución 4k
* Proyectos de caracteres de muestra
* Mostrar barra de progreso para tiempos de cálculo largos
* [Exportar] Añadir una pasada de dilatación antes del posproceso de difusión
* Argumentos de la línea de comandos en SP para operaciones simples
* Nuevos materiales y efectos
* Previsualización de herramientas (área separada de previsualización de materiales en tiempo real y prueba de trazos)
* No crear un documento predeterminado al iniciar Painter
* [Herramienta] Permite editar manualmente un valor de escala de grises
* Varias mejoras para los patrones (Ajustar, Restablecer)
* Las partículas son ahora subherramientas de las herramientas Pincel, Borrador y Proyección
* [Vista 3D] Usar AO hecho un bake en el renderizado de la ventana gráfica
* División de los controles de galerías de símbolos entre la vista 2D y 3D
* Ajuste de tamaño de pulgar pequeño en la biblioteca
* Los campos de búsqueda son específicos de cada ventana
* Ajuste de IU

**Corregido:**

* El conmutador [Substance] no funciona
* [Cuadro de diálogo Color] Degradado de tono no actualizado
* No es posible actualizar una malla si el nombre del archivo es idéntico
* La herramienta no está visible en las vistas cuando es demasiado pequeña
* La herramienta de pegatina de la pantalla Retina no funciona correctamente
* [Substance] Int1 se muestra como float1
* No se reconocen las entradas/salidas de [Substance] basecolor
* [Substance] los filtros no se pueden volver a cargar
* [Herramienta] El widget de escala de grises siempre está contraído

## Beta

### 0.12.1-beta

*(Lanzado: 18 de septiembre de 2014)*

**Agregado:**

* Ajuste preestablecido de exportación de Unity 5

**Corregido:**

* SOMBREADOR PBR, la calidad de representación debería mejorar mucho
* La función de enfoque está rota y las mallas se recortan de forma predeterminada

### 0.12.0-beta

*(Lanzado: 17 de septiembre de 2014)*

**Agregado:**

* Herramienta Cuentagotas
* Se ha añadido la opción &quot;Conservar posición de trazo&quot; a la reimportación de malla para cuando cambie el cuadro delimitador.
* Mapa de normales para la malla predeterminada de Cymourai
* Mejorar la interfaz de la vista de herramientas (los colores son nítidos)
* Mueva el menú &quot;Ayuda->Configuración&quot; a &quot;Editar->Configuración&quot;
* Guarde la ruta de exportación en la ventana &quot;Exportar todos los canales&quot;
* Nuevos niveles GUI con visualización de histograma
* Mejor gestión de activos (arrastrar y soltar, volver a cargar recursos, eliminar recursos no utilizados)
* Cambiar de &quot;difuso&quot; a &quot;color base&quot;
* Ajustes de edición de los reguladores: permitir puntos además de comas
* Capa de relleno: aumentar el valor máximo de segmentación
* Mapa de entorno predeterminado

**Corregido:**

* Artefactos de mal reflejo en ángulos extremos
* Exportación de speculares rotos/brillo
* Los vínculos de la ventana &quot;Acerca de&quot; de Painter no funcionan
* Bloqueo con OSX Yosemite
* Las mallas se guardan trianguladas
* El método abreviado de color de la ventana Herramienta se envía al emisor en lugar de a la escala de grises
* El selector de color permanece abierto al cambiar de capa a máscara
* No se puede guardar material de una capa de relleno
* Permitir el cambio de tamaño de las tres regiones del estante

### 0.11.0-beta

*(Lanzado: 4 de septiembre de 2014)*

**Agregado:**

* Agregar un divisor entre las vistas 3D y 2D
* Uso de un fondo degradado en las vistas 2D/3D
* Interfaz para el histograma de niveles
* Combinar estante y biblioteca
* No es necesario guardar nada al crear o actualizar un ajuste preestablecido
* Importar activos en el estante mediante arrastrar y soltar

**Corregido:**

* El nombre de los botones se muestra encima en la barra de herramientas principal

### 0.10.2-beta

*(Lanzado: 28 de agosto de 2014)*

**Corregido:**

* La exportación de todos los canales produce resultados incorrectos

### 0.10.1-beta

*(Lanzado: 26 de agosto de 2014)*

**Corregido:**

* Sombreador dar resultado negro con baja rugosidad
* Comprobación de GPU: manejar tarjetas &#39;Quadro&#39;, detectar todos los dispositivos y adaptar el mensaje de usuario en consecuencia
* La mayoría de los materiales de Substance tienen un límite de 256 en Beta 9
* El height se sujeta al exportar como mapa de bits
* La previsualización del pincel es diferente de la superposición de la proyección en Mac
* El uso de la herramienta Geometría para crear máscaras no se muestra en las ventanas gráficas
* La máscara rápida está rota
* Solucionar problema de fusión en el antiguo mac pro

### 0.10.0-beta

*(Lanzado: 07 de agosto de 2014)*

**Agregado:**

* Máscaras de galería de símbolos

**Corregido:**

* Compatibilidad con tarjetas Quadro
* Sombreador dar resultado negro con baja rugosidad
* Los materiales de Substance tienen un límite de 256
* La exportación de mapas de normales elimina el canal verde

### 0.9.0-beta

*(Lanzado: 17 de julio de 2014)*

**Agregado:**

* Procesamiento posterior de Yebis 2
* El asistente de nuevo proyecto le permite importar mapas de entrada (AO, curvatura, etc.)
* Conectar automáticamente mapas de entrada (AO, curvatura, etc.) a Efectos de Substance
* Control de escala sobre materiales aplicado a capas de relleno

### 0.8.2-beta

*(Lanzado: 11 de julio de 2014)*

**Corregido:**

* El regulador Tono se establece de forma predeterminada en Blanco
* Restablecimiento del proyecto si el nombre de material contiene caracteres especiales
* El cambio de nombre de material en un solo objeto de material no debe invalidar el proyecto.
* Las UV se estropean después de guardar el proyecto y volver a abrirlo

### 0.8.1-beta

*(Lanzado: 4 de julio de 2014)*

**Corregido:**

* Varios bloqueos de GPU
* Bloqueo al exportar canales

### 0.8.0-beta

*(Lanzado: 28 de junio de 2014)*

**Agregado:**

* Multimaterial : ahora puede realizar la pintura en varios materiales en el mismo documento
* Simetría
* Ya están disponibles todos los modos de fusión

**Corregido:**

* Varios bloqueos de GPU
* Restablecimiento del proyecto si el nombre de material contiene caracteres especiales
* Las UV se estropean después de guardar el proyecto y se vuelven a abrir con varias UV

### 0.7.0-beta

*(Lanzado: 18 de junio de 2014)*

**Agregado:**

* Efectos de capa
* Nuevos materiales de Substance Stencil
* Borrar máscara
* Permitir copiar/pegar capa/máscara
* Permitir duplicar capa
* Herramienta Cambiar al editar máscara de capa
* Los Substance ahora funcionan con GPU

**Corregido:**

* El dibujo de mapas de height no pinta valores negativos.
* La visualización del Selector de material no debe tener en cuenta el mapa normal muestreado
* Determinismo de partículas roto
* Matriz de galería de símbolos en vista 2D
* Nombres en archivos obj
* Varios bloqueos

### 0.6.0-beta

*(Lanzado: 04 de junio de 2014)*

**Agregado:**

* Nueva opción de exportación para exportar un mapa de Speculares desde una composición de canales de rugosidad y metálicos

**Corregido:**

* Compatibilidad con Windows Vista
* El mapa de height no pinta valores negativos

### 0.5.0-beta

*(Lanzado: 7 de mayo de 2014)*

**Agregado:**

* Conmutadores de vista 3D/2D
* Herramienta Selección de fragmentos UV
* La herramienta cambia automáticamente al pintar sobre máscaras.
* La resolución de los Substance depende de la

**Corregido:**

* Bloqueo al iniciarse
* Bloqueo con mallas ASCII
* Matriz de galería de símbolos fija en vista 2D
* Bloqueo con Borrador

### 0.4.0-beta

*(Lanzado: 17 de abril de 2014)*

**Agregado:**

* Vista 2D sin problemas
* Máscaras de capa de mapa de bits
* Control de exposición ambiental
* Las capas de relleno ahora utilizan las ventanas Herramientas para establecer sus propiedades
* Los materiales se pueden aplicar a las capas de relleno
* Se han añadido más galerías de símbolos en la biblioteca de galerías de símbolos
* Ajustes preestablecidos de partículas actualizados para un cálculo más rápido
* Optimización del sombreador de PBR y mejora de la calidad para ajustes de menor calidad

**Corregido:**

* Las miniaturas de capas están vinculadas al canal seleccionado actualmente
* Muchos bloqueos

### 0.3.0-beta

*(Lanzado: 4 de abril de 2014)*

**Agregado:**

* Permitir valores negativos en el selector de color para la pintura de mapas de altura
* Mostrar previsualización del material/color seleccionado
* Añadir accesos directos a las herramientas de la barra de herramientas (1,2,3,4)
* Cambiar el formato Normal (OpenGL frente a DirectX) globalmente en un proyecto
* Asistente para nuevo proyecto
* El regulador de espaciado ya no está sujeto
* Estilo de controles deslizantes actualizado
* Convertir el selector de color en no modal
* Al seleccionar un material en la biblioteca, se establece el tipo de herramienta en consecuencia

**Corregido:**

* Corregido: El trazado de malla de importación no se conserva
* Corregido: Generación de texturas incorrecta
* Corregido: Bloqueo al inicio

### 0.2.0-beta

*(Lanzado: 17 de marzo de 2014)*

**Agregado:**

* Cuentagotas de material (P método abreviado)
* Miniaturas bajo la vista previa de la herramienta 3d
* Sistema de licencias para versiones independientes
* [ y ] métodos abreviados de teclado para Tamaño de pincel
* Relleno en mapas exportados
* Estilo de ventana de herramientas actualizado
* Estilo de controles deslizantes actualizado
* Updated Default HDR. environment

**Corregido:**

* Esténcil: cambiar el valor de flujo en las paradas de Vista 3D en 52
* El bucle infinito en el motor al añadir teclas de presión 0 al trazo es fijo
* Herramienta: la variación de ángulo no devuelve valores por encima de +/- 90%
* Cambio en la visualización de la Vista 3D cuando se selecciona una máscara de capa
* Zoom invertido

### 0.1.0-beta

*(Lanzado: 2 de marzo de 2014)*

**Agregado:**

* Nueva administración de bibliotecas
* Nuevo contenido de pinceles y partículas
* Vista previa del pincel 3D
* Estilo de ventana de herramientas actualizado
* Estilo de controles deslizantes actualizado
* Rendimiento de caché actualizado

**Corregido:**

* Controles de cámara
* Rotación de pincel
