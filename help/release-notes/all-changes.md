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

&#x200B;* Actualizar el motor de Substance a la versión 9.4.6

**Corregido:**

&#x200B;* El selector [Escala de grises] permanece abierto después de cambiar la herramienta
&#x200B;* [Procesamiento de sesgo]: se producen saltos de corrección de sesgo al pintar y deshacer
&#x200B;* La herramienta de proyección [Projection Tool] bloquea la interacción de la ventana gráfica
&#x200B;* [Trazo dinámico]: faltan parámetros de trazo dinámico en las propiedades del pincel
&#x200B;* La exportación a una red ya no funciona

### 12.1.2

Fecha de publicación: **2026/08/03**

Resumen: **Versión secundaria**

**Corregido:**

&#x200B;* \[Bloqueo\] Algunos Substance pueden producir un bloqueo al procesarse
&#x200B;* \[Bloqueo\] Volver a importar la malla en el modo de procesamiento
&#x200B;* \[Bloqueo\] Si no se inicializa la visualización de gráficos, se puede producir un bloqueo
&#x200B;* \[Bloqueo\] La exportación de texturas puede producir bloqueos en algunos casos al actualizar el registro
&#x200B;* \[Bloqueo\] Bloqueo en modo de hace un bake en algunos casos al cargar o actualizar el mapa de entorno
&#x200B;* \[Hacer un bake\] Si se vuelve a iniciar hacer un bake después de modificar el archivo de alta poly, se puede producir un bloqueo
&#x200B;* \[Enviar a Photoshop\] No se puede exportar la máscara de capa
&#x200B;* \[Motor\] El resultado del punto de ancla no se procesa entre una máscara y un canal de color

### 12.1.1

Fecha de publicación: <b>2026/07/09</b>

Resumen: Versión secundaria

Añadido:

&#x200B;* [Sesgar Haciendo un bake] Exponer el modo normal de base de sesgo: malla o por triángulo
&#x200B;* [Propiedades] Hacer que los colores uniformes siempre se restablezcan al valor predeterminado de su canal
&#x200B;* [OpenPBR] reagrupa los canales por categorías en la ventana Exportar Texturas para crear plantillas de salida
&#x200B;* Actualizar el motor de Substance a la versión 9.4.5

Corregido:

&#x200B;* [Proyecto] Abrir y guardar algunos proyectos puede tardar más de lo habitual
&#x200B;* [Bloqueo] La recarga de varias mallas puede provocar un bloqueo
&#x200B;* [Bloqueo] Si se elimina un canal mientras se está en el modo de vista de máscara, se produce un bloqueo
&#x200B;* [Bloqueo] Algunos Substance pueden provocar un bloqueo cuando se procesan
&#x200B;* [Sesgo de Pintura] La herramienta seleccionada en el sesgo de pintura permanece seleccionada después de cambiar al modo de pintura
&#x200B;* [Haciendo un bake configuración común] La configuración de la distancia de la jaula no actualiza la visualización de la malla metálica de la jaula y del sombreador
&#x200B;* El modo &quot;Vecino del espacio 3D&quot; del relleno UV [Engine] no funciona bien en triángulos finos
&#x200B;* El resultado del punto de anclaje [Engine] no se procesa entre una máscara y un canal de color

### 12.1.0

Fecha de publicación: <b>2026/06/23</b>

Resumen: <b>Esta actualización es una versión importante, contiene mejoras de bakeres con el nuevo estado de IU predeterminado de hace un bake, mapa de sesgo de pintura, reprocesamiento automático, nueva opción para el desajuste UV automático para mallas de superficie dura y OpenPBRs. Para obtener más detalles, vea las notas de la versión completas.</b>

<b>Agregado</b>:

&#x200B;* [Skew baking] Herramientas de pintura de sesgo
&#x200B;* [Skew Baking] Añada sombreador de previsualización de sesgo y elementos visuales de dirección de sesgo al pintar el mapa de sesgo
&#x200B;* [Skew Baking] Añadir protección de bordes, opción
&#x200B;* [Sesgar la cocción] Auto rehacer
&#x200B;* [Skew Baking] Interfaz de usuario de lista de mapas de malla de reprocesamiento
&#x200B;* [Sesgar horneado] Dividir mapa de malla / Configuración común de horneado + Mover ajustes comunes de la lista de mapas de malla solo en color o máscara
&#x200B;* [Sesgar horneado] Cambiar botones de la barra de herramientas de la ventana gráfica
&#x200B;* [Sesgar horneado] Mostrar alternancia de simetría para el pincel en la barra de herramientas superior
&#x200B;* [Skew Baking] Cambiar nombre de opciones en el menú de sincronización de lista de mapa de malla
&#x200B;* [Skew Baking] Cuadro de diálogo Actualizar sincronización y estado marcado
&#x200B;* [Sesgar horneado] Crear variante del selector de color de escala de grises
&#x200B;* [Sesgar horneado] Icono Actualizar modo de horneado
&#x200B;* [Auto Unwrap] opción Integrar superficie dura
&#x200B;* [OpenPBR] Añadir apoyo para el OpenPBR 1.1
&#x200B;* [OpenPBR] Hacer que OpenPBR sea el flujo de trabajo y el sombreado predeterminados
&#x200B;* [OpenPBR] Importar materiales y texturas de OpenPBR a través de USD
&#x200B;* [OpenPBR] Exportar materiales y texturas de OpenPBR a través de USD
&#x200B;* [OpenPBR] Actualice la ventana Exportar texturas para mostrar la convención de nomenclatura del OpenPBR
&#x200B;* [OpenPBR] Añadir documentación sobre los cambios en el OpenPBR de asistencia
&#x200B;* [OpenPBR] [Israel] Añádase un nuevo MDL para prestar apoyo al OpenPBR 1.1 de Israel
&#x200B;* Varias mejoras menores de las exportaciones en dólares
&#x200B;* [UI] Añada una advertencia en la ventana gráfica al intentar pintar en otro conjunto de texturas
&#x200B;* [Aplanar] Permite acoplar todas las capas con instancias en los conjuntos de texturas
&#x200B;* [Ajustes del conjunto de texturas] Permite seleccionar varios canales a la vez mediante una nueva ventana
&#x200B;* [Historial] Actualizar &quot;valor&quot; Deshacer texto de entrada para reflejar el nombre del parámetro
&#x200B;* [Pila de capas] Los efectos de relleno de las máscaras se establecen de forma predeterminada en blanco (1.0)
&#x200B;* [Substance] Añadir nueva entrada de mapa del motor &quot;mesh_hard_edges_triangle&quot;
&#x200B;* [Substance] Añadir nueva entrada de mapa del motor &quot;mesh_hard_edges&quot;
&#x200B;* [Sombreador] Evitar que las instancias del sombreador compartan los mismos nombres
&#x200B;* [Sombreador] Utilice el sombreador de la plantilla de proyecto al importar un archivo USD o GLTF
&#x200B;* Actualizar Adobe Color Engine a la versión 7.0
&#x200B;* Actualizar la versión mínima de MacOSX a 13.0 (Ventura)
&#x200B;* [Contenido] Nuevas plantillas de proyecto para el OpenPBR
&#x200B;* [Contenido] Actualizar proyectos de muestra para utilizar el nuevo sombreador de OpenPBR
&#x200B;* [Python] Amplía la API de máscara de geometría para permitir modos de inclusión y exclusión como en la interfaz de usuario

<b>Corregido</b>:

&#x200B;* [Bloqueo] [Ajustes de Mapas de Malla] Aplicación de ajustes a otros conjuntos de texturas
&#x200B;* [Bloqueo] Al hacer un bake la curvatura del mapa sin espacio mundial normal
&#x200B;* [Bloqueo]&#x200B;[Hacer un bake] Hacer un bake con la jaula personalizada activada, pero sin bloqueos de archivo seleccionados
&#x200B;* [Bloqueo] Cancelación de hace un bake de AO
&#x200B;* [Auto-Cage] Carga infinita cuando la ruta del archivo de poli alto no es válida
&#x200B;* [Linux] [Windows] En ocasiones, el selector de color puede ser completamente negro o no aparecer
&#x200B;* [Herramienta Relleno poligonal] La herramienta no funciona con PBR
&#x200B;* &lbrack;[Pintura] Al eliminar el canal de color base no se elimina el color pintado anteriormente
&#x200B;* [USD] No se detectan correctamente todas las Instancias del sombreador
&#x200B;* [Substance] Solo se tiene en cuenta el primer uso de un nodo de entrada/salida
&#x200B;* [Sombreador] La Oclusión ambiental se aplica dos veces con los conjuntos de texturas usando diferentes métodos de mezcla
&#x200B;* [Motor] Las texturas normales con un canal azul vacío (negro) pueden producir resultados de mezclas incorrectos
&#x200B;* [Importación GLTF] La fusión alfa está activada en todos los conjuntos de texturas
&#x200B;* [GLTF Export] La fusión de Alpha siempre está activada al exportar
&#x200B;* [Exportar] La geometría de doble cara siempre está desactivada al importar un archivo GLTF
&#x200B;* [Javascript] La modificación de la configuración de los sombreadores no contribuye al historial de deshacer
&#x200B;* [Muestras] La dispersión subsuperficial no está activada en Configuración de visualización para Meet Mat

### 12.0.3

Fecha de publicación: **2026/05/05**

Resumen: **Versión secundaria**

**Agregado:**

&#x200B;* Actualice Bakers a la versión 3.2.2.
&#x200B;* Actualizar el motor de Substance a la versión 9.4.3
&#x200B;* \[Python\] Guardar un material inteligente en una ubicación específica

**Corregido:**

&#x200B;* \[Ubuntu\] Bloqueo al seleccionar material
&#x200B;* \[Mac\] Aparece una ventana emergente periódica para solicitar acceso a los datos de otras aplicaciones
&#x200B;* \[Horneado\] Pueden aparecer defectos en el mapa de curvatura
&#x200B;* \[Horneado\] El horneado es más lento en algunos casos
&#x200B;* \[Deformar en geometría\] En algunos casos, la opción Deformar en geometría se desactiva
&#x200B;* \[Mosaico UV\] El punto de anclaje extraído alfa omitido por otros mosaicos
&#x200B;* \[Python\]\[Mac\] Excepciones en la consola de Python con SSL
&#x200B;* \[Python\] Bloqueo de Painter al salir con widgets Qt sobrantes

### 12.0.2

Fecha de publicación: **2026/04/07**

Resumen: **Versión secundaria**

**Agregado:**

&#x200B;* [Gestión de color] Añadir nuevo OCIO para especificar el espacio de color predeterminado del selector de color
&#x200B;* [Python] Exponer la configuración de desajuste automático en la API de Python

**Corregido:**

&#x200B;* [Bloqueo] Si no hay suficiente espacio en disco, los proyectos se pueden bloquear o dañar
&#x200B;* [Bloqueo] [Cinta] El uso de la cinta puede producir bloqueos en algunos proyectos
&#x200B;* [Crash] [Baking] se bloquea cuando el archivo .assbin no se puede escribir en la carpeta
&#x200B;* [Importar] Las mallas OBJ de Stager pueden fallar en la creación del proyecto
&#x200B;* [Importar] A OBJ le falta cara en algunos casos
&#x200B;* [Importar] La malla USD sin material asignado puede bloquearse al importar
&#x200B;* [Ruta rellena] No se ve afectada por la simetría
&#x200B;* [Stencil] La previsualización tiene una resolución inferior a la del resultado pintado
&#x200B;* [UI] &#39;UV island&#39; sigue apareciendo en la información sobre herramientas de origen de color del mapa de ID
&#x200B;* [Display] Las sombras aparecen invertidas
&#x200B;* [Ventana gráfica] La transformación de proyección de deformación permanece después de cambiar al modo de deformación
&#x200B;* [Deformar] La cuadrícula desaparece cuando la escala se establece en 0 en el eje Z con la opción Deformar en geometría activada
&#x200B;* [Python] Error inesperado al agregar un canal con modificación de ámbito

### 12.0.1

Fecha de publicación: **2026/03/18**

Resumen: **Versión secundaria**

**Corregido:**

&#x200B;* \[Crash\]\[Freeze\] Exportar desde proyectos específicos

### 12.0.0

Fecha de publicación: <b>2026/03/09</b>
Resumen: <b>Esta es una versión importante. Esta versión contiene las funciones de acoplar capas, deformar en geometría, nuevos efectos posteriores, mejoras en la nueva ventana de proyecto y otras mejoras.</b>

<b>Agregado</b>:

&#x200B;* [Acoplar capas] Acoplar capas dentro de la pila de capas
&#x200B;* [Acoplar capas] Exportar capas acopladas a un disco
&#x200B;* [Deformar en geometría] Añadir nueva función de deformación automática a las proyecciones de deformación
&#x200B;* [Efectos posteriores] Reemplace los efectos posteriores por la adición de otros nuevos
&#x200B;* [Post-effects] Actualizar el asignador de tonos
&#x200B;* [Post-effects] Añadir nuevo uso para recursos Post-effects
&#x200B;* [Contenido]&#x200B;[Efectos posteriores] Integrar activos de efectos posteriores predeterminados en la biblioteca
&#x200B;* [Nuevo proyecto] Mejora de la interfaz de usuario para la creación de proyectos
&#x200B;* [Nuevo proyecto] Cambios en la función de reimportación de mallas
&#x200B;* [Nuevo proyecto] Permitir la apertura de archivos \*.geo.usd
&#x200B;* [Configuración del proyecto] Mejorar la interfaz de usuario para la configuración del proyecto
&#x200B;* Actualizar USD biblioteca a la versión 25.05
&#x200B;* Actualizar Substance Engine a la versión 9.3.4
&#x200B;* Aumentar controladores mínimos a 25.3.1/25.Q2 para las GPU AMD
&#x200B;* Actualizar Qt a 6.8.6
&#x200B;* [Scripting] Actualice la API de JavaScript a la versión 1.1.20
&#x200B;* Actualizar Python a 3.13

<b>Corregido:</b>

&#x200B;* [Bloqueo] El cambio de una salida de canal de material en una máscara puede generar un bloqueo
&#x200B;* [Import] Las texturas de EXR se fuerzan en sRGB en lugar de lineales al importar archivos USD
&#x200B;* [Mosaicos de UV] La secuencia de imágenes con una sola imagen también llena otros Mosaicos de UV
&#x200B;* [Hacer un bake] El AO es diferente entre la CPU y la GPU al hacer un bake
&#x200B;* [Gestión de color] [MacOS] Viewport BaseColor no coincide con el selector de color
&#x200B;* [USD] En algunos casos no se importan valores uniformes

## Versión 11

### 11.1.3

Fecha de publicación: <b>2026/02/12</b>
Resumen: <b>Versión secundaria</b>

<b>Corregido</b>:

&#x200B;* [Pintura] En algunos casos, el patrón y la simetría no funcionan
&#x200B;* [Ruta] No hay actualización al cambiar el regulador de opacidad del trazo de difuminado
&#x200B;* [Proyecto] No se puede realizar la pintura en alguna geometría
&#x200B;* [Cinta de opciones] La ruta instanciada desaparece al cambiar la resolución del conjunto de texturas
&#x200B;* [UI] El selector de color puede reducirse y desaparecer en algunos casos

### 11.1.2

Fecha de publicación: <b>2026/01/13</b>
Resumen: <b>Versión secundaria</b>

<b>Agregado</b>:

&#x200B;* [Hacer un bake] Mejorar el tiempo de hace un bake para el proyecto de Mosaicos de UV con el ahorro asíncrono
&#x200B;* [Shaders] Mención en cambios de registro de cambios tras la migración de Vulkan
&#x200B;* Actualizar OpenEXR a la versión 3.4.4

<b>Corregido</b>:

&#x200B;* [Bloqueo] Bloqueo durante el inicio en la serie Nvidia GTX 10xx
&#x200B;* [Bloqueo] El uso del selector de color en diferentes conjuntos de texturas puede provocar un bloqueo al salir de la aplicación
&#x200B;* [Rendimiento] Problema de rendimiento al pintar en un proyecto con muchas capas
&#x200B;* [Rendimiento] Retraso al pintar con el lápiz de Tablet PC gráfico
&#x200B;* [UI] Los ajustes de la cámara permanecen desactivados en el modo de procesamiento (Iray)
&#x200B;* [Cinta] En algunos casos, la ruta puede superponerse inesperadamente después de una esquina
&#x200B;* [Cinta] Problema de rendimiento con Mosaicos de UV
&#x200B;* [Substance]&#x200B;[UI] Las entradas de imagen desaparecen al contraerse
&#x200B;* [Substance] [IU] Los grupos anidados pueden permanecer aunque se muestren si los oculta
&#x200B;* [Haciendo un bake]&#x200B;[UI] No se puede establecer el radio de muestreo de curvatura más allá de 0,01
&#x200B;* [Haciendo un bake]&#x200B;[UI] No se puede establecer la distancia máxima del oclusor más allá de 1
&#x200B;* [Haciendo un bake] El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y hace un bake baja como alta
&#x200B;* [Haciendo un bake] El mapa de ID no hace un bake los colores de vértice de FBX en modo Bajo como Alto
&#x200B;* [Contenido] El filtro Paso alto genera colores atenuados en canales con gestión de color

### 11.1.1

Fecha de publicación: <b>2025/12/09</b>
Resumen: <b>Versión secundaria</b>

<b>Agregado</b>:

&#x200B;* [Rendimiento] Mejora del rendimiento de los Mosaicos de UV al calcular texturas parciales
&#x200B;* [Baker] Actualización a la versión 3.15.4

<b>Corregido</b>:

&#x200B;* [Bloqueo] [MacOS] Guardar siempre el bloqueo del proyecto de la versión anterior
&#x200B;* [Bloqueo] Cerrar un proyecto a veces puede provocar un bloqueo
&#x200B;* [Proyecto] Error &quot;los miembros no coinciden en el recuento&quot; al abrir el proyecto realizado en la versión anterior
&#x200B;* [Haciendo un bake] Los Mosaicos de UV no se combinan con los resultados hechos un bake anteriores, si los hay
&#x200B;* [Haciendo un bake] El dispositivo se pierde incluso con el trazado de rayos desactivado en la serie Nvidia GTX 10XX
&#x200B;* [Haciendo un bake] El AO con normal tiene defectos en los bordes porque no hay relleno
&#x200B;* [Haciendo un bake] El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y &quot;coincidencia por nombre&quot; en
&#x200B;* [Haciendo un bake] El mapa de ID es completamente negro si a alguna malla de alta densidad le faltan colores de vértice
&#x200B;* [Cinta] La información sobre herramientas del modo de fusión Alfa menciona el modo de fusión de pantalla en lugar de Sobreexposición lineal
&#x200B;* [Path] Las tangentes crean bucles inesperados cuando el punto se acerca a los extremos del trazado
&#x200B;* [Herramienta] La previsualización de material no funciona cuando se utiliza la proyección en una máscara
&#x200B;* [Motor] Pintar trazos pequeños puede dar como resultado artefactos de bloque
&#x200B;* [Sombreador] Al deshacer la creación de la instancia del sombreador, no se elimina correctamente
&#x200B;* El modo de Alpha [Export] para la exportación GLTF siempre está establecido en MASK
&#x200B;* [Python] Error inesperado al editar la pila de capas fuera del bloque de modificación de ámbito

<b>Problemas conocidos</b>:

&#x200B;* [Cinta] Problema de rendimiento con Mosaicos de UV
&#x200B;* [Cinta] En algunos casos, la ruta puede superponerse inesperadamente después de una esquina
&#x200B;* [Bloqueo] [Cinta de opciones] La creación de textos muy largos en la cinta de opciones puede generar bloqueos
&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] USD exportación desencadenada por TextureStateEvent
&#x200B;* [Motor] Pintura con la herramienta Clonar en colores de cambio de canal normales incorrectamente
&#x200B;* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.1.0

Fecha de publicación: <b>11/2025/18</b>
Sumario: <b>Esta actualización es una versión importante, contiene la nueva herramienta Cinta de opciones con contenido nuevo dedicado, soporte de simetría para capas de relleno, parámetro de tamaño físico para desplazamiento, rendimiento mejorado a través de los bakeres actualizados, soporte completo de Vulkan para Windows y Linux y otras mejoras.</b>

<b>Agregado</b>:

&#x200B;* Nueva herramienta de cinta
&#x200B;* [Herramienta] Agregar nueva herramienta Cinta para crear trazados sin problemas
&#x200B;* [Cinta de opciones] Añadir accesos directos preestablecidos de cinta en la ventana Propiedades
&#x200B;* [Cinta] Permite cambiar la opacidad de la Cinta por vértice en la ruta
&#x200B;* [Cinta de opciones] Permite cambiar el tamaño de la Cinta de opciones por vértice en la ruta
&#x200B;* [Cinta de opciones] Quitar el inicio o el final definido en un Substance cuando las rutas están cerradas
&#x200B;* [Cinta] Quitar vista previa de ruta/material en la ventana de propiedades para las herramientas de Pintura/Borrador/Difuminado de trazado
&#x200B;* [Cinta] Añadir modos de fusión para el canal alfa y algunos canales cuando se superponen automáticamente
&#x200B;* Rellenar simetría
&#x200B;* [Rellenar] Compatibilidad añadida para la simetría en capas y efectos de relleno
&#x200B;* [Relleno] [IU] Visualización de la configuración de simetría en la ventana de propiedades para la capa de relleno y los efectos
&#x200B;* [Fill] Interfaz de usuario de configuración de reprocesamiento de simetría tanto en el menú de la ventana como en la ventana de propiedades
&#x200B;* [Fill] Reorienta correctamente las texturas normales al proyectar en modo de deformación
&#x200B;* desplazamiento tamaño físico
&#x200B;* [Desplazamiento] Utilice tamaño físico como unidad de desplazamiento
&#x200B;* Mejora del rendimiento
&#x200B;* [Rendimiento] Mejora el procesamiento de trazos de pincel pequeños en triángulos grandes
&#x200B;* [Rendimiento] Mejorar el tiempo de compilación del Sombreador
&#x200B;* [Rendimiento] Compatibilidad total con Vulkan para Windows y Linux
&#x200B;* [Rendimiento] bakeres actualizados con procesamiento de GPU más rápido y compatibilidad con trazados de rayos AMD
&#x200B;* [UI] Reorganizar las propiedades de las herramientas en grupos y contraer algunas de forma predeterminada
&#x200B;* [Motor] Actualice Substance Engine a la versión 9.2.5.
&#x200B;* [Substance] Anulación de resolución de exposición para recursos de Substance en Herramientas y rellenos
&#x200B;* [Exportar] Actualizar el ajuste preestablecido de exportación de Mapas de malla para exportar texturas en escala de grises
&#x200B;* Python
&#x200B;* [Haciendo un bake] [Python] Indicar en el registro de cambios los cambios después de la actualización de bakeres
&#x200B;* [Python] Exposición de la configuración de simetría de relleno en Python
&#x200B;* Contenido y nuevo contenido
&#x200B;* [Contenido] Añadir 75 nuevos ajustes preestablecidos de herramientas para la herramienta Cinta de opciones
&#x200B;* [Contenido] Actualizar el recurso del generador de degradados para que sea compatible con la cinta de opciones

<b>Corregido</b>:

&#x200B;* [Bloqueo] La carga de otro proyecto mientras el ajuste de ruta está activado puede generar bloqueos
&#x200B;* [Bloqueo] Al hacer clic con el botón derecho en el panel Trazado con información de otra sesión del portapapeles, se puede crear un bloqueo
&#x200B;* [UI] La interfaz se desplaza hacia arriba en las propiedades de la herramienta al crear un trazado
&#x200B;* [UI] El cursor del ratón desaparece cuando la visualización de la ventanilla de trazado está oculta
&#x200B;* [Path] Copiar/pegar diferentes propiedades de herramienta en el panel Trazado genera propiedades inestables
&#x200B;* Los ajustes preestablecidos de las herramientas Borrador y Difuminado no siempre actualizan la selección de canales
&#x200B;* [Herramienta] El valor pintado es gris, pero la interfaz de usuario se muestra blanca después de cargar el ajuste preestablecido de herramienta de color en la máscara
&#x200B;* [Herramienta] El ajuste preestablecido creado a partir de la máscara conserva los valores de canales cargados de otro ajuste preestablecido
&#x200B;* [Substance] No se tiene en cuenta la anulación del espacio de color normal definido en el gráfico
&#x200B;* [Contenido] El recurso de forma de pincel predeterminado utiliza un Substance obsoleto

<b>Problemas conocidos</b>:

&#x200B;* El historial de instancias del sombreador no se rastrea correctamente
&#x200B;* [Ribbon] Problema de rendimiento con mosaicos UV
&#x200B;* [Cinta] En algunos casos, la ruta puede superponerse inesperadamente después de una esquina
&#x200B;* [Cinta] Las tangentes crean bucles no deseados cuando el punto se mueve de cerca a los extremos del trazado
&#x200B;* [Bloqueo] [Cinta] La creación de textos muy largos en la cinta de opciones puede bloquearse
&#x200B;* [Herramienta] La previsualización de material no funciona cuando se utiliza la proyección en una máscara
&#x200B;* [Haciendo un bake] El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y &quot;coincidencia por nombre&quot; activado
&#x200B;* [Haciendo un bake] El AO con normal tiene defectos en los bordes debido a la falta de relleno
&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
&#x200B;* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
&#x200B;* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.0.3

Fecha de publicación: <b>2025/08/05</b>
Resumen: <b>Versión secundaria</b>

<b>Agregado</b>:

&#x200B;* [Substance 3D Assets] Adición de un punto de notificación al panel Activos 3D
&#x200B;* [VFX Platform 2025] Añadir la configuración de ACES 2.0 en los ajustes de gestión de color
&#x200B;* [VFX Platform 2025] Actualice OCIO a la versión 2.4.2
&#x200B;* Actualizar Iray a la versión 2024.10
&#x200B;* [Motor] Actualización a Substance Engine v.9.2.3
&#x200B;* [Nvidia] Aumente la versión mínima de controladores de Nvidia a 572.60 (Windows) y 570.169 (Linux).

<b>Corregido</b>:

&#x200B;* [Python] La modificación de ámbito no aparece en la ventana Historial

<b>Problemas conocidos</b>:

&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
&#x200B;* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
&#x200B;* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.0.2

Fecha de publicación: <b>2025/06/10</b>
Resumen: <b>Versión secundaria</b>

<b>Agregado</b>:

&#x200B;* [Mac] Se añade una advertencia sobre una versión específica del sistema operativo que provoca artefactos
&#x200B;* [Actualización automática] Pequeñas mejoras de UX en el registro de errores de Activos
&#x200B;* [Auto-unwrap] Actualice a la versión 1.3.2 con mejoras de unión
&#x200B;* [USD]&#x200B;[FBX] Añade compatibilidad con varios conjuntos UV con datos dispersos
&#x200B;* [Exportar] Las mallas exportadas como FBX no tienen sus conjuntos UV adicionales si los había en la importación

<b>Corregido</b>:

&#x200B;* [MacOS]&#x200B;[Linux] Bloqueo al guardar en una unidad de red
&#x200B;* [Windows] [Tablet] Parpadeo al realizar una panorámica
&#x200B;* [SpaceMouse] Problema al trabajar con la herramienta Trazado
&#x200B;* [Jaula automática] No se puede hornear después de una recarga de malla
&#x200B;* [Actualización automática] La secuencia de imágenes no se vuelve a cargar cuando falta el primer mosaico
&#x200B;* [Path] La tangente personalizada puede afectar a otra tangente
&#x200B;* [Path] El trazado no aparece en el conjunto de texturas si el primer punto está en otro conjunto de texturas
&#x200B;* [UI] Algunos menús siempre se desactivan después de abrir un proyecto (por ejemplo: simetría)
&#x200B;* [Propiedades] No es posible utilizar ni cargar los ajustes preestablecidos de la herramienta Trazado relleno
&#x200B;* [USD] No se reconocen varios conjuntos UV en el sombreador personalizado al utilizar archivos USD
&#x200B;* [USD] Se reemplazan las cámaras con los mismos nombres
&#x200B;* [Exportar] Enviar a Photoshop genera un espacio de color incorrecto para los resultados de color y escala de grises
&#x200B;* [Exportar] Los canales en escala de grises con alfa se exportan como color en lugar de como escala de grises con formato PNG
&#x200B;* [Exportar] Al exportar un canal de escala de grises como PSD, el archivo resultante no es válido o está truncado
&#x200B;* [Contenido] El filtro de deformación en modo multidireccional no funciona
&#x200B;* [Python] No se puede asignar el error de lista al rastrear nodos de pila de capas

<b>Problemas conocidos</b>:

&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
&#x200B;* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
&#x200B;* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.0.1

Fecha de publicación: <b>2025/04/10</b>
Resumen: <b>Versión secundaria</b>

Nota: La versión de <b>Linux CCD se retrasará hasta el 29 de abril</b>

<b>Agregado:</b>

&#x200B;* Actualizar a Qt 6.5.8
&#x200B;* [Substance] Añadir mensaje de registro para filtros cuando varias entradas de imagen comparten el mismo uso
&#x200B;* [Nvidia] Añadir advertencia sobre los controladores más recientes de Nvidia (572.47)

<b>Corregido:</b>

&#x200B;* [Bloqueo] Al arrastrar y soltar una barra lateral con un uso en ranuras de un solo canal
&#x200B;* [Bloqueo]&#x200B;[Ruta] La opción Cambiar tipo de ruta no aparece atenuada al no hacer clic en una ruta específica
&#x200B;* [Rellenar trazado] No debe poder seleccionar material de Substance
&#x200B;* [Motor] Artefactos a lo largo de trazos de pincel
&#x200B;* [Motor] Los trazados se pueden romper con ajustes específicos
&#x200B;* Problema con el menú desplegable para el espacio de color del cuentagotas
&#x200B;* [Actualización automática] [Python] Mensaje de error incorrecto al utilizar ResourceID sin versión
&#x200B;* [Shader] Bloqueo al abrir algunos proyectos

<b>Problemas conocidos:</b>

&#x200B;* [SpaceMouse] Problema al trabajar con la herramienta Trazado
&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
&#x200B;* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
&#x200B;* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando

### 11.0.0

Fecha de publicación: <b>2025/03/11</b>
Resumen: <b>Versión principal, nueva función de actualización automática, herramienta de ruta rellena y otras mejoras en la ruta, así como nuevos filtros y una generación experimental de jaula automática para hornear</b>

<b>Agregado</b>:

&#x200B;* Actualización automática
&#x200B;* [Actualización automática] Actualización automática de activos modificados en el panel Activos
&#x200B;* [Actualización automática] Actualización automática de activos modificados en todo el proyecto
&#x200B;* [Actualización automática] Mantener la actualización automática desactivada de forma predeterminada
&#x200B;* [Actualización automática] Hacer que la actualización sea opcional si los parámetros del recurso no coinciden (.sbsar, .glsl, .ai, .svg)
&#x200B;* [Actualización automática] Añadir variable de entorno para desactivar la función de actualización automática
&#x200B;* [Actualización automática] [SBSAR] Convertir la actualización en opcional si los parámetros del recurso no coinciden
&#x200B;* Trazado relleno
&#x200B;* [Trazado]&#x200B;[Rellenar] Añadir una nueva herramienta para crear trazados rellenos
&#x200B;* Mejoras de ruta
&#x200B;* [Path] Crear un trazado que se ajusta a polígonos
&#x200B;* [Path] Permitir cambiar entre tipos de ruta
&#x200B;* [Ruta] Permite copiar y pegar datos de vértices de ruta entre contenido y máscara
&#x200B;* [Trazado] Permite restringir el ángulo al crear un nuevo punto
&#x200B;* [Ruta] Permite crear puntos de restricción en una línea
&#x200B;* [Path] Cierre la forma con un solo clic
&#x200B;* [Path] Visualización de la información de ruta
&#x200B;* [Path] Permita escalar y rotar los vértices del trazado
&#x200B;* [Path]&#x200B;[UX] Facilita el acceso a las herramientas de transformación
&#x200B;* [Path] Añadir vista previa de ruta
&#x200B;* [Trazado] Desactivar la previsualización de trazado con Mayús + P
&#x200B;* [Path] Mejora de la edición de tangentes desde la vista lateral
&#x200B;* [Trazado] Permitir que el enfoque se centre en un trazado 3D
&#x200B;* [Path] Los vértices deben conservar el estado de selección al activar o desactivar la IU de nuevo
&#x200B;* [Ruta] Permitir eliminar la ruta con la barra espaciadora
&#x200B;* [Path] Mantenga abierta la lista de rutas si el usuario la expande
&#x200B;* [Ruta]&#x200B;[Pila de capas] Cambiar correctamente el nombre de los duplicados al copiar y pegar
&#x200B;* [Path] Mejoras en la interfaz de usuario y la información sobre herramientas
&#x200B;* Rendimiento
&#x200B;* [Rendimiento] Mejore el rendimiento de la ventanilla al utilizar un nivel de teselación alto
&#x200B;* [Rendimiento] Habilite solo el primer canal en las nuevas capas/efectos de relleno
&#x200B;* [Rendimiento] Paralelizar el cálculo de trazos de pincel
&#x200B;* Baking
&#x200B;* [Hacer un bake] Añadir nueva opción de generación de jaulas totalmente automática para hacer un bake con mallas de alto contenido de polietileno (experimental)
&#x200B;* Contenido
&#x200B;* [Contenido] Añade 6 filtros nuevos: estilización, cuantificar, anisotrópico kuwahara, suavizado de bisel, distancia direccional, conversión de escala de grises
&#x200B;* [Contenido] Actualización de Noises y Grunges a la versión más reciente de Designer (con el nuevo 2D Voronoi)
&#x200B;* [Contenido] Añada 3 nuevos generadores de textura (Aleatorio de azulejos, Triangle Grid, Generador de Scratches)
&#x200B;* [Contenido] Cambiar nombre de plantilla de Unreal Engine y exportar ajustes preestablecidos
&#x200B;* Python
&#x200B;* [Shelf] [Python] Guardar material inteligente o máscara inteligente en disco desde Python
&#x200B;* [Python] Adición de la jaula automática de hace un bake a la API de Python
&#x200B;* [Python] Permite editar nombres y descripciones de conjuntos de texturas/Mosaicos de UV
&#x200B;* [Python] Compartir la configuración de resolución en fuentes de fuentes y vectores
&#x200B;* [Actualización automática] [Python] Exponer las funcionalidades de actualización automática del proyecto en Python
&#x200B;* Varios
&#x200B;* [Exportar] Facilite el acceso a las opciones de Enviar a con un nuevo panel
&#x200B;* [Nvidia] Añadir advertencia sobre los controladores más recientes de Nvidia (572.16)
&#x200B;* El ajuste de ángulo debe verse afectado por la selección de espacio Objeto/Mundo
&#x200B;* [Lista de conjuntos de texturas] Permitir agregar nombres personalizados a los Mosaicos de UV y utilizarlos en la exportación
&#x200B;* Mac
&#x200B;* [Mac] Uso de Metal en lugar de OpenGL para el procesamiento de gráficos
&#x200B;* [Mac] Se retira la asistencia de Mac Intel

<b>Corregido</b>:

&#x200B;* [Bloqueo] Eliminar entrada de imagen
&#x200B;* No se puede agregar una alfombra inteligente mediante el botón de pila de capas
&#x200B;* [Python] No se pueden encontrar efectos en GroupLayerNode

<b>Problemas conocidos</b>:

&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] USD exportación desencadenada por TextureStateEvent
&#x200B;* bloqueo [MacOS Intel] al importar algunos ajustes preestablecidos
&#x200B;* [Motor] Pintura con la herramienta Clonar en colores de cambio de canal normales incorrectamente
&#x200B;* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando
&#x200B;* [RedHat] Problemas con el selector de color

## Versión 10

### 10.1.2

Fecha de publicación: <b>2024/12/3</b>
Resumen: <b>versión secundaria, correcciones de errores</b>

<b>Corregido</b>:

&#x200B;* [Bloqueo] Eliminar entrada de imagen
&#x200B;* No se puede agregar una alfombra inteligente mediante el botón de pila de capas
&#x200B;* [Python] No se pueden encontrar efectos en GroupLayerNode

<b>Problemas conocidos</b>:

&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] USD exportación desencadenada por TextureStateEvent
&#x200B;* bloqueo [MacOS Intel] al importar algunos ajustes preestablecidos
&#x200B;* [Motor] Pintura con la herramienta Clonar en colores de cambio de canal normales incorrectamente
&#x200B;* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando
&#x200B;* [RedHat] Problemas con el selector de color

### 10.1.1

Fecha de publicación: <b>2024/11/5</b>
Resumen: <b>versión secundaria, correcciones de errores</b>

<b>Agregado</b>:

&#x200B;* [Project] Mantenga abierto el proyecto actual hasta que se valide la selección de nuevo proyecto
&#x200B;* [Desenvolvimiento automático] La densidad de los textos permite dividir mejor las Islas de UV en UDIM
&#x200B;* [Hacer un bake] Corregir copia ambigua en el menú contextual de Mapas de malla
&#x200B;* [Deformar] Eliminación de la escala en la ventana gráfica para el eje Z (profundidad)
&#x200B;* [Importar/Exportar] Quitar la compatibilidad de los formatos de archivo de imagen no utilizados
&#x200B;* Actualizar Substance Engine a 9.1.4

<b>Corregido</b>:

&#x200B;* [Bloqueo] Después de reubicar el recurso en Recursos y guardar el proyecto
&#x200B;* [Bloqueo] Problemas con la biblioteca de aiserver
&#x200B;* [Bloqueo] bloqueo del servidor Illustrator en algunos casos excepcionales
&#x200B;* [Bloqueo] Al salir de la aplicación en algunos casos raros
&#x200B;* No se pueden enviar informes de bloqueo en algunos equipos
&#x200B;* [Horneado] El color del vértice no se lee correctamente
&#x200B;* [UI] La ubicación de las ventanas y las novedades al inicio se cambian
&#x200B;* [Assimp] Maya&#39;s StandardSurface no reconocida en el baking de ID
&#x200B;* [Python] La biblioteca SSL que falta genera un error
&#x200B;* [Python]&#x200B;[Windows] Error al llamar a QColorConstants.Transparent
&#x200B;* [Python] Las miniaturas de capas creadas mediante Python no se actualizan hasta que se hace clic dentro de la pila de capas
&#x200B;* [Shader] Vínculo roto en el registro de cambios de API del sombreador
&#x200B;* [3D Assets] Usar la configuración del proxy del sistema operativo al acceder a 3D Assets

<b>Problemas conocidos</b>:

&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
&#x200B;* [MacOS Intel] Bloqueo al importar algunos ajustes preestablecidos
&#x200B;* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
&#x200B;* [Python] El widget que parece eliminado mediante el script sigue funcionando
&#x200B;* [RedHat] Problemas con el selector de color

### 10.1.0

Fecha de publicación: <b>2024/09/17</b>
Resumen: <b>Versión principal, nuevo contenido: Filtro de color/máscara de área de relleno, filtro de pegatinas de bordado y seis filtros de Substance genéricos, importación de USD con propiedades de materiales y sombreadores, mejora del rendimiento, compatibilidad con VFX Platform 2024 y migración a Linux RedHat</b>

<b>Agregado</b>:

&#x200B;* [Contenido] Añadir nuevo filtro de color/máscara de área de relleno
&#x200B;* [Contenido] Añadir nuevo filtro de pegatinas de bordado
&#x200B;* [Contenido] Añade 6 nuevos filtros de Substance genéricos (FXAA, pixelado, paso alto, posterizar, paso suave y umbral)
&#x200B;* [USD] Exportar capa USD con un material de ASM definido
&#x200B;* [USD] Importar USD con propiedades de materiales y sombreadores
&#x200B;* [Rendimiento] Habilitar miniaturas de pila de capas optimizadas de forma predeterminada
&#x200B;* [Rendimiento] Reducir el tiempo de apertura de archivos de proyecto y el consumo de memoria (descodificación de datos)
&#x200B;* Compatible con la plataforma VFX 2024
&#x200B;* [VFX Platform 2024] Actualización a Python 3.11
&#x200B;* [VFX Platform 2024] Actualización a OpenEXR 3.2
&#x200B;* [VFX Platform 2024] [USD] Actualización de OpenSubdiv 3.6.0
&#x200B;* [VFX Platform 2024] [Gestión de color] Actualización a OCIO 2.3.2
&#x200B;* [Linux] Migración a Linux RedHat
&#x200B;* [Linux] Actualice la versión principal del controlador Nvidia a 535.171.04
&#x200B;* [Importar] Añada una opción para voltear la asignación normal al importar una malla GLTF
&#x200B;* [UI] Usar el valor predeterminado del sistema operativo para la distancia de detección de eventos de arrastre
&#x200B;* [Substance Engine] Añada la función de tira de llamadas para eliminar los símbolos del ejecutable
&#x200B;* [Pantalla de bienvenida] Actualización al nuevo formato de pantalla de bienvenida
&#x200B;* Actualizar Substance Engine a la versión 9.1.3
&#x200B;* [Python] Mostrar vínculos a ejemplos en el menú de documentación de la pila de capas
&#x200B;* [JavaScript] Mover complementos de Javascript a la subcarpeta javascript/plugins

<b>Corregido</b>:

&#x200B;* [Illustrator] Bloqueo al exportar un azulejo UV con un gráfico .ai en casos específicos
&#x200B;* [Trazos dinámicos]&#x200B;[Trazado] La opción aleatoria por trazo no funciona en un trazado
&#x200B;* [UI]&#x200B;[Propiedades] El bloqueo está activado cuando el mosaico no es uniforme
&#x200B;* El archivo TXT de depuración se crea al hacer doble clic en el proyecto de Painter
&#x200B;* [USD]&#x200B;[Exportar] Es posible que falten algunas texturas
&#x200B;* [ASM] El canal de color de dispersión ignora el metal
&#x200B;* [Contenido] El filtro de desenfoque no funciona en espacios de color &quot;operativos&quot;
&#x200B;* [Contenido] Height Ajustar filtro también modifica el alfa de la capa

<b>Problemas conocidos</b>:

&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Win] [Bloqueo] [ACE] No se utiliza el espacio de color sRGB ICE para la transformación de la pantalla
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
&#x200B;* [MacOS Intel] Bloqueo al importar algunos ajustes preestablecidos
&#x200B;* [Bloqueo] Reubicar recurso y guardar proyecto
&#x200B;* [Motor] Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
&#x200B;* [Python] El widget fantasma aparece eliminado por la secuencia de comandos y sigue funcionando
&#x200B;* [RedHat] Problemas con el selector de color

### 10.0.1

Fecha de publicación: <b>2024/06/11</b>
Resumen: <b>Versión secundaria, correcciones de errores</b>

<b>Agregado:</b>

&#x200B;* [Biblioteca] Convertir fuentes de Substance en archivos de fuentes normales
&#x200B;* [Illustrator] [SVG] Aplica un fondo gris claro a las miniaturas en la selección de ámbito
&#x200B;* [Python] Añadir función en origen de mapa de bits para enumerar los espacios de color disponibles

<b>Corregido</b>:

&#x200B;* [Pila de capas] La carpeta siempre se cierra al entrar o salir de otras carpetas
&#x200B;* [Guardar] El archivo de proyecto se pierde cuando se produce un error al guardar como copia o al guardar automáticamente en casos específicos
&#x200B;* [Importar] Los recursos con el mismo nombre pero extensiones diferentes se anulan
&#x200B;* [Propiedades] Faltan opciones de configuración al utilizar un punto de anclaje en las entradas de imagen
&#x200B;* [Illustrator] No es posible importar archivos de Illustrator después de un bloqueo del servidor sin reiniciar Painter
&#x200B;* [Python] El padre de la instancia no se puede establecer con el tipo &quot;properties&quot;
&#x200B;* [Python] Al configurar el poli alto como parámetro de horneado, no se carga el poli alto
&#x200B;* [Python] El mensaje de error para set\_color\_space() es demasiado genérico
&#x200B;* [Python] Las fuentes de referencia permiten crear ciclos

<b>Problemas conocidos</b>:

&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Regresión]&#x200B;[IU] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] Exportación de USD desencadenada por TextureStateEvent
&#x200B;* [MacOS Intel] Bloqueo al importar algunos ajustes preestablecidos
&#x200B;* [Illustrator] Bloqueo al exportar un azulejo UV con un gráfico .ai en casos específicos
&#x200B;* [Trazos dinámicos]&#x200B;[Trazado] La opción aleatoria por trazo no funciona en un trazado

### 10.0.0

Fecha de publicación: <b>2024/05/16</b>
Resumen: <b>Versión principal, edición de la pila de capas con la API de Python, lectura de archivos nativos de Illustrator, integración de recursos 3D y nuevo recurso de texto</b>

<b>Agregado</b>:

&#x200B;* [Illustrator] Uso de archivos de Illustrator con mesas de trabajo en Painter
&#x200B;* [Illustrator] [SVG] Añadir vistas previas en la selección de ámbito
&#x200B;* [Substance 3D Assets] Busque, seleccione y descargue contenidos 3D directamente en Painter
&#x200B;* [Substance 3D Assets]&#x200B;[UI] Nuevo panel
&#x200B;* [Substance 3D Assets] Mapas y materiales del entorno de apoyo
&#x200B;* [Substance 3D Assets] Permite volver a cargar, navegar y abrir la carpeta de ubicación en el nuevo panel Substance 3D Assets.
&#x200B;* [Substance 3D Assets] Adición de un gestor de descargas
&#x200B;* [Recurso de texto] Permitir el uso de fuentes incrustables
&#x200B;* [Recurso de texto] Permitir procesar una fuente/texto en una malla
&#x200B;* [Recurso de texto] Visualización de fuentes del usuario y otras rutas compartidas en el panel Activos con una nueva categoría
&#x200B;* [Recurso de texto]&#x200B;[Propiedades] Añadir compatibilidad con propiedades de fuentes avanzadas
&#x200B;* [Recurso de texto] Permitir buscar/ver fuentes en miniestantes
&#x200B;* [Recurso de texto] Añadir mensaje/cuadro de diálogo de error al importar una fuente incompatible
&#x200B;* Miscelánea
&#x200B;* [Proyección de relleno] Mejora el comportamiento del manipulador Escala al utilizar valores pequeños
&#x200B;* [Manipuladores] Añadir nuevo modo preciso al pulsar el método abreviado CTRL
&#x200B;* [Manipuladores] Mejora la estabilidad del manipulador de superficie al trasladar
&#x200B;* [Exportar] Añadir nombre de espacio de color en salidas SBSAR
&#x200B;* [Rendimiento] Mejora el tiempo de detección de activos en la biblioteca en el disco
&#x200B;* [Substance] Actualización al motor de Substance versión 9.1.2
&#x200B;* [Arrastrar y soltar] Alinear la rotación de pegatinas con la cámara al soltar en la ventana gráfica
&#x200B;* [Python] Edición de la pila de capas
&#x200B;* [Python] Permite seleccionar capa, efecto, máscara o máscara geográfica en la interfaz de usuario.
&#x200B;* [Python] Permitir obtener/definir modos de fusión de capas
&#x200B;* [Python] Permitir obtener o establecer la configuración de proyección de la capa de relleno
&#x200B;* [Python] Permitir consultar el color de material de Substance desde una capa de relleno
&#x200B;* [Python] Permite consultar y establecer colores uniformes y recursos en capas y efectos
&#x200B;* [Python] Permita crear y editar recursos de texto en pila de capas
&#x200B;* [Python] Permite editar canales activos en capas y efectos
&#x200B;* [Python] Permitir que las acciones por lotes tengan una sola acción de deshacer/rehacer
&#x200B;* [Python] Permita cargar o editar parámetros de origen vectoriales
&#x200B;* [Python] Permite editar propiedades de color de capas y efectos con la gestión de color
&#x200B;* [Python] Permite consultar y crear capas con instancias
&#x200B;* [Python] Permitir la adición del efecto de selección de color
&#x200B;* [Python] Permite controlar la administración de color de la imagen de mapa de bits
&#x200B;* [Python] Permitir detener/anular la pausa del motor
&#x200B;* [Python] Permite navegar a nodos hermanos y principales
&#x200B;* [Python] Permitir la creación de un efecto de filtro/generador
&#x200B;* [Python] Permitir añadir un efecto de nivel
&#x200B;* [Python] Permitir añadir máscara inteligente en una capa
&#x200B;* [Python] Permitir crear o editar puntos de ancla
&#x200B;* [Python] Permitir obtener/Establecer máscara en capas
&#x200B;* [Python] Permitir la creación del efecto de máscara de comparación
&#x200B;* [Python] Permitir consultar y utilizar ajustes preestablecidos de recursos de Substance
&#x200B;* [Python] Permite enumerar los ajustes preestablecidos y sus valores mediante la función interna\_properties para los recursos del Substance
&#x200B;* [Python] Permite enumerar los ajustes preestablecidos de exportación predefinidos
&#x200B;* [Python] Se permite enumerar los ajustes preestablecidos de exportación disponibles en la biblioteca.
&#x200B;* [Python] Permite recuperar el contenido de los ajustes preestablecidos de exportación

<b>Corregido</b>:

&#x200B;* [Bloqueo] Deshaciendo &quot;Quitar instancia de sombreado&quot; con Ctrl-Z
&#x200B;* [Bloqueo] Crear una capa en una pila vacía si la última selección fue un efecto
&#x200B;* [SVG] Problema con el valor de área recortada personalizada
&#x200B;* [Auto-Unwrap] Si se vuelve a calcular solo el empaquetado sin ningún cambio en la orientación UV, se produce un bloqueo
&#x200B;* [Arrastrar y soltar] El retraso debido a los recursos externos se carga previamente varias veces
&#x200B;* [UI] Arrastrar y soltar la miniatura de un recurso puede ocultar un mensaje de advertencia en la pila de capas
&#x200B;* [Rendimiento] Los mosaicos UV enmascarados aún se calculan
&#x200B;* [USD] Resaltado incorrecto para la selección del ámbito
&#x200B;* [Recurso] La imagen de mapa de bits se daña después de pintar en el canal normal y guardar el proyecto
&#x200B;* [USD] Admite la solicitud de mallas de vértices con la mano izquierda
&#x200B;* [Substance] Restablecer los valores predeterminados volver siempre a cero para el widget de ángulo
&#x200B;* [Motor] Pintar con un SVG en una galería de símbolos no funciona
&#x200B;* [Motor] Los trazos normales del pincel de mapa se rompen después de deshacer una acción
&#x200B;* [Contenido] El filtro Gráfico a material tiene una fusión alfa y un espacio de color incorrectos
&#x200B;* [Contenido] Los modos de fusión del Tile Generator no funcionan
&#x200B;* [Contenido] El filtro de barrido de histograma produce bandas en algunos casos
&#x200B;* [Contenido] La iluminación Hecha un bake estilizada no tiene en cuenta el height pintado
&#x200B;* [Python] Error inesperado al recuperar información de capas instanciada después de un cambio de sombreador
&#x200B;* [Guardar] El archivo de proyecto se pierde cuando se produce un error en &quot;Guardar como&quot; en casos específicos

<b>Problemas conocidos</b>:

&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
&#x200B;* [Bloqueo]&#x200B;[Linux]&#x200B;[AMD] Arrastre y eliminación de recursos en la pila de capas en el sistema operativo Wayland
&#x200B;* [Regresión]&#x200B;[UI] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] USD exportación desencadenada por TextureStateEvent
&#x200B;* [Guardar] El archivo de proyecto de Spp se pierde cuando se produce un error en &quot;Guardar como copia&quot; en casos específicos
&#x200B;* bloqueo [MacOS Intel] al importar algunos ajustes preestablecidos
&#x200B;* [Illustrator] No es posible importar archivos de Ai después del bloqueo del servidor sin reiniciar Painter
&#x200B;* [Importar] Los recursos con el mismo nombre pero extensiones diferentes se anulan

## Versión 9

### 9.1.2

Fecha de publicación: <b>30/01/2024</b>
Resumen: <b>versión secundaria, correcciones de errores</b>

<b>Agregado</b>:

&#x200B;* [Rendimiento] Mejora el tiempo de creación de la primera capa de relleno en nuevos proyectos
&#x200B;* [Rendimiento] Reducir el tiempo de carga de mapas de entorno pesados
&#x200B;* [Substance] Permite guardar o cerrar proyectos incluso cuando se generan miniaturas

<b>Corregido</b>:

&#x200B;* La acción de guardar falla en proyectos de versiones anteriores cuando se modifica la ventana gráfica
&#x200B;* [Bloqueo] Reimportación de mallas al utilizar archivos AO y gestión de color personalizados
&#x200B;* [Rellenar la proyección] Al hacer clic en el manipulador de escala aparece el mensaje &quot;no puede pintarse&quot;
&#x200B;* [Pincel] Pintar con alineación UV provoca defectos
&#x200B;* [Pila de capas] El cambio de nombre de la capa es lento cuando la pila es muy larga
&#x200B;* [Pila de capas] Mensaje de error incorrecto al utilizar filtros incompatibles en la máscara
&#x200B;* [Pila de capas] La selección vuelve a la capa superior después de la eliminación
&#x200B;* [Exportar] La textura normal generada siempre está en el modo de relleno de vecinos del espacio 3D
&#x200B;* [Exportar] La Textura alfa no se genera con el ajuste preestablecido de exportación de vista 2D
&#x200B;* [Exportar] La exportación SBSAR tiene usos incorrectos con mapas convertidos
&#x200B;* [Sombreador] El registro de cambios de API del sombreador no está actualizado con los últimos cambios de ASM

<b>Problemas conocidos</b>:

&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
&#x200B;* [Bloqueo]&#x200B;[Linux]&#x200B;[AMD] Arrastre y eliminación de recursos en la pila de capas en el sistema operativo Wayland
&#x200B;* [Regresión]&#x200B;[UI] El menú contextual es demasiado pequeño en pantallas HD
&#x200B;* [Bloqueo] [Python] USD exportación desencadenada por TextureStateEvent

### 9.1.1

Fecha de publicación: <b>12/2023/05</b>
Resumen: <b>Versión secundaria, correcciones de errores y envío a la funcionalidad de After Effects</b>

<b>Agregado:</b>

&#x200B;* [Interop] Permitir el envío de una malla con textura a After Effects (Ae 24.1)

<b>Corregido:</b>

&#x200B;* [Relleno] La proyección del conjunto UV en UV no lee más de 2 conjuntos UV
&#x200B;* [Bloqueo] Uso del mapa de entorno de 16K
&#x200B;* [Bloqueo] Exr utilizado como entrada de imagen
&#x200B;* [Bloqueo] Copiar y pegar trazados en proyectos
&#x200B;* [QoL] Arrastrar y soltar un recurso de Alpha en modo de pegatina crea Proyección de UV en la máscara
&#x200B;* [Path] Al copiar vértices de trazado también se cambia el nombre de la ruta de destino al volver a abrir el proyecto
&#x200B;* [Linux] La selección de color se puede romper con varias pantallas
&#x200B;* [Auto Unwrap] Problema de interfaz de usuario para el control de densidad de texto
&#x200B;* Los comentarios de la interfaz de usuario de [Gestión de color] son razonables, pero el motor no
&#x200B;* [Gestión de color] Selección incorrecta del espacio de color en la máscara con anulación de datos de usuario

<b>Problemas conocidos:</b>

&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Crash]&#x200B;[Linux] con Linux Wayland en AMD al arrastrar y soltar el recurso en la pila de capas
&#x200B;* [Bloqueo] [Mac] Cambio del valor de filtrado anisotrópico en el sistema operativo Monterey
&#x200B;* [Regresión]&#x200B;[UI] El menú contextual es demasiado pequeño en la pantalla HD
&#x200B;* [Python] Bloqueo al exportar USD activado por TextureStateEvent

### 9.1.0

Fecha de publicación: <b>2023/11/07</b>
Resumen: <b>Versión principal con compatibilidad con SVG y transparencia, así como mejoras en la herramienta de arrastrar y soltar y ruta</b>

<b>Agregado:</b>

&#x200B;* [SVG] Permitir la importación de archivos vectoriales (SVG)
&#x200B;* [SVG]&#x200B;[IU] Añadir compatibilidad con propiedades específicas del SVG
&#x200B;* [SVG] Añada una opción para conservar fácilmente las proporciones originales de la imagen
&#x200B;* [SVG] Permitir el uso automático de alfa de SVG con transparencia
&#x200B;* [Interop] Permita el envío de una malla con textura a After Effects (Ae 24.1 beta).
&#x200B;* [Interop] Añadir configuración para Enviar a After Effects
&#x200B;* [QoL]&#x200B;[Assets]&#x200B;[UI] Activo de importación automática al arrastrar y soltar en la ranura de la IU
&#x200B;* [QoL] Permite arrastrar y soltar activos externos en la pila de capas
&#x200B;* [QoL] [Pila de capas] Arrastra y suelta texturas desde el panel de Recursos en la pila de capas
&#x200B;* [QoL] [Viewport] Permite arrastrar y soltar el generador, filtros en la malla
&#x200B;* [QoL]&#x200B;[Viewport] Permite soltar recursos externos en la malla
&#x200B;* [QoL]&#x200B;[Proyección] Añadir nuevo conjunto UV al modo de proyección Conjunto UV
&#x200B;* [QoL] Arrastrar y soltar máscaras inteligentes como nuevas capas en la ventana gráfica y la pila de capas
&#x200B;* [QoL] Añadir selector para generadores con varias salidas cuando se utiliza en la máscara
&#x200B;* [QoL] Permite arrastrar y soltar imágenes de un solo canal sobre un efecto de relleno
&#x200B;* [QoL] [Pila de capas] Utilice los modificadores CTRL/ALT con arrastrar y soltar para especificar dónde y cómo crear efectos o capas
&#x200B;* [Path] Cambiar la visibilidad de los trazados individualmente en el panel de trazados
&#x200B;* [Path] Permita el uso de manipuladores de transformación para puntos de trazado
&#x200B;* [Path] Permite controlar manualmente las tangentes por vértice
&#x200B;* [Path] Copiar y pegar propiedades de ruta
&#x200B;* [Path] Introducir un método abreviado vacío para el botón de tangente de rotura
&#x200B;* [Shader] Añadir compatibilidad con Opacidad y translucidez en sombreador de ASM
&#x200B;* [Shader] Añadir compatibilidad para canal de Color de absorción con sombreador de ASM
&#x200B;* [Shader] Mejora de la información sobre herramientas de parámetros de sombreado de ASM
&#x200B;* [Sombreado] Cambiar el color predeterminado del canal de translación a negro
&#x200B;* [Configuración de pantalla] Habilitar Suavizado temporal de forma predeterminada
&#x200B;* [Configuración de visualización] Activar configuración de dispersión subsuperficial de forma predeterminada
&#x200B;* [Substance] Se ha añadido compatibilidad con la propiedad ColorSpace desde la entrada/salida del gráfico.
&#x200B;* [Substance] Actualice el motor del Substance a la versión 9.0.3.
&#x200B;* [UI] Hacer accesible el botón de la barra de herramientas contextual incluso si la ventana de la aplicación es pequeña
&#x200B;* [Auto Unwrap] Control UV Azulejos número con Densidad de Texel
&#x200B;* [Banking] Desactivar Trazado de rayos de GPU en GPU AMD de forma predeterminada
&#x200B;* [Rendimiento] Aplique compresión sin pérdida en imágenes de 16 bits para reducir el espacio del proyecto
&#x200B;* [Python] Permita manipular la cámara predeterminada en la vista 3D
&#x200B;* [Python] Exponer la capacidad de exportar mallas mediante scripts
&#x200B;* [Contenido]&#x200B;[Muestras] Añadir nuevo proyecto de muestra &quot;French Restaurant Table&quot;
&#x200B;* [Contenido] Actualizar el logotipo de Substance alfa a una nueva versión
&#x200B;* [Contenido] Añade tres filtros de material enfocados en el SVG (pegatina personalizada, spray personalizado y gráfico en el material)

<b>Corregido:</b>

&#x200B;* [Bloqueo] Cambio del tamaño del manipulador cuando no se utiliza la herramienta de simetría
&#x200B;* [Bloqueo] [Pila de capas] Crear capa cuando no hay nada seleccionado
&#x200B;* [Proyecto] Las asignaciones de malla se pueden dañar después de eliminar los recursos no utilizados
&#x200B;* [Proyecto] Daños en los recursos tras volver a importar o hacer un bake la imagen
&#x200B;* [Assets] Al volver a cargar un activo, se elimina de Favoritos
&#x200B;* [Importar] No se pueden importar recursos cuando &quot;No se encuentra ningún resultado&quot; en el panel de recursos
&#x200B;* [UI] La flecha de la barra de herramientas contextual no aparece en algunos casos
&#x200B;* [Substance] No se admite el botón en paralelo para valores booleanos
&#x200B;* [Nivel] Etiqueta de canal incorrecta cuando se utiliza en la máscara
&#x200B;* [Export]&#x200B;[glTF] Los archivos glTF/GLB exportados desde Painter no tienen una unidad de tamaño físico
&#x200B;* [Contenido] La intensidad del filtro de desenfoque se fija en 16
&#x200B;* [Contenido] La entrada de imagen del filtro &quot;color de destino&quot; no está visible

<b>Problemas conocidos:</b>

&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
&#x200B;* [Bloqueo] [Linux] con Linux Wayland en AMD al arrastrar y soltar el recurso en la Pila de capas
&#x200B;* [Bloqueo] [Mac] Cambio del valor de filtrado anisotrópico en el sistema operativo Monterey
&#x200B;* [Bloqueo] Exr utilizado como entrada de imagen
&#x200B;* [Bloqueo] Uso del mapa de entorno de 16K
&#x200B;* [Auto Unwrap] Problema de interfaz de usuario para el control de densidad de texto
&#x200B;* [Regresión]&#x200B;[UI] El menú contextual es demasiado pequeño en la pantalla HD
&#x200B;* [Python] Exportación de Bloqueos USD activada por TextureStateEvent
&#x200B;* [QoL] Arrastrar y soltar un recurso de Alpha en modo de pegatina crea Proyección de UV en la máscara

### 9.0.1

Fecha de publicación: <b>2023/09/19</b>
Resumen: <b>Versión menor de corrección de errores con varias mejoras</b>

<b>Agregado:</b>

&#x200B;* [Importar] Establecer ubicación de importación predeterminada en la ventana de importación
&#x200B;* [Modo de Hace un bake] Permite restablecer los parámetros a sus valores predeterminados
&#x200B;* [Hacer un bake] Establecer hacer un bake a la resolución de pintura al crear un proyecto
&#x200B;* [Simetría] Desvincular manipulador específico de simetría de método abreviado Q
&#x200B;* [Menú] Añada la opción &quot;mostrar registro&quot; en el menú de ayuda
&#x200B;* [Ventana gráfica] Mejorar la velocidad de procesamiento de sombras
&#x200B;* [Substance] Actualice el motor a la versión 9.0.1
&#x200B;* [Gestión de color] OCIO archivo de configuración puede tener cualquier tipo de extensión
&#x200B;* [Assets] El recurso de Sbsar con uso de &quot;pegatina&quot; debe configurarse automáticamente para deformar la proyección
&#x200B;* [Path] Muestra un mensaje al intentar interactuar con la herramienta Ruta mientras la IU y los Gizmos están ocultos

<b>Corregido:</b>

&#x200B;* [Bloqueo] Alt + arrastrar en el panel Trazado
&#x200B;* [Importar recursos] bloqueo aleatorio al quitar recursos para importar
&#x200B;* Bloqueo al importar un archivo GLB comprimido
&#x200B;* Problema al pintar en mallas que comparten UV
&#x200B;* Parpadeo de malla negro al volver a calcular o cargar la caché
&#x200B;* [Propiedades] El menú contextual para restablecer parámetros no aparece en los menús desplegables
&#x200B;* [Nivel] Reguladores de entrada bloqueados por nivel anterior
&#x200B;* [AMD] [Disperso] La opción SVT si se activa genera artefactos
&#x200B;* bloqueo [Proyección] [Deformar] al hacer doble clic en los vértices
&#x200B;* [Path] Interfaz de usuario y ruta de acceso visibles en el modo de hacer un bake
&#x200B;* [AMD] Se pierde la Textura al jugar con la visibilidad
&#x200B;* Resolución [dispersa] demasiado baja al girar la malla

<b>Problemas conocidos:</b>

&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción

### 9.0.0

Fecha de publicación: <b>2023/06/20</b>
Resumen: <b>Versión principal con Pintura a lo largo de la ruta que permite curvas 3D, nuevos materiales base y la limpieza de materiales heredados y nuevos ajustes preestablecidos para curvas 3D</b>

<b>Agregado:</b>

&#x200B;* [Path] Herramienta Agregar nueva Pintura a lo largo del trazado
&#x200B;* [Path] Agregar un método abreviado vacío para la herramienta de trazado
&#x200B;* [Path] Permite añadir nuevos puntos a un trazado existente
&#x200B;* [Path] Agregar método abreviado para salir de la creación de la ruta actual
&#x200B;* [Path] Permitir la edición de las propiedades de pincel de trazados
&#x200B;* [Trazado] Ajuste automático de tangentes al colocar un punto
&#x200B;* [Trazado] Calcular tangentes al mover un punto
&#x200B;* [Trazado] Ajuste los puntos recién creados a la superficie de una malla
&#x200B;* [Trazado] Permitir editar la presión por vértice
&#x200B;* [Trazado] Ajuste la presión del punto recién creado desde los puntos vecinos
&#x200B;* [Trazado] Permite convertir puntos en suavizado/esquina (salto de tangente)
&#x200B;* [Ruta] Permite mover un punto recién añadido inmediatamente
&#x200B;* [Path] Permite quitar puntos de un trazado existente
&#x200B;* [Path] Permite invertir la dirección de un trazado
&#x200B;* [Ruta] Permite seleccionar una ruta en la ventana gráfica
&#x200B;* [Trazado] Permitir la selección de puntos de trazado con selección de recuadro
&#x200B;* [Trazado] Introduzca métodos abreviados de CTRL-A para seleccionar todos los puntos de un trazado
&#x200B;* [Ruta] Permitir cerrar ruta
&#x200B;* [Path] Permite especificar el eje ascendente de la ruta en Propiedades
&#x200B;* [Path] Agregar un menú de control de vértices a la barra de herramientas contextual
&#x200B;* [Path] Introducción de los modos de pintura, borrado y difuminado en la herramienta de trazado
&#x200B;* [Path] Creación de comentarios visuales para rutas en la ventana gráfica
&#x200B;* [Ruta] Agregar un indicador visual de la dirección de la ruta
&#x200B;* [Ruta] Agregar thickness de línea a la configuración de visualización de ruta
&#x200B;* [Path] Permitir ocultar la interfaz de usuario de rutas
&#x200B;* [Path] Panel Añadir trazado para ver los trazados de la capa seleccionada actualmente
&#x200B;* [Path] Añadir comentarios visuales al pasar el puntero sobre un trazado en el panel Trazado
&#x200B;* [Path] Muestra el panel de trazado siempre que se selecciona la herramienta Trazado
&#x200B;* [Trazado] Permita cambiar el nombre, eliminar, copiar, cortar o duplicar el trazado en el panel Trazado
&#x200B;* [Path] Aparece un mensaje al intentar interactuar en la ventana gráfica 2D con la herramienta Ruta
&#x200B;* [Biblioteca] Integrar nuevo contenido (herramientas de ruta y materiales base)
&#x200B;* [Trazos dinámicos] Agregar propiedad de distancia para trazos dinámicos
&#x200B;* [Trazos dinámicos] Añadir propiedades de tamaño y espaciado a los trazos dinámicos
&#x200B;* [Trazos dinámicos] Agregar propiedad de inicio/centro/fin para trazos dinámicos
&#x200B;* [Python]&#x200B;[USD] Exponer los parámetros de configuración del proyecto para el formato USD
&#x200B;* [Python]&#x200B;[USD] Exponer parámetros de creación de proyectos para el formato USD
&#x200B;* [Export]&#x200B;[USD] Añadir información de la ruta del proyecto dentro del archivo de USD exportado
&#x200B;* [GLTF] Actualización de texturas en la biblioteca al volver a cargar un archivo GLTF
&#x200B;* [Sombreador] Reducir los defectos de costura para Islas de UV con diferente orientación
&#x200B;* [Motor] Actualice a la versión 9.0 del motor de Substance

<b>Corregido:</b>

&#x200B;* [Import] Algunos GLB con texturas no reciben texturas en Painter
&#x200B;* [AMD] Artefactos en los bordes para todos los rellenos de proyección 3D
&#x200B;* [Motor] Las Texturas se rompen al alternar la visibilidad de las capas
&#x200B;* [Motor] Las Texturas están vacías en algunos lugares al cambiar el modo de fusión
&#x200B;* [Motor] La Textura/proyección está en modo de deformación vacío en algunos casos
&#x200B;* [Iray] Iteración restablecida a 0 al guardar procesamiento
&#x200B;* [Log] USD mensaje de error al hacer Archivo > Nuevo

<b>Problemas conocidos:</b>

&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Pila de capas] El origen de entrada no se guarda por capa

## Versión 8

### 8.3.1

Fecha de publicación: <b>2023/04/27</b>

<b>Agregado:</b>

&#x200B;* [Modo de panadería] Añada un método abreviado (vacío) para mostrar/ocultar la visualización de la ventanilla
&#x200B;* [Modo de cocción] Mostrar siempre la capa baja de polietileno al utilizar el botón &quot;Ocultar mallas de cocción&quot;
&#x200B;* [Modo de cocción] Mostrar sufijo para hacer coincidir por nombre en función del conjunto de texturas actual
&#x200B;* [Importar] Añadir soporte para archivos binarios GLTF (glb)
&#x200B;* [Lista Conjunto de texturas] Añadir menú para seleccionar o crear instancias de sombreado
&#x200B;* [Lista de conjuntos de texturas] Permita cambiar rápidamente la resolución del conjunto de texturas y el azulejo UV
&#x200B;* [Tamaño físico] Mejora el comportamiento del manipulador al utilizar tamaño físico en Proyección de UV
&#x200B;* [UI] Volver a &quot;Guardar como&quot; en el menú Archivo principal
&#x200B;* [UI] Guardar selección de vista (solo 2D, solo 3D, ambos) en diseño de IU
&#x200B;* [USD] Mensaje de error menos impreciso al crear un proyecto con formas USD no compatibles
&#x200B;* [Python] Añadir eventos de procesamiento para seguir el progreso de procesamiento
&#x200B;* [Python] Permitir la cancelación de una cocción
&#x200B;* [Python] Exponer &quot;Según plantilla de salida&quot; para tipo de archivo y profundidad de bits en la exportación
&#x200B;* [Python] Exponer el tiempo de actualización para TextureStateEvent.Update

<b>Corregido:</b>

&#x200B;* [Bloqueo] Bloqueo raro al cerrar un proyecto
&#x200B;* [Bloqueo] [Horneado] Activar la sincronización del mapa de malla con el Height o la curvatura en un proyecto específico
&#x200B;* [Crash]&#x200B;[Scripting] Bloqueo al añadir un material tras la creación de la instancia del sombreador
&#x200B;* [Modo de cocción] La intensidad de AO en material neutro no tiene efecto
&#x200B;* bloqueo [Modo de Hace un bake] al cambiar al modo de hace un bake antes de cargar el modelo
&#x200B;* [Modo de Hace un bake] Falta el mensaje de error en la ficha Hacer un bake proceso
&#x200B;* [Modo de Hace un bake] Los ajustes de material neutro no tienen efecto después de volver a importar una malla
&#x200B;* [Modo de Hace un bake] El separador de ventanilla se guarda globalmente y no por modo
&#x200B;* [Modo de Haga un bake] Problema de visualización: normal promedio no cambia la superficie de la jaula
&#x200B;* [Gestión de color] La opción Detección automática del espacio de color se desactiva cuando OCIO env var está presente
&#x200B;* [Contenido] El filtro Contorno de máscara tiene un artefacto con la entrada de height
&#x200B;* [Contenido] El regulador de intensidad del filtro de desenfoque de Pendiente se fija en 1.0
&#x200B;* [Interop] No se puede crear el proyecto con GLTF de Sampler
&#x200B;* [Pila de capas] El valor del mosaico de proyección no se actualiza correctamente con manipulador
&#x200B;* [Linux] Desplazamiento entre el lápiz gráfico de la tableta y el cursor con HDPI superior al 100 %
&#x200B;* [Python] Bloqueo al volver a importar una malla después de crear un proyecto
&#x200B;* [Substance] Los ruidos 3D se rompen después de volver a importar una malla
&#x200B;* [Mosaicos de UV] El desplazamiento de la Proyección de UV se fija en 1
&#x200B;* [Ventana gráfica] Los comentarios visuales de líneas rectas ya no son visibles
&#x200B;* [WhatsNew] Retorno de línea incorrecto en títulos de funciones

<b>Problemas conocidos:</b>

&#x200B;* [Import] Algunos GLB con texturas no reciben texturas en Painter

### 8.3.0

*(Lanzado: 10 de enero de 2023)*
Resumen: <b>Versión principal con nuevo modo de hacer un bake, nueva importación y exportación de archivos USD y compatibilidad de tamaño físico para la Proyección de UV</b>

<b>Agregado:</b>

&#x200B;* [Modo de Hacer un bake] Nuevo modo de hacer un bake dedicado a hacer un bake el proceso
&#x200B;* [Modo de Hacer un bake] Definir el método abreviado para cambiar al modo de hacer un bake a F8
&#x200B;* [Modo de Haga un bake] Botón Añadir Inicio y Cancelar hacer un bake en la ventana gráfica
&#x200B;* [Modo de Hace un bake] Añadir selección de hace un bake en la lista Conjunto de texturas
&#x200B;* [Modo de Hace un bake] Añada una nueva ventana Bakeres de mapa de malla para seleccionar bakeres
&#x200B;* [Modo de Hace un bake] Añadir nueva ventana Ajustes de mapa de malla para editar los ajustes de hace un bake
&#x200B;* [Modo de Hace un bake] Añadir nueva ventana Hacer un bake registro para seguir el proceso de hace un bake
&#x200B;* [Modo de Hace un bake] Añadir parámetros de hace un bake y acciones de deshacer a la ventana de historial
&#x200B;* [Modo de Hace un bake] Añadir rutas de navegación en Ajustes de mapa de malla
&#x200B;* [Modo de Hace un bake] Añadir miniaturas de mapas de malla en la ventana Bakeres de mapas de malla
&#x200B;* [Modo de Haga un bake] Añadir menú de ajustes de visualización contraíbles en la ventana gráfica 3D
&#x200B;* [Modo de Hace un bake] Añadir ajuste de visualización para mostrar/ocultar la malla de alta densidad
&#x200B;* [Modo de Haga un bake] Añadir ajuste de visualización para mostrar/ocultar la malla de la jaula y la malla metálica
&#x200B;* [Modo de Hace un bake] Añadir ajuste de visualización para mostrar/ocultar la malla de baja densidad
&#x200B;* [Modo de Haga un bake] Añada ajustes de visualización para mostrar bordes duros sin costuras UV como errores
&#x200B;* [Modo de Hace un bake] Informar en la ventanilla sobre los errores de malla y hacer un bake si el registro de Hace un bake no está visible
&#x200B;* [Modo de Hace un bake] Añadir acción para sincronizar la configuración de baker en todos los conjuntos de texturas

  En la ventana Bakeres de mapa de malla, cada baker (así como los ajustes comunes) se pueden sincronizar en los conjuntos de texturas haciendo clic en el icono de enlace junto a su nombre. Esta acción abrirá una ventana que permite seleccionar qué conjuntos de texturas compartirán los mismos parámetros.

&#x200B;* [Modo de Hace un bake] Añadir acciones para copiar y pegar ajustes de baker

  En la ventana Bakeres de mapa de malla hay acciones disponibles para copiar y pegar cada configuración de baker en los conjuntos de texturas, ya sea a través del menú específico en la parte superior de la ventana o el menú contextual del botón derecho.

&#x200B;* [Modo de Haga un bake] Botón Añadir en Hacer un bake registro para saltar del error a la configuración correcta

  Cuando un baker falla o una malla no se carga correctamente, aparece un mensaje de error en el registro de Hace un bake. Un botón junto al mensaje permite cambiar la ventana Bakeres de mapa de malla y ajustes de mapa de malla para mostrar los ajustes relacionados. Esto ayuda a aislar con mayor facilidad el origen de un problema para poder solucionarlo.

&#x200B;* [Modo de Hace un bake] Añadir menús para gestionar conjuntos de texturas y selecciones de Bakeres

  En las ventanas &quot;Lista de conjuntos de texturas&quot; y &quot;Bakeres de mapa de malla&quot; se ha añadido un pequeño menú de acciones para ayudar a copiar e invertir las selecciones.

&#x200B;* [Modo de Hace un bake] Dividir la lista de selección de baker por conjunto de texturas
&#x200B;* [Modo de Hace un bake] Dividir ajustes comunes por conjunto de texturas
&#x200B;* [Modo de Haga un bake] Cargar mallas de alta poly y jaula sin congelar la interfaz
&#x200B;* [Modo de Hace un bake] Utilice la barra de progreso de la ventanilla para mostrar la carga de malla
&#x200B;* [Modo de Hace un bake] Añadir estado de carga de malla en Hacer un bake registro
&#x200B;* [Modo de Haga un bake] Permitir girar la malla en la ventana gráfica durante la hace un bake
&#x200B;* [Modo de Hace un bake] Establecer el orden de hace un bake en función de la visibilidad actual de la ventana gráfica de la malla
&#x200B;* [Modo de Haga un bake] Visualización de la jaula de haga un bake implícita en la ventana gráfica

  Si no se utiliza un fichero de malla de jaula personalizado, se generará una malla de jaula automática y se mostrará en la ventana gráfica. Su tamaño se basará en el parámetro Distancia frontal máxima de los ajustes comunes que se hacen un bake. La malla de la jaula se utiliza para indicar hasta dónde llegará la coincidencia entre el poli bajo y alto.

&#x200B;* [Modo de Hace un bake] Mostrar la lista de nombres de malla coincidentes para Coincidencia por nombre en Registro de Hace un bake
&#x200B;* [Modo de Haga un bake] Utilice material neutro para mostrar el modelo 3D en la ventana gráfica
&#x200B;* [Modo de Hace un bake] Desactivar el cálculo del motor mientras se está en modo de hace un bake
&#x200B;* [Modo de Haga un bake] Mostrar una advertencia al salir de la aplicación mientras hay un haga un bake en curso
&#x200B;* [Bakeres] Actualizar etiquetas de configuración de suavizado

  Los valores del ajuste de suavizado se han cambiado de nombre a &quot;Supersampling&quot; (Supermuestreo) y con un número multiplicador explícito para aclarar su comportamiento.

&#x200B;* [Baker] Actualice baker a la versión 2.5.7.
&#x200B;* [USD] Importar y exportar archivos de Universal Scene Description (USD)
&#x200B;* [USD] Agregar USD opciones a la ventana Nuevo proyecto al seleccionar un archivo de USD
&#x200B;* [USD] Ventana de selección Agregar nuevo ámbito y variantes

  Al importar un fichero de USD, pulsar en el botón de cambio de la ventana Nuevo proyecto o Configuración del proyecto permite seleccionar qué parte y variantes de un fichero de USD se van a importar.

&#x200B;* [USD] Opción Añadir niveles de subdivisión

  Al crear un nuevo proyecto con un archivo de malla de USD que contiene subdivisiones, es posible seleccionar el nivel de subdivisiones mediante un regulador. El proyecto se creará con la malla subdividida. El nivel se puede modificar mediante la configuración del proyecto.

&#x200B;* [USD] Importación USD mallas desolladas en marcos específicos

  Al crear un nuevo proyecto con un archivo de malla de USD que contiene animación, es posible seleccionar el marco mediante un regulador que refleje la secuencia de cronología incrustada. El marco se puede modificar mediante la configuración del proyecto.

&#x200B;* [USD]&#x200B;[Exportar] Añadir una opción para exportar archivos USD

  Nueva casilla de verificación Exportar USD añadida a la ventana Exportar texturas. Cuando está activada, permite exportar archivos USD, así como mapas de textura, utilizando cualquier plantilla.

&#x200B;* [USD]&#x200B;[Exportar] Agregar USD formato de archivo a la exportación de malla
&#x200B;* [USD] Cambie el nombre del ajuste preestablecido de exportación existente &quot;USD PBR Metal Roughness&quot; para que sea más explícito

  Se puede acceder a la plantilla de exportación de USD conocida anteriormente como &quot;Rugosidad del metal de USD PBR&quot; a través de texturas de exportación > Plantilla de salida > USDz (Apple AR).

&#x200B;* [Auto Unwrap] Añadir orientación de bloqueo para el empaquetado

  Nueva opción para la configuración de desajuste automático que permite conservar la orientación de las Islas de UV existentes al utilizar la función de empaquetado. Se puede acceder a él desde Nuevo proyecto > Opciones de Desenvolvimiento automático > Orientación de la Isla de UV.

&#x200B;* [Tamaño físico] Añada una configuración para utilizar automáticamente el Tamaño físico en el efecto de relleno/capa

  Se ha añadido una nueva opción para cambiar automáticamente a la escala de tamaño físico al utilizar un material con tamaño físico incorporado. Se puede activar por proyecto a través de Nuevo proyecto o a través de Editar > Configuración del proyecto > Tamaño físico > Cambiar la escala de la capa de relleno a Tamaño físico al asignar materiales.

&#x200B;* [Tamaño físico] Exponer tamaño físico para Proyección de UV

  La escala de tamaño físico ahora está disponible para las Proyecciones de UV: permite el cambio de tamaño automático para un material en función del tamaño físico de una malla. Se puede seleccionar a través de Escala > Tamaño físico en la ventana Propiedades de la capa de relleno o del efecto.

&#x200B;* [Scripting] [Python] Permitir consultar la versión de la aplicación
&#x200B;* [Scripting] [JavaScript] Actualizar la API para que coincida con los nuevos parámetros de hace un bake
&#x200B;* [Scripting] [Python] Haciendo un bake módulo: editar hacer un bake parámetros
&#x200B;* [Scripting] [Python] Haciendo un bake módulo: iniciar/cancelar hacer un bake
&#x200B;* [Scripting] [Python] Haciendo un bake módulo: seleccionar método de curvatura
&#x200B;* [Scripting] [Python] Haciendo un bake módulo: selección de bakeres/mosaicos uv
&#x200B;* [Scripting] [Python] Haciendo un bake módulo: sincronizar la configuración del baker en todos los conjuntos de texturas
&#x200B;* [SVT] Habilitar la compatibilidad de hardware disperso en las GPU AMD

  La aceleración de hardware para el sistema de texturas virtuales dispersas ahora se puede activar con las GPU AMD. Este ajuste se activa automáticamente en las preferencias generales.

&#x200B;* [Proyección] Cambiar nombre de parámetros de proyección cilíndrica

  El parámetro &quot;Cylinder Cap Culling&quot; ha pasado a denominarse &quot;Backface Culling&quot; para representar mejor su acción. La información sobre herramientas asociada se ha ajustado en consecuencia.

&#x200B;* [Project] Guarde la versión de la aplicación en el proyecto y recuperarla mediante scripts

  Desde la versión 8.2, la versión de la aplicación se almacena ahora dentro del archivo spp al guardar.
  Este número de versión se puede recuperar con la función last\_saved\_substance\_painter\_version() en el módulo de proyecto de la API de Python.
  Para un proyecto realizado antes de la versión 8.2, el valor devuelto será nulo.

&#x200B;* [Importar] Mejora el tiempo de importación general de modelos 3D

  Mejoramos el tiempo general de importación de mallas. Por ejemplo, reducir el tiempo de espera al cargar mallas de alto contenido de polietileno para hornear. Esta optimización se aplica en particular a la carga de archivos OBJ.

<b>Corregido:</b>

&#x200B;* [Bloqueo] Cambio de canales en el filtro con una pila específica
&#x200B;* [Mac]&#x200B;[M1] Bloqueo al crear una capa de relleno y salir de la pila de capas

  Este problema se puede solucionar actualizando a Mac OS 13 (Ventura).

&#x200B;* [Scripting]&#x200B;[Python] Bloqueo al utilizar ui.add\_dock\_widget() con un tipo incorrecto
&#x200B;* [Horneado] Mensaje de error incompleto en el registro cuando se produce un error en el horneado
&#x200B;* [Horneado] La memoria no se libera cuando finaliza el horneado
&#x200B;* [Motor] La caché de texturas no se actualiza al cambiar la visibilidad del efecto
&#x200B;* [Exportar] La vista 2D exporta un mapa aleatoriamente uniforme
&#x200B;* [Proyecto] Error de asignación de memoria al guardar el proyecto con malla grande
&#x200B;* [Ventana gráfica] El TAA provoca defectos al pintar en algunos casos

<b>Problemas conocidos:</b>

&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
&#x200B;* [Pila de capas] El origen de entrada no se guarda por capa

### 8.2.0

*(Lanzado: 6 de octubre de 2022)*
Resumen: **Versión principal con nuevos paneles de incorporación (nuevo panel de bienvenida y nuevo panel), exportación a SBSAR, efectos para carpetas, varias mejoras para la calidad de vida y correcciones de errores.**

**Agregado:**

&#x200B;* [Onboarding] Panel de incorporación para dar la bienvenida a nuevos usuarios

  Se ha añadido una nueva pantalla de bienvenida cuando los nuevos usuarios de CC abren Painter por primera vez.

&#x200B;* [Incorporación] Panel Novedades para mejorar la detección de nuevas funciones

  Se ha añadido una nueva pantalla Novedades que muestra las principales funciones nuevas. Se muestra automáticamente la primera vez que se abre Painter después de una actualización importante, y se puede volver a acceder a él a través de Ayuda > Novedades.

&#x200B;* [Onboarding] Cambiar el nombre de la versión antigua Bienvenido a la &quot;pantalla de inicio&quot;

  Se ha cambiado el nombre de la pantalla de bienvenida para evitar confusiones con la nueva pantalla de bienvenida.

&#x200B;* [UI] Resolver problemas de escalado de pantallas de alta resolución

  Se ha mejorado la adaptación de la interfaz de usuario de Painter en pantallas de alta definición con escala de visualización personalizada.

&#x200B;* [UI] Evite los mensajes de error persistentes en la IU

  Los mensajes de error de proyectos anteriores ahora se eliminan de la barra de estado inferior.

&#x200B;* [UI] Menú para guardar repeticiones

  Las opciones de guardado adicionales ahora se agrupan en un submenú y se cambia el nombre de algunas de ellas por coherencia.

&#x200B;* [IU] Guardar y exportar/compartir diseños de IU

  En el menú Ventana hay nuevas acciones para guardar el diseño de interfaz de usuario en archivos y volver a cargarlos. Los diseños de pintura y procesamiento se guardan por separado.
  Se han añadido varias funciones a &quot;substance\_painter.ui&quot; para guardar, restablecer y cargar diseños de interfaz de usuario también.

&#x200B;* Añadir acciones de copiar/pegar para los modos de fusión/opacidad de una capa

  Se ha añadido una nueva entrada &quot;Opciones de fusión&quot; en el menú contextual de las capas. Permite copiar y pegar el modo de fusión y la opacidad de todos los canales de una capa a otra.

&#x200B;* Aplicar el modo de fusión/opacidad a todos los canales de una capa

  Se ha añadido una funcionalidad de clic con el botón derecho al modo de fusión y la opacidad de las capas, lo que permite aplicar la configuración en la que se ha hecho clic a todos los canales.

&#x200B;* Volver a cargar la malla con un método abreviado de teclado (CTRL+MAYÚS+R)

  Se ha añadido un método abreviado editable para volver a cargar el archivo de malla con los últimos ajustes disponibles. También se puede acceder a través de Editar > Reimportar malla.

&#x200B;* Restablecer los parámetros del Substance a sus valores predeterminados

  Se ha añadido un nuevo botón en Propiedades en la parte inferior de los recursos .sbsar que permite restablecer el recurso a sus valores predeterminados.

&#x200B;* Restablecer el pincel de pintura a sus valores predeterminados

  Se ha añadido un nuevo menú a la sección Pincel en Propiedades que permite restablecer el pincel básico predeterminado.

&#x200B;* Haga clic con el botón derecho para restablecer los parámetros individuales del Substance a sus valores predeterminados

  Se ha añadido la posibilidad de restablecer parámetros individuales dentro de un recurso .sbsar haciendo clic con el botón derecho.

&#x200B;* [Panel Activos] Los activos favoritos del &quot;Pin&quot; aparecen en la parte superior del panel Activos

  Se ha añadido una nueva opción de clic con el botón derecho en los recursos de la biblioteca que permite pin como favoritos en la parte superior del panel. También puede ver todos sus activos favoritos a través de Búsquedas guardadas.

&#x200B;* [Panel Activos] Eliminar, volver a cargar y cambiar el nombre de los activos

  Se han añadido opciones de menú contextual para eliminar, volver a cargar y cambiar el nombre de los activos en la biblioteca del usuario. Se eliminan directamente de la ubicación de su biblioteca en el disco y se vuelven a cargar desde la ubicación original. Los activos que forman parte de un paquete como .abr o .sbsar no se pueden editar individualmente.

&#x200B;* [Selección de color] Añadir modos de fusión al efecto Selección de color
&#x200B;* [Pila de capas] Añadir modo de fusión y opacidad en los filtros
&#x200B;* [Pila de capas] Permitir valores de mosaico mayores que 128 para capas/efectos de relleno
&#x200B;* [Pila de capas] Tapones cilíndricos para proyección cilíndrica en capa de relleno/efecto

  La proyección cilíndrica en Propiedades de capa de relleno ahora tiene la opción de eliminar tapas de cilindro.

&#x200B;* [Log] Mostrar un mensaje de error si los elementos de malla están en espacio negativo al intentar crear un proyecto de Mosaico de UV

  Se ha añadido un mensaje de error más claro al no crear un proyecto de Mosaico de UV porque las partes UV se encuentran en espacios negativos.

&#x200B;* [Project] Indica la versión en el mensaje de error &quot;Datos demasiado recientes&quot; al abrir un proyecto

  Al abrir un proyecto que es demasiado reciente para la aplicación, el mensaje de error indicará ahora la versión del proyecto para que sea más fácil identificar la versión correcta de la aplicación.

&#x200B;* [Ventana gráfica] Permite iluminar la malla desde abajo

  Se ha añadido un nuevo parámetro Alineación del entorno en Configuración de la pantalla > Cámara > Configuración del entorno para alinear la iluminación del mapa de entorno con la cámara cuando se establece en &quot;Local&quot;.

&#x200B;* [Ventana gráfica] Ver R, G, B y Alpha en la ventana gráfica (modo de visualización individual)

  En Configuración de visualización > Configuración de ventana gráfica > Visualización de canal , hay un nuevo ajuste de Canales de color que solo permite mostrar el componente R, G, B o Alpha de un canal en el modo de visualización única.

&#x200B;* [Shader] Permite definir canales de usuario como RGBA en sombreadores de capas de material

  Al definir la configuración de canales del conjunto de texturas dentro de un sombreado para la capa de material, ahora es posible especificar el formato del canal que se va a desviar del valor predeterminado. Esto permite en particular solicitar canales de usuario de color en lugar de solo escala de grises.

&#x200B;* [Exportar] Permitir exportar texturas como SBSAR

  Al exportar texturas a través de la ventana Archivo > Exportar Texturas, se puede elegir el formato de archivo SBSAR (Archivo de Substance) para reagruparlas. El contenido de la SBSAR depende de la plantilla de salida utilizada.
  El formato de archivo SBSAR también se puede establecer en los ajustes preestablecidos de exportación. Cuando se utiliza una configuración híbrida (SBSAR + otro formato), las texturas que tienen como destino un SBSAR se agrupan mientras que el resto se exporta junto a ellas.

&#x200B;* [Exportar] Opción de exposición de 16 bits para EXR formato de archivo

  Al exportar archivos de textura de EXR, ahora es posible elegir 16f bit (medio Flotante) o 32f bit (Flotante) en la ventana Exportar Texturas (tanto para ajustes de exportación como para ajustes preestablecidos de exportación). Los proyectos antiguos y los ajustes preestablecidos de exportación antiguos se establecerán de forma predeterminada en 16f bit para reflejar el comportamiento antiguo.

&#x200B;* [Python] Añadir evento para saber cuándo se modifican los conjuntos de texturas

  El nuevo &quot;substance\_painter.event.TextureStateEvent&quot; permite saber cuándo se ha modificado un conjunto de texturas debido a un trazo de pintura, un nuevo canal añadido o un canal eliminado.

&#x200B;* [Python] Permitir obtener y establecer recursos de mapa de malla en los ajustes de Conjunto de texturas

  Se han añadido nuevas funciones en el módulo &quot;substance\_painter.project&quot; para obtener y definir recursos de mapas de malla. Estas funciones se pueden utilizar para actualizar los mapas de malla a los que hace referencia la configuración de Conjunto de texturas.

&#x200B;* [Plugins] Opción Eliminar para obtener otros plugins de JS

  Se ha eliminado la opción para obtener los complementos de JavaScript, ya que se alojaban en el sitio web obsoleto Compartir .

&#x200B;* [Contenido] Añadir nueva plantilla Roblox y exportar ajuste preestablecido

  Se han añadido una nueva plantilla de proyecto &quot;Material Variant&quot; y &quot;Surface Appearance&quot; de Roblox y un ajuste preestablecido de exportación para facilitar la exportación de texturas PBR a Roblox. Se puede acceder a la plantilla desde la ventana Archivo > Nuevo proyecto.

&#x200B;* Actualizar Substance Engine a la última versión (8.6.3)
&#x200B;* [Steam] Compilación optimizada para chipset Apple Silicon (Apple M1 / M2)

**Corregido:**

&#x200B;* Bloqueo al utilizar 16k exr
&#x200B;* [Bloqueo] Ctrl Z Después de eliminar una instancia del sombreador
&#x200B;* [Iray] El valor de IoR está bloqueado en 1 para algunos sombreadores
&#x200B;* [Win]&#x200B;[Haciendo un bake] No se pueden cargar algunos archivos de alta calidad
&#x200B;* [Gestión de color] Nombre de espacio de color incorrecto en la IU con filtros
&#x200B;* [Python] Los objetos de recursos devueltos por la función de importación no tienen un tipo

  Al importar un paquete de Substance en Python, la función devolvía el paquete en lugar de sus gráficos. El módulo de recursos ahora proporciona funciones y parámetros para recuperar los gráficos de un paquete de Substance.

**Problemas conocidos:**

&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
&#x200B;* [Pila de capas] El origen de entrada no se guarda por capa
&#x200B;* [Pintura] El suavizado temporal provoca defectos al pintar en algunos casos
&#x200B;* [Exportar] exportaciones de vista 2D mapa aleatoriamente uniforme

### 8.1.3

*(Lanzado: 25 de agosto de 2022)*
Resumen: **Versión secundaria de corrección de errores**

**Agregado:**

&#x200B;* Actualizar a Iray SDK 1.6

**Corregido:**

&#x200B;* [Sombreador] Bloqueo con sombreador defectuoso
&#x200B;* [Material Layering] Los materiales pueden desaparecer al reabrir un proyecto

**Problemas conocidos:**

&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción
&#x200B;* [Pila de capas] El origen de entrada no se guarda por capa
&#x200B;* [Bloqueo] Ctrl Z Después de eliminar una instancia de sombreado
&#x200B;* [Iray] El IoR está bloqueado a 1 para algunos sombreadores

### 8.1.2

*(Lanzado: 19 de julio de 2022)*
Resumen: **Versión secundaria de corrección de errores**

**Agregado:**

&#x200B;* [Auto Unwrap] Nueva opción &quot;Optimizar para mallas orgánicas&quot; para seleccionar el algoritmo de segmentación
&#x200B;* [Tamaño físico] Opciones de unidad de exposición en Nueva configuración de proyecto y proyecto
&#x200B;* [Gestión de color] Usar la visualización del monitor de forma predeterminada al utilizar ACE
&#x200B;* [Gestión de color] [Python] Tenga en cuenta el archivo de ajuste preestablecido ACE env-var al crear el proyecto
&#x200B;* [Gestión de color] Restablecer la configuración de Gestión de color en la ventana Nuevo proyecto cuando cambie la configuración
&#x200B;* [Gestión de color] Desactivar el acceso a la configuración de OCIO cuando env-var está presente
&#x200B;* [Gestión de color] Actualice de forma segura la configuración de ACE cuando ya no exista un parámetro
&#x200B;* Actualizar Substance Engine a la versión 8.6.0
&#x200B;* [Exportar] Añada un nuevo ajuste preestablecido de exportación GLTF compatible con Desplazamiento
&#x200B;* [Scripting] [Python] Recuperar información de recursos (incluidos metadatos personalizados)
&#x200B;* [Scripting] [Python] Añadir función a la lista de consulta de nombres de malla por conjunto de texturas
&#x200B;* [Contenido] Añade una nueva plantilla de Blender y exporta un ajuste preestablecido

**Corregido:**

&#x200B;* [MacOS] Bloqueo al iniciar Iray en algunos casos
&#x200B;* [Miniaturas] Las miniaturas de los estantes no se cargan correctamente
&#x200B;* Se omiten varios canales UV
&#x200B;* [Auto Unwrap] Cálculo innecesario al dividir islas largas
&#x200B;* [Auto Unwrap] Opción para evitar las islas alargadas no tomada en cuenta
&#x200B;* [Auto Unwrap] Pérdida de datos adicionales (colores de vértice) al reempaquetar UV
&#x200B;* [UI] Barra de desplazamiento horizontal en la ventana de propiedades cuando está activada la gestión de color
&#x200B;* [Gestión de color] Faltan configuraciones de OCIO substance\_3d\_painter\_standard\_srgb rol
&#x200B;* [Generator] Uso incorrecto de datos de usuario &quot;deshabilitado&quot;
&#x200B;* [Gestión de color] No se debe hacer clic en el menú desplegable Espacio de color no compatible
&#x200B;* [Gestión de color]&#x200B;[Sombreador] La anulación de sRGB definida ya no funciona
&#x200B;* [Generator] Uso incorrecto de los datos de usuario &quot;desactivar&quot;
&#x200B;* [Pila de capas] Vistas previas rotas en proyectos de Mosaico de UV
&#x200B;* [Sombreador] La documentación de la API no está completamente actualizada con Normales dobladas
&#x200B;* [Export]&#x200B;[Interoperability] No se puede enviar a Stager con caracteres especiales
&#x200B;* [Contenido] Algunas miniaturas de ajustes preestablecidos de pincel están vacías o son demasiado oscuras

**Problemas conocidos:**

&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
&#x200B;* [Pila de capas] Las fuentes de entrada no se guardan por capa
&#x200B;* [Bloqueo] Ctrl Z Después de eliminar una instancia del sombreador
&#x200B;* [Iray] El valor de IoR está bloqueado en 1 para algunos sombreadores
&#x200B;* [Sombreador] Bloqueo con sombreador defectuoso

### 8.1.1

*(Lanzado: 28 de junio de 2022)*
Resumen: **Revisión de versión secundaria**

**Agregado:**

&#x200B;* [Pila de capas] Pulsar Alt en la máscara ya no anula la selección de efectos

**Corregido:**

&#x200B;* [Bloqueo] Abrir un proyecto antiguo guardado en modo de vista en solitario
&#x200B;* [Bloqueo] Eliminar un generador en propiedades
&#x200B;* [Ajustes del conjunto de texturas] Se interrumpe la mezcla de Oclusión normal/ambiental y el height con los métodos normales
&#x200B;* [Exportar] La exportación de texturas mediante relleno de difusión produce mapas negros

**Problemas conocidos:**

&#x200B;* [MacOS] Bloqueo al iniciar Iray en Monterey
&#x200B;* [Vista previa en miniatura] Las miniaturas simplificadas no se actualizan cuando se utiliza un anclaje
&#x200B;* [Gestión de color] Las conversiones de espacio de color HDR con ACE en Linux producen colores con sujeción

### 8.1.0

*(Lanzado: 7 de junio de 2022)*
Resumen: **Versión principal compatible con ICC, escalado de materiales basado en datos de tamaño físico, nuevos panaderos, mejoras en el cuentagotas de color y una amplia gama de contenido adicional**

**Agregado:**

&#x200B;* [Gestión de color] Añadir compatibilidad con perfiles ICC mediante Adobe Color Engine (ACE)
&#x200B;* [Gestión de color] Añada compatibilidad con &quot;RGB de Adobe 98&quot; como espacio de color de trabajo para ICC
&#x200B;* [Gestión de color] Permitir la configuración de ACE/ICC mediante un archivo de configuración
&#x200B;* [Gestión de color] Permitir la entrada de valores de color lineal en el Selector de color con el modo Heredado
&#x200B;* [Gestión de color] Permite especificar el perfil de color utilizado para seleccionar el color fuera de la interfaz de usuario
&#x200B;* [Gestión de color] Recordar el último valor de visualización elegido en la ventana gráfica
&#x200B;* [Gestión de color] [Substance] Hacer que los generadores/filtros funcionen correctamente con la gestión de color
&#x200B;* [Gestión de color]&#x200B;[Substance] Añadir nuevas palabras clave de anulación de espacio de color $working y $standardsrgb
&#x200B;* [Tamaño físico] [Motor] Extraer información de tamaño físico de la malla
&#x200B;* [Tamaño físico] [Motor] Cálculo del Tamaño físico
&#x200B;* [Tamaño físico] Opciones de exposición para utilizar tamaño físico en la interfaz de usuario
&#x200B;* [Tamaño físico] Añadir ayudantes visuales en la ventana gráfica
&#x200B;* [Horneando] Añadir panadero de Height
&#x200B;* [Horneado] Añadir el panadero de normales dobladas
&#x200B;* [Horneado] Añadir el panadero de opacidad
&#x200B;* [Cuentagotas] Nueva previsualización del cuentagotas de color junto al ratón y gestión del color
&#x200B;* [Cuentagotas] El panel del selector de color vuelve a aparecer en su última posición cuando se vuelve a abrir
&#x200B;* [Cuentagotas] Un nuevo icono para el Selector de material
&#x200B;* [Cuentagotas] Color para administrar la vista previa del canal del selector de color
&#x200B;* [Cuentagotas] Añada la funcionalidad de hacer clic para seleccionar al cuentagotas
&#x200B;* [Cuentagotas] El selector de material ya no activa los canales no activos
&#x200B;* [Cuentagotas] Permitir el uso de cuentagotas con un método abreviado
&#x200B;* [Cuentagotas] El cuentagotas selecciona el canal correspondiente, cuando corresponde
&#x200B;* [Cuentagotas] Al entrar en el modo del selector de color se desactivan todos los métodos abreviados
&#x200B;* [Cuentagotas] Eliminación de la selección automática del campo hexadecimal
&#x200B;* [Cuentagotas] No cerrar el panel al utilizar el selector de material
&#x200B;* [Cuentagotas] Nuevo estado deshabilitado cuando el canal no está disponible para seleccionar
&#x200B;* [Export] Añadir atributo de tangente a la exportación glTF
&#x200B;* Actualizar Substance Engine a v8.4
&#x200B;* Actualizar Auto Unwrap a 0.9.0
&#x200B;* Actualizar a Qt 5.15.8
&#x200B;* Actualizar a Python 3.9
&#x200B;* [Sombreador] Añadir compatibilidad con el sombreado de Normales dobladas
&#x200B;* [MacOS] Compatibilidad con SpaceMouse de conexión 3D
&#x200B;* [Python] Documentar la versión de Python utilizada en la API
&#x200B;* [Contenido] Añade 6 nuevos sonidos 3D con 105 ajustes preestablecidos
&#x200B;* [Contenido] 20 nuevos mapas de suciedad y 2 patrones de pliegues de tela
&#x200B;* [Contenido] Actualizar el ajuste preestablecido &quot;Mapas de malla&quot; para utilizar nuevos bakeres
&#x200B;* [Contenido] La Pendiente de desenfoque y el filtro de deformación dependen de la resolución del conjunto de texturas
&#x200B;* [Contenido] Actualizar proyectos de muestra para utilizar los 3 nuevos bakeres

**Corregido:**

&#x200B;* [glTF] No se puede abrir glTF con un carácter especial
&#x200B;* [Motor] Artefactos con anisotropía y SVT desactivados
&#x200B;* [MacOS]&#x200B;[M1] Los Materiales inteligentes no se muestran correctamente
&#x200B;* [Procesamiento de malla] No se pueden importar mallas desde Modeler
&#x200B;* [UI] Barra de desplazamiento horizontal en la ventana de nuevo proyecto con la gestión de color habilitada
&#x200B;* [Gestión de color] Falta el valor del espacio de trabajo en el selector de color con algunas configuraciones de OCIO
&#x200B;* [Gestión de color] La previsualización del pincel en la ventana gráfica no tiene gestión de color
&#x200B;* [SpaceMouse] La tabla dinámica no se actualiza inmediatamente con el cambio de enfoque y, a veces, se sale del modelo
&#x200B;* [Exportar] [USD] Los archivos de USD exportados tienen una estructura incorrecta
&#x200B;* [USD] Problema de Oclusión ambiental al exportar
&#x200B;* [Contenido] Actualice la malla de la miniatura para que coincida con el proyecto de ejemplo Previsualizar esfera

**Problemas conocidos:**

&#x200B;* La exportación de texturas mediante relleno de difusión produce mapas negros
&#x200B;* La mezcla normal o de Oclusión ambiental no funciona
&#x200B;* [MacOS] Bloqueo al lanzar Iray en algunos casos raros
&#x200B;* [Vista previa en miniatura] Las miniaturas simplificadas no se actualizan cuando se utiliza un delimitador
&#x200B;* [Gestión de color] HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción

## Versión 7

### 7.4.3

*(Lanzado: 11 de abril de 2022)*
Resumen: **Corrección de error compatible con SpaceMouse de conexión 3D en la ventana gráfica 2D**

**Agregado:**

&#x200B;* [SpaceMouse] Compatibilidad con SpaceMouse de conexión 3D en la ventana gráfica 2D

**Corregido:**

&#x200B;* [Selector de color] No se puede escribir en campos hexadecimales
&#x200B;* [Gestión de color] Los recursos utilizados en el modo de proyección no se administran por color en la superposición
&#x200B;* [Gestión de color] No se notifican errores en el registro
&#x200B;* [SpaceMouse] Quitar mensaje de error genérico si el usuario no tiene un SpaceMouse
&#x200B;* [SpaceMouse] Al cargar un proyecto, el punto de giro siempre está oculto
&#x200B;* [Panaderos] El ajuste &quot;Normal promedio&quot; no tiene efecto en los proyectos de azulejo UV
&#x200B;* [Mosaico UV] Las superposiciones de mosaicos uv inactivos desaparecen al volver a cargar mallas con diferentes mosaicos
&#x200B;* [Scripting] [Python] La secuencia de comandos remota no funciona
&#x200B;* [Scripting] [Python] No se pueden consultar varios canales desde la API y se produce un error.
&#x200B;* [Scripting]&#x200B;[Python] Bloqueo al utilizar el evento ProjectEditionEntered
&#x200B;* [Scripting]&#x200B;[Python] Bloqueo al llamar a get\_active\_stack()

**Problemas conocidos:**

&#x200B;* Conexión 3D con SpaceMouse no compatible en MacOS
&#x200B;* [UI] Barra de desplazamiento horizontal con administración de color que aparece en algunos casos en la ventana de nuevo proyecto
&#x200B;* [Mac M1] Los materiales inteligentes no se muestran correctamente

### 7.4.2

*(Lanzado: 8 de marzo de 2022)*
Resumen: **Corrección de error compatible con SpaceMouse de conexión 3D y mejoras en la administración de color (OCIO)**

**Agregado:**

&#x200B;* [SpaceMouse] [Windows] Compatibilidad con la conexión 3D de SpaceMouse en el área de visualización 3D para la navegación
&#x200B;* [SpaceMouse] [Windows] Métodos abreviados/teclas básicos para los modelos Pro y Enterprise SpaceMouse en la ventana gráfica 3D
&#x200B;* [SpaceMouse] [Windows] Icono de centro de rotación dedicado en la ventana gráfica 3D
&#x200B;* [Gestión de color] Utilice las funciones de la configuración de OCIO para cambiar la configuración predeterminada
&#x200B;* [Gestión de color] Gestión de color de la ventana de propiedades para widgets de color
&#x200B;* [Gestión de color] Gestión de color de la ventana de propiedades para la previsualización de materiales
&#x200B;* [Gestión de color] Gestión de color de muestras en el selector de color
&#x200B;* [Gestión de color] Añadir un ajuste para definir el espacio de color sRGB estándar
&#x200B;* [Gestión de color] Añadir el espacio de color sRGB estándar desde la configuración de OCIO en el selector de color Lista de selectores de visualización
&#x200B;* [Gestión de color] Mejoras en el menú de anulación del espacio de color
&#x200B;* [Gestión de color] Permita anular el espacio de color del mapa de entorno en Ajustes de visualización.
&#x200B;* [Gestión de color] Dibujo de degradados del selector de color en función de la visualización actual
&#x200B;* [Gestión de color] Ajustar valores HDR. de forma predeterminada en el editor de color
&#x200B;* [Gestión de color] Usar passthrough (sin espacio de color) para filtros en modo heredado
&#x200B;* [Gestión de color] Limitar la visualización de degradados en el editor de color para que coincidan con el rango [0-1]
&#x200B;* [Gestión de color] Ocultar el selector de visualización en el selector de color en el modo Heredado
&#x200B;* [Administración de color] Convertir el campo hexadecimal del selector de color siempre en espacio de color sRGB
&#x200B;* [Gestión de color] Desactivar el menú desplegable de visualización del selector de color para canales de datos
&#x200B;* [Optimización] La cuadrícula de deformación vuelve a calcular únicamente los mosaicos UV cubiertos
&#x200B;* [Exportar] Permitir la exportación de proyectos de Mosaico de UV para Sketchfab, USD y glTF
&#x200B;* [Scripting]&#x200B;[Python] Permitir el cambio de la función de asignación de tonos

**Corregido:**

&#x200B;* [Sketchfab] Al actualizar el modelo existente, se crea un nuevo modelo
&#x200B;* [Sketchfab] Bloqueo al buscar un modelo actualizado anteriormente
&#x200B;* Bloqueo al exportar a USD
&#x200B;* Bloqueo al crear una nueva instancia del sombreador en Máscara de geometría o cuando la geometría está oculta
&#x200B;* [Ventana Importar recurso] Bloqueo al cambiar el tipo de recursos importados
&#x200B;* Los mapas de malla normales se invierten cuando se utilizan en la pila de capas
&#x200B;* [Substance] No se tiene en cuenta el modo de fusión de datos de usuarios
&#x200B;* [Gestión de color] Los mapas de bits con espacio de color en el nombre de archivo se importan como secuencias de Mosaico de UV
&#x200B;* [Gestión de color] Las salidas con gestión de color del gráfico del Substance están en un espacio de color incorrecto
&#x200B;* [Gestión de color] La herramienta Relleno poligonal muestra un color incorrecto
&#x200B;* [Gestión de color] ACE ajuste de tono se aplica a los canales en modo solo
&#x200B;* [Gestión de color] La previsualización de la iluminación de la esfera de la herramienta no está gestionada por color
&#x200B;* [Administración de color] [Exportar] Los mapas convertidos aplican una conversión incorrecta
&#x200B;* [Scripting]&#x200B;[Python]&#x200B;[Gestión de color] Los proyectos creados con plantillas y OCIO variables de entorno están en modo heredado
&#x200B;* [Scripting] [Python] No se puede utilizar la función de evaluación de JavaScript al inicio
&#x200B;* [Oferta de Adobe 3D] No se puede iniciar Painter si se utiliza la configuración regional con idiomas no admitidos de forma predeterminada

**Problemas conocidos:**

&#x200B;* Conexión 3D con SpaceMouse no compatible en MacOS
&#x200B;* [UI] Barra de desplazamiento horizontal con administración de color que aparece en algunos casos en la ventana de nuevo proyecto
&#x200B;* [Bakeres] El ajuste &quot;Normales medias&quot; no tiene efecto en los proyectos de Mosaico de UV
&#x200B;* [Mac M1] Los Materiales inteligentes no se muestran correctamente
&#x200B;* [Gestión de color] Los recursos utilizados en el modo de proyección no se administran por color en la superposición
&#x200B;* [Selector de color] No se puede escribir en campos hexadecimales

### 7.4.1

*(Lanzado: 14 de diciembre de 2021)*
Resumen: **Corrección de error con mejoras en la administración de color**

**Agregado:**

&#x200B;* [Gestión de color] Usar función de datos en nombres de archivo exportados
&#x200B;* [Administración de color] Expanda la sección Administración de color de forma predeterminada cuando se selecciona OCIO en las nuevas ventanas de configuración de proyecto y proyecto
&#x200B;* [Gestión de color] Añadir ACE asignador de tonos en modo heredado
&#x200B;* [Gestión de color] Ajustar los valores de configuración predeterminados
&#x200B;* [Gestión de color]&#x200B;[Exportar] Rellenar $colorSpace en nombres de archivo para canales de datos
&#x200B;* [Exportar] Exportar proyecto de Mosaico de UV a Stager
&#x200B;* [Interoperabilidad] No disponible para las ediciones Steam y Substance
&#x200B;* [Interoperabilidad] Permitir el envío de un proyecto de Mosaico de UV a Stager

**Corregido:**

&#x200B;* [MacOS] [Bloqueo] Painter no se inicia con Catalina
&#x200B;* [Gestión de color] [Bloqueo] bloqueo aleatorio al reproducir con gestión de color/tipo de datos en el canal del usuario
&#x200B;* [Gestión de color] Recursos utilizados como escala de grises en la máscara visualización del espacio de color nuevo menú
&#x200B;* [Gestión de color] El canal del usuario es más oscuro en la ventana gráfica en el modo heredado + vista en solitario
&#x200B;* [Gestión de color] El mapa Env siempre es lineal cuando se utiliza en iRay
&#x200B;* [Gestión de color] El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
&#x200B;* [Gestión de color] El selector de color se interrumpe en el interior de un Substance en modo heredado
&#x200B;* [Gestión de color] Al cambiar entre vistas de canal solo en la ventana gráfica, no se muestra con el espacio de color correcto al utilizar el menú desplegable
&#x200B;* [Gestión de color] La exportación aplica la conversión incorrecta en canales de usuario con gestión de color en modo heredado
&#x200B;* Los trazos realizados en la máscara de vista solo no se muestran al volver a la vista de material
&#x200B;* [Exportar] Los mapas convertidos no se exportan como canales con gestión de color
&#x200B;* [Conjunto de texturas] Falta la información sobre herramientas con el nombre original en los canales de usuario con nombre cambiado
&#x200B;* [Steam] Faltan archivos al comprobar su integridad con Steam

**Problemas conocidos:**

&#x200B;* [Mac M1] Los materiales inteligentes no se muestran correctamente

### 7.4.0

*(Lanzado: de noviembre de 2021)*
Resumen: **Versión principal. Introducción de la primera versión de la administración de color, desacoplar vista 2D o 3D, nueva opción de desempaquetado UV automático para evitar islas alargadas, llamar a funciones de JavaScript desde la API de Python y nuevo contenido**

**Agregado:**

&#x200B;* [Gestión de color] Compatibilidad con la gestión de color OpenColorIO versión 2
&#x200B;* [Gestión de color] Añadir ajustes de gestión de color a los ajustes del proyecto
&#x200B;* [Gestión de color] Ventana de advertencia sobre los cambios de configuración de la gestión de color al abrir un proyecto
&#x200B;* [Gestión de color] Mostrar un mensaje de error si se selecciona un archivo de configuración de OCIO no válido
&#x200B;* [Gestión de color] Permite anular la configuración con la variable de entorno OCIO
&#x200B;* [Gestión de color] Varias configuraciones OCIO integradas de forma predeterminada en la aplicación
&#x200B;* [Gestión de color] Extraer nombre de espacio de color del nombre de archivo de mapa de bits importado
&#x200B;* [Gestión de color] Permita anular el espacio de color con un espacio de color desde la configuración de la ventana Propiedades
&#x200B;* [Gestión de color] Añadir opciones de gestión de color en Configuración del conjunto de texturas
&#x200B;* [Gestión de color]&#x200B;[Ventana] Permitir la gestión de color de vistas 2D y 3D por separado
&#x200B;* [Gestión de color] Cargar y convertir mapa de entorno en el espacio de color de trabajo
&#x200B;* [Gestión de color] Ajuste el selector de color y el editor con el espacio de color actual
&#x200B;* [Gestión de color] Permite seleccionar la visualización transformar espacio de color en la ventana gráfica con un nuevo menú desplegable.
&#x200B;* [Gestión de color] Aplicación de visualización transformar con resultados de procesamiento de Iray
&#x200B;* [Gestión de color] Exportar texturas con diferentes espacios de color
&#x200B;* [Administración de color] [Python] Aplicación de la configuración de administración de color de la variable de entorno (OCIO) a proyectos nuevos
&#x200B;* [Ventana gráfica] Permite desacoplar la ventana gráfica 2D o 3D
&#x200B;* [Auto Unwrap] Nueva opción para evitar islas alargadas
&#x200B;* [Scripting Python] Llamar a funciones de JavaScript desde la API de Python
&#x200B;* [Nueva ventana de proyecto] Hacer que la sección de mapas importados sea contraíble
&#x200B;* [Proyección]&#x200B;[Deformar] Permite ocultar las normales como una opción en los ajustes de Deformación
&#x200B;* [Contenido] 11 nuevos mapas de suciedades
&#x200B;* [Contenido] 8 nuevos ajustes preestablecidos de herramientas (cremallera, cordón de apriete, brillo)
&#x200B;* [Contenido] 8 materiales nuevos (cicatriz, bolsillo, ...)
&#x200B;* [Contenido] 1 generador nuevo (inflar encogimiento)

**Problemas conocidos:**

&#x200B;* [Mac M1] Los Materiales inteligentes no se muestran correctamente
&#x200B;* [Gestión de color] [Bloqueo] bloqueo aleatorio al reproducir con gestión de color/tipo de datos en el canal del usuario
&#x200B;* [Gestión de color] El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
&#x200B;* [Gestión de color] [Iray] Guardar el renderizado en EXR o TIFF mientras la Gestión de color está activada en la ventana gráfica siempre se guarda en lineal
&#x200B;* [Administración de color] Los recursos utilizados como escala de grises en la máscara muestran un menú de espacio de color incorrecto
&#x200B;* [Gestión de color] [Iray] El mapa Env siempre es lineal cuando se usa en Iray
&#x200B;* [Gestión de color] [Exportar] Los mapas convertidos no se exportan como canales con gestión de color
&#x200B;* [Gestión de color] [Exportar] La exportación ignora si el canal del usuario tiene gestión de color o no está en modo heredado

### 7.3.1

*(Lanzado: de noviembre de 2021)*
Resumen: **Corrección de error**

**Agregado:**

&#x200B;* [Proyección] La escala solo debería funcionar en el espacio de objetos

**Corregido:**

&#x200B;* [Mac M1] Las capas de materiales no funcionan
&#x200B;* [Mac M1] [Proyección] La deformación no funciona
&#x200B;* Los detalles del micro no se muestran correctamente
&#x200B;* [Proyección] [Bloqueo] Cambio al modo de deformación con una capa creada con una versión anterior
&#x200B;* [Proyección] [Deformar] El giro no funciona cuando la transformación se establece en espacio de entorno
&#x200B;* [Proyección] [Deformar] La opción Dividir permanece seleccionada después de realizar la división
&#x200B;* [Proyección] [UV] El punto de giro se restablece al voltear la proyección
&#x200B;* [Filter] El entorno de Bake Lighting cambia al volver a cargar o cambiar un parámetro
&#x200B;* [Interoperabilidad] No disponible para las ediciones Steam y Substance
&#x200B;* [Interoperabilidad] El botón &quot;Examinar recursos 3D en el mercado&quot; siempre debe abrir el CCD en la pestaña 3D de Stock y Mercado

**Problemas conocidos:**

&#x200B;* [Mac M1] Los materiales inteligentes no se muestran correctamente

### 7.3.0

*(Lanzado: 13 de octubre de 2021)*
Resumen: **Versión principal. Contiene una nueva proyección de deformación 3D, una nueva proyección cilíndrica, mejoras del selector de color, nuevas funciones en la API de Python y correcciones de errores**

**Agregado:**

&#x200B;* [Proyección] [Deformar] Exponer deformación 3D como un nuevo modo de proyección
&#x200B;* [Proyección] [Deformar] Permitir el modo de pegatina para Alpha, texturas y procedimientos con la función de arrastrar y soltar en la ventana gráfica
&#x200B;* [Proyección] [Deformar] Utilice la proyección de deformación con el método abreviado de pegatina (ALT)
&#x200B;* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Transformar la deformación como completa o por vértices
&#x200B;* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Añadir puntos de cuadrícula con opciones de deformación dividida en sentido cruzado, horizontal o vertical
&#x200B;* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Menú específico para acciones de restablecimiento
&#x200B;* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Opción para ajustar automáticamente las tangentes al mover puntos
&#x200B;* [Proyección]&#x200B;[Deformar]&#x200B;[Barra de herramientas] Menú específico para la edición de la cuadrícula (tamaño, restablecimiento, color y tamaño del control)
&#x200B;* [Proyección] [Deformar] Nuevo método abreviado de teclado para cambiar el modo de edición de deformación de vértices completos (MAYÚS+V)
&#x200B;* [Proyección] [Deformar] Al pulsar+Ctrl se puede cambiar entre la herramienta Superficie y otras herramientas
&#x200B;* [Proyección] [Cilíndrica] Exponer el modo de proyección cilíndrica
&#x200B;* [Proyección]&#x200B;[Barra de herramientas] Ajustes del manipulador de grupo (tamaño, pasos de cuadrícula, pasos de ángulo)
&#x200B;* [Selector de color] Nueva interfaz de usuario del selector de color
&#x200B;* [Selector de color] Uso de valores sRGB en widgets de selector de color
&#x200B;* [Selector de color] Permitir guardar y eliminar muestras de color
&#x200B;* [Selector de color] Cuentagotas accesible desde las ranuras normales y de color
&#x200B;* [Selector de color] Permite editar colores dinámicos entre 0 y 255 valores
&#x200B;* [Selector de color] Hacer que el estado de HSV/RGB sea común en toda la aplicación
&#x200B;* [Selector de color] La ventana del selector de color es semipersistente
&#x200B;* [Selector de color] Al pulsar Esc se cierra la ventana del selector de color
&#x200B;* Mejora del rendimiento para la interacción de la interfaz de usuario y la pintura
&#x200B;* [Motor] Actualización a la nueva versión del motor de Substance (8.3.0)
&#x200B;* [Scripting] [Python] Permite volver a cargar la malla del proyecto actual
&#x200B;* [Scripting] [Python] Permitir la actualización de recursos en proyectos
&#x200B;* [Scripting] [Python] Permite establecer y consultar la resolución de Mosaicos de UV
&#x200B;* [Interoperabilidad] No disponible para las ediciones Steam y Substance
&#x200B;* [Interoperabilidad] Recibir varios recursos de Bridge

**Corregido:**

&#x200B;* El selector de color no muestra el color correcto
&#x200B;* [Horneado] La lista de conjuntos de texturas no está ordenada correctamente
&#x200B;* [Importación FBX] No se tienen en cuenta las transformaciones de pivote de grupo 3ds Max
&#x200B;* [Substance Engine] Bloqueo al importar SBSAR dañado
&#x200B;* [MacOS] La opción de configuración de proyecto en diferentes idiomas no está presente
&#x200B;* El guardado automático puede congelar Painter durante procesos largos

**Problemas conocidos:**

&#x200B;* [Proyección] [Deformar] La opción Dividir permanece seleccionada después de realizar la división
&#x200B;* [Proyección] [Deformar] El giro no funciona cuando la transformación se establece en espacio de entorno
&#x200B;* [Proyección] [Deformación] Líneas de artefactos entre parches en algunos casos raros
&#x200B;* [Proyección] [UV] El punto de giro se restablece al voltear la proyección
&#x200B;* [Mac M1] Los materiales inteligentes no se muestran correctamente
&#x200B;* [M1]&#x200B;[Regresión] Las capas de materiales no funcionan

### 7.2.3

*(Lanzado: 24 de agosto de 2021)*
Resumen: **Versión secundaria, corrección de errores**

**Agregado:**

&#x200B;* [Bibliotecas] Agregar una forma de excluir archivos no deseados del rastreo

**Corregido:**

&#x200B;* [Windows] Problemas de suspensión y varias pantallas
&#x200B;* [MacOS] [Bloqueo] Cambio del sombreado al utilizar efectos
&#x200B;* [Ventana gráfica] El modo de previsualización completa ya no muestra el cursor del pincel sin alfa
&#x200B;* [UI] El widget de ángulo gira en la dirección equivocada
&#x200B;* [Pila de capas] Muchas subcarpetas crean bloqueos muy largos
&#x200B;* [Iray] Diferentes puntos de vista en Iray y OpenGL: Visible si no funciona
&#x200B;* [Iray] El índice de refracción no se tiene en cuenta y no aparece en las propiedades de mdl
&#x200B;* [JavaScript] ShowExportDialog() nunca devuelve true
&#x200B;* No se puede leer mtl desde Adobe Stock

### 7.2.2

*(Lanzado: 27 de julio de 2021)*
Resumen: **Versión secundaria, corrección de errores**

**Agregado:**

&#x200B;* Actualizar la versión de requisitos de controlador AMD

**Corregido:**

&#x200B;* [Mac M1] Detección de memoria incorrecta
&#x200B;* [Exportar] Los trazados muy largos no se muestran correctamente

**Problemas conocidos:**

&#x200B;* [Contenido] Sombreadores obsoletos de las muestras

### 7.2.1

*(Lanzado: 2 de julio de 2021)*
Resumen: **Versión secundaria, revisión**

**Agregado:**

&#x200B;* [Interop] Añada información sobre herramientas para indicar que el envío de proyectos de Mosaico de UV a Stager aún no se admite
&#x200B;* [Plugin]&#x200B;[UI] Actualización del icono de Livelink

**Corregido:**

&#x200B;* [Nvidia] La versión del controlador que comienza por 30 se considera obsoleta
&#x200B;* [Bibliotecas] El estado del panel Activos no se guarda a menos que esté abierto un proyecto
&#x200B;* [Bibliotecas] La nueva búsqueda guardada conserva la palabra clave de la antigua búsqueda guardada
&#x200B;* [Baker] [UVTiles] Los mapas de ID por meshID también tienen en cuenta los Mosaicos de UV
&#x200B;* [Exportar] Los archivos gLTF no importan el color del vértice
&#x200B;* [Iray] Faltan algunas sugerencias
&#x200B;* [Interop] Enviar a Stager no siempre está desactivado cuando Stager no se detecta
&#x200B;* [Resource Updater] No se puede actualizar el fabricante de pinceles de Photoshop
&#x200B;* [Contenido] Generador de desgaste de borde de fibra de vidrio roto

### 7.2.0

*(Lanzado: 23 de junio de 2021)*
Resumen: **Versión principal: proporciona una actualización del panel de recursos, un nuevo sombreador con acceso a nuevos canales y parámetros, una actualización general de la interfaz de usuario, algunas mejoras de rendimiento muy solicitadas, compatibilidad con más idiomas y mucho más.**

**Agregado:**

&#x200B;* [Bibliotecas] Nuevo panel Activos para sustituir el estante
&#x200B;* [Bibliotecas]&#x200B;[IU] Nuevo diseño del panel Activos
&#x200B;* [Bibliotecas]&#x200B;[IU] Cambiar la orientación y la interfaz de usuario predeterminadas del panel Activos
&#x200B;* [Bibliotecas]&#x200B;[IU] Introducir una opción de vista de lista en la biblioteca
&#x200B;* [Bibliotecas] [IU] Nueva navegación de rutas de navegación en el panel Activos
&#x200B;* [Bibliotecas]&#x200B;[UI] Seleccione &quot;Todas las bibliotecas&quot; al seleccionar una búsqueda guardada
&#x200B;* [Bibliotecas] [IU] Seleccione &quot;Todas las bibliotecas&quot; cuando se anule la selección de todas las carpetas
&#x200B;* [Bibliotecas]&#x200B;[IU] Nueva etiqueta para pinceles de partículas
&#x200B;* [Bibliotecas] [IU] Se ha sustituido &quot;estantería&quot; por &quot;Todas las bibliotecas&quot; en la aplicación.
&#x200B;* [Bibliotecas]&#x200B;[IU] Permitir ocultar carpetas vacías
&#x200B;* [Bibliotecas]&#x200B;[UI] La biblioteca de usuario predeterminada debe estar visible aunque esté vacía.
&#x200B;* [Bibliotecas]&#x200B;[IU] Nuevo método de filtrado mediante iconos de tipos de activos
&#x200B;* [Bibliotecas] Método abreviado &quot;CTRL&quot; para seleccionar varios tipos de recursos
&#x200B;* [Bibliotecas] Nueva variable de entorno para controlar el presupuesto de memoria de previsualización de activos
&#x200B;* [Bibliotecas]&#x200B;[Contenido] Nuevos mapas de entorno
&#x200B;* [Bibliotecas]&#x200B;[Contenido]&#x200B;[IU] desplazamiento de procesamiento en los materiales predeterminados
&#x200B;* [Bibliotecas]&#x200B;[Contenido] Establezca sombreador de Adobe Standard Material (ASM) como predeterminado para la generación de vistas previas
&#x200B;* [Bibliotecas]&#x200B;[Contenido]&#x200B;[ASM] Nuevas plantillas de proyecto para el nuevo sombreador de ASM
&#x200B;* [Bibliotecas]&#x200B;[Miniatura] Usar nuevo mapa de entorno de Studio 6
&#x200B;* [Bibliotecas]&#x200B;[Miniatura] Lea la miniatura del recurso en lugar de generarla
&#x200B;* [Bibliotecas]&#x200B;[Miniatura] Añadir desplazamiento a la generación de miniaturas
&#x200B;* [Ajustes del conjunto de texturas]
&#x200B;* [Ajustes del conjunto de texturas]&#x200B;[IU] Exponer el nuevo height al método de conversión normal
&#x200B;* [Ajustes del conjunto de texturas] [IU] Reorganización de la IU de los canales
&#x200B;* [Ajustes del conjunto de texturas] El límite de canales de usuario se eleva a 16 canales
&#x200B;* [Ajustes del conjunto de texturas] [IU] Indica qué canales son compatibles con el sombreado seleccionado actualmente
&#x200B;* [Shader]&#x200B;[ASM] Nuevo sombreador de Adobe Standard Material
&#x200B;* [Shader] [ASM] Se ha agregado compatibilidad con Anisotropía, capa transparente, dispersión subsuperficial, Specular edge color y brillo
&#x200B;* [Shader]&#x200B;[ASM] Cambiar los valores de color de los canales predeterminados
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Export] Plantilla de exportación actualizada de Adobe Dimension a Adobe Substance 3D Stager
&#x200B;* [Shader] [ASM] Se han añadido etiquetas y sugerencias de herramientas para los parámetros de sombreado y MDL
&#x200B;* [Shader]&#x200B;[ASM] Haga visible el color de la Dispersión en la vista 2D aunque no se admita SSS
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Iray] Se admite el sombreado de ASM en Iray con el nuevo MDL.
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Iray] Dispersión subsuperficial actualizada en brillo y revestimiento de especificaciones PBR heredadas
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Content] Se ha cambiado el tipo de SSS predeterminado para las muestras.
&#x200B;* [Shader]&#x200B;[ASM] Se ha añadido documentación para la API de ASM
&#x200B;* [Shader]&#x200B;[ASM] Optimizar sombreadores para ignorar los canales no utilizados
&#x200B;* [Shader] Exponer nuevos canales de conjunto de texturas
&#x200B;* [Shader] Dispersión subsuperficial mejorada
&#x200B;* [Shader] Se han ocultado nuevos parámetros de sombreado para algunos sombreadores.
&#x200B;* [Shader] Visible si para parámetros de sombreado
&#x200B;* [Rendimiento]
&#x200B;* [Bibliotecas] Mejoras en el tiempo de carga y el rendimiento de cálculo de la vista previa de recursos
&#x200B;* [Motor] Mejoras en el rendimiento de pintura
&#x200B;* [Auto Unwrap]
&#x200B;* [Auto Unwrap] Mejoras en el rendimiento del Empaquetado
&#x200B;* [Auto Unwrap] Auto unwrap compatible con el flujo de trabajo de Mosaico de UV
&#x200B;* [Desenvolvimiento automático] Nueva opción para colocar los UV según la orientación de la malla
&#x200B;* [Otros]
&#x200B;* [Configuración] Se ha cambiado la dirección de zoom predeterminada
&#x200B;* [UI] Actualización general de la IU
&#x200B;* [UI] Repaso del menú Ayuda
&#x200B;* [UI] Reemplazar el icono de inversión
&#x200B;* [UI]&#x200B;[Complemento] Icono Reemplazar para el vínculo de dcc del complemento
&#x200B;* [UI]&#x200B;[AMD] Mensaje emergente y versión mínima requerida de actualización
&#x200B;* [Pila de capas] Crear una nueva capa dentro de la carpeta vacía seleccionada
&#x200B;* Actualizar documentación de Python
&#x200B;* [Marca]
&#x200B;* [Branding]&#x200B;[UI] Se ha actualizado el nombre de la aplicación a Adobe Substance 3D Painter.
&#x200B;* [Marca]&#x200B;[IU] Se ha actualizado la versión independiente a &#39;Edición de Substance&#39;
&#x200B;* [Marca]&#x200B;[IU] Se ha actualizado el nombre del ejecutable de la aplicación, la ruta de instalación, el paquete y los iconos
&#x200B;* [Branding]&#x200B;[UI] Se ha cambiado el nombre de la biblioteca y la ruta predeterminadas
&#x200B;* [Branding]&#x200B;[UI] Acerca de la ventana
&#x200B;* [Branding]&#x200B;[UI] Pantalla de bienvenida actualizada
&#x200B;* [Marca]&#x200B;[IU] Se ha eliminado el número de versión anual
&#x200B;* [Localización] Nuevas traducciones en alemán, francés y chino simplificado
&#x200B;* [Interoperabilidad] No disponible para las ediciones Steam y Substance
&#x200B;* Interoperabilidad con el ecosistema de Adobe: Designer, Sampler, Stager y Bridge
&#x200B;* [Interoperabilidad] [IU] Recibir y actualizar recursos de Designer
&#x200B;* [Interoperabilidad] [IU] Recibir recursos de Sampler
&#x200B;* [Interoperabilidad]&#x200B;[IU] Enviar el recurso a Stager
&#x200B;* [Interoperabilidad]&#x200B;[IU] Mostrar en Adobe Bridge
&#x200B;* [Interoperabilidad]&#x200B;[IU] Permitir el acceso rápido a Adobe 3D Assets
&#x200B;* [Interoperabilidad] Nuevas etiquetas de uso de sbsar
&#x200B;* [Interoperabilidad] Gestionar tipos de activos recibidos
&#x200B;* [Interoperabilidad] Los recursos recibidos de Adobe Substance 3D Designer o Adobe Substance 3D Sampler se almacenan en la biblioteca predeterminada elegida por el usuario
&#x200B;* [Interoperabilidad]&#x200B;[UI] Nuevo icono en la barra de herramientas de la izquierda para enviar a Stager o Photoshop

**Corregido:**

&#x200B;* [Tablet] Bajo rendimiento al pintar con presión
&#x200B;* [Tablet] Problema en tabletas con controles deslizantes
&#x200B;* [Bloqueo] El nombre no coincide entre la lista de conjuntos de texturas y el exportador
&#x200B;* [Bloqueo] [Bibliotecas] Haga doble clic en una subbiblioteca
&#x200B;* [Bibliotecas] Problema al rastrear directorios de bibliotecas
&#x200B;* [Bibliotecas] La línea de comandos de generación de vista previa forzada no funciona del modo esperado
&#x200B;* [Bibliotecas]&#x200B;[Contenido] El filtro Entorno de luz horneada está en negro de forma predeterminada
&#x200B;* [Linux]&#x200B;[MacOS]&#x200B;[Export Mesh] No se puede importar glTF creado en Linux/MacOS
&#x200B;* [Linux] Arrastrar y soltar un archivo en el panel Activos puede provocar un bloqueo
&#x200B;* [Auto-Unwrap] Auto-Unwrap está disponible incluso si no se ha seleccionado una malla para recargar
&#x200B;* Comportamiento incorrecto de las partículas con la gravedad
&#x200B;* [Pila de capas] El histograma de niveles solo puede utilizar Luminancia con algunos canales
&#x200B;* [Máscara de geometría] El menú contextual de una carpeta al editar la máscara de geometría no funciona
&#x200B;* [Proyección] Costura con proyección esférica y filtrado bilineal
&#x200B;* [UV Tiles] Exportar máscara a archivo solo exporta el mosaico 0, 0
&#x200B;* [Exportar malla] La exportación de malla FBX está vacía
&#x200B;* [Iray] El mapa normal no se tiene en cuenta en los nuevos proyectos al procesar
&#x200B;* [Guardar] Guardar problemas en unidades compartidas
&#x200B;* [Horneado] Al volver a hornear una malla con parámetros modificados, se muestra una advertencia
&#x200B;* [Horneado] [Regresión] Resultado incorrecto cuando el cuadro delimitador global de mallas de poli altas no incluye el origen de la escena
&#x200B;* [Python] Las bibliotecas de usuarios personalizados no se tienen en cuenta

**Problemas conocidos:**

&#x200B;* [Bibliotecas] Las búsquedas guardadas no se guardan si no hay ningún proyecto abierto
&#x200B;* [NVIDIA] Mensaje para el controlador obsoleto incluso si el controlador está actualizado

### 7.1.1 (2021.1.1)

*(Lanzado: de marzo de 2021)*
Resumen: **Versión secundaria, corrección de errores con posibilidad de introducir valores hexadecimales en el selector de color**

**Agregado:**

&#x200B;* [Log] Advertencia a los usuarios sobre los controladores de GPU AMD incompatibles
&#x200B;* [Selector de color] Permita escribir valores hexadecimales

**Corregido:**

&#x200B;* [Baker] Disminución del rendimiento
&#x200B;* [Máscara de geometría] Pulsar Alt en el nombre de la malla puede provocar un bloqueo
&#x200B;* [Motor] La pintura no actualiza toda la vista cuando es necesario
&#x200B;* [Pila de capas] La selección se bloquea tras cambiar el sombreado
&#x200B;* [MacOS] [Selector de color] El color es ligeramente diferente del que se ha seleccionado
&#x200B;* [Export] El uso del formato de archivo de PSD no genera un archivo por Mosaico de UV
&#x200B;* [Scripting]&#x200B;[Javascript] alg.mapexport.getPathsExportDocumentMaps() no devuelve todos los valores
&#x200B;* [Scripting] [Python] Los complementos deshabilitados se vuelven a habilitar al volver a abrir Painter

### 7.1.0 (2021.1.0)

*(Lanzado: de enero de 2021)*
Resumen: **Versión principal, nueva máscara de geometría que permite seleccionar y pintar partes de la geometría, copiar y pegar efectos en la pila de capas, mejorar el flujo de trabajo del azulejo UV, actualizar Iray, Bakers, Substance Engine y nuevo contenido**

**Agregado:**

&#x200B;* Nueva máscara de geometría y pinte las partes seleccionadas de la geometría
&#x200B;* [Máscara de geometría] Permite pintar las partes seleccionadas de la geometría por nombres de malla
&#x200B;* [Geometry Mask] Selección rectangular en ambas ventanas gráficas
&#x200B;* [Máscara de geometría] Permite ocultar/ignorar la geometría excluida en cualquier capa
&#x200B;* [Máscara de geometría]&#x200B;[Propiedades] Selección rápida de casillas de verificación al hacer clic y arrastrar
&#x200B;* [Geometry Mask]&#x200B;[Properties]&#x200B;[UI] Include/Exclude all con un menú desplegable en la ventana Propiedades
&#x200B;* [Máscara de geometría]&#x200B;[Propiedades] Permite seleccionar rápidamente un elemento de una lista con ALT+CLIC IZQUIERDO
&#x200B;* [Máscara de geometría]&#x200B;[Propiedades] Superposición en las ventanas gráficas al pasar el cursor por los nombres/Mosaicos de UV de malla en la ventana Propiedades
&#x200B;* [Máscara de geometría] [Pila de capas] Añadir opciones de Copiar/Pegar a la máscara de geometría
&#x200B;* [Máscara de geometría] Nuevo icono para el botón Ocultar/ignorar geometría excluida
&#x200B;* [Máscara de geometría] Nueva información sobre herramientas para Ocultar/ignorar geometría excluida
&#x200B;* [Máscara de geometría] Método abreviado de teclado ALT + H para activar o desactivar el botón &quot;Ocultar geometría excluida&quot;.
&#x200B;* [UV Tiles] [Layer Stack] Nueva miniatura de vista previa de la esfera de capa de relleno para UV Tiles y modo simplificado
&#x200B;* [Mosaicos de UV]&#x200B;[Pila de capas] Permite salir fácilmente de la máscara de Mosaico de UV
&#x200B;* [Mosaicos UV]&#x200B;[Lista de conjuntos de texturas] Permite proporcionar una descripción por mosaico UV
&#x200B;* [UV Tiles]&#x200B;[Texture Set Settings]&#x200B;[UI] Dos nuevos títulos de sección en el menú desplegable para cambiar la resolución del azulejo UV
&#x200B;* [Mosaicos de UV] [Ventana gráfica] Salir de la máscara de Mosaico de UV al arrastrar un material a la ventana gráfica
&#x200B;* [Pila de capas] Añadir opciones de Copiar/Pegar para efectos
&#x200B;* [Pila de capas] Permite copiar y pegar efectos de un conjunto de texturas a otro
&#x200B;* [Pila de capas] Permitir selección múltiple de efectos
&#x200B;* [Pila de capas] Añadir opciones de copiar y pegar como métodos abreviados de efectos de capa
&#x200B;* [Pila de capas] Cambiar automáticamente entre máscara y contenido al arrastrar efectos a otra capa
&#x200B;* [Pila de capas] Crea automáticamente una máscara al pegar una máscara de otra capa
&#x200B;* [Pila de capas] Añada acciones de mover efectos dentro del menú contextual del botón derecho de los efectos
&#x200B;* [Pila de capas] Permite arrastrar y soltar efectos de una capa a otra
&#x200B;* [Pila de capas] Al arrastrar elementos a una carpeta, se colocan en la parte superior de la carpeta
&#x200B;* Actualizar Iray a la versión 2020.1.0
&#x200B;* [Bakers] Actualice Bakers a la versión 2.5.4
&#x200B;* [Bakeres] Mostrar Mosaicos de UV individuales en la ventana de progreso de hacer un bake
&#x200B;* [Bakers]&#x200B;[UI] Permite hornear rápidamente el conjunto de texturas actual con un nuevo botón
&#x200B;* [Panaderos] Permite al usuario seleccionar rápidamente uno de los panaderos con ALT+CLIC IZQUIERDO
&#x200B;* Actualizar Substance Engine a la versión 8.0.8
&#x200B;* [Substance Engine] Compatibilidad con el color predeterminado en los nuevos archivos .sbsar
&#x200B;* [Auto Unwrap] Mejora del rendimiento
&#x200B;* [Exportar] Añada comentarios visuales para indicar qué resolución del azulejo UV difiere de la predeterminada del proyecto
&#x200B;* [Exportar] Añada el factor de tamaño de escena al archivo json de sombreado exportado
&#x200B;* [Idioma] Añadir traducción al japonés
&#x200B;* [UI] Ventana Actualización Acerca de con control de versiones de dependencias internas
&#x200B;* [Scripting]&#x200B;[Python] Permita administrar recursos de Shelf
&#x200B;* [Scripting] [Python] Permite saber cuándo un proyecto está listo para su procesamiento y exportación
&#x200B;* [Scripting] [Python] Permite saber cuándo un Shelf ha terminado de rastrear recursos en el disco
&#x200B;* [Scripting] [Python] Permite consultar la lista de mosaicos UV por conjuntos de texturas
&#x200B;* [Scripts] [Python] Permite asignar una vista previa personalizada a los recursos de la estantería
&#x200B;* [Scripting] [Python] Permita administrar estantes personalizados
&#x200B;* [Scripting] [Python] Agregue un índice de método en cada submódulo de la documentación
&#x200B;* [Scripting] [Python] Nuevo estilo para la documentación
&#x200B;* [Scripting] [Python] Mejora de los recursos y de la documentación de la estantería
&#x200B;* [Contenido] Tres nuevos ajustes preestablecidos de herramientas para realizar puntos de sutura
&#x200B;* [Estante] Quitar temporalmente &quot;Exportar a Substance share&quot; al realizar la transición a la nueva plataforma de Substance share

**Corregido:**

&#x200B;* Bloqueo al utilizar monitores con diferentes resoluciones
&#x200B;* Bloqueo en Substance Engine con algunos proyectos raros
&#x200B;* La actualización de la ventana gráfica falla con Ocultar/Ignorar geometría excluida al cambiar de capa
&#x200B;* [vista 2D] Puede que falte la ventana gráfica 2D en algunos proyectos
&#x200B;* [Haciendo un bake] &quot;Coincidir por nombre de malla&quot; ignora partes del objeto
&#x200B;* [Pila de capas] Hacer clic en un efecto de capa abre una carpeta
&#x200B;* El Mosaico de UV [Máscara de geometría] se sigue contando en la máscara incluso al volver a importar la malla sin ella
&#x200B;* [Máscara de geometría] El menú contextual de la ventana gráfica no proporciona las herramientas correctas
&#x200B;* [Motor] Grandes retrasos en proyectos concretos
&#x200B;* [Scripting] Alta latencia con solicitudes remotas de POST JSON en Windows
&#x200B;* [Linux] La cantidad de Vram no se detecta correctamente con GPU integradas específicas
&#x200B;* [Auto Unwrap] Bloqueos o desempaquetado prolongado en algunos proyectos

## Versión 6

### 6.2.2 (2020.2.2)

*(Lanzado: de septiembre de 2020)*
Resumen: **Versión secundaria, corrección de errores con algunas funciones en la API de Python**

**Agregado:**

&#x200B;* [Rendimiento] No calcular todos los Mosaicos de UV al utilizar la selección de ID de color
&#x200B;* [Bakeres]&#x200B;[IU] Visualización de descripciones de conjuntos de texturas
&#x200B;* [Bakeres] Permitir guardar la configuración de hacer un bake
&#x200B;* [Bakeres] Añada las opciones contraer todo/expandir todo a la pestaña Selección
&#x200B;* [Lista de conjuntos de texturas] Ocultar descripción cuando está vacía
&#x200B;* [Mosaicos de UV]&#x200B;[Lista de conjuntos de texturas] Al hacer clic en el Mosaico de UV, se expande o se contrae la lista.
&#x200B;* [Export]&#x200B;[UI] Permite cambiar el tamaño horizontal del panel Lista de conjuntos de texturas
&#x200B;* [Exportar] [IU] Texto de información sobre herramientas coherente para el flujo de trabajo de Mosaicos de UV y Conjunto de texturas con texturas no seleccionadas
&#x200B;* [Scripting] [Python] Permitir el uso de ajustes preestablecidos de exportación para exportar texturas
&#x200B;* [Scripting] [Python] Añadir un registro de cambios en la documentación
&#x200B;* [Scripting] [Python] Permite consultar todos los canales disponibles en una pila determinada
&#x200B;* [Scripting] [Python] Mejoras en la IU de la consola

**Corregido:**

&#x200B;* [AMD] Detección incorrecta de la versión obsoleta del controlador
&#x200B;* Bloqueo al volver a importar una malla con un diseño de Mosaicos de UV diferente en algunos casos
&#x200B;* Bloqueo al utilizar partículas con UDIM en mallas muy pesadas
&#x200B;* [UV Tiles] Bloqueo al exportar una malla con información de desplazamiento en algunos casos
&#x200B;* [Exportar] [Bloqueo] Exportar una vista 2D en formato psd puede producir un bloqueo
&#x200B;* Importar imágenes como secuencias al crear un proyecto no funciona
&#x200B;* Motor atascado en un bucle infinito
&#x200B;* [Acceso directo] La cámara gira siempre en modo de ajuste al cambiar los métodos abreviados de modo de ajuste
&#x200B;* Las mallas siempre se desenvuelven automáticamente cuando se vuelven a importar aunque la opción esté desactivada
&#x200B;* [Lista de conjuntos de texturas] En ocasiones, el campo de texto Descripción no está totalmente visible durante la edición
&#x200B;* [Lista de conjuntos de texturas] El menú desplegable para ocultar/mostrar conjuntos de texturas no está completamente visible
&#x200B;* [Lista de conjuntos de texturas] Al hacer clic en el icono del ojo no se debe introducir el nombre &quot;Editar conjunto de texturas&quot;
&#x200B;* [Ajustes del conjunto de texturas] Al quitar un canal, también se elimina el canal siguiente
&#x200B;* [Exportar] Incluir todo y Restablecer todo no tiene en cuenta los mosaicos UV
&#x200B;* [Panaderos] Durante el proceso de cocción aparecen panaderos no seleccionados
&#x200B;* La actualización de la resolución no se tiene en cuenta para los mapas con bake utilizados como entrada
&#x200B;* [Mosaicos UV] [Ventana gráfica] La ventana gráfica 3D se bloquea al añadir material inteligente tras una carpeta con la máscara de mosaico UV seleccionada
&#x200B;* [Mosaicos UV] [Ventana gráfica] La Malla metálica sigue siendo visible para los mosaicos ocultos con el modo de pintar
&#x200B;* [Exportar] [Sketchfab] Problemas con el tipo de suscripción &quot;más&quot;
&#x200B;* [Sketchfab] La casilla &quot;Este recurso es privado&quot; no se muestra después de cambiar de cuenta
&#x200B;* [Exportar] [Contenido] Los ajustes preestablecidos de pincel &quot;ondulante&quot; pueden provocar problemas de rendimiento
&#x200B;* [Plugin Photoshop] Mensaje en el registro: no compatible con el flujo de trabajo de azulejo UV
&#x200B;* [Scripting]&#x200B;[Python] PYTHONPATH env var impide que se inicie la aplicación
&#x200B;* [Scripting] [Python] Error tipográfico en la documentación de Python

### 6.2.1 (2020.2.1)

*(Lanzado: 29 de julio de 2020)*
Resumen: **Versión secundaria, revisión**

**Agregado:**

&#x200B;* Añada la variable de entorno &quot;SUBSTANCE\_PAINTER\_VRAM\_BUDGET&quot; para anular la cantidad de GPU VRam
&#x200B;* [Mosaicos de UV]&#x200B;[Rendimiento] No calcular todos los mosaicos UV al utilizar la herramienta Relleno poligonal

**Corregido:**

&#x200B;* [Iray] Guardar renderizado devuelve un error que genera una imagen en negro
&#x200B;* [Linux] Bloqueo después de la pantalla de bienvenida en CentOS 7.3
&#x200B;* [Linux] La cantidad de Vram no se detecta correctamente con configuraciones específicas
&#x200B;* [Bloqueo] Apertura de un proyecto con el nombre de un conjunto de texturas duplicado
&#x200B;* [Motor] Problema de invalidación de caché al modificar una máscara
&#x200B;* [Lista de conjuntos de texturas] Efecto de fuente incorrecto al desactivar Conjunto de texturas

**Problemas conocidos:**

&#x200B;* [Texture Set List] No se puede ocultar la descripción
&#x200B;* [Lista de conjuntos de texturas] Problemas de IU
&#x200B;* [Iray] El procesamiento de PSD no se abre
&#x200B;* [Plugin de Photoshop] No compatible con el flujo de trabajo de Mosaicos de UV

### 6.2.0 (2020.2.0)

*(Lanzado: 23 de julio de 2020)*
Resumen: **Versión principal con nuevo flujo de trabajo de Mosaicos de UV, pintura entre Mosaicos de UV y mejora del rendimiento**

**Agregado:**

&#x200B;* Mosaicos de UV (UDIM)
&#x200B;* [Mosaicos de UV] Pintura en mosaicos UV
&#x200B;* [Mosaicos de UV] Permite elegir entre el flujo de trabajo nuevo y el heredado para Mosaicos de UV.
&#x200B;* [Mosaicos de UV] Importación de UDIM/secuencias de imágenes de Mosaico de UV como recurso
&#x200B;* [Mosaicos de UV] Añadir lista de Mosaicos de UV por conjunto de texturas en la ventana Lista de conjuntos de texturas
&#x200B;* [Mosaicos de UV] Permite editar la resolución de varios Mosaicos de UV a la vez en Ajustes de conjunto de texturas.
&#x200B;* [Mosaicos de UV]&#x200B;[vista 2D] Mostrar Mosaicos de UV como una cuadrícula
&#x200B;* [Mosaicos de UV]&#x200B;[vista 2D] Botón Nueva ventana para mostrar u ocultar información de Mosaicos de UV
&#x200B;* [Mosaicos de UV] Cambiar la herramienta de pintura a un solo canal de forma predeterminada para proyectos de Mosaico de UV
&#x200B;* [Mosaicos de UV] Botón nuevo en la barra de herramientas contextual para ignorar los Mosaicos de UV enmascarados mientras se pinta
&#x200B;* [Mosaicos de UV]&#x200B;[Pila de capas] Nuevos iconos de pila de capas para mejorar el rendimiento
&#x200B;* [Mosaicos de UV] [Pila de capas] Mejora de los iconos de Pintura y relleno en la barra de herramientas
&#x200B;* [Máscara de Mosaico de UV]&#x200B;[vista 2D] Permite incluir o excluir varios Mosaicos de UV a la vez (clic izquierdo, CTRL+clic izquierdo)
&#x200B;* [Máscara de Mosaico de UV] Nueva máscara de Mosaico de UV para incluir, excluir azulejos por capa con un nuevo icono
&#x200B;* [Máscara de Mosaico de UV] [Pila de capas] Mostrar el número de Mosaicos de UV en el icono de máscara de Mosaicos de UV cuando no se incluyen todos
&#x200B;* [Máscara de Mosaico de UV] [2D/Vista 3D] Añade el efecto de pasar por encima para visualizar los Mosaicos de UV bajo el cursor
&#x200B;* [Mosaicos de UV]&#x200B;[Bakeres] Permite seleccionar y hacer un bake Mosaicos de UV específicos
&#x200B;* [Mosaicos de UV]&#x200B;[Bakeres] Añadir opciones de selección para conjuntos de texturas/Mosaicos de UV
&#x200B;* [Mosaicos de UV] [Bakeres] Haga clic con el botón derecho en la opción de menú para seleccionar Mosaicos de UV dentro de un conjunto de texturas
&#x200B;* [Mosaicos de UV] [Bakeres] Permite una selección rápida en el conjunto de texturas/Mosaicos de UV arrastrando
&#x200B;* [Mosaicos de UV] [Bakeres] Reemplace los botones &quot;Todo&quot; y &quot;Ninguno&quot; en Mapas de malla por opciones de selección más explícitas
&#x200B;* [Mosaicos de UV]&#x200B;[Bakeres] Mostrar el número de texturas que se van a hacer un bake
&#x200B;* [Mosaicos de UV]&#x200B;[Exportar] Permitir la selección y exportación de Mosaicos de UV específicos
&#x200B;* [Mosaicos de UV] [Exportar] Permite una selección rápida de Mosaicos de UV arrastrándolos
&#x200B;* [Mosaicos de UV] [Exportar] Añadir opciones del menú desplegable para Mosaicos de UV
&#x200B;* [Mosaicos de UV] [Exportar] Hacer que algunos ajustes preestablecidos de exportación no estén disponibles si no funcionan con Mosaicos de UV (Adobe Dimension, Sketchfab, glTF, USD)
&#x200B;* [Mosaicos de UV]&#x200B;[Contenido] Actualice los ajustes preestablecidos de exportación para utilizar la nueva etiqueta $udim
&#x200B;* [Mosaicos de UV] Mejora de los informes de errores al importar mallas con Islas de UV superpuestas
&#x200B;* [Mosaicos de UV] Mosaicos de UV compatibles en Irak
&#x200B;* [UV Tiles]&#x200B;[Scripting] Añadir documentación de exportación de UV Tile a Python doc
&#x200B;* Rendimiento
&#x200B;* [Rendimiento] Botón nuevo en la barra de herramientas contextual para pausar el cálculo del motor al trabajar (MAYÚS+ESC)
&#x200B;* [Rendimiento] Apertura más rápida de proyectos al retrasar el cálculo de la caché del conjunto de texturas
&#x200B;* [Rendimiento] No espere a que se carguen los mapas de malla al abrir el proyecto
&#x200B;* [Rendimiento]&#x200B;[Vista 2D/3D] No calcular el canal de máscara en la ventana gráfica cuando no se utiliza
&#x200B;* [Rendimiento] No bloquee la aplicación al cargar los mapas de malla mostrados en las ventanas gráficas
&#x200B;* [Rendimiento] Mejora la velocidad de guardado incremental al guardar un proyecto
&#x200B;* [Rendimiento]&#x200B;[Bakeres] Cambie la configuración de dilatación predeterminada para ahorrar tiempo y mejorar el tamaño del proyecto
&#x200B;* [Rendimiento] [Panaderos] Cambie a escala de grises en Panaderos específicos para ahorrar tiempo y mejorar el tamaño del proyecto
&#x200B;* [Rendimiento]&#x200B;[Exportar] Mejorar el rendimiento del motor para exportar texturas más rápido
&#x200B;* [Rendimiento] [Exportar] Mejore la capacidad de respuesta al abrir el cuadro de diálogo de exportación con muchos conjuntos de texturas
&#x200B;* [Rendimiento]&#x200B;[Exportar] Mejorar el rendimiento al cambiar a la ficha &quot;Lista de exportaciones&quot;
&#x200B;* [Rendimiento]&#x200B;[Iray] Reducir el tiempo de inicio de Iray
&#x200B;* Otro
&#x200B;* [Bakers] Añadir opciones de selección para conjuntos de texturas
&#x200B;* Mover la administración de instancias del sombreador a la configuración del conjunto de texturas
&#x200B;* [Vista 2D/3D] Añada un mensaje en la parte inferior de la ventana gráfica para indicar qué tipo de máscara se ha editado
&#x200B;* [Pila de capas] Nueva opción en la configuración para cambiar entre las miniaturas nuevas y heredadas
&#x200B;* [Pila de capas] Añada comentarios visuales para indicar el estado de carga de las miniaturas
&#x200B;* [Proj] Nuevo modo de proyección &quot;Fill (Match Per UV-Tile)&quot; para cargar secuencias de imágenes
&#x200B;* [Proj] Cambie el modo de proyección de capas de relleno a &quot;Rellenar (coincidencia por mosaico UV)&quot; en casos específicos
&#x200B;* [Contenido] Optimización de los ajustes preestablecidos de pincel de carboncillo para mejorar el rendimiento
&#x200B;* Actualizar Iray a la versión 2020.0.0
&#x200B;* [Exportar] Desactive la ficha Lista de exportaciones si no hay nada seleccionado
&#x200B;* Desempaquetado automático
&#x200B;* [Auto Unwrap] Mejora la tasa de éxito del proceso de desajuste automático
&#x200B;* [Auto Unwrap] Parametrización mejorada para aumentar la velocidad y la estabilidad

**Corregido:**

&#x200B;* [Alembic] Las facetas se omiten al importar archivos
&#x200B;* [Alembic] Tiempo de carga infinito con archivos específicos
&#x200B;* [Import] Se importa una secuencia de imágenes de UDIM incorrecta cuando solo difiere la extensión del archivo
&#x200B;* [Bloqueo] Al intentar abrir un proyecto bloqueado por otro proceso, se produce un bloqueo
&#x200B;* [Proyección] Artefactos en malla duplicada al utilizar proyección triplanar
&#x200B;* [Exportar] El canal de Emisivo no se exporta con USD formato
&#x200B;* [Contenido] El Material inteligente &quot;Carboncillo&quot; contiene trazos de pintura

**Problemas conocidos:**

&#x200B;* [Texture Set List] No se puede ocultar la descripción
&#x200B;* [Lista de conjuntos de texturas] Problemas de IU

### 6.1.3 (2020.1.3)

*(Lanzado: 16 de junio de 2020)*
Resumen: **Corrección de error**

**Agregado:**

&#x200B;* [Exportar] Añadir ajustes de desplazamiento en el archivo json de parámetros de Sombreador

**Corregido:**

&#x200B;* bloqueo [Bloqueo] [Motor] al intentar borrar y sustituir canales existentes
&#x200B;* [Bloqueo] Cambio de sombreador después de pintar una máscara en capas de material
&#x200B;* [Bloqueo] [Motor] Bloqueos con algunos proyectos pesados
&#x200B;* [Bakeres] La coincidencia por nombre no funciona con OBJ exportados desde zBrush
&#x200B;* Las Texturas [Desplazamiento] [SVT] no se muestran al abrir el proyecto cuando el desplazamiento está activado
&#x200B;* [Exportar] Algunas texturas se exportan en gris uniforme
&#x200B;* [Exportar] Los conjuntos de texturas desactivados no se deben exportar para los ajustes preestablecidos de exportación de Dimension y Sketchfab
&#x200B;* [Scripting]&#x200B;[JavaScript] Bloqueo al utilizar la API JavaScript para acceder a la configuración de exportación en el evento onProjectOpened
&#x200B;* No se llama a [Scripting]&#x200B;[Javascript] onExportFinished() después de una exportación

### 6.1.2 (2020.1.2)

*(Lanzado: 28 de mayo de 2020)*
Resumen: **Corrección de error con la actualización de Substance Engine y Bakers**

**Agregado:**

&#x200B;* [Baker] Actualice a la versión más reciente
&#x200B;* [Panaderos] Nuevo método de muestreo en Oclusión ambiental, curvatura, panaderos de Thickness
&#x200B;* Actualizar a la versión más reciente de Substance Engine
&#x200B;* [Scripting]&#x200B;[Python] Permite la creación de ResourceID para los recursos del proyecto
&#x200B;* [Scripting]&#x200B;[Python] Permitir consultar información del canal
&#x200B;* [Scripting] [Python] Adición de funciones de ejecución en seco y devolución de llamada para simular la exportación de texturas

**Corregido:**

&#x200B;* [Panaderos] Normales incorrectas en el Panadero de Normales Espaciales Mundiales usando un mapa Normal tangente en casos específicos
&#x200B;* [Bakeres] Error al hacer un bake la Oclusión ambiental con Optix cuando no hay poli alta
&#x200B;* [Trazos dinámicos] Retraso al cargar un conjunto de texturas específico
&#x200B;* [Export] No se deben exportar los conjuntos de texturas desactivados para USD, glTF
&#x200B;* [Scripting] [JavaScript] No se puede editar la nueva configuración del panadero de curvatura
&#x200B;* [Scripting]&#x200B;[JavaScript] alg.texturesets.addChannel() no devuelve un error en algunos casos
&#x200B;* [Scripting] [JavaScript] Error tipográfico en la documentación de la API de Javascript para setProjectExportOptions()
&#x200B;* [Scripting] [JavaScript] Exporta siempre todos los conjuntos de texturas
&#x200B;* [Scripting]&#x200B;[Python] sys.ejecutable devuelve una ruta de acceso a python.exe en lugar de Substance Painter
&#x200B;* La caché de textura no es compatible en los sistemas operativos Mac y Windows/Linux
&#x200B;* [Livelink UE4] Solo se usa el último material para todos los conjuntos de texturas en una malla combinada

**Problemas conocidos:**

&#x200B;* [Export]&#x200B;[Dimension]&#x200B;[Skecthfab] No se deben exportar los conjuntos de texturas desactivados
&#x200B;* [Bloqueo] Cambiar el sombreador después de haber pintado una máscara en capas de material

### 6.1.1 (2020.1.1)

*(Lanzado: 5 de mayo de 2020)*
Resumen: **Revisión**

**Agregado:**

&#x200B;* [Export] Comentarios visuales de estado anulado en TextureSet

**Corregido:**

&#x200B;* [Exportar] El tamaño de la ventana del Exportador es demasiado grande en un monitor con resolución especial y no se puede cambiar de tamaño
&#x200B;* [Exportar] Las opciones no se guardan después de la exportación
&#x200B;* [Exportar] Bloqueo o no se puede exportar con el ajuste preestablecido exportar &quot;desde caché&quot;
&#x200B;* [Exportar] Al cancelar la exportación, se genera un mapa vacío adicional inesperado
&#x200B;* [Exportar] Corregir ajustes preestablecidos de exportación virtual
&#x200B;* [Python] PYTHONPATH env var no se tiene en cuenta
&#x200B;* [Python] [Exportar] Si se cancela la exportación mediante Python, se devuelve un error de excepción
&#x200B;* [Python]&#x200B;[Export] export\_project\_texturas resultado incorrecto con formato de archivo psd
&#x200B;* [Bakeres] Bloqueo en Linux con Trazado de rayos de GPU

**Problemas conocidos:**

&#x200B;* [JavaScript] No se puede editar la nueva configuración del baker de curvatura
&#x200B;* [JavaScript] [Exportar] Exporta siempre todos los conjuntos de texturas
&#x200B;* [Export]&#x200B;[USD] No se deben exportar los conjuntos de texturas desactivados
&#x200B;* [Bloqueo] Cambiar el sombreador después de haber pintado una máscara en capas de material

### 6.1.0 (2020.1.0)

*(Lanzado: 22 de abril de 2020)*
Resumen: **Versión principal con nueva textura y exportador de malla (con desplazamiento y teselación), desempaquetado UV actualizado con más controles, nuevos bakeres, nueva API python de scripts, mejor experiencia de usuario para la proyección de pegatinas y nuevo contenido**

**Agregado:**

&#x200B;* Nueva textura y exportador de malla
&#x200B;* [Exportar] Nueva interfaz de exportador
&#x200B;* [Exportar] [ficha Exportar] Permite seleccionar qué canales de mapas se exportan por conjunto de texturas
&#x200B;* [Exportar] [ficha Exportar] Permite modificar el tamaño del conjunto de texturas para todos los conjuntos de texturas en una sola acción
&#x200B;* [Exportar] [Ficha Exportar] Permitir una plantilla diferente por conjunto de texturas (excepto USD, glTF, Sketchfab y Dimension)
&#x200B;* [Exportar] [Ficha Exportar] Activación y desactivación rápidas de mapas y conjuntos de texturas
&#x200B;* [Exportar] [Ficha Exportar] La resolución de exportación 8192x8192 ya no es experimental
&#x200B;* [Exportar] [ficha Exportar] Permite modificar el formato de archivo y la profundidad de bits por mapa
&#x200B;* [Exportar] [ficha Exportar] Permite restablecer los valores de los parámetros predeterminados
&#x200B;* [Exportar] [ficha Exportar] Permite guardar la configuración sin exportar
&#x200B;* [Exportar] [ficha Plantillas de salida] Cambie el nombre de la ficha &quot;Configuración&quot; a la ficha &quot;Plantillas de salida&quot;
&#x200B;* [Exportar] [ficha Plantillas de salida] Permite definir el formato de archivo y la profundidad de bits por mapa preestablecido
&#x200B;* [Exportar] [ficha Lista de exportaciones] Nueva ficha de vista previa para resumir y ver el proceso de exportación
&#x200B;* [Import/Export Mesh] Optimización del rendimiento del tiempo de importación/exportación
&#x200B;* [Exportar malla] Exportar malla en FBX
&#x200B;* [Exportar malla] Exportar malla con desplazamiento y teselación
&#x200B;* [Exportar malla] [IU] Nuevos ajustes para volver a calcular el vértice normal, aplicar triangulación
&#x200B;* [Exportar malla] Exportar topología de malla original con nuevas UV generadas por el desajuste automático
&#x200B;* Se ha actualizado el desajuste automático de UV con más controles
&#x200B;* [Desempaquetado UV]&#x200B;[UI] Añadir configuración para activar el desempaquetado UV automático en la ventana de nuevo proyecto
&#x200B;* [Desempaquetado UV]&#x200B;[UI] Nuevas opciones para controlar los pasos de desempaquetado (costuras, desempaquetado, empaquetado)
&#x200B;* [UV Unwrapping]&#x200B;[UI] Permitir la conservación de las costuras de desenvolvimiento existentes/desenvolvimiento/empaquetado
&#x200B;* [Desajuste UV]&#x200B;[UI] Nuevas opciones para volver a calcular completamente los pasos de desajuste
&#x200B;* [Desajuste UV]&#x200B;[UI] Nueva opción para controlar el tamaño del margen (ninguno, pequeño, mediano y grande)
&#x200B;* Nuevos Bakeres
&#x200B;* [Panaderos] Reemplace la curvatura antigua por la nueva curvatura de la malla
&#x200B;* [Panaderos] Añadir la opción de coincidencia por nombre para ignorar la cara posterior en el panadero de &quot;Oclusión ambiental&quot;
&#x200B;* [Bakeres] Opción Añadir plano de tierra en el baker &quot;Oclusión ambiental&quot;
&#x200B;* Nueva API de Python de scripts (3.7.6)
&#x200B;* [Python]&#x200B;[UI] Nuevo menú de scripts para Python
&#x200B;* [Python]&#x200B;[UI] Nueva documentación de Python en el menú Ayuda
&#x200B;* [Python] Exponer módulos de Python de Substance Painter: substance\_painter, alg, display, project.setting, project, texturesets, ui
&#x200B;* [Python] Exponer nuevo módulo Python &quot;substance\_painter&quot;
&#x200B;* [Python] Exponer nuevo submódulo de Python: alg, display, log, project, resource, texturesets, ui
&#x200B;* [Python] Listener para cambios de proyecto
&#x200B;* [Python] Nuevos ejemplos en la documentación de Python
&#x200B;* [JavaScript] [IU] Menú de complementos reemplazado por JavaScript
&#x200B;* [Ventana gráfica] Permite crear una proyección de pegatinas &quot;arrastrando/soltando + ALT&quot; de un recurso desde la estantería
&#x200B;* Nuevo contenido
&#x200B;* [Contenido] 5 nuevos materiales de pegatina de Substance Source
&#x200B;* [Contenido] Añadir nuevas plantillas de proyecto y ajustes preestablecidos de exportación para el procesador Maxwell
&#x200B;* [Contenido] Añadir plantilla de proyecto para la exportación de Keyshot 9
&#x200B;* [Contenido] Actualización del ajuste preestablecido de exportación de Keyshot 9 para admitir el desplazamiento y el emisivo
&#x200B;* [Contenido] [Exportador] Actualización de todos los ajustes preestablecidos de exportación para que coincidan con las últimas versiones de motores de juegos y procesadores
&#x200B;* [Contenido]&#x200B;[Exportador] Actualice los archivos de ajustes preestablecidos de exportación para utilizar el nuevo formato y la nueva configuración de tramado
&#x200B;* [Contenido] Nuevas plantillas y sombreadores para admitir material de VRay (VRayMtl)
&#x200B;* [Pila de capas] Permita la eliminación de efectos de capa mediante el icono de la papelera o el método abreviado del teclado Eliminar
&#x200B;* Eliminar el Substance Source de plugins (utilizar el iniciador con la funcionalidad &quot;enviar a&quot;)
&#x200B;* [Windows] No se muestra ninguna advertencia de TDR en las GPU de gama alta

**Corregido:**

&#x200B;* Problemas de traducción en el cuadro de diálogo Nuevo archivo de proyecto
&#x200B;* [Bakeres] La configuración &quot;Guardar archivo de escena preprocesado&quot; ya no funciona
&#x200B;* [Proyección plana] La proyección no funciona en mallas con UV repetidos
&#x200B;* [Decal] Diferencia de comportamiento en el canal normal al utilizar distintos modos de proyección de la capa de relleno
&#x200B;* [Difuminado] [Clonar] El artefacto puede aparecer al pintar en una máscara
&#x200B;* [Motor] Bloqueo con contenido de capa específico
&#x200B;* [Motor] Bloqueo aleatorio al pintar en algunos casos
&#x200B;* [Punto de anclaje] La referencia a una máscara vacía siempre devuelve blanco
&#x200B;* [Exportar] Capa no tenida en cuenta en algunas configuraciones de pila concretas
&#x200B;* [Exportar malla] No se puede exportar con una ruta que contenga caracteres especiales
&#x200B;* [Export Mesh] No se pueden leer archivos glTF al exportar desde Linux o MacOS
&#x200B;* [Importar malla] La reimportación de DAE, PLY o glTF no funciona según lo previsto

**Problemas conocidos:**

&#x200B;* [Scripting] [JavaScript] No se puede editar la nueva configuración del panadero de curvatura
&#x200B;* [Bakers] Bloqueo en Linux con Trazado de rayos de GPU
&#x200B;* [Export]&#x200B;[USD] No se deben exportar los conjuntos de texturas desactivados
&#x200B;* [Bloqueo] Cambiar sombreado después de pintar una máscara en capas de material

## Versión 5

### 5.3.3 (2019.3.3)

*(Lanzado: 6 de febrero de 2020)*
Resumen: **Corrección de error con actualización a Iray 2019.3**

**Agregado:**

&#x200B;* Actualización a Irak 2019.3
&#x200B;* [Log] Indicar bios obsoletos para la CPU Ryzen que conduce a un bloqueo durante el procesamiento
&#x200B;* [ABR] Extraer alfa de ABR al estante

**Corregido:**

&#x200B;* [Baker] La cocción falla si la malla High-poly no tiene UV
&#x200B;* [Linux] Los métodos abreviados de ratón personalizados no se guardan
&#x200B;* [Pincel] El contorno desaparece con algunas formas alfa
&#x200B;* [Tablet] Detección incorrecta al mover los reguladores
&#x200B;* [Accesos directos] No se puede configurar ningún acceso directo con &quot;Ctrl+Alt+Clic del ratón&quot;
&#x200B;* [Estante] No se ve información sobre herramientas de recursos al utilizar una tableta con lápiz
&#x200B;* [Vista 2D] [Exportar] El ajuste preestablecido de vista 2D no tiene en cuenta la información normal
&#x200B;* Bloqueo al pintar en alineación UV con determinados pinceles
&#x200B;* Pintar bajo un filtro crea artefactos en el trazo en curso
&#x200B;* [Ventana gráfica] Caché de textura incorrecta en la ventana gráfica después de volver a importar una malla
&#x200B;* [Bloqueo] Error al guardar después de exportar a Photoshop
&#x200B;* [Bloqueo] Escribir símbolos especiales en el prefijo al importar recursos
&#x200B;* [Bloqueo] Haga clic en la referencia en Propiedades de punto de anclaje
&#x200B;* [Puntos de anclaje] El canal no se actualiza cuando hay un filtro entre el punto de anclaje y la referencia
&#x200B;* El vínculo de la URL de Iray en el menú Ayuda no funciona

**Problemas conocidos:**

&#x200B;* [Desempaquetado de UV] El procesamiento de mallas de alto contenido de polietileno puede tardar mucho tiempo
&#x200B;* [Desempaquetado UV] Se combinan vértices en las mismas coordenadas exactas
&#x200B;* La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
&#x200B;* [Desempaquetado UV] Relación de textil no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
&#x200B;* [Desempaquetado UV] Relación de textura no uniforme entre conjuntos de texturas
&#x200B;* [Desempaquetado UV] La Isla de UV generada puede ser muy alargada y, en algunos casos, no cabe en el espacio UV
&#x200B;* [Desempaquetado de UV] Las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no pueden desenvolverse con UV

### 5.3.2 (2019.3.2)

*(Lanzado: de enero de 2020)*
Resumen: **Corrección de error**

**Corregido:**

&#x200B;* Al abrir un proyecto guardado en el modo de canal solo, no se muestra la malla
&#x200B;* La ventana gráfica no siempre se actualiza al pintar en una capa con la herramienta de clonación

**Problemas conocidos:**

&#x200B;* [Bakers] Bloqueo relacionado con subprocesos múltiples en CPU Ryzen
&#x200B;* [Desempaquetado de UV] El procesamiento de mallas de alto contenido de polietileno puede tardar mucho tiempo
&#x200B;* [Desempaquetado UV] Se combinan vértices en las mismas coordenadas exactas
&#x200B;* La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
&#x200B;* [Desempaquetado UV] Relación de textil no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
&#x200B;* [Desempaquetado UV] Relación de textura no uniforme entre conjuntos de texturas
&#x200B;* [Desempaquetado UV] La Isla de UV generada puede ser muy alargada y, en algunos casos, no cabe en el espacio UV
&#x200B;* [Desempaquetado de UV] Las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no pueden desenvolverse con UV

### 5.3.1 (2019.3.1)

*(Lanzado: de diciembre de 2019)*
Resumen: **Revisión**

**Corregido:**

&#x200B;* Bloqueo al trabajar en mallas con Proyecciones de UV específicas
&#x200B;* [ABR] Bloqueo al cambiar entre ajustes preestablecidos de Photoshop
&#x200B;* [Linux] No se puede iniciar Substance Painter en CentOS 7.4 debido a un problema de dependencia libGLX
&#x200B;* [Bakers] Bloqueo al realizar el procesamiento después de utilizar Archivo > Limpiar
&#x200B;* [Panaderos] El cuadro de diálogo Progreso de panificación se bloquea después de cancelar
&#x200B;* [Panaderos] La cocción de mallas después de exportar texturas no funciona
&#x200B;* [Panaderos] El uso de resultados de &quot;Coincidir por nombre&quot; con mapas de malla negros
&#x200B;* [Panaderos] No se tiene en cuenta la jaula
&#x200B;* [Shelf] La importación de archivos de PSD genera imágenes rotas
&#x200B;* [Muestra] El proyecto de muestra &quot;Mat&quot; tiene cámaras rotas y un ajuste preestablecido de exportación incorrecto

**Problemas conocidos:**

&#x200B;* [Bakers] Bloqueo relacionado con subprocesos múltiples en CPU Ryzen
&#x200B;* [Desempaquetado de UV] El procesamiento de mallas de alto contenido de polietileno puede tardar mucho tiempo
&#x200B;* [Desempaquetado UV] Se combinan vértices en las mismas coordenadas exactas
&#x200B;* La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
&#x200B;* [Desempaquetado UV] Relación de textil no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
&#x200B;* [Desempaquetado UV] Relación de textura no uniforme entre conjuntos de texturas
&#x200B;* [Desempaquetado UV] La Isla de UV generada puede ser muy alargada y, en algunos casos, no cabe en el espacio UV
&#x200B;* [Desempaquetado de UV] Las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no pueden desenvolverse con UV

### 5.3.0 (2019.3.0)

*(Lanzado: 17 de diciembre de 2019)*
Resumen: **Versión principal con mejora de la experiencia del usuario al pintar a mano, uso de tabletas, desempaquetado automático de UV en versión beta (0.3.0) y nuevo contenido diverso para pintar a mano**

**Agregado:**

&#x200B;* Integrar la versión 0.3.0 del desempaquetado automático de UV en Substance Painter
&#x200B;* [Desempaquetado de UV] Desempaquetado automático de UV en el Substance Painter cuando no hay UV o UV parciales
&#x200B;* [Desempaquetado UV] Una configuración global para activarla y desactivarla
&#x200B;* [Desempaquetado UV] Versión registrada en el archivo de registro
&#x200B;* [Desempaquetado UV]&#x200B;[IU] Indicar el progreso del desempaquetado UV
&#x200B;* [UI] Nuevos ajustes en la barra de herramientas contextual para seleccionar la vista previa del pincel: Vista previa completa, contorno de pincel y forma de cruz
&#x200B;* [Herramienta] Nuevo modo de fusión avanzado en la sección alfa: Aclarar (máximo) además de Normal
&#x200B;* [Pila de capas] Opción de corrección de gamma por capa para alfa o máscara (menú del botón derecho)
&#x200B;* [Pila de capas]&#x200B;[IU] Se añade el icono &quot;i&quot; cuando se corrige la gamma de una capa alfa
&#x200B;* [Tablet] [Herramienta] Exponer presión mínima para tamaño y flujo
&#x200B;* [Tablet]&#x200B;[UI] Nueva configuración en la barra de herramientas contextual para seleccionar la presión de curva: lineal, fácil de entrar, fácil de salir
&#x200B;* [Tablet]&#x200B;[UX] Pulse Ctrl+Alt y haga clic para desplazarse
&#x200B;* Importar ajustes preestablecidos de pincel de Photoshop (formato ABR)
&#x200B;* [ABR] Compatibilidad con parámetros de forma
&#x200B;* [ABR] Compatibilidad con parámetros de dinámica de forma
&#x200B;* [ABR] Parámetros de transferencia de soporte
&#x200B;* [ABR] Compatibilidad con parámetros de dispersión
&#x200B;* [ABR]&#x200B;[Trazos dinámicos] Compatibilidad con redondez y volteo
&#x200B;* [ABR]&#x200B;[Estante] Se muestra la estructura de carpetas del pincel en el Editor de filtros.
&#x200B;* [ABR]&#x200B;[Estante] Añadir icono de Photoshop en miniaturas
&#x200B;* [ABR]&#x200B;[Shelf] Añadir una lista de parámetros no admitidos en la miniatura detallada de ABR
&#x200B;* [Herramienta]&#x200B;[Trazos dinámicos] Nuevo ajuste de trazo dinámico para controlar cuántas semillas aleatorias se van a generar
&#x200B;* [Herramienta]&#x200B;[IU] Añadir nuevos ajustes de distribución y eje para la variación de dispersión
&#x200B;* [Método abreviado] Pulse Ctrl+Mayús+B para abrir la ventana que Hace un bake
&#x200B;* [UI]&#x200B;[Menu] Añadir entrada en el menú &quot;Editar&quot; para abrir la ventana Hornear
&#x200B;* [UI]&#x200B;[Configuración] Mejora de la alineación de la lista de métodos abreviados
&#x200B;* [UI] Reemplazar los controles de presión (tamaño y flujo) por botones de activación/desactivación
&#x200B;* [Ventana gráfica] Permite enfocar la ventana gráfica 2D y 3D por separado
&#x200B;* Actualización a QT 5.12.5
&#x200B;* [UI] Indicar el progreso de carga de malla
&#x200B;* [Substance] Añade compatibilidad con rangos suaves y no sujetos con reguladores
&#x200B;* [Substance] Aumentar la precisión de los parámetros del Substance hasta 6 decimales
&#x200B;* [Substance] Tenga en cuenta el paso definido por un parámetro
&#x200B;* [Substance] Optimizar la generación de trazos dinámicos con compatibilidad con condiciones en los datos de usuario
&#x200B;* [Substance] Permite designar una salida de gráfico como una máscara para todos los canales a través de los datos de usuario.
&#x200B;* [Contenido] Actualizar proyecto de muestra &quot;Mat&quot; con topología compatible con desplazamientos, nuevo mapa de ID y nuevas cámaras
&#x200B;* [Content] Integra 3 filtros nuevos (MatFx): Cómic, Acuarela, Pintura al óleo (inspirado en el trabajo de Cubukcu emrecano)
&#x200B;* [Contenido] Integrar 102 ajustes preestablecidos de pinceles de Photoshop de los paquetes de Kyle T. Webster
&#x200B;* [Contenido] Integrar 18 nuevos ajustes preestablecidos de pincel: Flecha de rodillo de pintura, texto de advertencia de rodillo de pintura, carboncillo fino y más
&#x200B;* [Contenido] Integrar 9 nuevos alfa: Rodillo de Pintura del creador de pinceles, Photoshop del creador de pinceles, patrones de pinceles y mucho más
&#x200B;* [Contenido] Integra 2 nuevos ajustes preestablecidos de herramientas: Gouache denso y Gouache descolorido
&#x200B;* [Content] Integrar 1 nuevo generador: Comprobador UV (Islas de UV de realce y costuras)
&#x200B;* [Contenido] Integrar 2 nuevos ajustes preestablecidos de exportación: Keyshot 9+ y Spark AR Studio
&#x200B;* [Contenido] Integra 1 nueva plantilla de proyecto : Spark AR Studio (Facebook)

**Corregido:**

&#x200B;* [Tablet] Al deshacer trazos de lápiz (Ctrl+Z) se produce un retraso mayor que al deshacer trazos del ratón
&#x200B;* [Tablet] La presión inicial y final no se tiene en cuenta al dibujar una línea recta
&#x200B;* [Tablet] El primer sello se dibuja dos veces cuando se usa una línea recta
&#x200B;* [Tablet] Mejorar la compatibilidad con los métodos abreviados de la tableta Huion
&#x200B;* [Tablet] Mejorar la compatibilidad con los botones del lápiz Huion
&#x200B;* [Tablet] Desplazamiento entre la vista previa del pincel y el sello dibujado
&#x200B;* [Tablet] Los métodos abreviados para modificar pinceles con lápiz suelen dar lugar a un rendimiento bajo en casos excepcionales
&#x200B;* [Tablet] Retraso al pintar en una capa específica
&#x200B;* En raras ocasiones, pueden producirse texturas borrosas al cambiar la ventana gráfica
&#x200B;* [UI]&#x200B;[Substance] No siempre se muestran las entradas de imagen
&#x200B;* Limpiar no elimina los ajustes preestablecidos del estante que se hayan importado en un proyecto
&#x200B;* [Herramienta] [Trazo dinámico] Problema de rendimiento al ajustar el recuento cíclico de sello
&#x200B;* Problemas de actualización al pintar en modo de ventanilla 3D/2D en casos excepcionales
&#x200B;* Pintar un trazo muy largo puede provocar un congelamiento
&#x200B;* [Herramienta] Problema de rendimiento al pintar con trazos dinámicos específicos
&#x200B;* [UI] La barra de herramientas contextual sigue mostrando las propiedades del pincel al seleccionar una carpeta
&#x200B;* Los valores del eje de simetría no se restablecen
&#x200B;* La importación de texturas EXR con valores de coma flotante es totalmente negra
&#x200B;* Pulsar Alt+clic en un canal para aislar no funciona para el filtro y el generador
&#x200B;* [Exportar] El proyecto específico se bloquea durante la exportación
&#x200B;* [Substance] Valor predeterminado incorrecto en el menú desplegable si el parámetro está oculto por Visible If
&#x200B;* [Sombreador] Los canales definidos mediante Material Layering no se ordenan de la misma forma en la interfaz de usuario
&#x200B;* [Shelf] Los metadatos de ajustes preestablecidos no se guardan en el disco

**Problemas conocidos:**

&#x200B;* [Desempaquetado de UV] El procesamiento de mallas de alto contenido de polietileno puede tardar mucho tiempo
&#x200B;* [Desempaquetado UV] Se combinan vértices en las mismas coordenadas exactas
&#x200B;* La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
&#x200B;* [Desempaquetado UV] Relación de textil no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
&#x200B;* [Desempaquetado UV] Relación de textura no uniforme entre conjuntos de texturas
&#x200B;* [Desempaquetado UV] La Isla de UV generada puede ser muy alargada y, en algunos casos, no cabe en el espacio UV
&#x200B;* [Desempaquetado de UV] Las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no pueden desenvolverse con UV
&#x200B;* El ejemplo de reunión tiene algunos problemas con cámaras importadas

### 5.2.3 (2019.2.3)

*(Lanzado: 23 de octubre de 2019)*
Resumen: **Versión de corrección de errores**

**Agregado:**

&#x200B;* [Lista de conjuntos de texturas] Botón Añadir para activar o desactivar rápidamente el modo de enfoque
&#x200B;* [Log] Añadir número de versión de Windows 10 en el archivo de registro
&#x200B;* Actualizar a la versión más reciente de Substance Engine
&#x200B;* [MacOS] Notarizó el software para seguir los nuevos requisitos de distribución de MacOS Catalina

**Corregido:**

&#x200B;* [Plugin] El complemento de origen no funciona
&#x200B;* [MacOS] [Sombreador] Mac OS 10.14.5 y AMD: la colocación de los materiales en capas no funciona como se pretende

**Problemas conocidos:**

&#x200B;* No se pueden importar archivos Alembic con subdivisiones
&#x200B;* Bloqueos raros al importar algunos archivos Alembic
&#x200B;* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.2 (2019.2.2)

*(Lanzado: 20 de septiembre de 2019*
Resumen: **Versión de corrección de errores**

**Corregido:**

&#x200B;* La importación de recursos mediante secuencias de comandos puede provocar un bloqueo
&#x200B;* [Plugin] Descargar material de la fuente puede llevar a un bloqueo

**Problemas conocidos:**

&#x200B;* No se pueden importar archivos Alembic con subdivisiones
&#x200B;* Bloqueos raros al importar algunos archivos Alembic
&#x200B;* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.1 (2019.2.1)

*(Lanzado: 17 de septiembre de 2019*
Resumen: **Versión de corrección de errores**

**Corregido:**

&#x200B;* [Mac]&#x200B;[USD] Los archivos USDZ exportados de MacOS no se pueden abrir
&#x200B;* [Conjunto de texturas] No es posible aislar un conjunto de texturas con el modificador ALT
&#x200B;* [Shelf] Los ajustes preestablecidos, Materiales inteligentes y Máscaras inteligentes siempre se modifican al salir de la aplicación
&#x200B;* [Pila de capas] No se puede seleccionar el efecto después de eliminar otro efecto
&#x200B;* Parpadeo al utilizar un regulador dentro del panel de propiedades de la herramienta
&#x200B;* Bloqueo al exportar ajustes preestablecidos a la estantería
&#x200B;* Bloqueo al exportar un ajuste preestablecido con espacio insuficiente
&#x200B;* Bloqueo al crear un ajuste preestablecido con espacio insuficiente

**Problemas conocidos:**

&#x200B;* No se pueden importar archivos Alembic con subdivisiones
&#x200B;* Bloqueos raros al importar algunos archivos Alembic
&#x200B;* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.0 (2019.2.0)

*(Lanzado: 25 de julio de 2019)*
Resumen: **Versión principal con actualizaciones de los bakeres en términos de rendimiento y un nuevo modo de previsualización + nuevo contenido**

**Agregado:**

&#x200B;* [Bakeres] Se ha agregado compatibilidad para Trazado de rayos de GPU con DXR y OptiX (Oclusión ambiental, Thickness)
&#x200B;* [Baker] Optimizaciones y aceleraciones para el Trazado de rayos de la CPU
&#x200B;* [Bakeres]&#x200B;[Modo Vis]&#x200B;[IU] Nuevo modo de visualización de hace un bake en la ventana gráfica
&#x200B;* [Bakeres]&#x200B;[Preferencias]&#x200B;[IU] Nueva opción de hacer un bake para activar y desactivar el Trazado de rayos de GPU
&#x200B;* [Bakeres]&#x200B;[IU] Repaso del cuadro de diálogo de la barra de progreso
&#x200B;* [Bakeres] Mejora de los mensajes de advertencia y error
&#x200B;* [Bakeres] Permitir una cancelación más receptiva del proceso de hacer un bake
&#x200B;* [Baker] Vuelva a abrir la ventana hacer un bake después de hacer clic en Cancelar
&#x200B;* [Proj]&#x200B;[UX] Mejora de la usabilidad del manipulador de rotación
&#x200B;* [Configuración] Opción para mejorar el rendimiento reduciendo la resolución de la ventana gráfica para las pantallas HDPI
&#x200B;* [Scripting] Cambiar la resolución del conjunto de texturas
&#x200B;* [Scripting] Obtener conjunto de texturas seleccionado
&#x200B;* [Scripting] Permite que el usuario seleccione un conjunto de texturas
&#x200B;* [Scripting] Función para saber cuándo se ha cambiado la selección del conjunto de texturas
&#x200B;* [Estante] Se han añadido 40 materiales inteligentes nuevos
&#x200B;* [Estante] Se han añadido 20 máscaras inteligentes nuevas

**Corregido:**

&#x200B;* [Pila de capas] Bloqueo de la interfaz de usuario al seleccionar varias capas
&#x200B;* [Pila de capas] Agrupar muchas capas bloquea la interfaz de usuario más tiempo del habitual
&#x200B;* [Pila de capas] En algunos casos, se pueden seleccionar simultáneamente una capa y un efecto
&#x200B;* Los gráficos de Substance utilizados dentro de las herramientas de pintura no se generan con la resolución adecuada
&#x200B;* [Baker] El botón &quot;Hacer un bake todos los conjuntos de texturas&quot; no se desactiva si no se ha seleccionado ningún baker
&#x200B;* [MacOS] Desactivar el mensaje de advertencia sobre la teselación
&#x200B;* La herramienta Proyección no tiene previsualización cuando se utiliza con una máscara
&#x200B;* Bloqueos y proyectos dañados al intentar ahorrar con espacio en disco insuficiente
&#x200B;* [Shelf] Bloqueo al importar un recurso en el disco a través de la estantería con espacio insuficiente
&#x200B;* [Shelf] Bloqueo al restaurar el ajuste preestablecido de sesión
&#x200B;* [Estante] Al importar un ajuste preestablecido con un nombre que termina en un espacio, se crea un bloqueo
&#x200B;* [Shelf] Importar un recurso con un prefijo que termina con un espacio vacío conduce a un bloqueo

**Problemas conocidos:**

&#x200B;* No se pueden importar archivos Alembic con subdivisiones
&#x200B;* Bloqueos raros al importar algunos archivos Alembic
&#x200B;* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.1.3 (2019.1.3)

*(Lanzado: 1 de julio de 2019)*
Resumen: **Corrección de error con 2 nuevas características**

**Agregado:**

&#x200B;* Permite especificar el presupuesto de VRam con una línea de comandos (p. ej. —vram-budget 4096)
&#x200B;* [QML] Exponer las propiedades wrapMode y elide de los botones y casillas de verificación QML

**Corregido:**

&#x200B;* &quot;Seguir ruta&quot; no funciona todo el tiempo
&#x200B;* La asignación de canales no funciona con SBSAR utilizado en ranuras de un solo canal
&#x200B;* [Pila de capas] Bajo rendimiento al desplazarse con capas ocultas
&#x200B;* bloqueo [TextureSet] al hacer clic entre máscaras
&#x200B;* [SVT] El Desplazamiento no se muestra correctamente y parpadea en algunos casos
&#x200B;* [Alembic] Bloqueo con malla usando normales de punto en lugar de normales de vértice
&#x200B;* [Alembic]&#x200B;[Log] Informar de un error en Log si no se admite el archivo Alembic durante la importación

**Problemas conocidos:**

&#x200B;* No se pueden importar archivos Alembic con subdivisiones
&#x200B;* Bloqueos raros al importar algunos archivos Alembic

### 5.1.2 (2019.1.2)

*(Lanzado: 21 de mayo de 2019*
Resumen: **Revisión**

**Corregido:**

&#x200B;* Bloqueo al seleccionar dos recursos con una entrada de imagen

### 5.1.1 (2019.1.1)

*(Lanzado: 20 de mayo de 2019*
Resumen: **Revisión**

**Agregado:**

&#x200B;* Actualización a la versión más reciente de Substance Engine con la última versión de Substance Designer 2019.1

**Corregido:**

&#x200B;* [Substance] Visible Si no se tiene en cuenta para las imágenes de entrada
&#x200B;* [SVT]&#x200B;[Motor] El cambio de la resolución del conjunto de texturas provoca un bloqueo en algunos casos
&#x200B;* [Motor] En algunos casos aparecen texturas negras aleatorias
&#x200B;* [Pila de capas] [IU] Al alternar una máscara con MAYÚS, se pueden seleccionar varias capas al mismo tiempo
&#x200B;* [Pila de capas] La opacidad no afecta al efecto Pintura con el modo de fusión PassThrough
&#x200B;* [Pila de capas] La entrada de Height a filtro normal no se actualiza correctamente con el trazo del pincel borrador
&#x200B;* [LayersStack] Bloqueo al deshacer la caída de una máscara inteligente
&#x200B;* Malla metálica parpadeando con sombras y anti-aliasing temporal activado
&#x200B;* [Desplazamiento] Retraso en AMD con algunas mallas pesadas
&#x200B;* [Windows] Bloqueo al abrir algunos proyectos mediante el explorador de archivos
&#x200B;* [Histograma] Bloqueo al quitar la máscara con punto de anclaje en algunos casos
&#x200B;* Bloqueo en la generación de vistas previas en algunos casos raros
&#x200B;* [Bloqueo] No se puede volver a abrir un proyecto con demasiadas herramientas de clonación y difuminado
&#x200B;* No se muestra ninguna malla en el modo de material después de guardarla en algunos casos
&#x200B;* [Scripting] alg.mapexport.documentStructure() devuelve valores incorrectos para las carpetas

**Problemas conocidos:**

&#x200B;* Al hacer doble clic en el nombre del conjunto de texturas, se seleccionará antes de entrar en el modo de cambio de nombre

### 5.1.0 (2019.1.0)

*(Lanzado: 23 de abril de 2019)*
Resumen: **Trazo dinámico con contenido nuevo dedicado, Desplazamiento y teselación en tiempo real e Iray, efecto Máscara de comparación, simetría radial, Plano y Proyección esférica**

**Agregado:**

&#x200B;* [Herramienta] Trazo dinámico: Variación Substance junto a un trazo de pincel
&#x200B;* [Trazo dinámico] Exponer nuevo parámetro de índice de sello con opciones
&#x200B;* [Trazo dinámico] Tenga en cuenta el parámetro $time
&#x200B;* [Trazo dinámico] Generar un nuevo parámetro $randomseed por trazo y por sello
&#x200B;* [Trazo dinámico] Iniciar un índice de trazo dinámico a partir de un número aleatorio
&#x200B;* [Trazo dinámico] [Estante] Ayuda para buscar un recurso de trazo dinámico con un icono nuevo dedicado
&#x200B;* Desplazamiento y teselación en la ventana gráfica en tiempo real
&#x200B;* Desplazamiento y teselado en Iray
&#x200B;* [Configuración de sombreado]&#x200B;[IU] Nueva ficha para controlar el desplazamiento y la teselación
&#x200B;* [Pila de capas] Nuevo efecto CompararMáscara: generar una máscara comparando dos canales
&#x200B;* [Pila de capas]&#x200B;[IU] Nueva entrada en el menú contextual &quot;Añadir máscara con combinación de heightes&quot; para insertar un efecto Comparar máscara
&#x200B;* [Simetría] Nuevo modo de simetría: pintura radial
&#x200B;* [Configuración de simetría] Expanda las secciones &quot;Configuración&quot; y &quot;Pantalla&quot;
&#x200B;* [Ajustes de simetría] [IU] Vista previa para pintura radial
&#x200B;* Exponga dos nuevos modos de proyección: planar y esférico
&#x200B;* [Proj] Nuevo modo de recorte de forma para todas las proyecciones
&#x200B;* [Proj] Modo plano con nuevo manipulador: Herramienta Superficie
&#x200B;* [Proj]&#x200B;[Acceso directo] Método abreviado MAYÚS+W para la herramienta Superficie
&#x200B;* [Proj] Enmascaramiento de proyección plana con selección de profundidad y sacrificio de la cara posterior
&#x200B;* [Manipulador] Mejora del manipulador de rotación en los tres ejes para triplanar
&#x200B;* [Herramienta] [Experiencia de usuario] Al pulsar Alt y hacer clic en un canal, se selecciona ese canal (lo activa o desactiva todos los demás).
&#x200B;* [Motor] Actualizar a la versión más reciente de Substance Engine
&#x200B;* [Conjunto de texturas] Selección múltiple y resolución de cambios
&#x200B;* [Conjunto de texturas] Activación y desactivación rápidas de los conjuntos de texturas
&#x200B;* [Conjunto de texturas] Combina solo y todas las opciones en un nuevo menú
&#x200B;* [Conjunto de texturas] [Pila de capas] Nuevo icono para activación y desactivación
&#x200B;* [Pila de capas]&#x200B;[UX] Inserta efectos por encima de los que ya están seleccionados
&#x200B;* [Pila de capas]&#x200B;[IU] Reprocesamiento de la vista de la pila de capas
&#x200B;* [Pila de capas] El modo de fusión para capas con instancias ahora está en modo Pass Through de forma predeterminada
&#x200B;* [Exportar] Opción para activar y desactivar el tramado
&#x200B;* [Plugin] Compatibilidad con el modificador de precisión para reguladores (MAYÚS)
&#x200B;* [Plugin]&#x200B;[UI] Nuevo icono para autoguardar
&#x200B;* [Scripting] Enumera el contenido de una carpeta
&#x200B;* [Scripting] Permitir la eliminación de archivos
&#x200B;* [Scripting] Lea toda la información de la pila, incluidos los recursos utilizados
&#x200B;* [Contenido]&#x200B;[Trazo dinámico] Nuevas herramientas y ajustes preestablecidos de pincel
&#x200B;* [Content]&#x200B;[Dynamic stroke] Dos nuevos degradados de procedimiento: Tono de degradado y Generador de degradado
&#x200B;* [Contenido] 11 nuevos filtros: Pintura descascarillada MatFx, gotas de agua MatFx y más
&#x200B;* [Contenido] 7 nuevos generadores: Stitcher automático, UV Random Color, UV Texel Density y más
&#x200B;* [Contenido] 93 alfas nuevas: nuevos textos, flechas y otras formas
&#x200B;* [Contenido] 2 nuevos procedimientos: Tono de degradado, Generador de degradados y mucho más
&#x200B;* [Contenido] 21 nuevos ajustes preestablecidos de herramienta y pincel para Trazos dinámicos : Guijarros, Huellas, Spray y más
&#x200B;* [Contenido] 2 HDR nuevos: Canopus Ground y Autumn Forest
&#x200B;* [Contenido] Actualizar el contenido con la selección aleatoria de semillas en el estante
&#x200B;* [Contenido] Nuevo icono con parámetro de semilla aleatoria expuesto en la estantería

**Corregido:**

&#x200B;* [Pila de capas] La pila de capas se sigue arrastrando para siempre
&#x200B;* [Mac] La opción &quot;Mostrar en Finder&quot; puede provocar la congelación
&#x200B;* [Scripting] La configuración guardada mediante la interfaz de usuario personalizada se pierde si se mueve el archivo de sombreado
&#x200B;* El número de versión de la API [Scripting] es incorrecto y no está actualizado
&#x200B;* [Efecto] El contenido del histograma no se muestra correctamente
&#x200B;* [Efecto] El efecto del histograma no se actualiza en algunos casos
&#x200B;* [Estante] Los puntos no se alinean correctamente en el material &quot;Pirámide de tela plástica&quot;

**Problemas conocidos:**

&#x200B;* Al hacer doble clic en el nombre del conjunto de texturas, se seleccionará antes de entrar en el modo de cambio de nombre
&#x200B;* [Pila de capas] [IU] Al alternar una máscara con MAYÚS, se pueden seleccionar varias capas al mismo tiempo

## Versión 4

### 4.3.3 (2018.3.3)

*(Lanzado: 7 de marzo de 2019)*
Resumen: **corrección de errores**

**Agregado:**

&#x200B;* [Contenido] Integrar nueva plantilla de proyecto: &quot;PBR - Mezcla Alpha de rugosidad metálica&quot;
&#x200B;* El orden de búsqueda de la biblioteca dinámica de Linux ha cambiado para priorizar las bibliotecas en el directorio de instalación antes de lo que está instalado en el sistema

**Corregido:**

&#x200B;* La malla desaparece a veces de la ventana gráfica 3D (presione F para restablecer la cámara)
&#x200B;* Actualizar el cargador de Substance Painter de Sketchfab con los nuevos tipos de licencia de Sketchfab
&#x200B;* [Import]&#x200B;[glTF] Modulación incorrecta de la textura de entrada definida en los archivos glTF
&#x200B;* [Import]&#x200B;[glTF] El plano de tierra se muestra incorrectamente con la importación de glTF en algunos casos
&#x200B;* [Export]&#x200B;[USD] La opacidad no funciona en Arkit
&#x200B;* [Export]&#x200B;[USD] La exportación de USDz se bloquea en algunos casos
&#x200B;* [Export]&#x200B;[USD] Exportar a USD sin guardar provoca un bloqueo
&#x200B;* [Export]&#x200B;[USD] Modo de mosaico incorrecto para texturas, modo de subdivisión para mallas y tipos de salida para sombreadores
&#x200B;* [Export]&#x200B;[USD] Exportaciones dispersas de solo algunos conjuntos de texturas con toda la geometría
&#x200B;* [Instancia] Bloqueo al intentar eliminar una capa de instancia rota
&#x200B;* [Regresión]&#x200B;[Exportar] Algunos mapas no exportados en la profundidad de bits elegida
&#x200B;* [Linux] Problema con library libtbb.so.2

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
&#x200B;* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.3.2 (2018.3.2)

*(Lanzado: 24 de enero de 2019)*
Resumen: **Revisión con nuevas características (exportación USDZ y filtrado de texturas en la ventana gráfica)**

**Agregado:**

&#x200B;* [Exportar] Permitir exportación a USDZ
&#x200B;* [Ventana gráfica] Permite controlar la calidad de la textura en los Ajustes de visualización
&#x200B;* [Viewport] Se ha añadido el ajuste de sesgo mip en la configuración de visualización
&#x200B;* [Ventana gráfica] Se ha añadido un filtrado anisotrópico en la configuración de visualización
&#x200B;* [complementos] Actualizar los complementos oficiales para usar el estilo de Substance Painter 2018
&#x200B;* [Licencia] Instalar la licencia de forma predeterminada en una carpeta de usuario

**Corregido:**

&#x200B;* Bloqueo vinculado a la descompresión
&#x200B;* Añadir TAA en material solo
&#x200B;* Ruido con sombra, TAA y sombreador de prueba alfa con tramado
&#x200B;* Eliminar el tramado de specular para todos los sombreadores PBR clásicos
&#x200B;* Bloqueo en la configuración del sombreado en algunos casos
&#x200B;* La activación de la dispersión no está sincronizada entre los procesamientos de OpenGL e Iray
&#x200B;* Las herramientas de difuminado y clonación ya no funcionan en mallas específicas
&#x200B;* Algunos conjuntos de texturas no pueden aparecer en el procesamiento de Iray
&#x200B;* Los conjuntos de texturas renombrados no se guardan después de cerrar el proyecto
&#x200B;* Artefactos de malla metálica al arrastrar y soltar materiales en mapas de ID
&#x200B;* [Scripting] La creación de la ruta de archivo no se fuerza al guardar un proyecto
&#x200B;* [Scripting] La devolución de llamada &quot;onProjectAboutToSave()&quot; ya no funciona
&#x200B;* Vínculos de foro rotos en la ventana de informe de errores

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
&#x200B;* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.3.1 (2018.3.1)

*(Lanzado: 6 de diciembre de 2018)*
Resumen: **Revisión**

**Agregado:**

&#x200B;* [Simetría] [Ventana gráfica] El dibujo de la Simetría en la Vista 2D ha vuelto y ahora se ha corregido una previsualización del pincel clónico

**Corregido:**

&#x200B;* La exportación de Vista 2D genera una textura negra en algunos casos
&#x200B;* [Iray] La información normal se vuelve incorrecta en Iray después de crear instancias de una capa de material
&#x200B;* Los conjuntos de texturas no cuadrados pueden provocar en algunos casos bloqueos
&#x200B;* [Deshacer] Varias teclas Ctrl+Z pueden llevar al bloqueo de forma aleatoria en algunos casos
&#x200B;* [QML] AlgScrollView puede crear una advertencia en el registro en algunos casos (bucles de enlace)

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
&#x200B;* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows
&#x200B;* El suavizado y las sombras cuando están activos juntos pueden dar resultados inesperados

### 4.3.0 (2018.3.0)

*(Lanzado: 20 de noviembre de 2018)*
Resumen: <b>Actualizaciones de la ventana gráfica, exportación adecuada de la vista 2D, nuevos ayudantes de interfaz de usuario, una herramienta de simetría mejorada, nuevo contenido y un gran aumento en el rendimiento</b>

<b>Agregado:</b>

&#x200B;* [Suavizado] [Ventana gráfica] Nuevo filtrado de suavizado temporal para la ventana gráfica 3D (mediante Configuración de visualización)
&#x200B;* [Exportar] Exporte el contenido de la ventana gráfica 2D como una única textura
&#x200B;* [Exportar] [Tramado] Exponer tramado en la exportación
&#x200B;* [Pila de capas] Colores en capas y carpetas
&#x200B;* [Pila de capas] Activación y desactivación rápidas de varias capas y efectos
&#x200B;* [Pila de capas] Navegación más sencilla por los modos de fusión con las teclas hacia arriba y el desplazamiento del ratón
&#x200B;* [Proj]&#x200B;[UI] Manipulador de rotación adicional en los tres ejes para triplanar
&#x200B;* [Proj]&#x200B;[Atajos] : y + para cambiar el tamaño del manipulador de Proyección de UV
&#x200B;* [Shader] Controle los parámetros de capa revestida con canales en el sombreador recubierto de PBR
&#x200B;* [Substance] Expone nuevas entradas de textura basadas en malla para filtros y generadores
&#x200B;* [Simetría]&#x200B;[Ventana gráfica]&#x200B;[IU] Controlar el desplazamiento de simetría con manipuladores
&#x200B;* [Simetría]&#x200B;[Barra de herramientas contextual]&#x200B;[IU] Nuevo panel de simetría con opciones
&#x200B;* [Simetría] Nuevo modo de intersección de línea de simetría
&#x200B;* [Simetría] Nuevo cursor de clonación de simetría
&#x200B;* [Simetría] [Métodos abreviados] Q para ocultar y -, + para cambiar el tamaño y cambiar para ajustar
&#x200B;* [Log] Mejore los mensajes de error cuando no se pueden exportar texturas
&#x200B;* [Scripting] Permite cambiar o actualizar los recursos en Configuración de visualización
&#x200B;* [Scripting] Permite crear o quitar canales en conjuntos de texturas
&#x200B;* [Contenido]&#x200B;[Shaders] Añadir compatibilidad para la anisotropía con un sombreado específico (pbr-metal-rough-anisotropía-angle)
&#x200B;* [Contenido] Actualización de la esfera de previsualización con anisotropía y ángulo modificado
&#x200B;* [Contenido] Se ha actualizado el obturador de matFx
&#x200B;* [Contenido] Nueva digitalización de caras sin problemas Texturing.XYZ
&#x200B;* [Contenido] Nuevos procedimientos anisotrópicos
&#x200B;* [Content] Nuevo filtro: entorno de iluminación generado
&#x200B;* [Contenido] Nuevo mapa de entorno: studio automotive neutral
&#x200B;* [Contenido] Nueva plantilla de proyecto: PBR - Ángulo de anisotropía de rugosidad metálica (con canales de anisotropía)
&#x200B;* [Contenido] Nueva plantilla de proyecto: PBR - rugosidad metálica recubierta
&#x200B;* [SVT]&#x200B;[Motor] Texturas virtuales dispersas (SVT)
&#x200B;* [SVT]&#x200B;[Preferencias]&#x200B;[IU] Opción de aceleración de compatibilidad de hardware SVT
&#x200B;* [SVT]&#x200B;[Log] Información adicional para la función de texturas virtuales dispersas (p. ej., disco de tamaño)
&#x200B;* [SVT]&#x200B;[UI] Ventana de mensaje al inicio si el tamaño del disco es demasiado bajo para la caché
&#x200B;* [SVT]&#x200B;[Preferencias]&#x200B;[IU] Ubicación de caché global del Substance Painter
&#x200B;* [SVT] Nueva variable de entorno para especificar la ruta de acceso de la caché del Substance Painter
&#x200B;* [SVT] Nueva variable de entorno para activar la aceleración de compatibilidad de hardware SVT
&#x200B;* [SVT] Detectar compatibilidad dispersa por hardware
&#x200B;* [SVT]&#x200B;[Hardware disperso] Aumentar la versión mínima del controlador para la GPU Nvidia
&#x200B;* [SVT]&#x200B;[Sombreador]&#x200B;[Viewport]&#x200B;[UI] Advertencia al usuario si hay artefactos con texturas virtuales dispersas al abrir el proyecto

<b>Corregido:</b>

&#x200B;* [Selector de color] Cursor de pintura que aparece al intentar seleccionar un color
&#x200B;* El bloqueo al seleccionar o anular la selección de capas en un orden específico puede provocar bloqueos
&#x200B;* Bloqueo al pegar como instancia una capa con una máscara
&#x200B;* [Canal de usuario]&#x200B;[Regresión] Bloqueo al cambiar el nombre del canal de usuario
&#x200B;* [Canal de usuario] Vista previa de pincel atenuado
&#x200B;* [Alembic] Solo un conjunto de texturas de varios materiales tras la importación
&#x200B;* [Motor] La textura exportada difiere de la ventana gráfica para los sellos de pincel
&#x200B;* [Motor] La inversión con un efecto de nivel no afecta completamente a una textura
&#x200B;* El selector de material está aplicando un trazo de pincel al seleccionar
&#x200B;* Cambiar la resolución a 128x128px conduce a un bloqueo
&#x200B;* Los vínculos de mapa de malla no se actualizan correctamente al rehornear o crear instancias de capas
&#x200B;* [Substance] UserData ColorSpace no funciona en la malla Hecha un bake Normal solicitada como entrada
&#x200B;* No coincide la asociación MDL al utilizar varias instancias de sombreado
&#x200B;* [Simetría] [Capa de relleno] Plano de Simetría y su manipulador activo en Capa de relleno
&#x200B;* [Ventana gráfica] El punto de tabla dinámica para la traducción no siempre se actualiza después de hacer clic
&#x200B;* [UI] Se han corregido los iconos y la eliminación de marcadores de posición para los monitores HDPI

<b>Problemas conocidos:</b>

&#x200B;* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
&#x200B;* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows
&#x200B;* El suavizado y las sombras cuando están activos juntos pueden dar resultados inesperados

### 4.2.3 (2018.2.3)

*(Lanzado: 25 de septiembre de 2018)*

**Corregido:**

&#x200B;* [vista 2D] La vista 2D se rompe con algunas mallas al crear un nuevo proyecto
&#x200B;* [Bloqueo] El cambio de la Proyección de UV a la proyección triplana conduce a un bloqueo
&#x200B;* [RayCollider] Varios bloqueos debido a &quot;RayCollider&quot;
&#x200B;* [Herramienta] Al cambiar las capas, se pierden las propiedades de pincel modificadas
&#x200B;* La configuración del pincel se restablece al cambiar al borrador

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en GPU AMD VEGA
&#x200B;* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.2.2 (2018.2.2)

*(Lanzado: 11 de septiembre de 2018)*
Resumen: **Revisión con actualización de contenido, nuevas funcionalidades de secuencias de comandos y poder deshabilitar la actualización automática**

**Agregado:**

&#x200B;* [Contenido]&#x200B;[Estante] Añadir un ajuste preestablecido de Estante de piel
&#x200B;* [Contenido] [estante] Conversión de 19 normales de piel en materiales para dispersión subsuperficial
&#x200B;* [Scripting] Crear una plantilla de proyecto a partir de un proyecto abierto
&#x200B;* [Scripts] Obtener o establecer la configuración de exportación de un proyecto abierto
&#x200B;* [Actualizaciones] Puede desactivar la ventana emergente de actualización automática de la variable de entorno y configuración
&#x200B;* [Actualizaciones] No se muestra hasta la próxima versión en la ventana emergente de mantenimiento obsoleta

**Corregido:**

&#x200B;* [Cámara] Zoom incorrecto al cambiar de ortográfico a Perspectiva
&#x200B;* [Display] Algunos mapas se muestran en línea en lugar de sRGB
&#x200B;* [Ventanas] El enfoque de malla no se comporta correctamente
&#x200B;* [vista 2D] El proyecto con la cámara rota ha desaparecido UV
&#x200B;* [SSS] [Información sobre herramienta] aparece información sobre herramientas de dispersión subsuperficial en el registro
&#x200B;* Algunos proyectos no se pueden abrir en 2018.2 y el mensaje de error no puede guardar un paquete de substance nulo
&#x200B;* [Máscara] El color de la herramienta de Pintura se puede bloquear en algunos casos al trabajar en una máscara
&#x200B;* [Material] Mapas que no aparecen en situaciones específicas
&#x200B;* [Proj]&#x200B;[Tools] Manipulador activo con un generador
&#x200B;* [Substance] Faltan grupos de parámetros de Substance
&#x200B;* [Scripting] Nombre de software incorrecto en la documentación
&#x200B;* [UDIM] No hay información en el registro acerca de los proyectiles de UV en múltiples mosaicos de UV

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en GPU AMD VEGA
&#x200B;* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.2.1 (2018.2.1)

*(Lanzado: 03 de agosto de 2018)*

**Corregido:**

&#x200B;* Faltan parámetros de sombreador de dispersión subsuperficial en los proyectos de actualización

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en GPU AMD VEGA
&#x200B;* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.2.0 (2018.2.0)

*(Lanzado: 2 de agosto de 2018)*
Resumen: **Versión de verano, compatibilidad con dispersión subsuperficial, mejoras en la proyección y el relleno, importación y selección de cámaras, compatibilidad con Alembic y glTF, arrastrar y soltar en mapa de ID, compatibilidad de formato de Substance mejorada y nuevo contenido**

**Agregado:**

&#x200B;* [SSS]&#x200B;[Viewport]&#x200B;[Iray] Dispersión subsuperficial genérica
&#x200B;* [SSS] Sincronización de MDL y parámetros de dispersión subsuperficial
&#x200B;* [SSS] Se ha añadido un nuevo canal de escala de grises denominado Dispersión
&#x200B;* [SSS]&#x200B;[Configuración del sombreador] Parámetro de tipo de dispersión para dispersión subsuperficial (piel o translúcido)
&#x200B;* [SSS]&#x200B;[Configuración de sombreado] Parámetro de escala de dispersión para dispersión subsuperficial
&#x200B;* [SSS]&#x200B;[Configuración de sombreado] Parámetro de color de dispersión para dispersión subsuperficial
&#x200B;* [SSS]&#x200B;[Configuración de pantalla] Dispersión Recuento de muestras para dispersión subsuperficial
&#x200B;* [Shader] [Iray] Integrar MDL de dispersión subsuperficial para Iray
&#x200B;* [Shader] Actualización del sombreado mediante el actualizador de recursos
&#x200B;* [Shader] Actualizar la API y la documentación del registro de cambios
&#x200B;* [Tool Properties]&#x200B;[Proj] Nuevos parámetros para la proyección triplanar
&#x200B;* [Ventana gráfica]&#x200B;[Proyecto] Controle las propiedades de la capa de relleno en la vista 3D directamente con los manipuladores (proyección triplanar)
&#x200B;* [Atajos]&#x200B;[Proj] Nuevos atajos Q, W, E, R, T para manipuladores de proyección triplanar
&#x200B;* [Viewport]&#x200B;[Proj] Controle las propiedades de la capa de relleno en la vista 2D directamente con los manipuladores (Proyección de UV)
&#x200B;* [Atajos]&#x200B;[Proj] Nuevo atajo Q para manipuladores de Proyección de UV
&#x200B;* [Barra de herramientas contextual]&#x200B;[Proj] Controlar manipuladores de proyección triplanar
&#x200B;* [Barra De Herramientas Contextual]&#x200B;[Proj] Controlar Manipuladores De Proyección de UV
&#x200B;* [Propiedades de la herramienta] Desactivar el mosaico de texturas con las herramientas Proyección y Galería de símbolos
&#x200B;* [Galería de símbolos] Usar imágenes no cuadradas con la herramienta o galería de símbolos Proyección
&#x200B;* [Stencil] Permitir el control del modo de mosaico en la ventana Propiedades
&#x200B;* [Stencil] El zoom no está centrado en una galería de símbolos que no sea de mosaico
&#x200B;* [Cámaras] Importar cámaras de Maya, Max, Blender, Modo, DAE
&#x200B;* [Cámaras] [Ventana gráfica] Seleccione y controle las cámaras importadas en la ventana gráfica
&#x200B;* [Cámaras] [Israel] Seleccione y controle las cámaras importadas en Irán
&#x200B;* [Cámaras]&#x200B;[IU]&#x200B;[Nuevo proyecto]&#x200B;[Configuración del proyecto] Importar cámaras está marcado de forma predeterminada
&#x200B;* [Cámaras] [Accesos directos] Añadir accesos directos para cambiar de cámara
&#x200B;* [Cámaras]&#x200B;[Ventana gráfica] Añadir marco en la ventana gráfica
&#x200B;* [Cámaras] [Configuración de la ventana gráfica] Control de la opacidad del marco
&#x200B;* [Cámaras]&#x200B;[Configuración de la cámara] distancia focal máxima de 500 mm
&#x200B;* [Cámaras]&#x200B;[Configuración de la cámara] Relación de exposición
&#x200B;* [Cámaras]&#x200B;[Configuración de la cámara] Añadir una opción de bloqueo
&#x200B;* [Cámaras]&#x200B;[Configuración de la cámara] Añadir una opción de restauración
&#x200B;* [Cámaras]&#x200B;[Configuración de la cámara] Añadir el atributo de distancia de enfoque
&#x200B;* [glTF] Importación de un archivo glTF
&#x200B;* [glTF] Importar mapa de oclusión ambiental
&#x200B;* [Alembic] Importar marco Alembic 1 con geometría estática
&#x200B;* [Estante] Arrastre y suelte materiales directamente en la malla mediante mapas de ID con un modificador (CTRL/Comando)
&#x200B;* [Pila de capas] Creación automática de máscaras de ID con arrastrar y soltar materiales en la malla con mapas de ID
&#x200B;* [Pila de capas] Desplazamiento automático de capas arrastrando y soltando por la pila de capas
&#x200B;* [UI]&#x200B;[Propiedades de la herramienta] Exponer el ajuste preestablecido de Substance
&#x200B;* [UI]&#x200B;[menú Ayuda] Mejora del menú Ayuda
&#x200B;* [UI]&#x200B;[Nuevo proyecto]&#x200B;[Configuración del proyecto] Reorganización de la ventana
&#x200B;* [UI]&#x200B;[Nuevo proyecto]&#x200B;[Configuración del proyecto] Reemplazar término de malla por archivo
&#x200B;* [UI]&#x200B;[Substance] Visualización de atributos de Substance en IU
&#x200B;* [Métodos abreviados] F4 cambia entre la vista 2D y 3D
&#x200B;* [Accesos directos] Nuevos métodos abreviados para alternar la galería de símbolos N y la máscara rápida U
&#x200B;* [Substance integration] Tenga en cuenta las sentencias &#39;visible if&#39; en los parámetros del Substance
&#x200B;* [Ventana gráfica] Las sombras no se ven forzadas a computarse después de mover la cámara
&#x200B;* [Contenido] Actualizar MeetMat con cámaras importadas
&#x200B;* [Contenido] Añadir una muestra con la dispersión subsuperficial activada - JadeToad
&#x200B;* [Contenido] Añade una nueva plantilla de proyecto PBR con la dispersión subsuperficial activada
&#x200B;* [Contenido] Se han actualizado los ajustes preestablecidos de exportación para añadir un nuevo canal de dispersión
&#x200B;* [Content]&#x200B;[Shelf] Se ha añadido compatibilidad de dispersión subsuperficial para: pbr-metal-rough, pbr-metal-rough-alpha-test, recubierto de pbr, pbr-spec-gloss
&#x200B;* [Contenido] [Estante] Se ha añadido un canal de dispersión a 5 materiales inteligentes (mármoles y máscaras)
&#x200B;* [Contenido]&#x200B;[Estante] 1 nuevo material de jade
&#x200B;* [Contenido]&#x200B;[Estante] 1 nuevo material de cera

**Corregido:**

&#x200B;* [CMD] Diferentes resultados usando la misma línea de comandos con diferentes versiones
&#x200B;* [TDR] Si se configura TdrLevel, no hay errores en el registro
&#x200B;* [Baker] El mapa de Oclusión ambiental está volteado
&#x200B;* [Mapa de ID] Bloqueo al seleccionar fuera del rango 0-1
&#x200B;* [Iray] Bloqueo al cambiar conjuntos de texturas y volver al modo de Pintura
&#x200B;* [Ventana gráfica] Sincronizar áreas de colocación entre ventanas gráficas para arrastrar y soltar
&#x200B;* [Motor] Artefacto de moiré al aplicar mosaico a capas de relleno o pintar pinceles pequeños
&#x200B;* [Licencia] Comprobación de versión de software errónea del servicio de licencias
&#x200B;* [Licencia] Cambiar la forma de gestionar la autenticación
&#x200B;* [API] Llame al evento de API de scripts onNewProjectCreated incluso al crear con una plantilla
&#x200B;* [Sombreador] El sombreador compilado no se carga de la memoria caché cuando el archivo de sombreador no se compila
&#x200B;* [Shelf] Al exportar el archivo HDR. de la estantería, se generará un archivo con valores de sujeción
&#x200B;* [Exportar] EXR exportar abrazaderas RGB valores de color entre 0 y 1
&#x200B;* [Contenido] Ruido Procedimiento 3D Perlin Noise Fractal se pixeló

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en GPU AMD VEGA
&#x200B;* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.1.3 (2018.1.3)

*(Lanzado: 28 de junio de 2018)*

**Agregado:**

&#x200B;* [Preferencias] Propuesta de guardar el proyecto cuando se reinicie Painter

**Corregido:**

&#x200B;* [Plugin] El Substance Source de búsqueda no funciona
&#x200B;* [Materiales inteligentes] La importación de Materiales inteligentes provoca un bloqueo en algunos casos
&#x200B;* [Materiales inteligentes] Al eliminar Materiales inteligentes, en algunos casos se produce un bloqueo
&#x200B;* [Guardar] Guardar conduce a un bloqueo en algunos casos raros
&#x200B;* [Estante] Invertir no funciona en las Celdas 2 y 3
&#x200B;* [Estante] Error tipográfico en algunos Alpha
&#x200B;* [Estante] Algunos materiales de Substance no se procesan correctamente

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.2 (2018.1.2)

*(Lanzado: 12 de junio de 2018)*
Resumen: **Mejora en la velocidad de Hace un bake, Sistema de guardado mejorado, Reguladores actualizados, Plugin API actualizado, Traducción al chino, Relleno mejorado ahora Opcional**

**Agregado:**

&#x200B;* [Bakeres] Mejora del rendimiento con la nueva versión de baker
&#x200B;* Cuadro de diálogo Forzar visualización con GPU no compatible
&#x200B;* [Guardar] Exponer nueva funcionalidad de proyecto compacto (modo de guardado completo/compacto)
&#x200B;* [Guardar] Informar al usuario en caso de error de guardado
&#x200B;* [Limpiar] A continuación, guarde en modo completo/compacto
&#x200B;* [Reguladores] Mejora de la precisión de las barras y los reguladores de color/escala de grises
&#x200B;* [Reguladores] Adición de controles de flecha arriba/abajo
&#x200B;* [Reguladores] Misma zona de detección para los reguladores de barras de color y escala de grises
&#x200B;* [Plugin] Autoguardar siempre en modo incremental
&#x200B;* [Plugin] Opción para cambiar los complementos al nuevo estilo de interfaz
&#x200B;* [Idioma] Añadir traducción al chino
&#x200B;* [Padding] Opción para cambiar entre el relleno UV y el relleno contiguo de espacio 3D por conjunto de texturas en Ajustes de conjunto de texturas
&#x200B;* [Script] Exponer modo de guardado: completo/compacto o incremental
&#x200B;* [Script] Actualizar documentación de scripts/QML
&#x200B;* [Log] Indicar modo de guardado en log (completo/compacto o incremental)

**Corregido:**

&#x200B;* [Herramienta] La ranura de canal se transforma en una ranura de material en rellenos de un solo canal
&#x200B;* Bloqueo al cargar una malla (FBX) con algunas caras no asignadas por un material
&#x200B;* Bloqueo en Irán con NVIDIA GRID 5.2 en una máquina virtual
&#x200B;* Bloqueo al deshacer la eliminación de un ajuste preestablecido de material
&#x200B;* Bloqueo al cargar algunos proyectos
&#x200B;* [Línea de comandos] Nueva línea de comandos para las mallas UDIM divididas por udim
&#x200B;* [Barra de herramientas] Reducción de la barra de herramientas
&#x200B;* [Instanciación] No se pueden crear instancias de mapas de bits en varios conjuntos de texturas
&#x200B;* [Ventana gráfica] La actualización no se completa al pintar en malla con UV en mosaico
&#x200B;* [Iray] El mapa normal se aplica dos veces para los dieléctricos
&#x200B;* [Shelf] Errores tipográficos en algunos parámetros del Substance (alfas, procedimientos y matfx)
&#x200B;* [Shelf] Error tipográfico para el mapa de bits &quot;Solo personal autorizado&quot;
&#x200B;* [Script] La función alg.shaders.materials() ya no funciona

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.1 (2018.1.1)

*(Lanzado: 3 de abril de 2018)*

**Corregido:**

&#x200B;* [Tablet] Problema al cambiar las opciones de interacción predeterminadas
&#x200B;* [Baker] Bloqueo con la biblioteca Assimp
&#x200B;* [Bakeres] Regresión en el rendimiento con el mapa A.O
&#x200B;* [Iray] La Distorsión de lente no se aplica al canal Alfa
&#x200B;* [Controladores] Actualización de los requisitos mínimos de controladores
&#x200B;* [3Dview] Las normales no se generan correctamente en las mallas del UDIM sin información de normales
&#x200B;* [Intel] Bloqueo con Substance Painter 2018.1.0
&#x200B;* [Intel]&#x200B;[Viewport] Problema con relleno (defectos negros)

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.0 (2018.1.0)

*(Lanzado: 15 de marzo de 2018)*

**Agregado:**

&#x200B;* Nuevo estilo general (iconos, color, comportamiento)
&#x200B;* Nuevo diseño predeterminado
&#x200B;* [Tablet] Mejora de la experiencia del usuario al pintar
&#x200B;* [Menú principal] Ordenar primero los elementos nativos de las vistas y barras de herramientas
&#x200B;* [Menú principal] Sección Mover acciones de máscara rápida en la ventana gráfica
&#x200B;* [Menú principal] Sección Mover las acciones del botón derecho al área de visualización
&#x200B;* [Menú principal] Cambiar el nombre del menú &quot;Ver&quot; por &quot;Ventana&quot;
&#x200B;* [Menú rápido] Nuevas propiedades de la herramienta haciendo clic con el botón derecho en la ventana gráfica
&#x200B;* [Widget de Dock] Nueva barra de herramientas de Dock para reducir/recuperar rápidamente
&#x200B;* [Configuración de la pantalla] Ventana de configuración de la cámara y del visor combinada
&#x200B;* [Pila de capas] Menú contextual del botón derecho
&#x200B;* [Pila de capas] Arrastra y suelta para mover cualquier efecto dentro de la misma capa
&#x200B;* [Barra de herramientas] Reorganización de la barra de herramientas y nueva barra de herramientas contextual
&#x200B;* [Barra de herramientas Herramientas] Dividir la herramienta Clonar en dos herramientas independientes
&#x200B;* [Herramientas, propiedades] Valor de escala de grises de fondo más claro en la previsualización
&#x200B;* [Herramientas propiedades] Organización en fichas (rellenar y herramientas)
&#x200B;* [Herramienta] El resultado de la pintura coincide con la galería de símbolos
&#x200B;* [Ventana gráfica] Nuevo cursor para la capa de relleno
&#x200B;* [Ventana gráfica] Navegación y pintura más fluidas (velocidad de fotogramas más alta)
&#x200B;* [Ventana gráfica] Cuadro combinado de selección de material/canal/mapa en la ventana gráfica
&#x200B;* [Ventana gráfica] Reducción del parpadeo durante la rotación (sombra activada)
&#x200B;* [Shelf] Mostrar materiales de forma predeterminada al abrir Painter
&#x200B;* [Estante] Mejora del tiempo de carga de texturas y materiales Substance (2 a 6 veces más rápido)
&#x200B;* [Estante] Reorganizar las carpetas de materiales para que se ajusten a la estructura del Substance Source
&#x200B;* [Estante] Arrastre y suelte los materiales directamente en la malla en la ventana gráfica
&#x200B;* [Shelf] Nuevos ruidos 3D (Perlin, Perlin Fractal, Simplex y Worley)
&#x200B;* [Shelf] Nuevo generador de máscara de 3D linear gradient usando posición de malla
&#x200B;* [Estante] Ruidos básicos actualizados para admitir la expansión no cuadrada
&#x200B;* [Estante] Se ha añadido una nueva plantilla y un ajuste preestablecido de exportación para Lens Studio (aplicación Snap)
&#x200B;* [Estante] Se han actualizado los materiales y las máscaras inteligentes para utilizar la última versión del editor de máscaras (microdetalles).
&#x200B;* [Estante] Nuevo proyecto de muestra &quot;TilingMaterial&quot; para crear materiales de mosaico sin costuras
&#x200B;* [Estante] Nuevos ajustes preestablecidos de pincel (caligrafía, mojado, sombreado, etc.)
&#x200B;* [Reguladores] Nuevos reguladores y estilo y comportamiento de las barras de escala de grises y de color
&#x200B;* [Bakers] Permite el uso del cuadro delimitador de escena completo para calcular el mapa de posición
&#x200B;* [Shader] Se elimina el parámetro de fuerza de height de los parámetros de sombreado predeterminados.
&#x200B;* [Motor] Motor del Substance actualizado
&#x200B;* [Motor] No hay discontinuidades o menos en los fragmentos UV
&#x200B;* [Complementos] Importa materiales descargados de Substance Source con mayor rapidez
&#x200B;* [Plugins] Actualice todos los plugins para que coincidan con el nuevo estilo general
&#x200B;* [Preferencias] La vista previa del color de fondo cambia automáticamente
&#x200B;* [Limpio] Menor riesgo de corrupción de proyectos
&#x200B;* [Abrir] Mejora del tiempo de apertura del proyecto
&#x200B;* [Nuevo proyecto] Nuevo proyecto: mejora del tiempo de actualización de la malla
&#x200B;* [Guardar] Ahorro de tiempo del proyecto
&#x200B;* [Log] Tipo de licencia registrado en el registro
&#x200B;* [TextureSet] Cambie el nombre del botón &quot;Hacer un bake Texturas&quot; por &quot;Hacer un bake mapas de malla&quot;
&#x200B;* Cambie el nombre de &quot;Mapas adicionales&quot; por &quot;Mapas de malla&quot;

**Corregido:**

&#x200B;* [Viewport] Mal rendimiento con mallas que contienen muchos subobjetos
&#x200B;* [Herramientas > Propiedades] Canal desactivado al arrastrar y soltar una imagen en la ranura de material
&#x200B;* [Herramientas, propiedades] La vista previa del pincel se rompe con las herramientas de difuminado y clonado
&#x200B;* [Conjunto de texturas] El orden de los canales es incorrecto al utilizar plantillas
&#x200B;* [Shelf] Falta icono para el generador de Conversión de escala de grises
&#x200B;* [Estante] El número de círculo de Sign alfa está roto (falta fuente)
&#x200B;* Detección incorrecta de GPU integradas al iniciarse
&#x200B;* [Bloqueo] Arrastrar y colocar un recurso importado cuyo nombre tenga el carácter #
&#x200B;* [Motor] Problema de detección de Vram en la GPU integrada
&#x200B;* [Motor] Se han solucionado numerosos bloqueos en Substance Engine Linker
&#x200B;* [Motor] Artefactos cuadrados al cambiar la resolución
&#x200B;* [Efectos de posprocesamiento] El cambio de tamaño de la interfaz es lento cuando los efectos de posprocesamiento están activados
&#x200B;* [Bakeres] La unidad de escena no se respeta correctamente para los valores de distancia de rayos
&#x200B;* [Bakeres] El AO de la distancia del Mesh Occluder se fija en 1 independientemente del valor de entrada
&#x200B;* [Bakeres] La coincidencia por nombre ignora algunas mallas con nombres específicos
&#x200B;* [Bakeres] El color de la configuración de Polygroup de malla e ID de submalla siempre devuelve una imagen en negro
&#x200B;* [Bakeres] La Hace un bake de ID falla con mallas de FBX binarias de Blender
&#x200B;* [Sombreador] Ruido en el vista 2D con dota-2 y non-pbr-spec-gloss
&#x200B;* [Linux] Sólo se utiliza un subproceso de CPU al hacer un bake
&#x200B;* [MacOS] Bloqueo con el cursor del pincel moviéndose por la ventana gráfica

**Problemas conocidos:**

&#x200B;* Bloqueo de cálculos en GPU AMD VEGA
&#x200B;* El proceso posterior de distorsión no se tiene en cuenta al exportar en IRay (alfa)

## Versión 3

### 3.4.2 (2017.4.2)

*(Lanzado: 24 de enero de 2018)*

**Agregado:**

&#x200B;* [Exportar] Obtenga el estado de una exportación con el progreso del paso
&#x200B;* [Exportar] Permitir cancelar una exportación
&#x200B;* [Exportar] Exportar texturas a Sketchfab sin perder calidad de mapa de normales
&#x200B;* [Export] Exportación en formato binario glTF (glb)
&#x200B;* [Exportar] Permitir cambiar el tamaño de las columnas en la ficha de configuración de la ventana de exportación
&#x200B;* [Sombreador] Agregar un registro de cambios para la API del sombreador
&#x200B;* [Scripting] Agregar funciones de devolución de llamada Antes y Después al exportar texturas
&#x200B;* [Israel] Actualización a SDK 2017.1 (compatibilidad con las GPU Volta)

**Corregido:**

&#x200B;* Bloqueo al salir de la aplicación antes de mostrar la ventana principal
&#x200B;* [MAC] Bloqueo al cargar mapas en escala de grises con IRA
&#x200B;* [MAC] VRAM detección no es correcta con el nuevo sistema operativo High Sierra
&#x200B;* [Complemento] La descarga de recursos de Substance Source ya no funciona
&#x200B;* [Scripting] Detección de versión mínima de plugin incorrecta
&#x200B;* [Exportar] Error al guardar el ajuste preestablecido de exportación después de exportar texturas
&#x200B;* [Instancing] Problema en generadores instanciados en un TextureSet sin Mapas Adicionales
&#x200B;* [Ventana gráfica] El tramado no funciona con una resolución superior a 4k
&#x200B;* [Ventana gráfica] La visualización de material de vista 2D está cubierta de ruido
&#x200B;* [Estante] Mejorar el tiempo de carga para los ajustes preestablecidos de estante
&#x200B;* [Motor] Fusión incorrecta al pintar en la selección de color

### 3.4.1 (2017.4.1)

*(Lanzado: 15 de diciembre de 2017)*

**Agregado:**

&#x200B;* [Scripting] Exportar malla mediante la API de scripting
&#x200B;* [Importar] Desactivar la importación de formatos de archivo de malla no compatibles (permitir solo obj, fbx, dae, ply)
&#x200B;* [Log] Indique con mayor precisión el problema de TDR en el archivo de registro

**Corregido:**

&#x200B;* Bloqueo si la aplicación se cierra antes de que finalice el rastreo de recursos
&#x200B;* Bloqueo al abrir proyectos con la herramienta Dedo/Clonar
&#x200B;* Bloqueo al utilizar rehacer después de deshacer un cambio de sombreado en la configuración del visor
&#x200B;* [Motor] Las texturas difieren entre Painter 2017.2 y 2017.4
&#x200B;* [Ventana gráfica] Al seleccionar un mapa de ID de una instancia, se muestra un color incorrecto
&#x200B;* bloqueo [Export] al exportar una textura normal o de oclusión no válida
&#x200B;* [Exportar] Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6
&#x200B;* [Plugin] El plugin de Photoshop ignora la selección de canales y siempre exporta todo
&#x200B;* [Capas] Los anclajes se rompen al copiar o pegar entre conjuntos de texturas
&#x200B;* [Capas] Algunas referencias de anclaje no se pueden restaurar si se rompen
&#x200B;* [Sombreador] el parámetro de rugosidad secundaria con revestimiento de pbr está roto
&#x200B;* [Steam] La ventana emergente del comprobador de versiones no debería estar visible al iniciarse

**Problemas conocidos:**

&#x200B;* [AMD] Bloqueos y bloqueos al intentar realizar la pintura en una malla. Se puede solucionar con una actualización del controlador de la GPU.

### 3.4.0 (2017.4.0)

*(Lanzado: 23 de noviembre de 2017)*

**Agregado:**

&#x200B;* [Instanciación] Permite crear instancias de parámetros en capas
&#x200B;* [Instancing] Permite saltar entre una capa de origen y una instancia
&#x200B;* [Instanciación] Añadir una acción &quot;Crear instancias en conjuntos de texturas&quot;
&#x200B;* [Instanciación] Indicar en la pila de capas las instancias de reentrada (ciclos)
&#x200B;* [Instanciación] Elimina instancias cuando se elimina un origen
&#x200B;* [Instanciación] No permitir referencias de delimitador desde fuera de una carpeta con instancias
&#x200B;* [UI] Mueva la pila Deshacer a su propia ventana llamada &quot;Historial&quot;
&#x200B;* [Plugin] Integrar el plugin Live-Link de DCC
&#x200B;* [Motor] Mejore el rendimiento de la pintura con pintura dispersa
&#x200B;* [Exportar] Añadir opciones de borrador y reexportación al exportador de Sketchfab
&#x200B;* [Shelf] Añadir control &quot;flip&quot; para las sustancias de fuentes
&#x200B;* [Estante] Añadir 20 nuevos materiales de procedimientos
&#x200B;* [Estante] Añadir 40 nuevos mapas grunges (basados en mapa de bits y procedimientos)
&#x200B;* [Ventana gráfica] Activar colisiones de previsualización de pincel en otros conjuntos de texturas visibles
&#x200B;* Requisitos mínimos de actualización de controladores de GPU AMD

**Corregido:**

&#x200B;* Bloqueo Al calcular Substance con resoluciones demasiado grandes
&#x200B;* Bloqueo al pintar con partículas
&#x200B;* [Ventana gráfica] Reflejo de specular incorrecto en el Vista 2D con mallas específicas
&#x200B;* [UI] Aparecen algunas acciones no deseadas en la ventana Historial

**Problemas conocidos:**

&#x200B;* [Capas] Algunas referencias de anclaje no se pueden restaurar si se rompen
&#x200B;* Bloqueo al utilizar rehacer después de deshacer un cambio de Sombreador en Configuración del visor

### 3.3.3 (2017.3.3)

*(Lanzado: 01 de diciembre de 2017)*

**Corregido:**

&#x200B;* [Steam] La ventana emergente del comprobador de versiones no debería estar visible al iniciarse
&#x200B;* [Exportar] Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6

### 3.3.2 (2017.3.2)

*(Lanzado: 20 de noviembre de 2017)*

**Agregado:**

&#x200B;* [UI] Mejora el diálogo de la nueva versión y añade el registro de cambios
&#x200B;* [IU] Indique si el mantenimiento ha caducado en el cuadro de diálogo Nueva versión
&#x200B;* [Licencia] Actualizar el sistema de licencias para gestionar las fechas de mantenimiento
&#x200B;* [Exportar] Cambiar nombre de Adobe Standard Material a Adobe Dimension

**Corregido:**

&#x200B;* [Mac] La pintura conduce a cuadrados negros y a corrupciones de textura
&#x200B;* [Motor] La caché puede desaparecer en ocasiones en la ventana gráfica
&#x200B;* [Motor] Aparecen artefactos de bloqueo cuando se activa la compresión de memoria
&#x200B;* [Hacer un bake] Mensajes de error extraños al hacer un bake mallas específicas
&#x200B;* [Export] PSD no se han escrito correctamente y Photoshop no los reconoce correctamente
&#x200B;* [Capas] No debería ser posible copiar y pegar capas en varios proyectos
&#x200B;* [Substance] El espacio de color UserData para la entrada Normal se invierte en algunos casos
&#x200B;* [Estante] Micro-normal en generadores genera curvatura invertida
&#x200B;* [Estante] HSL filtro también afecta al canal alfa
&#x200B;* [Linux] La instalación en Centos falla debido a la falta de dependencias
&#x200B;* El instalador no elimina todos los recursos de la instalación anterior en ciertos casos

### 3.3.1 (2017.3.1)

*(Lanzado: 26 de octubre de 2017)*

**Agregado:**

&#x200B;* [Exportar] Permita exportar la malla desde un proyecto
&#x200B;* [Estante] Quitar &quot;Sub-Shelf&quot; de los títulos de las pestañas
&#x200B;* Guardar la configuración posterior al proceso en plantillas
&#x200B;* Haz que el mensaje TDR sea más comprensible
&#x200B;* Mejorar la ventana Configuración para informar de errores

**Corregido:**

&#x200B;* Bloqueo al borrar varios subestantes
&#x200B;* Bloqueo al cambiar de un nivel a otro durante un cálculo del motor
&#x200B;* bloqueo [Mac] en la GPU Intel durante los cálculos del motor
&#x200B;* [Mac] [Ventana gráfica] Se producen errores de rendimiento cuando el tramado está activado
&#x200B;* [Mac] MacOS 10.13 se reconoce como &quot;Versión desconocida&quot; en el archivo de registro.
&#x200B;* [Baker] Hacer un bake con una jaula ya no funciona
&#x200B;* [Layers] Ctrl+C método abreviado (copia) no funciona más
&#x200B;* [Capas] Al pegar capas, no se actualiza la interfaz de usuario con las referencias del anclaje
&#x200B;* [Anclaje] Duplicar o Copiar/Pegar capa con referencias rompe vínculos
&#x200B;* [Export] En algunos casos, la exportación en 8K puede provocar bloqueos o interbloqueos en las aplicaciones
&#x200B;* [Exportar] Varios problemas en el formato de archivo glTF generado
&#x200B;* [Importar] Volver a importar una malla con el mismo nombre de archivo ya no funciona
&#x200B;* [Plugin] La ventana de guardado automático siempre aparece encima de todo
&#x200B;* [UI] Bucle infinito al pulsar &quot;Escape&quot; en el cuadro de diálogo TDR
&#x200B;* [UI] Restaurar IU muestra una segunda barra de título en la ventana de la estantería

### 3.3.0 (2017.3.0)

*(Lanzado: 28 de septiembre de 2017)*

**Agregado:**

&#x200B;* [Exportar] Permitir la exportación de mallas y texturas para el proyecto de Adobe Felix
&#x200B;* [Export] Permitir la exportación al formato de archivo glTF
&#x200B;* [Motor] Optimice el tamaño de las texturas en VRAM mediante la compresión de bloques
&#x200B;* [Ventana gráfica] Puede arrastrar y soltar una malla o un proyecto en la ventana gráfica
&#x200B;* [UI] Mejora el mensaje de advertencia sobre TDR
&#x200B;* [UI] El registro solo se debe mostrar si se solicita
&#x200B;* [UI] Permitir borrar el contenido de la ventana de registro
&#x200B;* [UI] Mostrar advertencias y errores en la barra de estado
&#x200B;* [UI] Mostrar pestañas en la parte superior como en los navegadores web
&#x200B;* [UI] Mejorar el contexto y los mensajes &quot;no puede pintarse&quot;
&#x200B;* [IU] Añada una acción &quot;guardar como copia&quot; en el menú Archivo
&#x200B;* [Capa] Establecer el ajuste de mosaico predeterminado en 1 de forma predeterminada
&#x200B;* [Shelf] Filtro de degradado mejorado para admitir 10 colores dinámicos
&#x200B;* [Estante] Agregue un espacio en la consulta predeterminada de la miniestantería
&#x200B;* [Estante] Agregue una acción &quot;Abrir en el explorador&quot; para los recursos locales en el estante
&#x200B;* [Estante] Añadir plantilla y sombreador para Adobe Material Estándar (Proyecto Félix)
&#x200B;* [Estante] Aumentar el mosaico máximo a 128 en sombreadores de capas de material
&#x200B;* [Estante] Se ha añadido curvatura sobel para microdetalles de Generadores de máscaras
&#x200B;* [Plugin] Añadir complemento de guardado automático con intervalo de tiempo personalizable
&#x200B;* [Scripting] Añadir una función &quot;Guardar como copia&quot;

**Corregido:**

&#x200B;* [UI] El diseño se interrumpe al iniciarse por primera vez
&#x200B;* El PSD [Export] generado en la exportación tiene errores de formato
&#x200B;* [Exportar] EXR siempre exporta el mapa de altura de 8 bits
&#x200B;* [Exportar] Bloqueo al exportar mapas adicionales dañados
&#x200B;* [Importar] En algunos casos, los bordes duros no se conservan en mallas de polietileno bajas
&#x200B;* [Importar] Mensajes de error mejorados al importar mallas con problemas
&#x200B;* [Baker] Error al Hacer un bake la asignación de ID. si la opción Coincidir por nombre está activada
&#x200B;* [Ventana gráfica] El espacio tangente no se sincroniza con los bakeres
&#x200B;* [Efecto] Al retroceder una capa no se restaura la referencia de un anclaje
&#x200B;* [Efecto] Problema de actualización al crear un vínculo entre dos máscaras con anclajes
&#x200B;* [Efecto] No se deben enumerar los anclajes de máscaras encima de la máscara
&#x200B;* [Efecto] La opción Extraer Alpha de Anclajes no funciona
&#x200B;* [Motor] La máscara se invierte a sí misma tras el primer trazo del pincel
&#x200B;* [Motor] Bloqueo al cambiar el conjunto de texturas en un proyecto específico
&#x200B;* [Shelf] Bloqueo al eliminar un ajuste preestablecido de un proyecto
&#x200B;* [Shelf] Error en el filtro avanzado Tri-Plano
&#x200B;* [Estante] La escala de ruido de MG Mask Builder AO no funciona correctamente
&#x200B;* [Estante] MG Mask Builder tiene parámetros de curvatura invertidos
&#x200B;* [Estante] Los alfa importados generan una previsualización de esfera de material en lugar de una plana

### 3.2.0 (2017.2.0)

*(Lanzado: 27 de julio de 2017)*

**Agregado:**

&#x200B;* Puntos de anclaje: sistema de referencia de capas y máscaras
&#x200B;* [Layers] Capacidad de renombrar efectos de relleno y Pintura
&#x200B;* [Plugin] Complemento de Substance Source actualizado
&#x200B;* [Scripting] Permitir consultar la resolución del conjunto de texturas
&#x200B;* [Scripting] Permite obtener el estado del motor de pintura
&#x200B;* [Performance] Mejoras en la carga de proyectos y en las optimizaciones de estampado de pinceles

**Corregido:**

&#x200B;* [Herramienta] Problemas de rendimiento al ajustar parámetros de material
&#x200B;* [Motor] Trazos de pincel que desaparecen al cambiar la resolución (4K>2K)
&#x200B;* [Vista 3D] El espacio tangente no se sincroniza con los panaderos
&#x200B;* [Estante] La ruta de los estantes en los documentos de usuario no se crea automáticamente
&#x200B;* [Shelf] Hacer ajustes preestablecidos compatibles con versiones anteriores después de una actualización
&#x200B;* [Shader] El sombreado que no sea PBR ya no funciona
&#x200B;* [Bakers] Error de procesamiento de asignación de ID con la opción Coincidir por nombre activada
&#x200B;* [Ejemplo] Los nombres de los conjuntos de texturas del proyecto de muestra Meet Mat son incorrectos
&#x200B;* Guardar un proyecto antes de crear una plantilla devuelve errores de permisos de escritura

### 3.1.0 (2017.1.0)

*(Lanzado: 20 de junio de 2017)*

**Agregado:**

&#x200B;* [Plugin] Nuevo plugin de Substance Source (permite descargar recursos en el estante)
&#x200B;* [Estante] 4 Fuentes Nuevas (Japonés + Chino Simplificado, Typewriter, Segmento)
&#x200B;* [Estante] 230 nuevos Alpha (Mezcla de patrones, pinceles y digitalizaciones de huellas digitales)
&#x200B;* [Estante] 50 Nuevos Procedurales (Patrones de tela de ropa medieval y contemporánea)
&#x200B;* [Estantería] 2 Nuevos mapas ambientales (Mondarrain y Villa Nova Street)
&#x200B;* [Estante] 9 filtros nuevos (Edge Wear de detalle MatFx, abrazadera, HBAO, etc.)
&#x200B;* [Estante] Se ha mejorado el mapa de entorno de panorama predeterminado
&#x200B;* [Shelf] Nuevos ajustes preestablecidos de exportación de Arnold 5
&#x200B;* [Scripting] Permite importar recursos en la estantería

**Problemas conocidos:**

&#x200B;* [Exportar] La edición de un ajuste preestablecido de exportación es muy lenta

## Versión 2

### 2.6.2

*(Lanzado: 20 de octubre de 2017)*

<b>Agregado:</b>

&#x200B;* [Conjunto de texturas] Permitir la eliminación de conjuntos de texturas deshabilitados
&#x200B;* [Estante] Permite que varios usuarios escriban dentro de la misma carpeta de estante
&#x200B;* [Scripting] Poder recargar la carpeta de plugins
&#x200B;* [Scripting] Añada una versión mínima de API necesaria en los metadatos del plugin para garantizar la compatibilidad
&#x200B;* [IRay] Mejoras en el cuadro de diálogo Exportar imagen

<b>Corregido:</b>

&#x200B;* [Motor] Problema de desaparición de trazos al cambiar la resolución (4K>2K)
&#x200B;* [Baker] Error al Hacer un bake la asignación de ID. si la opción Coincidir por nombre está activada
&#x200B;* [Bakeres] Los mensajes de error no son lo suficientemente explícitos
&#x200B;* [Vista 3D] El espacio tangente no se sincroniza con los bakeres
&#x200B;* [Herramienta] Artefactos negros al utilizar la herramienta de difuminado
&#x200B;* [Sombreador] El sombreador que no es PBR ya no funciona
&#x200B;* [Sombreador] &quot;recubierto de pbr&quot; está roto
&#x200B;* [Sombreador] La rugosidad del revestimiento de sombreadores &quot;recubiertos de pbr&quot; ya no tiene impacto
&#x200B;* [Sombreador] El sombreador de brillo de especificaciones no coincide con Iray y SD
&#x200B;* [Shelf] Bloqueo al cargar dos archivos con el mismo nombre pero diferentes extensiones
&#x200B;* [Estante] Ya no se pueden editar los ajustes preestablecidos en los estantes
&#x200B;* [Estante] No se puede establecer una vista previa personalizada para los recursos importados en el estante
&#x200B;* Los recursos cargados desde la caché pierden sus usos
&#x200B;* Guardar un proyecto antes de crear una plantilla devuelve errores de permisos de escritura
&#x200B;* Guardado de proyecto incorrecto si el nombre de archivo contiene dos puntos
&#x200B;* Importación de archivos con varios puntos (.) en el nombre de archivo causa problemas

### 2.6.1

*(Lanzado: 12 de mayo de 2017)*

**Agregado:**

&#x200B;* [TextureSet] No permitir la reasignación de materiales de malla a nada

**Corregido:**

&#x200B;* Bloqueo al cambiar TextureSet después de reemplazar mapa con bake
&#x200B;* Bloqueo al hacer &quot;Deshacer y Rehacer&quot; después de cambiar el modo de fusión de la capa
&#x200B;* Bloqueo o congelación al utilizar el efecto &quot;selección de color&quot; con mapa de ID grande
&#x200B;* [Exportar] Los conjuntos de texturas cuyo nombre se ha cambiado no se ordenan alfabéticamente en la ventana de exportación
&#x200B;* [TextureSet] Restablecer el nombre predeterminado no comprueba la unicidad
&#x200B;* [TextureSet] El conjunto de texturas renombrado se desactiva después de volver a abrir el proyecto
&#x200B;* [Shelf] Falta contenido de plantillas predeterminadas
&#x200B;* [Estante] Las texturas no cuadradas se muestran como cuadradas
&#x200B;* [Sombreador] Cuando se desactiva un conjunto de texturas, se destruye el sombreador asociado
&#x200B;* [Scripting] alg.haga un bake.setTextureSetBakingParameters() ya no funciona
&#x200B;* [Scripting] Tutorial de error tipográfico en websocket
&#x200B;* [Scripting] Varios problemas en AlgWidgets
&#x200B;* [Log] Detección incorrecta de memoria virtual disponible en algunos casos

### 2.6.0

*(Lanzado: 27 de abril de 2017)*

**Agregado:**

&#x200B;* Agregar nuevo proyecto de muestra &quot;Meet Mat&quot;
&#x200B;* [Plugin] Nuevo plugin &quot;Resources Updater&quot;
&#x200B;* [TextureSet] Permite cambiar el nombre de los conjuntos de texturas y añadir una descripción a ellos
&#x200B;* [TextureSet] Permitir reasignar materiales
&#x200B;* [TextureSet] Añadir un botón de configuración en la ventana de lista de conjuntos de texturas
&#x200B;* [TextureSet] Mostrar conjuntos de texturas &quot;desactivados&quot; en la parte inferior de la lista
&#x200B;* [Substance] Utilice mapas adicionales con la resolución actual del conjunto de texturas para mejorar el rendimiento
&#x200B;* [Scripting] Permite actualizar un recurso utilizado en un proyecto (material, generador, etc.)
&#x200B;* [Scripting] Agregar una forma de agregar o quitar un estante
&#x200B;* [Scripting] Permitir consultar información de recursos en proyectos
&#x200B;* [Scripting] Permite recuperar una lista de shelfs disponibles
&#x200B;* [Scripting] Tutorial para mejorar la miniatura de AlgWidget
&#x200B;* [Exportar] Desactivar/Activar profundidad de bits según la compatibilidad con el formato de archivo
&#x200B;* [Log] Añadir nombre de plugin para imprimir en la consola
&#x200B;* [Log] Quitar error sobre conjuntos de texturas ocultos
&#x200B;* Actualizar la pantalla de bienvenida con nuevos iconos y texto para los ejemplos

**Corregido:**

&#x200B;* Bloqueo al actualizar una malla en proyectos específicos
&#x200B;* [Ventana gráfica] El color interior del plano de Simetría ya no es visible
&#x200B;* [Ventana gráfica] Algunos efectos posteriores al proceso se activan al utilizar la vista en solitario
&#x200B;* [Shaders] La fusión &quot;over\_premult&quot; no funciona correctamente
&#x200B;* [Shaders] Advertencia sobre la prueba alfa con el sombreador predeterminado
&#x200B;* [Shelf] Análisis incorrecto de etiquetas de Substance
&#x200B;* [Shelf] El intemperismo del Óxido MatFX no funciona correctamente
&#x200B;* [Shelf] HSL filtro está activado de forma predeterminada en canales incorrectos
&#x200B;* [Estante] El enfoque está activado de forma predeterminada en el canal Height/Normal
&#x200B;* [Exportar] Los ajustes preestablecidos de exportación no utilizan un mapa de normales OpenGL
&#x200B;* [Herramienta] Problemas de imprecisión al crear artefactos con la herramienta clonar/difuminar

### 2.5.3

*(Lanzado: 15 de marzo de 2017)*

**Corregido:**

&#x200B;* [Baker] Bloqueo al hacer un bake con mallas específicas

**Problemas conocidos:**

&#x200B;* [Mac] Las partículas pueden dañar la textura en algunos casos

### 2.5.2

*(Lanzado: 14 de marzo de 2017)*

**Corregido:**

&#x200B;* [Herramienta] Las tabletas Wacom no funcionan en Linux
&#x200B;* [Herramienta] Artefactos negros al utilizar la herramienta de difuminado
&#x200B;* [Baker] Se produce un error al Hacer un bake si se utiliza la coincidencia por nombre con una jaula
&#x200B;* [Bakeres] Oclusión ambiental rota al hacer un bake solo con Mapa de normales
&#x200B;* [Shelf] Los filtros genéricos no manejan alfa correctamente (contraste/luminosidad, paso alto, etc.)
&#x200B;* [Ventana gráfica] Problema de rendimiento al cargar un proyecto con sombras activadas
&#x200B;* [Ventana gráfica] Problema de tramado en Vista 3D en MacOS
&#x200B;* [Ventana gráfica] Las previsualizaciones de objetos se muestran incorrectamente cuando el perfil de color está activado
&#x200B;* [Iray] Bloqueo al volver a cambiar el proyecto a OpenGL si Iray no se inicializa
&#x200B;* El Brillo [IRay] se omite al procesar el sombreador SpecGloss/mdl
&#x200B;* [Sombreador] El sombreador Spec/Gloss no coincide con Iray y SD
&#x200B;* [Sombreador] La conversión de sRGB difiere de la conversión de LUT lineal a sRGB
&#x200B;* [Sombreador] Procesamiento incorrecto al cargar el proyecto con sombreadores obsoletos
&#x200B;* [Sombreador] Los sombreadores &quot;recubiertos de pbr&quot; ya no funcionan
&#x200B;* [Exportar] Algunos canales aún se exportan aunque no estén presentes en el conjunto de texturas
&#x200B;* [Capas] El modo de fusión &quot;mapa de normales de detalle inverso&quot; no funciona en canales en escala de grises
&#x200B;* [UI] Problema en &quot;Ventana de selección de color&quot; con monitor HDPI y zoom de visualización al 150 %

**Problemas conocidos:**

&#x200B;* [Mac] Las partículas pueden dañar la textura en algunos casos

### 2.5.1

*(Lanzado: 27 de febrero de 2017)*

**Corregido:**

&#x200B;* [Mac] La entrada de la tableta Wacom se rompe en 3D y Vista 2D
&#x200B;* [Bakeres] La coincidencia por nombre ya no funciona
&#x200B;* [Bakeres] El ajuste &quot;Normales medias&quot; ya no funciona
&#x200B;* [Iray] Procesamiento incorrecto con falta de mapa de normales hecho un bake
&#x200B;* [Iray] Los perfiles de color se comportan de forma diferente en comparación con el procesador OpenGL
&#x200B;* [Iray] Al exportar el procesamiento como mapa de bits, no se incluye la corrección del perfil de color
&#x200B;* [Substance] Los Filtros de material ya no funcionan
&#x200B;* [Herramienta] La opacidad del trazo no se almacena en los ajustes preestablecidos del pincel
&#x200B;* [Herramienta] La alineación UV del pincel del Clonar ya no funciona
&#x200B;* [Exportar] El canal de Desplazamiento debe estar centrado en 0,5 al exportar en entero
&#x200B;* [Plantilla] La ruta absoluta se almacena en Plantillas
&#x200B;* [TextureSet] La textura del canal se mantiene después de quitar el canal

**Problemas conocidos:**

&#x200B;* [Linux] Las entradas de tabletas Wacom no funcionan en 3D ni en Vista 2D
&#x200B;* [Mac] Las partículas pueden dañar la textura en algunos casos
&#x200B;* [Exportar] En casos muy raros, pueden aparecer rectángulos negros en las GPU AMD

### 2.5.0

*(Lanzado: 21 de febrero de 2017)*

**Agregado:**

&#x200B;* Compatibilidad añadida para las GPU AMD Radeon Pro y AMD FirePro
&#x200B;* [Herramienta] Compatibilidad añadida con la opacidad del trazo
&#x200B;* [Herramienta] Agregue un modificador que permita continuar con el último trazo de pincel
&#x200B;* [Iray] Actualización compatible con las GPU Pascal
&#x200B;* [Ventana gráfica] Compatibilidad añadida con perfiles de color (LUT)
&#x200B;* [Substance] Integrar nueva estructura (motor SD6)
&#x200B;* [UI] Aumentar la lista de tamaño de &quot;archivo reciente&quot; en el menú Archivo
&#x200B;* [Importar] Utilice la categoría de sustancias para rellenar el prefijo en el cuadro de diálogo de importación
&#x200B;* [Bakeres] Permitir hacer un bake texturas 8K
&#x200B;* [Bakeres] Permitir hacer un bake resoluciones no cuadradas
&#x200B;* [Bakeres] Mejora el consumo de memoria al hacer un bake mallas pesadas de alto contenido de poli
&#x200B;* [Estante] Bloquear estantes (y proyectos) para prohibir la edición simultánea y evitar daños
&#x200B;* [Shelf] Lea la categoría y las palabras clave de las sustancias para usarlas para filtrar
&#x200B;* [Shelf] Permite excluir recursos del resultado de una consulta de búsqueda
&#x200B;* [Shelf] Cálculo del tiempo de las miniaturas mejorado
&#x200B;* [Estante] Permitir la incrustación de ajustes preestablecidos en proyectos
&#x200B;* [Estante] Permita contraer o expandir rápidamente la vista de árbol con MAYÚS
&#x200B;* [Estante] Permite guardar miniaturas cuando los recursos son de solo lectura (caché local)
&#x200B;* [Estante] Nuevo contenido : nuevos filtros (transformar, espejo, tri-plana, etc.)
&#x200B;* [Estante] Nuevo contenido : nuevos perfiles de LUT (clásicos y artísticos, como Film Noir, Vintage, etc.)
&#x200B;* [Estante] Nuevo contenido : 10 nuevos Substance de fuentes para generar rápidamente textos personalizados
&#x200B;* [Estante] Nuevas plantillas : Unity 5 y Unreal Engine 4
&#x200B;* [Estante] Se ha mejorado el filtro de HSL para que sea más fácil de usar por los artistas
&#x200B;* [Sombreador] Se ha agregado la compatibilidad con el canal de specular level en sombreadores PBR
&#x200B;* [Sombreador] Añadir soporte para tramado en sombreador de prueba de Alpha
&#x200B;* [Sombreador] Añadir compatibilidad para la asignación de oclusión de paralaje en sombreadores PBR
&#x200B;* [Sombreador] Permite definir una interfaz de usuario personalizada para los parámetros de sombreador.
&#x200B;* [MatLayering] Creación de un nuevo canal de máscara para el flujo de trabajo de capas de materiales
&#x200B;* [Scripting] Permita escribir metadatos en un proyecto de SP
&#x200B;* [Scripting] Permitir la exportación con un ajuste preestablecido de exportación específico
&#x200B;* [Scripting] Permite recuperar parámetros de sombreador como JSON
&#x200B;* [Scripting] Agregar compatibilidad para conexiones WebSocket
&#x200B;* [Scripting] Añadir la posibilidad de cargar instancias del sombreador
&#x200B;* [Scripting] Añadir la posibilidad de crear un nuevo proyecto
&#x200B;* [Scripting] Permite recuperar la URL de la malla importada en un proyecto
&#x200B;* [Scripting] Permitir hagas un bake no cuadrados
&#x200B;* [Scripting] Informar de errores al configurar datos mediante la API de scripts
&#x200B;* [Substance] Añadir etiqueta de datos de usuario para especificar el formato de mapa de normales

**Corregido:**

&#x200B;* Bloqueo al elegir color con substancias
&#x200B;* Bloqueo al cargar una imagen que no es RGBA32f como mapa de entorno
&#x200B;* Bloqueo relacionado con la pintura en GPU AMD
&#x200B;* [Mesh] OBJ importación no reconoce materiales sin el archivo mtl
&#x200B;* [Mesh] La generación del nombre del conjunto de texturas del UDIM puede ser incorrecta en algunas mallas
&#x200B;* [UI] Botón Deshacer/Rehacer en la configuración del visor para robar el foco y detener el desplazamiento del ratón
&#x200B;* [UI] Algunas etiquetas se recortan incorrectamente en alta resolución
&#x200B;* [Capa] El modo de sustitución del efecto pintura se comporta de forma incorrecta en Máscara
&#x200B;* El modo de fusión de Restar [Layer] se comporta de forma incorrecta con alfa
&#x200B;* [Herramienta] El tamaño del pincel se vuelve enorme en vista 2D al pintar en bordes UV
&#x200B;* [Herramienta] La línea recta ajustada tiene un comportamiento errático con alta PPP
&#x200B;* [Herramienta] La resolución de la galería de símbolos a veces es incorrecta
&#x200B;* [Bakeres] Los valores de &quot;Distancia máxima del oclusor&quot; se fijan si &quot;relativo al cuadro delimitador&quot; está &quot;Desactivado&quot;
&#x200B;* [Sombreador] Las definiciones de canal de pilas y parámetros automáticos no coinciden
&#x200B;* [Vista 3D] Visualización incoherente del canal normal según la configuración del proyecto
&#x200B;* [Ventana gráfica] Algunos mapas de normales tienen valores sujetos que aparecen como artefactos
&#x200B;* [Ventana gráfica] Los efectos posteriores siempre están desactivados de forma predeterminada
&#x200B;* [Exportar] El ajuste de mezcla normal es incorrecto si falta un canal normal
&#x200B;* [Exportar] Generación de textura incorrecta en algunos casos en GPU AMD
&#x200B;* [Exportar] Los parámetros de Sombreador no se exportan correctamente si se encuentran dentro de un grupo
&#x200B;* [Exportar] Al editar un ajuste preestablecido de exportación en una estantería personalizada, se genera un error de registro
&#x200B;* [Shelf] El filtrado de vista de árbol no coincide exactamente con el nombre de la carpeta
&#x200B;* [Estante] Es difícil cambiar el nombre de un ajuste preestablecido de estante
&#x200B;* [Estante] El recurso de Sombreador importado en la Estantería no se conserva después de reiniciar
&#x200B;* [Estante] Contenido : Falta el ajuste preestablecido de la herramienta Soldadura
&#x200B;* [Estante] Contenido : El Tile Generator no funciona correctamente
&#x200B;* [Estante] Contenido : Se ha corregido una máscara incorrecta en el material inteligente sucio del neumático de goma
&#x200B;* [Estante] Contenido : Se ha corregido un nombre de grupo incorrecto en el material de la bolsa de cuero
&#x200B;* [Iray] La mitad de las mallas están desaparecidas en Irak
&#x200B;* [Linux] Bloqueo al arrastrar un recurso sobre la Vista 3D
&#x200B;* [Mac] Las preferencias se restablecen en cada inicio en Sierra

**Problemas conocidos:**

&#x200B;* [Exportar] En casos muy raros, pueden aparecer rectángulos negros en las GPU AMD
&#x200B;* [Iray] Los perfiles de color pueden comportarse de formas extrañas a veces

### 2.4.1

*(Lanzado: 28 de octubre de 2016)*

**Corregido:**

&#x200B;* Bloqueo al crear un proyecto con una plantilla
&#x200B;* Bloqueo al cerrar el cuadro de diálogo de exportación durante una exportación
&#x200B;* [Mac] Errores al guardar el proyecto (error al guardar el ajuste preestablecido de exportación)
&#x200B;* [Shelf] Al crear un nuevo ajuste preestablecido, este se mostrará dos veces
&#x200B;* [Estante] Los ajustes preestablecidos no se pueden cargar en modo de solo lectura sin derechos de administrador

### 2.4.0

*(Lanzado: 27 de octubre de 2016)*

**Agregado:**

&#x200B;* [Shelf] Nueva interfaz para examinar los recursos (vista de árbol, filtros, etc.)
&#x200B;* [Estante] Permitir guardar una búsqueda como ajuste preestablecido
&#x200B;* [Estante] Permite crear una nueva ventana a partir de un ajuste preestablecido
&#x200B;* [Shelf] Nueva interfaz para importar recursos
&#x200B;* [Shelf] No copiar la bandeja algorítmica predeterminada en la carpeta Documentos
&#x200B;* [Shelf] Nuevos ajustes preestablecidos de partículas : Circuito eléctrico, Líneas eléctricas, Rococó, Venas pequeñas
&#x200B;* [Estante] Se han mejorado los ajustes preestablecidos de partículas antiguas para que sean más fáciles de usar (como &quot;Lluvia&quot;).
&#x200B;* [Shelf] Añadir nueva información en el menú contextual de recursos
&#x200B;* [Viewport] Mejora del rendimiento al cargar mapas de entorno
&#x200B;* [Viewport] Añada compatibilidad con mapas de entorno que no sean potencia de dos

**Corregido:**

&#x200B;* Bloqueo al quitar una máscara
&#x200B;* Bloqueo al pintar después de guardar un ajuste preestablecido
&#x200B;* Bloqueo con el desenfoque de entorno en algunas GPU
&#x200B;* Bloqueo al asignar un recurso incorrecto con el estante mini
&#x200B;* [Estante] Limpiar y guardar las etiquetas y los metadatos de eliminación de los recursos del proyecto
&#x200B;* [Estante] al importar un ajuste preestablecido, sus recursos se mostrarán en el estante
&#x200B;* [Exportar] El mapa normal generado a partir del canal de height tiene una intensidad baja
&#x200B;* [Exportar] Normal desde malla no siempre está presente en el mapa normal final
&#x200B;* [Exportar] La dilación con transparencia puede resultar en ocasiones sin transparencia
&#x200B;* [Scripting] &quot;alg.plugin\_root\_directory&quot; puede devolver una ruta de red truncada
&#x200B;* El botón Bloquear [TextureSet] se activa al volver a abrir proyectos no cuadrados

### 2.3.1

*(Lanzado: 07 de octubre de 2016)*

**Agregado:**

&#x200B;* [Plugin] [Photoshop] Permite especificar qué material/pila/canales se van a exportar
&#x200B;* [Scripting] Los nombres de función tienen algunas incoherencias

**Corregido:**

&#x200B;* [Export] El Alpha se puede descartar en los ajustes preestablecidos de exportación personalizados
&#x200B;* [Exportar] El Alpha obtiene una conversión de gamma incorrecta en canales sRGB
&#x200B;* [Exportar] Los documentos no cuadrados se exportan como cuadrados
&#x200B;* [Exportar] No es posible exportar mapas adicionales si falta uno
&#x200B;* [Iray] Algunos parámetros (como la Intensidad del emisivo) no tienen efecto
&#x200B;* bloqueo [NVIDIA] al inicio con NVIDIA Quadro K2200/GTX 750/760
&#x200B;* [AMD] Conjunto incorrecto de colores para miniaturas y vistas previas
&#x200B;* [AMD] Bloqueos y error del controlador al abrir archivos nuevos y abiertos
&#x200B;* [Log] Falta &quot;software-version&quot; en el archivo de registro

### 2.3.0

*(Lanzado: 15 de septiembre de 2016)*

**Agregado:**

&#x200B;* [Plugin] Nuevo plugin &quot;Exportar a Photoshop&quot; (exportar pila de capas completa)
&#x200B;* [Exportar] Permite especificar la anchura del relleno (en píxeles o infinito)
&#x200B;* [Exportar] Permite definir el tipo de fondo fuera de las UV
&#x200B;* [Estante] sombreador de capas de material nuevo para mezclar 10 materiales
&#x200B;* [Estante] Nuevo sombreador de arcilla para ver los detalles con el height / canal normal
&#x200B;* [Estante] Nuevo filtro de iluminación hecho un bake con entrada de entorno
&#x200B;* [Estante] Se han actualizado algunos generadores de máscaras para añadir transformaciones que no son cuadradas
&#x200B;* [Ventana gráfica] Añadir mapa de normales compuesto (normal+height+hacer un bake) al modo solo
&#x200B;* [Scripting] Permitir la exportación de mapas adicionales
&#x200B;* [Scripting] Permitir consultar mapas adicionales disponibles por conjunto de texturas
&#x200B;* [Scripting] Permitir recuperar el formato de canal
&#x200B;* [Scripting] Añadir ejemplos en la documentación de haga un bake
&#x200B;* [Scripting] Permite consultar la visibilidad de una capa
&#x200B;* [Scripting] Permite consultar el modo de fusión y la opacidad de la capa
&#x200B;* [Scripting] Permite exportar mapas convertidos (mapas de normales finales, archivos AO mixtos, etc.)
&#x200B;* [Substance] Lectura y conexión de usos personalizados
&#x200B;* [Métodos abreviados] Añadir tecla modificadora (MAYÚS) para retroceder en el modo solo cíclico
&#x200B;* [Exportar] Se ha actualizado el ajuste preestablecido de exportación predeterminado para desactivar alfa.
&#x200B;* [UI] Las miniaturas ahora solo se calculan si el motor está disponible
&#x200B;* [UI] Mostrar una mención cuando las miniaturas se están calculando

**Corregido:**

&#x200B;* Bloqueo con algunos proyectos antiguos al abrirlos
&#x200B;* Bloqueo con caché de canales de textura dañada
&#x200B;* Bloqueo al mezclar más de 4 materiales con el flujo de trabajo de capas de material
&#x200B;* [UI] Los métodos abreviados de herramientas no funcionan si la barra de herramientas está oculta
&#x200B;* [UI] La barra de herramientas de Iray se etiqueta &quot;Sin título&quot; en el menú Ver
&#x200B;* [UI] Las barras de herramientas de los complementos se denominan &quot;Sin inclinación&quot; en el menú Ver
&#x200B;* [Baker] Al pulsar Intro mientras se edita un ajuste de hacer un bake, se inicia el proceso de hacer un bake
&#x200B;* [Baker] Rangos incorrectos para algunos parámetros
&#x200B;* [Importar] Imposible importar OBJ mallas debido a números muy grandes
&#x200B;* [Importar] Algunos archivos OBJ se importan con demasiados subobjetos
&#x200B;* [Exportar] el fondo del canal se rellena con negro en lugar del color predeterminado en la exportación
&#x200B;* [Herramienta] Las partículas no funcionan correctamente si FOV es demasiado bajo
&#x200B;* [Herramienta] El color de previsualización del pincel es incorrecto con las máscaras en las subpilas
&#x200B;* [Ventana gráfica] Cuando el pincel entra en áreas vacías de la Vista 2D se vuelve gigantesco
&#x200B;* [Ventana gráfica] Vista previa del pincel en blanco al pintar texturas normales
&#x200B;* [Scripting] Documentación incorrecta: &quot;ao&quot; en lugar de &quot;ambientocclusion&quot;
&#x200B;* [Scripting] El proceso iniciado con subprocess() se cierra al cerrar Painter
&#x200B;* [Estante] El filtro de iluminación Hecho un bake utiliza una entrada de AO incorrecta
&#x200B;* [MacOS] Se ha eliminado el proyecto Fire Hydrant (incompatible).
&#x200B;* El proyecto predeterminado se abre al cargar un archivo \*.spt (en lugar de \*.spp)

**Problemas conocidos:**

&#x200B;* [Plugin] Debido a Photoshop, el height y el canal normal no se pueden traducir tal cual

### 2.2.0

*(Lanzado: 22 de julio de 2016)*

**Agregado:**

&#x200B;* [Estante] Mejorar el sistema de búsqueda y las consultas
&#x200B;* [Estante] Añadir campo de búsqueda para miniestantes
&#x200B;* [Sombreador] Permite definir la precisión de paso de los reguladores
&#x200B;* [Sombreador] Añadir un botón Deshacer/Rehacer para parámetros de sombreador
&#x200B;* [Sombreador] La recarga de un sombreador no debe restablecer sus parámetros
&#x200B;* [MatLayering] Añadir compatibilidad para Controles dinámicos de capas de materiales y subpilas
&#x200B;* [MatLayering] Permita importar el archivo json para configurar los ajustes de sombreador
&#x200B;* [MatLayering] Desbloquear el límite de muestras de textura (cambiar a texturas sin enlace)
&#x200B;* [Scripting] Permite establecer la configuración de bakeres e iniciar su cálculo
&#x200B;* [Substance] Usar &quot;usage&quot; para conexiones de entradas/salidas además de identificadores
&#x200B;* [Herramienta] Permite seleccionar el canal de previsualización en la ventana gráfica de la herramienta Proyección

**Corregido:**

&#x200B;* Bloqueo durante el lanzamiento si las sustancias se encuentran en una carpeta incorrecta
&#x200B;* El informe de bloqueo a veces no funciona debido a un archivo de registro incorrecto
&#x200B;* [Iray] Los Efectos de posprocesamiento no se actualizan cuando Iray está en pausa
&#x200B;* [Iray] El método abreviado de enfoque automático ya no funciona
&#x200B;* [Iray] El comportamiento del regulador de apertura cambia en función del tamaño del activo
&#x200B;* [Capas] El primer canal de materiales no está activado de forma predeterminada si todos están desactivados
&#x200B;* [Sombreador] No se imprimen errores si un &quot;param auto&quot; es incorrecto

**Problemas conocidos:**

&#x200B;* [Mac] El límite de muestras de Textura está bloqueado en 16 (problema del controlador de la GPU)

### 2.1.1

*(Lanzado: 01 de julio de 2016)*

**Agregado:**

&#x200B;* [Licencia] Cambiar la ubicación del archivo de licencia
&#x200B;* [Ventana gráfica] Añada un método abreviado &quot;B&quot; para desplazarse entre mapas adicionales
&#x200B;* [Importar] Permitir la importación FBX 2016/2017 correctamente
&#x200B;* [Herramienta] Quitar fichas al utilizar la máscara rápida
&#x200B;* [Iray] Añadir información de dimensiones de escena
&#x200B;* [Iray] Permita aumentar el número máximo de muestras y el tiempo de procesamiento
&#x200B;* [UI] Actualizar el resultado inmediatamente al utilizar el botón +/- en los reguladores
&#x200B;* [UI] Mayor precisión de los reguladores de escala de grises
&#x200B;* [Exportar] No exportar un canal alfa para texturas que solo sean de RGB
&#x200B;* [Exportar] Actualizar ajuste preestablecido de exportación de Dota 2
&#x200B;* [Estante] Nuevo patrón de &quot;Azulejos hexagonales&quot;
&#x200B;* [Estante] Nueva herramienta &quot;Soldadura&quot;
&#x200B;* [Estante] Filtros de acabado actualizados para proporcionar controles de dirección

**Corregido:**

&#x200B;* [Export] Imposible exportar archivos de PSD en 8 bits
&#x200B;* [Exportar] La exportación en 8K no está disponible en algunas configuraciones de hardware
&#x200B;* [Exportar] La ventana de Sketchfab se recorta
&#x200B;* [Exportar] Mapa de rugosidad incorrecto en el ajuste preestablecido de exportación de especificaciones/brillo
&#x200B;* [UI] Escribir en los reguladores de escala de grises ya no funciona
&#x200B;* [UI] Imposible colocar filtros en las entradas de sustancias (como Generadores)
&#x200B;* [UI] Algunos reguladores tienen comportamientos extraños
&#x200B;* [UI] El paso DeltaTime +/- para partículas es demasiado grande
&#x200B;* [Iray] Algunos proyectos bloquean la aplicación al cambiar a Iray
&#x200B;* [Iray] Bloqueo al detectar hardware
&#x200B;* [Herramienta] El color de previsualización del pincel es incorrecto en el modo Máscara
&#x200B;* [Herramienta] El selector de materiales se puede utilizar con herramientas incompatibles
&#x200B;* [Herramienta] La previsualización de proyección no cambia al flujo de trabajo Difusión con especificación/brillo
&#x200B;* [Estante] Al cambiar el sombreado predeterminado, se rompen las previsualizaciones de máscaras inteligentes/máscaras inteligentes
&#x200B;* [Estante] Algunos materiales inteligentes tienen nombres incorrectos
&#x200B;* [Shelf] Las formas alfa adicionales están dañadas y no se cargan
&#x200B;* [Viewport] Al cambiar al modo &quot;Mapa adicional&quot;, se muestra primero &quot;otro&quot;
&#x200B;* [Ventana gráfica] La ventana gráfica vuelve a cambiar a &quot;otro&quot; cuando no existe ningún mapa adicional
&#x200B;* [Crash]&#x200B;[Linux] El informe de fallos no funciona en Ubuntu (Steam)
&#x200B;* [Crash]&#x200B;[Linux] Los vínculos de URL web no funcionan en Ubuntu (Steam)
&#x200B;* [Bloqueo] [Windows] Quitar &quot;Crashwatcher&quot; cuando Substance Painter ya no se ejecuta
&#x200B;* [Bloqueo] [Mac] El sistema de informes de fallos no funciona correctamente
&#x200B;* [Bloqueo] Importar una malla mientras se importa una malla provoca un bloqueo
&#x200B;* El método abreviado de selección de conjunto de texturas se restablece en nada después de reiniciar

### 2.1.0

*(Lanzado: 02 de junio de 2016)*

**Agregado:**

&#x200B;* [UDIM] Importación de mosaicos UDIM de una malla como conjuntos de texturas
&#x200B;* [Linux] Se ha agregado la compatibilidad con CentOS 6.6 y Ubuntu 12.4
&#x200B;* [Exportar] Añadir resolución 8K (experimental)
&#x200B;* [Exportar] Permite elegir la profundidad de bits durante la exportación
&#x200B;* [Baker] Permita hornear varios conjuntos de texturas a la vez
&#x200B;* Compatibilidad con monitores de alta resolución (escala de PPP alta)
&#x200B;* [Scripts] Establecer resolución y relleno personalizados por textura en la exportación
&#x200B;* [Ventana gráfica] Permite cambiar entre el conjunto de texturas haciendo clic en la malla (mediante Ctrl+Alt+Clic)
&#x200B;* [Ventana gráfica] Vaya a donde se encuentra el cursor del ratón al hacer zoom con la rueda del ratón
&#x200B;* [UI] Actualizar la visualización predeterminada del color de fondo y el mapa de entorno
&#x200B;* [UI] Añadir información sobre herramientas con nombres originales para los canales de usuario
&#x200B;* [UI] Cambiar el color de fondo de los canales a los que no se puede cambiar el nombre
&#x200B;* [Herramienta] Quitar fichas al utilizar la máscara rápida
&#x200B;* [Sombreador] Permite definir grupos para parámetros de sombreador y materiales/máscaras
&#x200B;* [Motor] Optimización del estampado de tamaño pequeño
&#x200B;* [Stencil] Añada &quot;W&quot; como método abreviado para cambiar temporalmente la máscara
&#x200B;* [Estante] Añada un botón de cruz para borrar el campo de búsqueda
&#x200B;* [Estante] Cargar el Alpha con un solo clic
&#x200B;* [Shelf] Nuevo ajuste preestablecido de exportación : UDIM Vray, Arnold UDIM, Especificación/Brillo de Metal/Rugoso
&#x200B;* [Shelf] Nuevos alfa : formas geométricas, vetas y signos
&#x200B;* Agregar nombre y versión en las propiedades del ejecutable de Substance Painter

**Corregido:**

&#x200B;* [Substance] Imposible utilizar el canal normal y el mapa adicional al mismo tiempo
&#x200B;* [Iray] La refracción de MDL y el ajuste de absorción no funcionan
&#x200B;* [Iray] No se conserva la escala de escenas original
&#x200B;* [Estante] El Specular/plantilla de Brillo usa un sombreador incorrecto
&#x200B;* [Exportar] El ajuste preestablecido de exportación predeterminado no exporta algunos mapas (como AO)
&#x200B;* [Ventana gráfica] El punto de tabla dinámica no se actualiza al hacer clic fuera de las coordenadas UV en la vista 2D
&#x200B;* [UI] Los valores del regulador se redondean
&#x200B;* [UI] A veces, al editar los valores de los reguladores, hay un espacio libre muy pequeño
&#x200B;* [Nuevo proyecto] La lista desplegable de plantillas no se ha actualizado correctamente (de 1.x a 2.x)
&#x200B;* [Scripts] Se ha corregido el comportamiento de &quot;pasar cursor&quot; en los botones personalizados
&#x200B;* [Mac] Al deshacer un proyecto vacío, se bloquea la cámara

**Problemas conocidos:**

&#x200B;* El informe de bloqueo no está disponible en Ubuntu
&#x200B;* Es posible que algunos botones de URL no funcionen. Consulta nuestras preguntas frecuentes para obtener una solución alternativa

### 2.0.5

*(Lanzado: 29 de abril de 2016)*

**Agregado:**

&#x200B;* [Estante] Se ha añadido o actualizado una plantilla que no es de pbr, sombreador y ajuste preestablecido de exportación
&#x200B;* [Estante] Se ha actualizado el ajuste preestablecido de exportación UE4 para incluir la Oclusión ambiental

**Corregido:**

&#x200B;* Bloqueo al abrir y guardar algunos proyectos con recursos dañados
&#x200B;* [Ventana gráfica] La Malla metálica aparece rota en la Vista 2D
&#x200B;* [Shelf] Rendimiento mejorado de algunos mapas de entorno de estudio
&#x200B;* [Shelf] Algunos mapas de entorno de estudio están duplicados
&#x200B;* [Estante] Falta &quot;Material de iluminación Hecho un bake&quot;
&#x200B;* [Shelf] Falta el generador de conversión de escala de grises

### 2.0.4

*(Lanzado: 26 de abril de 2016)*

**Agregado:**

&#x200B;* Mejora de los choques de malla y optimiza la representación de mallas metálicas
&#x200B;* Mejorar el rendimiento y la gestión de la memoria con grandes proyectos
&#x200B;* Mejorar la precisión y el paso del regulador
&#x200B;* [UI] El motor de actualización solo se actualiza al validar un control deslizante (no al introducir un valor).
&#x200B;* [UI] Mover Iray cambiar a un botón dedicado en la barra de herramientas principal (y cambiar su método abreviado)
&#x200B;* [Herramienta] Agregar configuración para el comportamiento de ubicación de origen de la herramienta de clonación
&#x200B;* [Sombreador] Permitir la lectura de colores de vértices de malla en sombreadores personalizados
&#x200B;* [Scripting] Permite recuperar la lista de conjuntos de texturas, canales y capas
&#x200B;* [Scripting] Añadir funciones auxiliares (url a ruta, obtener ruta de exportación del proyecto)
&#x200B;* [Mac] Detectar la versión &quot;El Capitan&quot; de Mac Os en el archivo de registro

**Corregido:**

&#x200B;* Bloqueo después de la segunda exportación a Substance share
&#x200B;* Bloqueo al copiar una capa entre conjuntos de texturas con datos de Máscara rápida.
&#x200B;* Algunos proyectos tienen un actualizador muy largo que consume mucha memoria
&#x200B;* [Herramienta] Bloqueo al seleccionar un ajuste preestablecido de objeto con la herramienta de clonar/difuminar
&#x200B;* [Baker] La carga de archivos de FBX tarda demasiado en ejecutarse en mallas pesadas
&#x200B;* [Viewport] Mapa de entorno Estirado en algunos equipos
&#x200B;* [Ventana gráfica] Conversión de gamma incorrecta del alfa del pincel
&#x200B;* [Export] Alpha se almacena como transparencia en lugar de como canal independiente con archivos Tiff.
&#x200B;* [Exportar] El canal normal siempre se exporta como OpenGL
&#x200B;* [Iray] Faltan nombres de reguladores para la configuración de Iray
&#x200B;* [Iray] El procesamiento se realiza con una resolución incorrecta en Retina/High DPI
&#x200B;* [Iray] Bloqueo al cambiar el tamaño de la interfaz en modo Iray
&#x200B;* [Israel] Gran ralentización del rendimiento al renderizar en algunas resoluciones bajas
&#x200B;* [Iray] La pausa no funciona (Iray sigue computando en segundo plano)
&#x200B;* El canal normal a veces tiene defectos de cuadrados negros
&#x200B;* El canal normal se invierte mediante filtros de escala de grises
&#x200B;* El canal normal no se fusiona correctamente si la pila tiene alfa
&#x200B;* El proyecto se edita en el disco al abrir un proyecto aunque no se haya guardado todavía
&#x200B;* La reimportación de una malla en algunos proyectos produce un rendimiento de GPU muy malo
&#x200B;* La orientación del pincel no es correcta al no tocar una malla
&#x200B;* Falta el logotipo de substance share en la pantalla de bienvenida

### 2.0.2

*(Lanzado: 25 de marzo de 2016)*

**Agregado:**

&#x200B;* [Iray] Actualizar la plantilla Spec/Gloss y el sombreador para que sean compatibles con Iray
&#x200B;* [Exportar] Exportar capturas de pantalla a ArtStation
&#x200B;* [Scripting] Ejecución de soporte desde el directorio de plugins
&#x200B;* [Scripting] Permitir &quot;Guardar como&quot;
&#x200B;* [UI] Permita hacer doble clic en un regulador para editar su valor
&#x200B;* Mover muestra de Vela al Substance share
&#x200B;* Nuevo proyecto de muestra : Previsualización de esfera
&#x200B;* Advertencia a los usuarios sobre el conflicto de extensión de shell

**Corregido:**

&#x200B;* El instalador anula la instalación de Substance Painter 1.x
&#x200B;* [UI] El diseño de la lista de canales se rompe con los filtros
&#x200B;* [UI] No se muestran los parámetros de Sombreador
&#x200B;* [UI] Cambiar el tamaño de la ventana de capa recorta incorrectamente el contenido
&#x200B;* [Herramienta] El canal de opacidad no siempre se usa correctamente
&#x200B;* [Herramienta] El difuminado/Clonar no funciona con la Simetría
&#x200B;* [Herramienta] La opacidad de la vista previa del pincel es incorrecta en algunos canales
&#x200B;* [Iray] Bloqueo al utilizar Iray cuando todavía no se ha creado
&#x200B;* [Iray] No se pueden cargar datos de configuración de iris del proyecto
&#x200B;* [Iray] Iray no se ocupa de la modificación de la configuración después de haber sido pausado
&#x200B;* [Estante] Importar un material al estante no funciona
&#x200B;* La galería de símbolos no funciona con el canal Normal
&#x200B;* Bloqueo al pintar en algunos proyectos
&#x200B;* Bloqueo al pintar con partículas en algunos proyectos
&#x200B;* Bloqueo con el Procesador de píxeles durante algunos cálculos

### 2.0.0

*(Lanzado: 16 de marzo de 2016)*

**Agregado:**

&#x200B;* Método abreviado a Substance Almacén en la barra de herramientas principal
&#x200B;* Procesador Iray con modo de visualización y exportación de capturas de pantalla
&#x200B;* Compatibilidad con la creación y el uso de &quot;Máscaras inteligentes&quot;
&#x200B;* Compatibilidad con el flujo de trabajo de PBR de Specular y glosinas (con el nuevo canal difuso)
&#x200B;* Encadenamiento de Substance (enchufe de sustancias en las entradas de imagen de sustancias)
&#x200B;* Compatibilidad de scripts con complementos personalizados
&#x200B;* Mejorar la conversión de Height a Normal utilizando un filtro Sobel
&#x200B;* Cambiar resolución de previsualización de proyección/galería de símbolos a 2K
&#x200B;* Agregar canal normal de forma predeterminada para proyectos nuevos
&#x200B;* Leer la etiqueta de datos de usuario del nodo de salida para activar o desactivar canales de una sustancia de forma predeterminada
&#x200B;* Exponer fusión Normal/AO en ajustes de TextureSet
&#x200B;* [Herramienta] Nueva herramienta de difuminado para fusionar y difundir colores
&#x200B;* [Herramienta] Nueva herramienta de Clonar para copiar parte de las texturas
&#x200B;* [Herramienta] Permite seleccionar canales para las herramientas Dedo, Clonar y Borrador
&#x200B;* [Capa] Añadir nombre de Substance para el nombre del efecto Rellenar
&#x200B;* [Layer] Permite exportar la máscara al portapapeles
&#x200B;* [Ventana gráfica] Cambiar entre el modo de Perspectiva y el modo ortográfico
&#x200B;* [Ventana gráfica] Permitir el control del campo de visión en modo de Perspectiva
&#x200B;* [Ventana gráfica] Permite definir la Profundidad de la distancia del campo con CTRL+clic central
&#x200B;* [Ventana gráfica] Permite arrastrar y soltar mapas de entorno en la Vista 3D.
&#x200B;* [Ventana gráfica] Se han mejorado los comentarios cuando el motor realiza cálculos potentes.
&#x200B;* [Export] Permite exportar parámetros de sombreador en un archivo json
&#x200B;* [UI] Interfaz de actualización con nuevos iconos, colores y diseño
&#x200B;* [UI] Añadir nombres de recursos a los miniestantes
&#x200B;* [UI] Contraer &quot;asignación de canales&quot; de forma predeterminada
&#x200B;* [Sombreado] Seleccione un color personalizado para los parámetros de textura del sombreado
&#x200B;* [Estante] Pregunte dónde importar archivos al arrastrar y soltar recursos
&#x200B;* [Estante] Nueva esfera de previsualización para generadores y materiales inteligentes
&#x200B;* [Estante] Añadir sombreador de brillo de Specular
&#x200B;* [Estante] Nuevas formas de superficie dura
&#x200B;* [Estante] Nuevas texturas y formas de Alpha
&#x200B;* [Estante] Nuevas texturas de piel
&#x200B;* [Estante] Nuevos materiales basados en escaneo y materiales inteligentes
&#x200B;* [Estante] Nuevos materiales inteligentes y soporte de especificaciones/brillo de los antiguos
&#x200B;* [Estante] Nuevos filtros de acabado para la simulación de superficies metálicas
&#x200B;* [Estante] Nuevo generador de máscara potente &quot;Editor de máscara&quot;
&#x200B;* [Estante] Materiales antiguos retrabajados y limpiados
&#x200B;* Nuevo proyecto de muestra &quot;Vela&quot;

**Corregido:**

&#x200B;* [Ajustes] El proyecto anula la velocidad de zoom y la rotación de la cámara
&#x200B;* [Ventana gráfica] Un problema de precisión en la textura normal predeterminada genera reflejos incorrectos
&#x200B;* [Ventana gráfica] La viñeta está activada de forma predeterminada
&#x200B;* [Ventana gráfica] Aparecen artefactos en los bordes del mapa de entorno (GPU Nvidia)
&#x200B;* [Ventana gráfica] La miniatura en modo de proyección/galería de símbolos es muy larga de cargar
&#x200B;* [Baker] Almacenar texturas horneadas en enteros de 16 bits en lugar de 32 bits
&#x200B;* [Capa] Las sustancias obsoletas se muestran incorrectamente en la pila
&#x200B;* El color predeterminado y la profundidad de bits de algunos canales son incorrectos (p. ej.: Specular, Brillo)
&#x200B;* Se ha corregido el comportamiento del borrador para deshabilitar la fusión en modo de paso a través

**Problemas conocidos:**

&#x200B;* La simetría no funciona con las herramientas Dedo y Clonar
&#x200B;* Falta la exportación de ArtStation

## Versión 1

### 1.7.3

*(Lanzado: 1 de marzo de 2016)*

**Agregado:**

&#x200B;* [Exportar] Añadir una opción para desactivar el relleno
&#x200B;* [Estante] Compatibilidad con la jerarquía de subestantes dentro de una carpeta de estante

**Corregido:**

&#x200B;* Bloqueo al guardar sobre un archivo de solo lectura anterior
&#x200B;* Bloqueo al abrir un segundo proyecto
&#x200B;* Bloqueo al cargar algunas miniaturas (estanterías, capas o información sobre herramientas)
&#x200B;* La desactivación de &quot;Conservar posiciones de trazos en la malla&quot; no funciona
&#x200B;* [Exportar] El aumento de escala de los mapas de bits se realiza con el filtrado más cercano
&#x200B;* [Shelf] El descubrimiento de recursos es muy lento
&#x200B;* [Shelf] Los filtros de desenfoque no son compatibles con 16 bits
&#x200B;* [Herramienta] La simetría no funciona si se carga un ajuste preestablecido antiguo de la herramienta
&#x200B;* El cuadro de diálogo Color del canal de Specular no convierte el espacio de color

### 1.7.2

*(Lanzado: 13 de enero de 2016)*

**Agregado:**

&#x200B;* [Capas] Permite especificar el segmentado predeterminado para las capas de relleno

**Corregido:**

&#x200B;* [Exportar] La exportación de Sketchfab ya no funciona
&#x200B;* [Layer] El filtrado bilineal se aplica incluso en Relleno sin ninguna transformación
&#x200B;* [Herramienta] Rendimiento deficiente al utilizar Substance con entradas de imagen en modo de proyección
&#x200B;* [Herramienta] El selector de material está roto

### 1.7.1

*(Lanzado: 18 de diciembre de 2015)*

**Corregido:**

&#x200B;* Bloqueo al cambiar el conjunto de texturas
&#x200B;* Reproducciones lentas al pintar

### 1.7.0

*(Lanzado: 17 de diciembre de 2015)*

**Agregado:**

&#x200B;* [Interpretaciones] Calcula el contenido de las capas y sus miniaturas al mismo tiempo
&#x200B;* [Exportar] Guarde la ruta de exportación como relativa cuando esté al lado del proyecto
&#x200B;* [Capas] Se ha añadido un nuevo modo de fusión : restar y agregar/sub
&#x200B;* [Layers] Nuevo filtrado HQ bilineal para capas de relleno
&#x200B;* [Sombreador] Establezca un sombreador predeterminado para la generación de miniaturas en las preferencias.
&#x200B;* [Sombreador] Permite especificar un sombreador por conjunto de texturas
&#x200B;* [Sombreador] Dejar tomar muestras de las texturas de la estantería
&#x200B;* [Herramienta] Nuevo comportamiento de pincel &quot;Ajustar&quot; para pintar
&#x200B;* [Herramienta] Mejora del filtrado y reducción del suavizado al pintar
&#x200B;* [Herramienta] Calidad de pintura de subpíxeles mejorada
&#x200B;* [Herramienta] Se ha eliminado la visualización &quot;básica&quot; de la configuración del pincel y se ha mejorado el icono de apertura/cierre del marco.
&#x200B;* [Menú] Añadir iconos de efectos en el menú contextual
&#x200B;* Creación de plantillas desde Proyectos
&#x200B;* [Estante] Nuevas plantillas : PBR, Dota 2
&#x200B;* [Shelf] Nuevo ajuste preestablecido de exportación : Dota 2
&#x200B;* [Shelf] Nuevos sombreadores : Dota 2, pintura de coches PBR, revestimiento PBR, terciopelo PBR
&#x200B;* [Estante] Material nuevo : Óxido de acero y desgaste, iluminación estilizada
&#x200B;* [Shelf] Nuevos filtros : Difuminado direccional, iluminación estilizada
&#x200B;* [Estante] Nuevo pincel : disco duro por defecto suave y duro por defecto con un nuevo alfa para un mejor control de la dureza
&#x200B;* [Estante] Nuevos generadores : Distancia y luz 3D
&#x200B;* [Estante] Pinceles actualizados con proyección de ceñido y sacrificio de caras posteriores (activado de forma predeterminada)
&#x200B;* [Estante] Se ha actualizado el ruido blanco con la versión de procesador de píxeles para agilizar el cálculo.

**Corregido:**

&#x200B;* [Pantalla de bienvenida] Vínculo de Tutorials para enviar a vídeos antiguos
&#x200B;* [Canales] Si se indica &quot;no&quot; para rellenar la creación de capas con AO, se sigue creando la capa.
&#x200B;* [Canales] Los nombres de canales de UserX no se propagan en la interfaz
&#x200B;* [Ventana gráfica] La entrada de máscara está vacía en la lista de canales solo
&#x200B;* [Compartir] Al exportar un alfa a Compartir desde SP, se crea un archivo .image ilegible
&#x200B;* [Licencia] Solucionar problemas de activación para nombres de usuario que no tengan caracteres ASCII
&#x200B;* [Sombreador] El cuadro de diálogo de parámetros de color desaparece al seleccionar un color
&#x200B;* [Shelf] Las miniaturas no se descargan de la memoria cuando no se utilizan
&#x200B;* [Estante] Filtro de degradado fijo
&#x200B;* [Herramienta] La Simetría no funciona con la galería de símbolos o la proyección
&#x200B;* [Herramienta] Nombre incorrecto al crear un nuevo ajuste preestablecido de pincel
&#x200B;* La opción Conservar trazo permanece desactivada incluso al volver a importar una malla
&#x200B;* Restablecimiento del controlador (TDR) al calcular partículas con un tamaño grande.

### 1.6.1

*(Lanzado: 09 de noviembre de 2015)*

**Corregido:**

&#x200B;* Bloqueo al abrir el proyecto si Vista 2D está visible
&#x200B;* Bloqueo al crear un nuevo ajuste preestablecido de exportación si el estante actual no existe
&#x200B;* [Herramienta] El icono del selector de material puede permanecer visible
&#x200B;* [Herramienta] El selector de material oculta el cursor del ratón al pintar al mismo tiempo
&#x200B;* [Shelf] Los metadatos se escriben en el disco después de cada salida

### 1.6.0

*(Lanzado: 29 de octubre de 2015)*

**Agregado:**

&#x200B;* Compatibilidad oficial con Windows 10
&#x200B;* [Substance] Contraer grupos de parámetros de sustancia de forma predeterminada
&#x200B;* [Substance] Añadir nueva estructura (Mejorar el rendimiento de los Procesadores de píxeles)
&#x200B;* [Ventana gráfica] Permite desactivar la visualización del plano de simetría en modo de simetría.
&#x200B;* [Ventana gráfica] Mejora del procesamiento y el rendimiento de las sombras
&#x200B;* [Ventana gráfica] Pausar cálculo de sombras al pintar
&#x200B;* [Viewport] Mejora del rendimiento de representación de mallas metálicas
&#x200B;* [Motor] Mejore la administración de la memoria Vram para reducir su espacio
&#x200B;* [Motor] Mejore la actualización de la textura en las GPU AMD para obtener un mejor rendimiento
&#x200B;* [Motor] Desactive la configuración de optimización de subprocesos en las GPU NVIDIA para obtener un mejor rendimiento
&#x200B;* [Effect] Añade una etiqueta para solicitar la entrada de imagen &quot;acolchada&quot;
&#x200B;* [Layer] Aumenta la precisión del Desplazamiento de UV/escala en el relleno
&#x200B;* [Capa] Haga que el regulador de escala sea exponencial en el relleno
&#x200B;* [Capa] Permite arrastrar y soltar materiales directamente en la pila de capas.
&#x200B;* [Capa] Permite arrastrar y soltar filtros directamente en la pila de capas
&#x200B;* [Capa] Ajuste el color del pincel de máscara al color de máscara recién creado
&#x200B;* [Sombreador] Exposición de varias texturas
&#x200B;* [Sombreador] Expone la función de asignación de gamma y tono para permitir funciones personalizadas
&#x200B;* [Bakeres] Cambiar la configuración predeterminada del baker de posición para el uso TriPlanar
&#x200B;* [Herramienta] Cambie el nombre &quot;Geometry Decal&quot; por &quot;Polygon Fill&quot;
&#x200B;* [Shelf] Actualice los generadores para que sean compatibles con TriPlanar : MG Desgaste del borde del metal, MG Constructor de la máscara, MG Fibra de vidrio, MG Dirt
&#x200B;* [Estante] Actualizar los materiales con nuevos ajustes y eliminar los materiales no utilizados
&#x200B;* [Estante] 22 materiales inteligentes nuevos (plástico, hierro, tela, acero y más)
&#x200B;* [Estante] Actualiza los filtros Enfocar, Desenfocar y Deformar con entrada de imagen acolchada para evitar costuras
&#x200B;* [Estante] Mejorar la configuración de deformación para facilitar el uso
&#x200B;* [Estante] 2 Nuevos ruidos procedimientos : Ruido de Perlin 3D y ruido de Worley 3D

**Corregido:**

&#x200B;* [Motor] La detección de la cantidad de Vram para la GPU dedicada es incorrecta en Mac
&#x200B;* [Motor] Las Texturas se convierten en una versión más oscura en la ventana gráfica
&#x200B;* [Motor] Rendimiento deficiente al pintar debajo de varias capas
&#x200B;* [Motor] Las capas calculadas al abrir el proyecto difieren de la versión almacenada en caché
&#x200B;* [Substance] Resultados incorrectos en 4K en Mac
&#x200B;* Los parámetros de [Substance] están en el orden incorrecto
&#x200B;* [Sombreador] Los sombreadores de tono y pixelado son totalmente negros
&#x200B;* [Sombreador] Los parámetros desaparecen después de cambiar el mapa de env
&#x200B;* [Shelf] Bloqueo al colocar archivos png en generator folder
&#x200B;* [Estante] Las miniaturas se generan con poca rugosidad
&#x200B;* [Herramienta] Bloqueo al utilizar un mapa de bits en el pincel alfa en Windows
&#x200B;* [Exportar] El ajuste preestablecido de exportación de mapa adicional ahora exporta un mapa del RGB para Posición

### 1.5.7

*(Lanzado: 24 de septiembre de 2015)*

**Corregido:**

&#x200B;* El informe de bloqueos ya no funciona

### 1.5.6

*(Lanzado: 21 de septiembre de 2015)*

**Agregado:**

&#x200B;* [Shelf] Mejora la calidad de la representación de miniaturas (utiliza texturas de 1K)

**Corregido:**

&#x200B;* [Compartir] Imposible firmar con otra cuenta
&#x200B;* [Estante] Las miniaturas pesan demasiado en el disco
&#x200B;* [Estante] Los Materiales inteligentes son muy lentos de cargar
&#x200B;* [Windows] Solucionar problemas de instalación del servicio de licencias
&#x200B;* [Canales] El mapa de Transmisivo se crea como G8 de forma predeterminada

### 1.5.5

*(Lanzado: 15 de septiembre de 2015)*

**Agregado:**

&#x200B;* [Estante] Exportar recursos al Substance share
&#x200B;* [Estante] Añadir nueva vista previa de esfera para materiales
&#x200B;* [Estante] Utilice el mapa de env &quot;Patio acristalado&quot; para generar miniaturas
&#x200B;* [Estante] Aumenta la resolución del tamaño de la miniatura a 512x512 píxeles
&#x200B;* [Vista 3D] Exponer el valor de rotación del entorno
&#x200B;* [Windows] Firme la aplicación

**Corregido:**

&#x200B;* [Bakeres] Resultados incorrectos al hacer un bake mapas al mismo tiempo
&#x200B;* [Vista 3D] El mapa de env se muestra cuando no hay ningún proyecto abierto.
&#x200B;* [Capas] Los Generadores de máscaras no funcionan en el contenido de las capas
&#x200B;* [Layers] Puede realizar la pintura en capas ocultas
&#x200B;* [Shelf] Dirt\_5 y Dirt\_6 son idénticos
&#x200B;* [Estante] Algunos generadores de máscaras están pixelados o son de baja calidad
&#x200B;* [Herramienta] Rotación de gizmo incorrecta en determinados ángulos.
&#x200B;* [Herramienta] Si hay demasiados canales, los botones de canal se recortan
&#x200B;* [Herramienta] El método abreviado de inversión de máscara para Máscara rápida no funciona
&#x200B;* [Export] Sketchfab: el botón de cancelación no se ha tenido en cuenta correctamente
&#x200B;* [Licencia] Error de activación cuando no se puede copiar la licencia
&#x200B;* El limitador de velocidad de fotogramas ya no funciona en la IU

### 1.5.0

*(Lanzado: 20 de agosto de 2015)*

<b>Agregado:</b>

&#x200B;* [Shader] Añadir número de línea en Shader compilando mensajes de error
&#x200B;* [Shelf] Mejora la calidad de las vistas previas en miniaturas
&#x200B;* [Shelf] Automatiza la generación de miniaturas para materiales inteligentes
&#x200B;* [Herramienta] Método abreviado para controlar la configuración de dureza en la sustancia
&#x200B;* [Herramienta] Usar el widget de escala de grises para la calcomanía geométrica sobre una máscara
&#x200B;* [Herramienta] Método abreviado para invertir el color de la pintura al pintar en un mapa de escala de grises
&#x200B;* [Ventana gráfica] Permite mostrar la malla metálica y cambiar su color
&#x200B;* [Ventana gráfica] Desenfocar el fondo del entorno
&#x200B;* [Controles] Añadir rotación a los métodos abreviados de pincel del ratón
&#x200B;* [Exportar] Exportar a Sketchfab
&#x200B;* [Exportar] Creación de ajustes preestablecidos de exportación para procesadores
&#x200B;* [Exportar] Añadir reflejo de mapa convertido, F0 y 1/IOR
&#x200B;* [UI] Pantalla Añadir bienvenida
&#x200B;* [UI] Actualizar diseño predeterminado
&#x200B;* [UI] Añade información sobre herramientas que faltan y cambia el nombre de alguna entrada del menú
&#x200B;* [Layers] Exportar la máscara seleccionada actualmente como mapa de bits
&#x200B;* [Capas] Añade la acción &quot;invertir máscara&quot; en el menú contextual

<b>Corregido:</b>

&#x200B;* [Proyecto] Si los pivotes de mallas son diferentes en el FBX, las mallas se explotan al importar
&#x200B;* [Substance] Los Substance utilizados en las herramientas de proyección están bloqueados en 256\*256
&#x200B;* [Layers] Bloqueo al utilizar la máscara transparente
&#x200B;* [Exportar] Conversión de gamma incorrecta en texturas muy oscuras
&#x200B;* [Exportar] El mapa de posición solo se puede utilizar en los ajustes preestablecidos de exportación como mapa de escala de grises
&#x200B;* [Herramienta] El color de inicio de la calcomanía geométrica es negro cuando se utiliza en una máscara
&#x200B;* [Herramienta] El método abreviado de rotación no funciona si no hay dureza en el alfa

### 1.4.2

*(Lanzado: 15 de julio de 2015)*

**Corregido:**

&#x200B;* [Herramienta] Bloqueo al utilizar la calcomanía geométrica con máscara rápida
&#x200B;* La actualización de un proyecto de la versión 1.4.0 a la 1.4.1 consume toda la memoria del equipo
&#x200B;* Importación incorrecta del formato de proyecto antiguo
&#x200B;* Los estantes personalizados analizan toda la jerarquía y duplican activos en todas partes

### 1.4.1

*(Lanzado: 23 de junio de 2015)*

**Agregado:**

&#x200B;* [Ventana gráfica] Permite acoplar paneles en paralelo
&#x200B;* [Efecto] Agregue un fondo y una regla para el efecto de nivel
&#x200B;* [Efecto] Agregue un efecto de Pintura que permita trabajar sobre otro efecto

**Corregido:**

&#x200B;* [Shelf] La generación de miniaturas se interrumpe si no hay ningún proyecto abierto
&#x200B;* [Estante] La previsualización de ajustes preestablecidos de material no se genera
&#x200B;* [Estante] Las previsualizaciones de material se generan en una malla con normales invertidas
&#x200B;* [Shelf] Las miniaturas siempre se vuelven a calcular debido a una función hash incorrecta
&#x200B;* [Estante] Hacer clic en un material de Substance no conecta mapas adicionales
&#x200B;* [Herramienta] Valor incorrecto muestreado con el selector de material
&#x200B;* [Herramienta] Selector de color seleccionar color de cursor de ventanilla
&#x200B;* [vista 2D] Velocidad de fotogramas/rendimiento muy baja
&#x200B;* [Export] al abrir la ventana de exportación con ajustes preestablecidos de exportación demasiado recientes.
&#x200B;* [Exportar] El canal de Height al Mapa de normales se convierte en el espacio incorrecto
&#x200B;* [Mac] El color base de los efectos de Substance se muestra como lineal
&#x200B;* [Mac] El widget de líneas rectas se dibuja incorrectamente en Retina
&#x200B;* Las líneas rectas pueden permanecer activadas incluso con el método abreviado liberado.
&#x200B;* Las líneas rectas del guizmo desaparecen después de rotar el mapa de entorno
&#x200B;* Las salidas de oclusión ambiental de sustancias no se conectan automáticamente al canal AO
&#x200B;* Solucionar el problema de copia de licencia en Windows con un carácter especial en el nombre de usuario

### 1.4.0

*(Lanzado: 10 de junio de 2015)*

**Agregado:**

&#x200B;* [Exportar] Añada asignaciones adicionales en la lista de los mapas de entrada disponibles
&#x200B;* [Estante] Usar materiales sbsar como ajustes preestablecidos de materiales
&#x200B;* [Estante] Permitir el uso de rutas de biblioteca personalizadas
&#x200B;* [Estante] Cambiar el tamaño mínimo
&#x200B;* [Estante] Nuevo contenido : 20 materiales inteligentes nuevos
&#x200B;* [Estante] Nuevo contenido : nueva sustancia procedimienta (tejido, malla)
&#x200B;* [Shelf] Filtro de desenfoque actualizado
&#x200B;* Dibujo de líneas rectas mediante una tecla modificadora
&#x200B;* Adición de un canal de Oclusión ambiental y modificación del comportamiento AO/Normal en la pila de capas
&#x200B;* Leer el color predeterminado de la entrada de imagen definida en los datos de usuario del Substance
&#x200B;* Permitir la exportación del registro desde el menú de ayuda

**Corregido:**

&#x200B;* [Baker] [Mac] Bloqueo con baker Normal desde malla
&#x200B;* [Baker] Bloqueo si no hay UV en el archivo de jaula
&#x200B;* [Baker] La coincidencia por nombres no funciona con OBJ exportados desde zBrush
&#x200B;* [Baker] Hacer un bake con una jaula sobrescribe hacer un bake si se utilizan varios conjuntos de texturas y UV superpuestos
&#x200B;* [Baker] Los archivos OBJ específicos generan texturas negras
&#x200B;* [Shelf] No se pueden leer recursos si se establece como de solo lectura
&#x200B;* [Estante] Los archivos de recursos se escriben en Painter si se han utilizado en el proyecto.
&#x200B;* [Estante] Las sustancias de recarga también actualizan la capa
&#x200B;* [Export] Tiff exporta imágenes de 32 bits que Photoshop o los motores de juegos no pueden leer correctamente
&#x200B;* [Exportar] El ajuste preestablecido de canales predeterminados siempre se exporta como RGB
&#x200B;* [Material] La asignación de color base a los canales de Difuso anula la asignación de materiales
&#x200B;* [Vista 3D] Iluminación incorrecta con mapas de entorno específicos
&#x200B;* [Herramienta] No se puede rotar un pincel a un ángulo específico
&#x200B;* La ventana gráfica se enfoca al pasar el cursor por encima mientras se escribe en un campo de texto
&#x200B;* Bloqueo con ajustes preestablecidos demasiado recientes para la versión actual del estante
&#x200B;* Bloqueo después de reemplazar la malla
&#x200B;* Bloqueo al volver a cargar una sustancia con un número diferente de entradas
&#x200B;* FBX mallas de la importación de Cinema4D con nombres de material incorrectos

### 1.3.5

*(Lanzado: 29 de mayo de 2015)*

**Agregado:**

&#x200B;* [Licencia] Problema de activación cuando ya hay un archivo de licencia
&#x200B;* [Mac] Bloqueo al cargar archivos FBX específicos
&#x200B;* [Mac]&#x200B;[Vista 3D] Reflejo incorrecto para la GPU integrada
&#x200B;* [Vista 3D] La fuente de la Máscara rápida está rota
&#x200B;* [Vista 3D] El selector de material hace que la ventana gráfica sea totalmente negra
&#x200B;* Bloqueo después de abrir proyectos creados en 1.3.3
&#x200B;* La previsualización de material está vacía al utilizar sombreadores con alfa
&#x200B;* La pintura deja de funcionar en mallas específicas
&#x200B;* Las prestaciones disminuyen mucho con mallas OBJ específicas
&#x200B;* Los canales de usuario no se asignan al utilizar efectos
&#x200B;* Las carpetas temporales no se limpian al inicio

**Corregido:**

&#x200B;* Mejoras de tiempo de cálculo en el proyecto extremadamente largo de carga
&#x200B;* Cambie la ventana &quot;Solución de problemas de GPU&quot; para que sea más comprensible
&#x200B;* [Capas] Guarde el estado del bloqueo de proporción para las capas de relleno y active esta opción de forma predeterminada
&#x200B;* [Bakers] La coincidencia por nombre ahora usa el sufijo como separador

### 1.3.4

*(Lanzado: 27 de abril de 2015)*

**Agregado:**

&#x200B;* [Mac] Bloqueo con Mac OS X Yosemite (10.10)
&#x200B;* [Mac] No es posible salir del modo de pantalla completa
&#x200B;* [Panaderos] La opción Coincidencia de horneado por nombre no funciona
&#x200B;* [Panaderos] El espacio tangente de la tinta utilizado en SP no funciona con UE4
&#x200B;* [Panaderos] El panadero de ID no puede hornear colores de ID de material
&#x200B;* [Vista 2D] La Malla metálica no aparece al utilizar la herramienta Calcomanía geométrica
&#x200B;* [Herramienta] El canal alfa del pincel se muestra como verificador en lugar de como transparencia con los materiales
&#x200B;* [Herramienta] Bloqueo con la pegatina geométrica
&#x200B;* [Capas] La ranura de material se contrae de forma predeterminada en la capa de relleno
&#x200B;* [Export] Bloqueo al exportar a un tamaño superior a la resolución del conjunto de texturas
&#x200B;* El canal de specular no se reconoce en los filtros.
&#x200B;* Limpiar y guardar no quita correctamente los recursos del archivo spp
&#x200B;* No almacenar la transformación de bajo contenido de poli en el archivo de asignación de alto contenido de poli
&#x200B;* El archivo FBX se importa con demasiados conjuntos de texturas

**Corregido:**

&#x200B;* Efectos: La abrazadera de niveles debe estar activada de forma predeterminada para imitar los niveles &quot;clásicos&quot;
&#x200B;* Capas: Cambio del nivel mínimo y máximo en la acción Rellenar
&#x200B;* Capas: Guardar y restaurar el estado de la pila
&#x200B;* Bakeres: BAKER AO tener en cuenta el mapa de normales si no se especifica ningún HP
&#x200B;* Bakeres: Se ha añadido información sobre herramientas e información adicional en la ventana hacer un bake
&#x200B;* Crear un archivo de copia de seguridad al guardar un proyecto

### 1.3.3

*(Lanzado: 01 de abril de 2015)*

**Agregado:**

&#x200B;* Añadir la versión de software y el nombre del proyecto en la barra de título
&#x200B;* Corregir nombres de TextureSet y nombres de Materiales inteligentes
&#x200B;* Actualizar el motor del Substance a V5
&#x200B;* [Shelf] Añadir nuevos mapas de entorno : Corsica beach, studio 05, Tornoco studio y más
&#x200B;* [Shelf] Actualizar MG Mask Builder con nuevos parámetros
&#x200B;* [Shelf] Actualizar y calibrar mapas de entorno antiguos

**Corregido:**

&#x200B;* Bloqueo al abrir la ventana de exportación
&#x200B;* No es posible arrastrar y soltar en el widget de interfaz de usuario cuando no está acoplado
&#x200B;* &quot;Buscar actualizaciones&quot; no funciona
&#x200B;* [Capas] No seleccionar la máscara al pulsar ALT + clic en ella
&#x200B;* [Herramienta] Tri-plana no funciona con el canal Normal
&#x200B;* [Vista 3D] La iluminación de la Difuso del mapa env es incorrecta
&#x200B;* [Vista 3D] El cálculo de la exposición es diferente de Designer
&#x200B;* [Vista 3D] Las sombras no deben ser visibles en superficies 100 % metálicas
&#x200B;* [Vista 3D] La malla con UV reflejados ha volteado la tangente/los binomales
&#x200B;* [Vista 3D] Las sombras producen resultados incorrectos en determinadas mallas
&#x200B;* [Bakeres] Quitar la carpeta &quot;.alg\_meta&quot; creada por los archivos de asignación
&#x200B;* [Baker] Bloqueo al hacer un bake si Painter vuelve a calcular un TextureSet al mismo tiempo
&#x200B;* [Mac] Error de IU de White Box al iniciar la aplicación

### 1.3.2

*(Lanzado: 6 de marzo de 2015)*

**Corregido:**

&#x200B;* [Vista 3D] No es posible volver a cargar un mapa env guardado con el proyecto

### 1.3.1

*(Lanzado: 5 de marzo de 2015)*

**Agregado:**

&#x200B;* [Bakeres] Agregue una versión en caché de mallas de alto contenido de poli para acelerar el cálculo
&#x200B;* [Bakeres] Añada un icono de advertencia si no se ha cargado ninguna malla de alta densidad
&#x200B;* [Bakeres] Si no se carga ninguna malla de alta densidad, utilice en su lugar la malla del proyecto

**Corregido:**

&#x200B;* [Bakeres] Al pulsar &quot;Intro&quot; al editar el valor de un regulador, cierre la ventana.
&#x200B;* [Bakeres] Al activar o desactivar un baker, también se activa el botón
&#x200B;* [Bakeres] Imposible de hacer un bake si utiliza el botón &quot;all/none&quot;
&#x200B;* [Bakeres] La ordenación de los botones del baker no está en el orden correcto
&#x200B;* [Bakeres] La casilla de verificación se omite y todos los bakeres siempre se procesan
&#x200B;* [Bakeres] Progreso fijo de la barra de progreso

### 1.3.0

*(Lanzado: 4 de marzo de 2015)*

**Agregado:**

&#x200B;* [Bakeres]&#x200B;[Vista 3D] Utilice el cálculo de espacio de tangente Mikkt si no encuentra tangentes/binormales
&#x200B;* [Bakeres] Se han añadido nuevos bakeres : Normal, ID, Oclusión, Curvatura, Thickness, Posición
&#x200B;* [Efectos] La pila de efectos ahora se invierte y se muestra de arriba abajo (como capas)
&#x200B;* [Efectos] Añadir nuevos iconos en la pila de efectos
&#x200B;* [Efectos] Añadir modo de fusión entre acciones de relleno en la pila de efectos
&#x200B;* [Efectos] Cambiar nombre de efectos (efecto de sustancia = filtro, etc.)
&#x200B;* Añadir un archivo &quot;lock&quot; durante el proceso de guardado
&#x200B;* [Effects] Acción Añadir relleno en la pila de efectos
&#x200B;* Se ha añadido un nuevo recurso : Materiales inteligentes
&#x200B;* [Capas] Permite reordenar los efectos de capa
&#x200B;* [Herramienta] Agregar proyección triplana
&#x200B;* [Vista 3D] Añadir compatibilidad con sombras
&#x200B;* [Vista 3D] Posibilidad de establecer los estados necesarios de OpenGL en sombreadores personalizados
&#x200B;* [Vista 3D] Compatibilidad con alfa mediante nuevos sombreadores
&#x200B;* [Vista 3D] Ahora los sombreadores tienen versiones y se guardan por completo en un proyecto
&#x200B;* [Vista 3D] Avisar al usuario si el sombreador ya no se compila

**Corregido:**

&#x200B;* [Capas] Se corrige el soltar debajo de una carpeta contraída
&#x200B;* [Estante] Corrección del filtrado de contenido en miniestantes
&#x200B;* [Shelf] Cambiar el nombre de las categorías y reorganizar las pestañas

### 1.2.1

*(Lanzado: 12 de febrero de 2015)*

**Agregado:**

&#x200B;* Los archivos \*.spp ahora se pueden abrir haciendo doble clic en el explorador
&#x200B;* [Exportar] Nueva etiqueta &quot;$project&quot; para los ajustes preestablecidos de exportación
&#x200B;* [Exportar] Añadir lista de mapas (con nomenclatura) debajo de cada conjunto de texturas
&#x200B;* [Exportar] Añada un botón Todo/Ninguno para seleccionar los conjuntos de texturas
&#x200B;* [Exportar] Los mapas vacíos se descartan durante la exportación

**Corregido:**

&#x200B;* [Exportar] Los ajustes preestablecidos de Unity5 tienen mapas invertidos
&#x200B;* [Exportar] Si se añade una barra diagonal en un nombre de ajuste preestablecido, se creará una carpeta dañada
&#x200B;* El canal de Height [Export] exportado en formatos de 32 bits no está correctamente sujeto
&#x200B;* [Exportar] La lista de conjuntos de texturas no se ordena como en el proyecto
&#x200B;* [Herramienta] El sacrificio de la cara posterior ya no funciona
&#x200B;* Guardar no funciona con caracteres especiales en el trazado

### 1.2.0

*(Lanzado: 28 de enero de 2015)*

**Agregado:**

&#x200B;* Nuevo canal Normal que permite la pintura de datos de mapa de normales y combinar los resultados
&#x200B;* [Exportar] Nueva ventana de exportación con la capacidad de crear empaquetados personalizados y definir nombres personalizados
&#x200B;* El formato del archivo de proyecto ahora es un único archivo en lugar de carpetas
&#x200B;* [Export] Admite diferentes formatos normales (DirectX, OpenGL)
&#x200B;* [Exportar] Crear un archivo de bloqueo temporal durante la exportación
&#x200B;* [Capas] Mayús + clic izquierdo del ratón se puede utilizar para alternar una máscara
&#x200B;* [Parámetros] Expone el espacio de color en la parte inferior de una entrada de imagen
&#x200B;* [Shelf] Efecto &quot;MG Mask Builder&quot; ahora tiene nuevos ajustes
&#x200B;* [Vista 3D] El mapa de Oclusión ambiental ahora oculta el aporte difuso, no el specular

**Corregido:**

&#x200B;* El material de proyección o la previsualización de la galería de símbolos no se muestran correctamente en la ventana gráfica
&#x200B;* [Vista 3D] La información sobre el Método abreviado no se muestra al utilizar el método abreviado &quot;S&quot; (plantilla).
&#x200B;* [Shelf] El efecto &quot;MatFx Skin Scale&quot; tiene ahora mejores prestaciones en baja resolución
&#x200B;* [Exportar] Las Texturas de la exportación solo se aumentan al especificar un tamaño de documento mayor

### 1.1.2

*(Lanzado: 15 de enero de 2015)*

**Agregado:**

&#x200B;* Añadido: Nuevos ajustes de Traducir, Rotar y Escalar en la capa de Relleno
&#x200B;* Filtrado mejorado para capas de pinceles y de relleno
&#x200B;* La versión de prueba ya está totalmente disponible (se puede exportar), pero tiene un tiempo limitado.

**Corregido:**

&#x200B;* Imposible importar mallas OBJ con muy pequeñas precisiones
&#x200B;* Problema al activar una licencia en Windows 7 y 8
&#x200B;* Bloqueo durante la operación Guardar como de un proyecto
&#x200B;* Bloqueo al eliminar el último canal de un conjunto de texturas
&#x200B;* Bloqueo al eliminar una capa en un contexto específico

### 1.1.1

*(Lanzado: 25 de diciembre de 2014)*

**Agregado:**

&#x200B;* [Capa] Seleccione la capa superior al abrir un proyecto o cambiar el conjunto de texturas
&#x200B;* Se ha mejorado la velocidad de &quot;Guardar&quot; y &quot;Guardar como&quot; con el nuevo algoritmo de compresión
&#x200B;* Mostrar un error al abrir un proyecto demasiado reciente para Painter

**Corregido:**

&#x200B;* [Herramienta] La pegatina geométrica produce corrupciones de memoria
&#x200B;* [Pincel] No es posible introducir manualmente valores flotantes por debajo de 1 para el tamaño de pincel.
&#x200B;* [Capa] Al crear un efecto de selección de color, no se añade a la pila de capas
&#x200B;* [Capa] Al mover el ratón sobre las capas, Painter se mueve por la barra de tareas
&#x200B;* [Capa] Añadir un mapa de bits como máscara puede provocar un bloqueo
&#x200B;* La interfaz gráfica de usuario para el modo solo con el canal de Height es incorrecta
&#x200B;* &quot;Guardar proyecto&quot; puede dar error y dañar un proyecto
&#x200B;* Bloqueo al abrir un proyecto después de cargar otro con un sombreador obsoleto

### 1.1.0

*(Lanzado: 16 de diciembre de 2014)*

**Agregado:**

&#x200B;* [Effect] Nuevo creador de máscaras de ID de material
&#x200B;* Nueva línea punteada blanca/negra para el gizmo del pincel
&#x200B;* Nuevo parámetro de seguimiento de ángulo
&#x200B;* Nuevo parámetro de sacrificio de la cara posterior
&#x200B;* Nuevo parámetro de Ratón perezoso
&#x200B;* [Layers] Soporte para múltiples selecciones y administración
&#x200B;* [Capas] Copie y pegue de un conjunto de texturas entre sí
&#x200B;* [Exportar] Formato de PSD de Adobe Photoshop
&#x200B;* [Estante] Nueva herramienta : piel, puntadas metálicas y cremallera
&#x200B;* [Estante] Nuevo pincel : molde, lápiz, línea afilada y puntada
&#x200B;* [Shelf] Nuevo alfa : Ruido gaussiano, línea afilada, molde, pluma, salpicadura, puntada, cremallera
&#x200B;* Se han mejorado las prestaciones de pintura actualizando solo partes de las texturas necesarias

**Corregido:**

&#x200B;* [Estante] Imposible cargar una sustancia con un gráfico que tenga etiquetas idénticas
&#x200B;* El modo de fusión Pasar por [capas] no funciona con máscaras
&#x200B;* [Esténcil] La escala se rompe en la Vista 2D
&#x200B;* Problemas y bloqueo en el sistema operativo Mac Yosemite

### 1.0.2

*(Lanzado: 09 de noviembre de 2014)*

**Agregado:**

&#x200B;* Rendimiento mejorado en la previsualización de materiales con sustancias
&#x200B;* Se han mejorado las prestaciones con la vista previa del trazo de pincel al actualizar el documento
&#x200B;* Rendimiento mejorado en la ventana gráfica con una velocidad de actualización más baja para el área no operativa
&#x200B;* [Efectos de posprocesamiento] Se ha mejorado la interfaz de usuario para administrar la configuración
&#x200B;* [Efectos de posprocesamiento] Restablecer los valores predeterminados
&#x200B;* Operaciones de capas y efectos de Substance en el menú contextual
&#x200B;* Apoyo a los insumos/productos premultiplicados en sustancias

**Corregido:**

&#x200B;* [Vista 3D] Los parámetros de sombreador personalizados están separados por un espacio grande
&#x200B;* [Exportar] Falta la conversión sRGB para el ajuste preestablecido Unity4
&#x200B;* Posible Bloqueo al cargar mallas fbx
&#x200B;* Bloqueo a veces al cargar mallas obj simples
&#x200B;* La barra de cálculo permanece bloqueada al 100% al cargarse
&#x200B;* Volver a cargar una sustancia la coloca en todas las categorías
&#x200B;* Interruptor DirectX/OpenGL roto

### 1.0.1

*(Lanzado: 27 de octubre de 2014)*

**Agregado:**

&#x200B;* [Herramienta] Uso mejorado de parámetros de material
&#x200B;* Nuevo método abreviado para el sitio web uservoice en el menú Ayuda
&#x200B;* Varias mejoras de rendimiento en el motor

**Corregido:**

&#x200B;* Los valores de los parámetros están limitados a 2 decimales para Partículas
&#x200B;* El Substance cargado desde la caché no se muestra en la interfaz de usuario como obsoleto
&#x200B;* Bloqueo al cargar una malla desde una URL de red
&#x200B;* Painter ahora se reconoce como firmado en Mac OS X

### 1.0.0

*(Lanzado: 15 de octubre de 2014)*

**Agregado:**

&#x200B;* Compatibilidad con Sombreador personalizado
&#x200B;* Compatibilidad con resolución 4k
&#x200B;* Proyectos de caracteres de muestra
&#x200B;* Mostrar barra de progreso para tiempos de cálculo largos
&#x200B;* [Exportar] Añadir una pasada de dilatación antes del posproceso de difusión
&#x200B;* Argumentos de la línea de comandos en SP para operaciones simples
&#x200B;* Nuevos materiales y efectos
&#x200B;* Previsualización de herramientas (área separada de previsualización de materiales en tiempo real y prueba de trazos)
&#x200B;* No crear un documento predeterminado al iniciar Painter
&#x200B;* [Herramienta] Permite editar manualmente un valor de escala de grises
&#x200B;* Varias mejoras para los patrones (Ajustar, Restablecer)
&#x200B;* Las partículas son ahora subherramientas de las herramientas Pincel, Borrador y Proyección
&#x200B;* [Vista 3D] Usar AO hecho un bake en el renderizado de la ventana gráfica
&#x200B;* División de los controles de galerías de símbolos entre la vista 2D y 3D
&#x200B;* Ajuste de tamaño de pulgar pequeño en la biblioteca
&#x200B;* Los campos de búsqueda son específicos de cada ventana
&#x200B;* Ajuste de IU

**Corregido:**

&#x200B;* El conmutador [Substance] no funciona
&#x200B;* [Cuadro de diálogo Color] Degradado de tono no actualizado
&#x200B;* No es posible actualizar una malla si el nombre del archivo es idéntico
&#x200B;* La herramienta no está visible en las vistas cuando es demasiado pequeña
&#x200B;* La herramienta de pegatina de la pantalla Retina no funciona correctamente
&#x200B;* [Substance] Int1 se muestra como float1
&#x200B;* No se reconocen las entradas/salidas de [Substance] basecolor
&#x200B;* [Substance] los filtros no se pueden volver a cargar
&#x200B;* [Herramienta] El widget de escala de grises siempre está contraído

## Beta

### 0.12.1-beta

*(Lanzado: 18 de septiembre de 2014)*

**Agregado:**

&#x200B;* Ajuste preestablecido de exportación de Unity 5

**Corregido:**

&#x200B;* SOMBREADOR PBR, la calidad de representación debería mejorar mucho
&#x200B;* La función de enfoque está rota y las mallas se recortan de forma predeterminada

### 0.12.0-beta

*(Lanzado: 17 de septiembre de 2014)*

**Agregado:**

&#x200B;* Herramienta Cuentagotas
&#x200B;* Se ha añadido la opción &quot;Conservar posición de trazo&quot; a la reimportación de malla para cuando cambie el cuadro delimitador.
&#x200B;* Mapa de normales para la malla predeterminada de Cymourai
&#x200B;* Mejorar la interfaz de la vista de herramientas (los colores son nítidos)
&#x200B;* Mueva el menú &quot;Ayuda->Configuración&quot; a &quot;Editar->Configuración&quot;
&#x200B;* Guarde la ruta de exportación en la ventana &quot;Exportar todos los canales&quot;
&#x200B;* Nuevos niveles GUI con visualización de histograma
&#x200B;* Mejor gestión de activos (arrastrar y soltar, volver a cargar recursos, eliminar recursos no utilizados)
&#x200B;* Cambiar de &quot;difuso&quot; a &quot;color base&quot;
&#x200B;* Ajustes de edición de los reguladores: permitir puntos además de comas
&#x200B;* Capa de relleno: aumentar el valor máximo de segmentación
&#x200B;* Mapa de entorno predeterminado

**Corregido:**

&#x200B;* Artefactos de mal reflejo en ángulos extremos
&#x200B;* Exportación de speculares rotos/brillo
&#x200B;* Los vínculos de la ventana &quot;Acerca de&quot; de Painter no funcionan
&#x200B;* Bloqueo con OSX Yosemite
&#x200B;* Las mallas se guardan trianguladas
&#x200B;* El método abreviado de color de la ventana Herramienta se envía al emisor en lugar de a la escala de grises
&#x200B;* El selector de color permanece abierto al cambiar de capa a máscara
&#x200B;* No se puede guardar material de una capa de relleno
&#x200B;* Permitir el cambio de tamaño de las tres regiones del estante

### 0.11.0-beta

*(Lanzado: 4 de septiembre de 2014)*

**Agregado:**

&#x200B;* Agregar un divisor entre las vistas 3D y 2D
&#x200B;* Uso de un fondo degradado en las vistas 2D/3D
&#x200B;* Interfaz para el histograma de niveles
&#x200B;* Combinar estante y biblioteca
&#x200B;* No es necesario guardar nada al crear o actualizar un ajuste preestablecido
&#x200B;* Importar activos en el estante mediante arrastrar y soltar

**Corregido:**

&#x200B;* El nombre de los botones se muestra encima en la barra de herramientas principal

### 0.10.2-beta

*(Lanzado: 28 de agosto de 2014)*

**Corregido:**

&#x200B;* La exportación de todos los canales produce resultados incorrectos

### 0.10.1-beta

*(Lanzado: 26 de agosto de 2014)*

**Corregido:**

&#x200B;* El sombreador proporciona un resultado en negro con poca rugosidad
&#x200B;* Comprobación de GPU: manejar tarjetas &#39;Quadro&#39;, detectar todos los dispositivos y adaptar el mensaje de usuario en consecuencia
&#x200B;* La mayoría de los materiales de Substance tienen un límite de 256 en Beta 9
&#x200B;* El height se sujeta al exportar como mapa de bits
&#x200B;* La previsualización del pincel es diferente de la superposición de la proyección en Mac
&#x200B;* El uso de la herramienta Geometría para crear máscaras no se muestra en las ventanas gráficas
&#x200B;* La máscara rápida está rota
&#x200B;* Solucionar problema de fusión en el antiguo mac pro

### 0.10.0-beta

*(Lanzado: 07 de agosto de 2014)*

**Agregado:**

&#x200B;* Máscaras de galería de símbolos

**Corregido:**

&#x200B;* Compatibilidad con tarjetas Quadro
&#x200B;* El sombreador proporciona un resultado en negro con poca rugosidad
&#x200B;* Los materiales de Substance tienen un límite de 256
&#x200B;* La exportación de mapas de normales elimina el canal verde

### 0.9.0-beta

*(Lanzado: 17 de julio de 2014)*

**Agregado:**

&#x200B;* Procesamiento posterior de Yebis 2
&#x200B;* El asistente de nuevo proyecto le permite importar mapas de entrada (AO, curvatura, etc.)
&#x200B;* Conectar automáticamente mapas de entrada (AO, curvatura, etc.) a Efectos de Substance
&#x200B;* Control de escala sobre materiales aplicado a capas de relleno

### 0.8.2-beta

*(Lanzado: 11 de julio de 2014)*

**Corregido:**

&#x200B;* El regulador Tono se establece de forma predeterminada en Blanco
&#x200B;* Restablecimiento del proyecto si el nombre de material contiene caracteres especiales
&#x200B;* El cambio de nombre de material en un solo objeto de material no debe invalidar el proyecto.
&#x200B;* Las UV se estropean después de guardar el proyecto y volver a abrirlo

### 0.8.1-beta

*(Lanzado: 4 de julio de 2014)*

**Corregido:**

&#x200B;* Varios bloqueos de GPU
&#x200B;* Bloqueo al exportar canales

### 0.8.0-beta

*(Lanzado: 28 de junio de 2014)*

**Agregado:**

&#x200B;* Múltiples materiales : ahora puede pintar en varios materiales en el mismo documento
&#x200B;* Pintura de simetría
&#x200B;* Ya están disponibles todos los modos de fusión

**Corregido:**

&#x200B;* Varios bloqueos de GPU
&#x200B;* Restablecimiento del proyecto si el nombre de material contiene caracteres especiales
&#x200B;* Las UV se estropean después de guardar el proyecto y se vuelven a abrir con varias UV

### 0.7.0-beta

*(Lanzado: 18 de junio de 2014)*

**Agregado:**

&#x200B;* Efectos de capa
&#x200B;* Nuevos materiales de Substance Stencil
&#x200B;* Borrar máscara
&#x200B;* Permitir copiar/pegar capa/máscara
&#x200B;* Permitir duplicar capa
&#x200B;* Herramienta Cambiar al editar máscara de capa
&#x200B;* Los Substance ahora funcionan con GPU

**Corregido:**

&#x200B;* El dibujo del mapa de altura no pintura valores negativos.
&#x200B;* La visualización del Selector de material no debe tener en cuenta el mapa de normales muestreado
&#x200B;* Determinismo de partículas roto
&#x200B;* Matriz de esténcil en Vista 2D
&#x200B;* Nombres en archivos obj
&#x200B;* Varios bloqueos

### 0.6.0-beta

*(Lanzado: 04 de junio de 2014)*

**Agregado:**

&#x200B;* Nueva opción de exportación para exportar un mapa de Speculares desde una composición de canales de rugosidad y metálicos

**Corregido:**

&#x200B;* Compatibilidad con Windows Vista
&#x200B;* El mapa de altura no pintura valores negativos

### 0.5.0-beta

*(Lanzado: 7 de mayo de 2014)*

**Agregado:**

&#x200B;* Interruptores 3D/Vista 2D
&#x200B;* Herramienta Selección de fragmentos UV
&#x200B;* La herramienta cambia automáticamente al pintar sobre máscaras.
&#x200B;* La resolución de los Substance depende de la

**Corregido:**

&#x200B;* Bloqueo al iniciar
&#x200B;* Bloqueo con mallas ASCII
&#x200B;* Matriz de galería de símbolos fija en Vista 2D
&#x200B;* Bloqueo con Borrador

### 0.4.0-beta

*(Lanzado: 17 de abril de 2014)*

**Agregado:**

&#x200B;* Vista 2D Fluida
&#x200B;* Máscaras de capa de mapa de bits
&#x200B;* Control de exposición ambiental
&#x200B;* Las capas de relleno ahora utilizan las ventanas Herramientas para establecer sus propiedades
&#x200B;* Los materiales se pueden aplicar a las capas de relleno
&#x200B;* Se han añadido más galerías de símbolos en la biblioteca de galerías de símbolos
&#x200B;* Ajustes preestablecidos de partículas actualizados para un cálculo más rápido
&#x200B;* Optimización y mejora de la calidad del sombreador PBR para ajustes de menor calidad

**Corregido:**

&#x200B;* Las miniaturas de capas están vinculadas al canal seleccionado actualmente
&#x200B;* Muchos bloqueos

### 0.3.0-beta

*(Lanzado: 4 de abril de 2014)*

**Agregado:**

&#x200B;* Permitir valores negativos en el selector de color para la pintura de mapas de height
&#x200B;* Mostrar previsualización del material/color seleccionado
&#x200B;* Añadir accesos directos a las herramientas de la barra de herramientas (1,2,3,4)
&#x200B;* Cambiar el formato Normal (OpenGL frente a DirectX) globalmente en un proyecto
&#x200B;* Asistente para nuevo proyecto
&#x200B;* El regulador de espaciado ya no está sujeto
&#x200B;* Estilo de controles deslizantes actualizado
&#x200B;* Convertir el selector de color en no modal
&#x200B;* Al seleccionar un material en la biblioteca, se establece el tipo de herramienta en consecuencia

**Corregido:**

&#x200B;* Corregido: El trazado de malla de importación no se conserva
&#x200B;* Corregido: Generación de texturas incorrecta
&#x200B;* Corregido: Bloqueo al inicio

### 0.2.0-beta

*(Lanzado: 17 de marzo de 2014)*

**Agregado:**

&#x200B;* Cuentagotas de material (P método abreviado)
&#x200B;* Miniaturas bajo la vista previa de la herramienta 3d
&#x200B;* Sistema de licencias para versiones independientes
&#x200B;* [ y ] métodos abreviados de teclado para Tamaño de pincel
&#x200B;* Relleno en mapas exportados
&#x200B;* Estilo de ventana de herramientas actualizado
&#x200B;* Estilo de controles deslizantes actualizado
&#x200B;* Updated Default HDR. environment

**Corregido:**

&#x200B;* Esténcil: cambiar el valor de flujo en las paradas de Vista 3D en 52
&#x200B;* El bucle infinito en el motor al añadir teclas de presión 0 al trazo es fijo
&#x200B;* Herramienta: la variación de ángulo no devuelve valores por encima de +/- 90%
&#x200B;* Cambio en la visualización de la Vista 3D cuando se selecciona una máscara de capa
&#x200B;* Zoom invertido

### 0.1.0-beta

*(Lanzado: 2 de marzo de 2014)*

**Agregado:**

&#x200B;* Nueva administración de bibliotecas
&#x200B;* Nuevo contenido de pinceles y partículas
&#x200B;* Vista previa del pincel 3D
&#x200B;* Estilo de ventana de herramientas actualizado
&#x200B;* Estilo de controles deslizantes actualizado
&#x200B;* Rendimiento de caché actualizado

**Corregido:**

&#x200B;* Controles de cámara
&#x200B;* Rotación de pincel
