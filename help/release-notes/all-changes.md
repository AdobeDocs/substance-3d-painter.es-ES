---
breadcrumb-title: ''
description: Revisa todos los cambios y actualizaciones en las versiones de Substance 3D Painter para realizar un seguimiento de la evolución y las mejoras de las funciones a lo largo del tiempo.
title: Todos los cambios
user-guide-description: ''
user-guide-title: ''
source-git-commit: 479eb327180dd223bbff362e3f200995565cbcfa
workflow-type: tm+mt
source-wordcount: '40713'
ht-degree: 0%
---

# Todos los cambios

Esta página contiene notas de la versión de todas las versiones anteriores de Substance 3D Painter, ordenadas de la más reciente a la más antigua.

>[!NOTE]
>
> Para ver los problemas conocidos que pueden afectar a Painter, consulte la [página de documentación dedicada](known-issues.md).

## Versión 12

### 12.2.0

Fecha de publicación: **2026/10/21**

Resumen: **Esta actualización es una versión importante, agrega una nueva característica de pintura en jaula para hacer un bake y mejora la funcionalidad de relleno de polígono. Para obtener más detalles, vea las notas de la versión completas.**

**Agregado:**

* Hacer un bake, Jaula
* &amp;lbrack;Pintura de jaula&amp;rbrack; Crear interfaz de usuario básica de Pintura de jaula
* &amp;lbrack;Pintura de jaula&amp;rbrack; Nuevas opciones de visualización de jaulas
* &amp;lbrack;Pintura de jaula&amp;rbrack; Herramienta Selección/Relleno editable
* &amp;lbrack;Pintura de jaula&amp;rbrack; Mostrar modo de Fusión en la barra de herramientas
* &amp;lbrack;Pintura de jaula&amp;rbrack; HDR. cambios de IU del regulador
* &amp;lbrack;Pintura de jaula&amp;rbrack; Sombreador de visualización
* &amp;lbrack;Pintura de jaula&amp;rbrack; Restablecer opciones de pila
* Mejoras de la herramienta Relleno poligonal
* &amp;lbrack;Relleno poligonal&amp;rbrack; Añadir parche de polígono
* &amp;lbrack;Relleno poligonal&amp;rbrack; Añadir bucle de polígono
* &amp;lbrack;Relleno poligonal&amp;rbrack; Compatibilidad de simetría con Bucle/Parche
* &amp;lbrack;Relleno poligonal&amp;rbrack; Vista previa de borde de simetría
* &amp;lbrack;Relleno poligonal&amp;rbrack; Eliminar triángulos con bucles y bucles parciales
* &amp;lbrack;Relleno poligonal&amp;rbrack; Malla metálica visible solo para el conjunto de texturas activo
* &amp;lbrack;Relleno poligonal&amp;rbrack; Resaltado de borde rojo en triángulos que no se pueden hacer clic
* &amp;lbrack;Relleno poligonal&amp;rbrack; No desactive las opciones del modo de relleno
* &amp;lbrack;Relleno poligonal&amp;rbrack; Permitir definir todas las propiedades de canal con Relleno poligonal
* &amp;lbrack;Relleno poligonal&amp;rbrack; El trazo anterior de la reanudación funciona con el relleno poligonal
* &amp;lbrack;Relleno poligonal&amp;rbrack; Mostrar el cursor prohibido en conjuntos de texturas no activos
* &amp;lbrack;Relleno poligonal&amp;rbrack; Previsualización instantánea ALT
* &amp;lbrack;Relleno poligonal&amp;rbrack; Método abreviado para cambiar temporalmente a Polyloop (MAYÚS+A)
* &amp;lbrack;Viewport&amp;rbrack; Mostrar conjunto de texturas/resaltado de selección de Mosaico de UV
* &amp;lbrack;Viewport&amp;rbrack; Añadir soporte para Transparencia Independiente de Pedidos en la ventana gráfica en tiempo real
* &amp;lbrack;Configuración de visualización&amp;rbrack; Reorganizar la configuración de visualización en nuevos grupos
* &amp;lbrack;Herramienta&amp;rbrack; Añadir compatibilidad con la fusión aditiva con trazos de pincel
* &amp;lbrack;Herramienta&amp;rbrack; Añadir compatibilidad con la fusión aditiva con relleno poligonal
* &amp;lbrack;USD&amp;rbrack; Las USD exportadas con mapa de opacidad se vuelven transparentes en Arnold
* &amp;lbrack;Nvidia&amp;rbrack; Agregar advertencia sobre los controladores más recientes de NVIDIA (616.56 a 617.14)
* Añadir nueva entrada de mapa del motor &quot;mesh_uv_next&quot;
* Actualizar bakeres a la versión 3.23.0
* Actualizar el motor de Substance a la versión 9.6.1

**Corregido:**

* &amp;lbrack;Haciendo un bake&amp;rbrack; La oclusión ambiental Ignorar cara posterior por nombre de malla no funciona
* &amp;lbrack;Haciendo un bake&amp;rbrack; &amp;lbrack;AMD&amp;rbrack; Dispositivo perdido al hacer un bake con mallas de polietileno altas y pesadas
* &amp;lbrack;Performance&amp;rbrack; Uso de cerdos VRAM Painter
* &amp;lbrack;Viewport&amp;rbrack; Faltan texturas al abrir proyectos en pantallas HDPI
* &amp;lbrack;Herramienta&amp;rbrack; El modo de fusión aparece atenuado al pintar en una máscara
* Carpetas temporales no eliminadas después de la exportación en la red
* &amp;lbrack;USD&amp;rbrack; La geometría de USD exportada se divide a lo largo de los bordes UV
* &amp;lbrack;USD&amp;rbrack; Bloqueo al cargar USDz mal formado

### 12.1.5

Fecha de publicación: **2026/09/15**

Resumen: **Versión secundaria**

**Corregido:**

* La exportación de imágenes de un estante a una red ya no funciona
* &amp;lbrack;Generador&amp;rbrack; Si se establece &quot;usar textura&quot; en false, no se desactiva el uso de la entrada de textura
* Bloqueo de la ventana gráfica al guardar mientras se edita la proyección 3d
* La resolución de capas de material es demasiado baja

### 12.1.4

Fecha de publicación: **2026/09/04**

Resumen: **Versión secundaria**

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; Bloqueo al importar o exportar archivos cuyo nombre de archivo contiene caracteres no ASCII

### 12.1.3

Fecha de publicación: **2026/08/26**

Resumen: **Versión secundaria**

**Agregado:**

* Actualizar el motor de Substance a la versión 9.4.6

**Corregido:**

* &amp;lbrack;Selector de escala de grises&amp;rbrack; El selector permanece abierto después de cambiar la herramienta
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; La corrección de sesgo se rompe al pintar y deshacer
* &amp;lbrack;Herramienta de proyección&amp;rbrack; La herramienta de proyección bloquea la interacción Ventana gráfica
* &amp;lbrack;Trazo dinámico&amp;rbrack; Faltan parámetros de trazo dinámico en las propiedades del pincel
* La exportación a una red ya no funciona

### 12.1.2

Fecha de publicación: **2026/08/03**

Resumen: **Versión secundaria**

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; Algunos Substance pueden provocar un bloqueo cuando se procesan
* &amp;lbrack;Bloqueo&amp;rbrack; Volver a importar malla en modo hacer un bake
* &amp;lbrack;Bloqueo&amp;rbrack; Si no se inicializa la visualización de gráficos, se puede producir un bloqueo
* &amp;lbrack;Bloqueo&amp;rbrack; La exportación de texturas puede producir bloqueos en algunos casos al actualizar el registro
* &amp;lbrack;Bloqueo&amp;rbrack; Bloqueo en el modo de hacer un bake en algunos casos al cargar/actualizar el mapa de entorno
* &amp;lbrack;Haciendo un bake&amp;rbrack; Si se vuelve a iniciar hacer un bake después de modificar el archivo de alta poly, se puede producir un bloqueo
* &amp;lbrack;Enviar a Photoshop&amp;rbrack; No se puede exportar la máscara de la capa
* &amp;lbrack;Motor&amp;rbrack; El resultado del punto de anclaje no se procesa entre una máscara y un canal de color

### 12.1.1

Fecha de publicación: **2026/07/09**

Resumen: Versión secundaria

Añadido:

* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Exponer sesgo base modo normal: malla o por triángulo
* &amp;lbrack;Propiedades&amp;rbrack; Hacer que los colores uniformes siempre se restablezcan al valor predeterminado de su canal
* &amp;lbrack;OpenPBR&amp;rbrack; Reagrupar canales por categorías en la ventana Exportar Texturas para crear plantillas de salida
* Actualizar el motor de Substance a la versión 9.4.5

Corregido:

* &amp;lbrack;Proyecto&amp;rbrack; Abrir y guardar algunos proyectos puede tardar más de lo habitual
* &amp;lbrack;Bloqueo&amp;rbrack; La recarga de varias mallas puede provocar un bloqueo
* &amp;lbrack;Bloqueo&amp;rbrack; Eliminar un canal mientras está en el modo de vista de máscara provoca un bloqueo
* &amp;lbrack;Bloqueo&amp;rbrack; Algunos Substance pueden provocar un bloqueo cuando se procesan
* &amp;lbrack;Pintura Skew&amp;rbrack; La herramienta Seleccionado en el sesgo de pintura permanece seleccionada después de cambiar al modo de pintura
* &amp;lbrack;Haciendo un bake configuración común&amp;rbrack; La configuración de la distancia de la jaula no actualiza la visualización de la malla metálica de la jaula y el sombreador
* &amp;lbrack;Motor&amp;rbrack; El relleno UV del modo &quot;3D Space Neighbor&quot; no funciona bien en triángulos finos
* &amp;lbrack;Motor&amp;rbrack; El resultado del punto de anclaje no se procesa entre una máscara y un canal de color

### 12.1.0

Fecha de publicación: **2026/06/23**

Resumen: **Esta actualización es una versión importante, contiene mejoras de bakeres con el nuevo estado de IU predeterminado de hace un bake, mapa de sesgo de pintura, reprocesamiento automático, nueva opción para el desajuste UV automático para mallas de superficie dura y OpenPBRs. Para obtener más detalles, vea las notas de la versión completas.**

**Agregado**:

* &amp;lbrack;Sesgar hacer un bake&amp;rbrack; Herramientas de pintura de sesgo
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Adición de sombreadores de previsualización de sesgo y elementos visuales vectoriales de dirección de sesgo al pintar un mapa de sesgo
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Opción Añadir protección de bordes
* &amp;lbrack;Sesgar hacer un bake&amp;rbrack; Reprocesamiento automático
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Interfaz de lista de mapa de malla de reprocesamiento
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Dividir mapa de malla / Configuración de Haga un bake común + Mover configuración común fuera de la lista de mapas de malla solo para colores o máscaras
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Cambiar botones de la barra de herramientas
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Mostrar el conmutador de Simetría para el pincel en la barra de herramientas superior
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Opciones de cambio de nombre en el menú Sincronización de lista de mapa de malla
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Cuadros de diálogo Actualizar estado de sincronización y activado
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Crear variante del selector de color de escala de grises
* &amp;lbrack;Sesgar Hacer un bake&amp;rbrack; Icono Actualizar modo de hacer un bake
* &amp;lbrack;Auto Unwrap&amp;rbrack; Opción Integrar superficie dura
* &amp;lbrack;OpenPBR&amp;rbrack; Añadir soporte para OpenPBR 1.1
* &amp;lbrack;OpenPBR&amp;rbrack; Convertir OpenPBR en el flujo de trabajo y sombreador predeterminados
* &amp;lbrack;OpenPBR&amp;rbrack; Importar materiales y texturas de OpenPBR mediante USD
* &amp;lbrack;OpenPBR&amp;rbrack; Exportar materiales y texturas de OpenPBR mediante USD
* &amp;lbrack;OpenPBR&amp;rbrack; Actualizar la ventana Exportar Texturas para mostrar la convención de nomenclatura del OpenPBR
* &amp;lbrack;OpenPBR&amp;rbrack; Añadir documentación sobre los cambios al OpenPBR de asistencia
* &amp;lbrack;OpenPBR&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Añada un nuevo MDL para apoyar al OpenPBR 1.1 en Israel
* Varias mejoras menores de las exportaciones USD
* &amp;lbrack;UI&amp;rbrack; Adición de una advertencia en la ventana gráfica al intentar realizar una pintura en otro conjunto de texturas
* &amp;lbrack;Aplanar&amp;rbrack; Permitir acoplar todas las capas con instancias en los conjuntos de texturas
* &amp;lbrack;Configuración del conjunto de texturas&amp;rbrack; Permitir seleccionar varios canales a la vez a través de una nueva ventana
* &amp;lbrack;Historial&amp;rbrack; Actualizar &quot;valor&quot; Deshacer el texto de la entrada para reflejar el nombre del parámetro
* &amp;lbrack;Pila de capas&amp;rbrack; Hacer que los efectos de relleno de las máscaras se vean en blanco de forma predeterminada (1.0)
* &amp;lbrack;Substance&amp;rbrack; Añadir nueva entrada de mapa del motor &quot;mesh_hard_edges_triangle&quot;
* &amp;lbrack;Substance&amp;rbrack; Añadir nueva entrada de mapa del motor &quot;mesh_hard_edges&quot;
* &amp;lbrack;Sombreador&amp;rbrack; Impedir que las instancias del sombreador compartan los mismos nombres
* &amp;lbrack;Sombreador&amp;rbrack; Utilice el sombreador de la plantilla de proyecto al importar un archivo USD o GLTF
* Actualizar Adobe Color Engine a la versión 7.0
* Actualizar la versión mínima de MacOSX a 13.0 (Ventura)
* &amp;lbrack;Contenido&amp;rbrack; Nuevas plantillas de proyecto para el OpenPBR
* &amp;lbrack;Contenido&amp;rbrack; Actualizar proyectos de muestra para utilizar el nuevo sombreador de OpenPBR
* &amp;lbrack;Python&amp;rbrack; Expanda la API de máscara de geometría para permitir modos de inclusión y exclusión como en la interfaz de usuario

**Corregido**:

* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Configuración de mapas de malla&amp;rbrack; Aplicación de ajustes a otros conjuntos de texturas
* &amp;lbrack;Bloqueo&amp;rbrack; Al hacer un bake la curvatura del mapa sin el espacio del mundo normal
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Hacer un bake&amp;rbrack; Hacer un bake con jaula personalizada activada pero sin bloqueos de archivo seleccionados
* &amp;lbrack;Bloqueo&amp;rbrack; Cancelación de hace un bake de AO
* &amp;lbrack;Auto-Cage&amp;rbrack; Carga infinita cuando la ruta del archivo de poli alto no es válida
* &amp;lbrack;Linux&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; El selector de color a veces puede ser completamente negro o no aparecer
* &amp;lbrack;Herramienta Relleno poligonal&amp;rbrack; La herramienta no funciona con sistemas que no sean PBR
* &amp;lbrack;&amp;lbrack;Pintura&amp;rbrack; Al eliminar el canal de color base no se elimina el color pintado anteriormente
* &amp;lbrack;USD&amp;rbrack; No se detectan correctamente todas las instancias del sombreador
* &amp;lbrack;Substance&amp;rbrack; Solo se tiene en cuenta el primer uso de un nodo de entrada/salida
* &amp;lbrack;Sombreador&amp;rbrack; La oclusión ambiental se aplica dos veces con conjuntos de texturas utilizando diferentes métodos de mezcla
* &amp;lbrack;Motor&amp;rbrack; Las texturas normales con un canal azul vacío (negro) pueden producir resultados de mezclas incorrectos
* &amp;lbrack;GLTF Import&amp;rbrack; La fusión alfa está activada en todos los conjuntos de texturas
* &amp;lbrack;GLTF Export&amp;rbrack; La fusión alfa siempre está activada en la exportación
* &amp;lbrack;Exportar&amp;rbrack; La geometría de doble cara siempre está desactivada al importar un fichero GLTF
* &amp;lbrack;Javascript&amp;rbrack; La modificación de la configuración de sombreadores no contribuye al historial de deshacer
* &amp;lbrack;Muestras&amp;rbrack; La dispersión subsuperficial no está activada en la configuración de visualización para Meet Mat

### 12.0.3

Fecha de publicación: **2026/05/05**

Resumen: **Versión secundaria**

**Agregado:**

* Actualizar bakeres a la versión 3.2.2
* Actualizar el motor de Substance a la versión 9.4.3
* &amp;lbrack;Python&amp;rbrack; Guardar un material inteligente en una ubicación específica

**Corregido:**

* &amp;lbrack;Ubuntu&amp;rbrack; Bloqueo al seleccionar material
* &amp;lbrack;Mac&amp;rbrack; Aparece una ventana emergente recurrente para solicitar acceso a los datos de otras aplicaciones
* &amp;lbrack;Haciendo un bake&amp;rbrack; Pueden aparecer defectos en el mapa de curvatura
* &amp;lbrack;Haciendo un bake&amp;rbrack; Hacer un bake es más lento en algunos casos
* &amp;lbrack;Deformar a geometría&amp;rbrack; La deformación de la geometría se desactiva en algunos casos
* &amp;lbrack;Mosaico de UV&amp;rbrack; El alfa extraído del punto de anclaje es ignorado por otros mosaicos
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Excepciones en la consola de Python con SSL
* &amp;lbrack;Python&amp;rbrack; bloqueo de Painter a la salida con widgets Qt sobrantes

### 12.0.2

Fecha de publicación: **2026/04/07**

Resumen: **Versión secundaria**

**Agregado:**

* &amp;lbrack;Administración de color&amp;rbrack; Añada nuevos OCIO para especificar el espacio de color predeterminado del selector de color
* &amp;lbrack;Python&amp;rbrack; Exponer la configuración de desajuste automático en la API de Python

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; Si no hay suficiente espacio en disco, los proyectos se pueden dañar o almacenar en bloqueo
* &amp;lbrack;Bloqueo&amp;rbrack; &amp;lbrack;Cinta&amp;rbrack; El uso de la cinta puede causar bloqueos en algunos proyectos
* &amp;lbrack;Bloqueo&amp;rbrack; &amp;lbrack;Haciendo un bake&amp;rbrack; bloqueo cuando el archivo .assbin no se puede escribir en la carpeta
* &amp;lbrack;Importar&amp;rbrack; OBJ mallas de Stager pueden fallar en la creación del proyecto
* &amp;lbrack;Importar&amp;rbrack; OBJ ha perdido la cara en algunos casos
* &amp;lbrack;Importar&amp;rbrack; USD malla sin ningún material asignado puede generar bloqueo al importarla
* &amp;lbrack;Ruta de acceso rellena&amp;rbrack; No se ve afectado por la simetría
* &amp;lbrack;Stencil&amp;rbrack; La previsualización tiene una resolución inferior a la del resultado pintado
* &amp;lbrack;UI&amp;rbrack; &#39;uv island&#39; sigue apareciendo en la información sobre herramientas de origen de color del mapa de ID
* &amp;lbrack;Mostrar&amp;rbrack; Las sombras aparecen invertidas
* &amp;lbrack;Viewport&amp;rbrack; La proyección de deformación transforma los restos después de cambiar al modo de hacer un bake
* &amp;lbrack;Deformar&amp;rbrack; La cuadrícula desaparece cuando la escala se establece en 0 en el eje Z con la opción Deformar en geometría activada
* &amp;lbrack;Python&amp;rbrack; Error inesperado al agregar un canal con modificación de ámbito

### 12.0.1

Fecha de publicación: **2026/03/18**

Resumen: **Versión secundaria**

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Congelar&amp;rbrack; Exportación desde proyectos específicos

### 12.0.0

Fecha de publicación: **2026/03/09** Resumen: **Esta es una versión importante. Esta versión contiene las funciones de acoplar capas, deformar en geometría, nuevos efectos de posprocesamiento, mejoras en la nueva ventana de proyecto y otras mejoras.**

**Agregado**:

* &amp;lbrack;Acoplar capas&amp;rbrack; Acoplamiento de capas dentro de la pila de capas
* &amp;lbrack;Acoplar capas&amp;rbrack; Exportar capas acopladas al disco
* &amp;lbrack;Deformar a geometría&amp;rbrack; Adición de una nueva función de deformación automática a las proyecciones de deformación
* &amp;lbrack;Post-effects&amp;rbrack; Sustituya los efectos de posprocesamiento por otros nuevos
* &amp;lbrack;Post-effects&amp;rbrack; Actualizar asignador de tonos
* &amp;lbrack;Post-effects&amp;rbrack; Añadir nuevo uso para recursos posteriores a los efectos
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Post-effects&amp;rbrack; Integrar activos predeterminados posteriores a los efectos en la biblioteca
* &amp;lbrack;Nuevo proyecto&amp;rbrack; Mejorar la interfaz de usuario para la creación de proyectos
* &amp;lbrack;Nuevo proyecto&amp;rbrack; Cambios en la función de reimportación de malla
* &amp;lbrack;Nuevo proyecto&amp;rbrack; Permitir la apertura de archivos \*.geo.usd
* &amp;lbrack;Configuración del proyecto&amp;rbrack; Mejorar la interfaz de usuario para la configuración del proyecto
* Actualizar USD biblioteca a la versión 25.05
* Actualizar Substance Engine a la versión 9.3.4
* Aumentar controladores mínimos a 25.3.1/25.Q2 para las GPU AMD
* Actualizar Qt a 6.8.6
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Actualizar la API de JavaScript a la versión 1.1.20
* Actualizar Python a 3.13

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; El cambio de una salida de canal de material en una máscara puede provocar un bloqueo
* &amp;lbrack;Importar&amp;rbrack; Las texturas de EXR se fuerzan en sRGB en lugar de lineales al importar archivos USD
* &amp;lbrack;Mosaicos de UV&amp;rbrack; La secuencia de imágenes con una sola imagen también llena otros Mosaicos de UV
* &amp;lbrack;Haciendo un bake&amp;rbrack; El AO es diferente entre la CPU y la GPU al hacer un bake
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack; El color base de la ventana gráfica no coincide con el selector de color
* &amp;lbrack;USD&amp;rbrack; Los valores uniformes no se importan en algunos casos

## Versión 11

### 11.1.3

Fecha de publicación: **2026/02/12** Resumen: **Versión secundaria**

**Corregido**:

* &amp;lbrack;Pintura&amp;rbrack; La plantilla y la simetría no funcionan en algunos casos
* &amp;lbrack;Ruta&amp;rbrack; No hay actualizaciones al cambiar el regulador de opacidad del trazo de difuminado
* &amp;lbrack;Proyecto&amp;rbrack; No se puede realizar la pintura en alguna geometría
* &amp;lbrack;Cinta&amp;rbrack; El trazado instanciado desaparece al cambiar la resolución del conjunto de texturas
* &amp;lbrack;UI&amp;rbrack; El selector de color se puede reducir y desaparecer en algunos casos

### 11.1.2

Fecha de publicación: **2026/01/13** Resumen: **Versión secundaria**

**Agregado**:

* &amp;lbrack;Haciendo un bake&amp;rbrack; Mejorar el tiempo de hace un bake del proyecto de Mosaicos de UV con el guardado asíncrono
* &amp;lbrack;Shaders&amp;rbrack; Mención en cambios de registro de API del sombreador tras migración de Vulkan
* Actualizar OpenEXR a la versión 3.4.4

**Corregido**:

* &amp;lbrack;Bloqueo&amp;rbrack; Bloqueo durante el inicio en la serie Nvidia GTX 10xx
* &amp;lbrack;Bloqueo&amp;rbrack; El uso del selector de color en diferentes conjuntos de texturas puede provocar un bloqueo al salir de la aplicación
* &amp;lbrack;Rendimiento&amp;rbrack; Problema de rendimiento al pintar en un proyecto con muchas capas
* &amp;lbrack;Rendimiento&amp;rbrack; Retraso al pintar con un lápiz de Tablet PC gráfico
* &amp;lbrack;UI&amp;rbrack; Los ajustes de la cámara permanecen desactivados en el modo de procesamiento (Iray)
* &amp;lbrack;Cinta&amp;rbrack; El trazado puede superponerse inesperadamente después de una esquina en algunos casos
* &amp;lbrack;Cinta&amp;rbrack; Problema de rendimiento con Mosaicos de UV
* &amp;lbrack;Substance&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Las entradas de imagen desaparecen al contraerse
* &amp;lbrack;Substance&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Los grupos anidados pueden permanecer aunque Visible si los oculte
* &amp;lbrack;Haciendo un bake&amp;rbrack;&amp;lbrack;UI&amp;rbrack; No se puede establecer el radio de muestreo de curvatura más allá de 0,01
* &amp;lbrack;Haciendo un bake&amp;rbrack;&amp;lbrack;UI&amp;rbrack; No se puede establecer la distancia máxima del oclusor más allá de 1
* &amp;lbrack;Haciendo un bake&amp;rbrack; El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y hago un bake bajo como alto
* &amp;lbrack;Haciendo un bake&amp;rbrack; El mapa de ID no hace un bake los colores de vértice de FBX en modo Bajo como Alto
* &amp;lbrack;Contenido&amp;rbrack; El filtro Paso alto genera colores atenuados en canales con gestión de color

### 11.1.1

Fecha de publicación: **2025/12/09** Resumen: **Versión secundaria**

**Agregado**:

* &amp;lbrack;Rendimiento&amp;rbrack; Mejorar el rendimiento de los Mosaicos de UV al calcular texturas parciales
* &amp;lbrack;Bakeres&amp;rbrack; Actualizar a la versión 3.15.4

**Corregido**:

* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack; Bloqueo de guardar siempre el proyecto de la versión anterior
* &amp;lbrack;Bloqueo&amp;rbrack; El cierre de un proyecto a veces puede provocar un bloqueo
* &amp;lbrack;Proyecto&amp;rbrack; Error &quot;los miembros no coinciden en el recuento&quot; al abrir el proyecto realizado en la versión anterior
* &amp;lbrack;Haciendo un bake&amp;rbrack; Los Mosaicos de UV no se combinan con los resultados hechos un bake anteriores, si los hay
* &amp;lbrack;Haciendo un bake&amp;rbrack; Dispositivo perdido incluso con el trazado de rayos desactivado en la serie Nvidia GTX 10XX
* &amp;lbrack;Haciendo un bake&amp;rbrack; El AO con normal tiene defectos en los bordes porque no hay relleno
* &amp;lbrack;Haciendo un bake&amp;rbrack; El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y &quot;coincidencia por nombre&quot; en
* &amp;lbrack;Haciendo un bake&amp;rbrack; El mapa de ID es totalmente negro si a alguna malla de alta densidad le faltan colores de vértice
* &amp;lbrack;Cinta&amp;rbrack; La información sobre herramientas del modo de fusión Alfa menciona el modo de fusión de pantalla en lugar de Sobreexposición lineal
* &amp;lbrack;Ruta&amp;rbrack; Las tangentes crean un bucle inesperado cuando el punto se mueve de cerca a los extremos del trazado
* &amp;lbrack;Herramienta&amp;rbrack; La previsualización de material no funciona cuando se utiliza la proyección en una máscara
* &amp;lbrack;Motor&amp;rbrack; Pintar trazos pequeños puede dar como resultado artefactos de bloque
* &amp;lbrack;Sombreador&amp;rbrack; Al deshacer la creación de la instancia del sombreador, no se elimina correctamente
* &amp;lbrack;Exportar&amp;rbrack; El modo de Alpha para la exportación GLTF siempre está establecido en MASK
* &amp;lbrack;Python&amp;rbrack; Error inesperado al editar la pila de capas fuera del bloque de modificación del ámbito

**Problemas conocidos**:

* &amp;lbrack;Cinta&amp;rbrack; Problema de rendimiento con Mosaicos de UV
* &amp;lbrack;Cinta&amp;rbrack; El trazado puede superponerse inesperadamente después de una esquina en algunos casos
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Cinta&amp;rbrack; La creación de textos muy largos en la cinta de opciones puede causar bloqueo
* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;Motor&amp;rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &amp;lbrack;Python&amp;rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.1.0

Fecha de lanzamiento: **18/11/2025** Resumen: **Esta actualización es una versión importante, contiene la nueva herramienta Cinta de opciones con contenido nuevo dedicado, compatibilidad de simetría para capas de relleno, parámetro de tamaño físico para desplazamiento, rendimiento mejorado a través de los bakeres actualizados, compatibilidad total con Vulkan para Windows y Linux y otras mejoras.**

**Agregado**:

* Nueva herramienta de cinta
* &amp;lbrack;Herramienta&amp;rbrack; Agregar nueva herramienta Cinta para crear trazados perfectos
* &amp;lbrack;Cinta&amp;rbrack; Añadir métodos abreviados de cinta preestablecidos en la ventana Propiedades
* &amp;lbrack;Cinta&amp;rbrack; Permitir cambiar la opacidad de la cinta de opciones por vértice en el trazado
* &amp;lbrack;Cinta&amp;rbrack; Permitir cambiar el tamaño de la cinta de opciones por vértice en el trazado
* &amp;lbrack;Cinta&amp;rbrack; Quitar el inicio/fin definido en un Substance cuando las rutas están cerradas
* &amp;lbrack;Cinta&amp;rbrack; Vista previa de Eliminar trazado/material en la ventana de propiedades para las herramientas Pintura/Borrador/Dedo de trazado
* &amp;lbrack;Cinta&amp;rbrack; Añada modos de fusión para el alfa y algunos canales cuando se superpongan automáticamente
* Rellenar simetría
* &amp;lbrack;Rellenar&amp;rbrack; Añadir compatibilidad con la simetría en capas y efectos de relleno
* &amp;lbrack;Fill&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Mostrar la configuración de simetría en la ventana de propiedades para capas y efectos de relleno
* &amp;lbrack;Rellenar&amp;rbrack; Interfaz de usuario de reprocesamiento de la configuración de simetría tanto en el menú Ventana como en la ventana Propiedades
* &amp;lbrack;Rellenar&amp;rbrack; Reorientar correctamente las texturas normales al proyectar en modo de deformación
* desplazamiento tamaño físico
* &amp;lbrack;Desplazamiento&amp;rbrack; Usar tamaño físico como unidad de desplazamiento
* Mejora del rendimiento
* &amp;lbrack;Rendimiento&amp;rbrack; Mejorar la representación de trazos de pincel pequeños en triángulos grandes
* &amp;lbrack;Rendimiento&amp;rbrack; Mejorar el tiempo de compilación del Sombreador
* &amp;lbrack;Rendimiento&amp;rbrack; Compatibilidad total con Vulkan para Windows y Linux
* &amp;lbrack;Rendimiento&amp;rbrack; Bakeres actualizados con procesamiento de GPU más rápido y compatibilidad con trazados de rayos AMD
* &amp;lbrack;UI&amp;rbrack; Reorganizar las propiedades de las herramientas en grupos y contraer algunos de forma predeterminada
* &amp;lbrack;Motor&amp;rbrack; Actualizar Substance Engine a la versión 9.2.5
* &amp;lbrack;Substance&amp;rbrack; Anulación de resolución de exposición para recursos de Substance en Herramientas y rellenos
* &amp;lbrack;Exportar&amp;rbrack; Actualizar ajuste preestablecido de exportación de Mapas de malla para exportar texturas en escala de grises
* Python
* &amp;lbrack;Haciendo un bake&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Indicar en el registro de cambios los cambios después de actualizar bakeres
* &amp;lbrack;Python&amp;rbrack; Exponer la configuración de simetría de relleno en Python
* Contenido y nuevo contenido
* &amp;lbrack;Contenido&amp;rbrack; Añadir 75 nuevos ajustes preestablecidos de herramientas para la herramienta Cinta de opciones
* &amp;lbrack;Contenido&amp;rbrack; Actualizar el recurso generador de degradados para que sea compatible con la cinta de opciones

**Corregido**:

* &amp;lbrack;Bloqueo&amp;rbrack; La carga de otro proyecto mientras el ajuste de ruta está activado puede causar bloqueos
* &amp;lbrack;Bloqueo&amp;rbrack; Al hacer clic con el botón derecho en el panel Trazado con información de otra sesión del portapapeles, se puede crear un bloqueo
* &amp;lbrack;UI&amp;rbrack; La interfaz se desplaza hacia arriba en las propiedades de la herramienta al crear un trazado
* &amp;lbrack;UI&amp;rbrack; El cursor del ratón desaparece cuando la visualización de la ventanilla de trazado está oculta
* &amp;lbrack;Ruta&amp;rbrack; Copiar/pegar diferentes propiedades de herramienta en el panel Trazado genera propiedades inestables
* &amp;lbrack;Herramienta&amp;rbrack; Los ajustes preestablecidos de las herramientas Borrador y Difuminado no siempre actualizan la selección de canales
* &amp;lbrack;Herramienta&amp;rbrack; El valor pintado es gris, pero la interfaz de usuario muestra blanco después de cargar el ajuste preestablecido de herramientas de color en la máscara
* &amp;lbrack;Herramienta&amp;rbrack; El ajuste preestablecido creado a partir de la máscara conserva los valores de canales cargados de otro ajuste preestablecido
* &amp;lbrack;Substance&amp;rbrack; No se tiene en cuenta la anulación del espacio de color normal definido en el gráfico
* &amp;lbrack;Contenido&amp;rbrack; El recurso de forma de pincel predeterminado utiliza un Substance obsoleto

**Problemas conocidos**:

* El historial de instancias del sombreador no se rastrea correctamente
* &amp;lbrack;Cinta&amp;rbrack; Problema de rendimiento con Mosaicos de UV
* &amp;lbrack;Cinta&amp;rbrack; El trazado puede superponerse inesperadamente después de una esquina en algunos casos
* &amp;lbrack;Cinta&amp;rbrack; Las tangentes crean bucles no deseados cuando el punto se mueve de cerca a los extremos del trazado
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Cinta&amp;rbrack; La creación de textos muy largos en la cinta de opciones puede causar bloqueo
* &amp;lbrack;Herramienta&amp;rbrack; La previsualización de material no funciona cuando se utiliza la proyección en una máscara
* &amp;lbrack;Haciendo un bake&amp;rbrack; El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y &quot;coincidencia por nombre&quot; activado
* &amp;lbrack;Haciendo un bake&amp;rbrack; El AO con normal tiene defectos en los bordes debido a la falta de relleno
* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;Motor&amp;rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &amp;lbrack;Python&amp;rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.0.3

Fecha de publicación: **2025/08/05** Resumen: **Versión secundaria**

**Agregado**:

* &amp;lbrack;Substance 3D Assets&amp;rbrack; Adición de un punto de notificación al panel Activos 3D
* &amp;lbrack;VFX Platform 2025&amp;rbrack; Añadir ACE configuración 2.0 en la configuración de gestión de color
* &amp;lbrack;VFX Platform 2025&amp;rbrack; Actualice OCIO a la versión 2.4.2
* Actualizar Iray a la versión 2024.10
* &amp;lbrack;Motor&amp;rbrack; Actualizar a Substance Engine v.9.2.3
* &amp;lbrack;Nvidia&amp;rbrack; Aumentar la versión mínima de controladores de NVIDIA a 572.60 (Windows) y 570.169 (Linux)

**Corregido**:

* &amp;lbrack;Python&amp;rbrack; La modificación de ámbito no aparece en la ventana Historial

**Problemas conocidos**:

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;Motor&amp;rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &amp;lbrack;Python&amp;rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.0.2

Fecha de publicación: **2025/06/10** Resumen: **Versión secundaria**

**Agregado**:

* &amp;lbrack;Mac&amp;rbrack; Agregar advertencia sobre versiones específicas del sistema operativo que producen artefactos
* &amp;lbrack;Actualización automática&amp;rbrack; Mejoras menores de UX en el registro de errores de Activos
* &amp;lbrack;Desenvolvimiento automático&amp;rbrack; Actualice a la versión 1.3.2 con mejoras de unión
* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;FBX&amp;rbrack; Añade compatibilidad con varios conjuntos UV con datos dispersos
* &amp;lbrack;Exportar&amp;rbrack; Las mallas exportadas como FBX no tienen sus conjuntos UV adicionales si los hay durante la importación

**Corregido**:

* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; Bloqueo al guardar en la unidad de red
* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;Tablet&amp;rbrack; Parpadeo al realizar una panorámica
* &amp;lbrack;SpaceMouse&amp;rbrack; Problema al trabajar con la herramienta Trazado
* &amp;lbrack;Auto-cage&amp;rbrack; No se puede hacer un bake después de una recarga de malla
* &amp;lbrack;Actualización automática&amp;rbrack; La secuencia de imágenes no se vuelve a cargar cuando falta el primer mosaico
* &amp;lbrack;Ruta&amp;rbrack; La tangente personalizada puede afectar a otras tangentes
* &amp;lbrack;Ruta&amp;rbrack; El trazado no aparece en el conjunto de texturas si el primer punto está en otro conjunto de texturas
* &amp;lbrack;UI&amp;rbrack; Algunos menús siempre se desactivan después de abrir un proyecto (por ejemplo: simetría)
* &amp;lbrack;Propiedades&amp;rbrack; No es posible utilizar/cargar ajustes preestablecidos de herramientas con la herramienta Trazado relleno
* &amp;lbrack;USD&amp;rbrack; No se reconocen varios conjuntos UV en el sombreador personalizado al utilizar archivos USD
* &amp;lbrack;USD&amp;rbrack; Las cámaras con los mismos nombres se anulan
* &amp;lbrack;Exportar&amp;rbrack; Enviar a Photoshop genera un espacio de color incorrecto para los resultados de color y escala de grises
* &amp;lbrack;Exportar&amp;rbrack; Los canales de escala de grises con alfa se exportan como color en lugar de como escala de grises con formato PNG
* &amp;lbrack;Exportar&amp;rbrack; La exportación de un canal de escala de grises como PSD genera un archivo no válido o truncado
* &amp;lbrack;Contenido&amp;rbrack; El filtro de deformación en modo multidireccional no funciona
* &amp;lbrack;Python&amp;rbrack; No se puede asignar el error de lista al rastrear nodos de pila de capas

**Problemas conocidos**:

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;Motor&amp;rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &amp;lbrack;Python&amp;rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.0.1

Fecha de publicación: **2025/04/10** Resumen: **Versión secundaria**

Nota: La versión de **Linux CCD se retrasará hasta el 29 de abril**

**Agregado:**

* Actualizar a Qt 6.5.8
* &amp;lbrack;Substance&amp;rbrack; Agregar mensaje de registro para filtros cuando varias entradas de imagen comparten el mismo uso
* &amp;lbrack;Nvidia&amp;rbrack; Agregar advertencia sobre los controladores más recientes de NVIDIA (572.47)

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; Al arrastrar y soltar una barra lateral con un uso en ranuras de un solo canal
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Path&amp;rbrack; La opción Cambiar tipo de trazado no está atenuada al no hacer clic en un trazado específico
* &amp;lbrack;Rellenar ruta&amp;rbrack; No debería poder seleccionar material de la sustancia
* &amp;lbrack;Motor&amp;rbrack; Artefactos a lo largo de trazos de pincel
* &amp;lbrack;Motor&amp;rbrack; Los trazados se pueden romper con ajustes específicos
* Problema con el menú desplegable para el espacio de color del cuentagotas
* &amp;lbrack;Actualización automática&amp;rbrack; &amp;lbrack;Python&amp;rbrack; Mensaje de error incorrecto al utilizar ResourceID sin versión
* &amp;lbrack;Sombreador&amp;rbrack; Bloqueo al abrir algunos proyectos

**Problemas conocidos:**

* &amp;lbrack;SpaceMouse&amp;rbrack; Problema al trabajar con la herramienta Trazado
* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;Motor&amp;rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &amp;lbrack;Python&amp;rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.0.0

Fecha de lanzamiento: **2025/03/11** Resumen: **Versión principal, nueva función de actualización automática, herramienta Ruta de acceso rellena y otras mejoras en la ruta, así como nuevos filtros y una generación experimental de Jaula automática para hacer un bake**

**Agregado**:

* Actualización automática
* &amp;lbrack;Actualización automática&amp;rbrack; Actualización automática de activos modificados en el panel Activos
* &amp;lbrack;Actualización automática&amp;rbrack; Actualización automática de activos modificados en todo el proyecto
* &amp;lbrack;Actualización automática&amp;rbrack; Mantener desactivada la actualización automática de forma predeterminada
* &amp;lbrack;Actualización automática&amp;rbrack; Hacer que la actualización sea opcional si los parámetros del recurso no coinciden (.sbsar, .glsl, .ai, .svg)
* &amp;lbrack;Actualización automática&amp;rbrack; Añadir variable de entorno para desactivar la función de actualización automática
* &amp;lbrack;Actualización automática&amp;rbrack;&amp;lbrack;SBSAR&amp;rbrack; Convertir la actualización en opcional si los parámetros del recurso no coinciden
* Trazado relleno
* &amp;lbrack;Ruta&amp;rbrack;&amp;lbrack;Rellenar&amp;rbrack; Añadir una nueva herramienta para crear trazados rellenos
* Mejoras de ruta
* &amp;lbrack;Ruta&amp;rbrack; Crear trazado que se ajusta a polígonos
* &amp;lbrack;Ruta&amp;rbrack; Permitir cambiar los tipos de ruta
* &amp;lbrack;Ruta&amp;rbrack; Permitir copiar y pegar datos de vértices de trazado entre contenido y máscara
* &amp;lbrack;Ruta&amp;rbrack; Permitir para restringir el ángulo al crear un nuevo punto
* &amp;lbrack;Ruta&amp;rbrack; Permitir la creación de puntos de restricción en una línea
* &amp;lbrack;Ruta&amp;rbrack; Cerrar forma con un solo clic
* &amp;lbrack;Ruta&amp;rbrack; Mostrar información de ruta
* &amp;lbrack;Ruta&amp;rbrack; Permitir escalar y rotar vértices de trazado
* &amp;lbrack;Path&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Facilita el acceso a las herramientas de transformación
* &amp;lbrack;Ruta&amp;rbrack; Añadir previsualización de trazado
* &amp;lbrack;Ruta&amp;rbrack; Desactivar la previsualización de trazado con Mayús + P
* &amp;lbrack;Ruta&amp;rbrack; Mejorar la edición de tangentes desde la vista lateral
* &amp;lbrack;Ruta&amp;rbrack; Permitir el enfoque en una ruta 3D
* &amp;lbrack;Ruta&amp;rbrack; Los vértices deben conservar el estado de selección al activar o desactivar la IU de nuevo
* &amp;lbrack;Ruta&amp;rbrack; Permitir la eliminación de la ruta mediante Retroceso
* &amp;lbrack;Ruta&amp;rbrack; Mantener lista de rutas abierta si el usuario la expande
* &amp;lbrack;Ruta&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Cambiar el nombre de los duplicados al copiar y pegar correctamente
* &amp;lbrack;Ruta&amp;rbrack; Mejoras en la IU y la información sobre herramientas
* Rendimiento
* &amp;lbrack;Rendimiento&amp;rbrack; Mejorar el rendimiento de la ventanilla al utilizar un nivel de teselación alto
* &amp;lbrack;Rendimiento&amp;rbrack; Habilitar solo el primer canal en nuevas capas/efectos de relleno
* &amp;lbrack;Rendimiento&amp;rbrack; Paralelizar cálculo de trazo de pincel
* Baking
* &amp;lbrack;Haciendo un bake&amp;rbrack; Añadir nueva opción de generación de jaulas totalmente automática para hacer un bake con mallas de alto contenido de polietileno (experimental)
* Contenido
* &amp;lbrack;Contenido&amp;rbrack; Añade 6 filtros nuevos: estilización, cuantificar, anisotrópico kuwahara, suavizado de bisel, distancia direccional, conversión de escala de grises
* &amp;lbrack;Contenido&amp;rbrack; Actualizar Noises y Grunges a la última versión de Designer (con el nuevo 2D Voronoi)
* &amp;lbrack;Contenido&amp;rbrack; Añadir 3 nuevos generadores de textura (Azulejo Aleatorio, Triangle Grid, Generador de Scratches)
* &amp;lbrack;Contenido&amp;rbrack; Cambiar nombre de plantilla de Unreal Engine y exportar ajustes preestablecidos
* Python
* &amp;lbrack;Shelf&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Guardar material inteligente o máscara inteligente en disco desde Python
* &amp;lbrack;Python&amp;rbrack; Añadir la jaula automática de hace un bake a la API de Python
* &amp;lbrack;Python&amp;rbrack; Permitir editar nombres y descripciones de conjuntos de texturas/Mosaicos de UV
* &amp;lbrack;Python&amp;rbrack; Compartir la configuración de resolución en fuentes vectoriales y de fuentes
* &amp;lbrack;Actualización automática&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exponer las funcionalidades de actualización automática del proyecto en Python
* Varios
* &amp;lbrack;Exportar&amp;rbrack; Facilitar el acceso a las opciones Enviar a con un nuevo panel
* &amp;lbrack;Nvidia&amp;rbrack; Agregar advertencia sobre los controladores más recientes de NVIDIA (572.16)
* El ajuste de ángulo debe verse afectado por la selección de espacio Objeto/Mundo
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Permitir agregar nombres personalizados a los Mosaicos de UV y utilizarlos en la exportación
* Mac
* &amp;lbrack;Mac&amp;rbrack; Uso de Metal en lugar de OpenGL para el procesamiento de gráficos
* &amp;lbrack;Mac&amp;rbrack; Retirar la asistencia de Mac Intel

**Corregido**:

* &amp;lbrack;Bloqueo&amp;rbrack; Eliminar entrada de imagen
* No se puede agregar una alfombra inteligente mediante el botón de pila de capas
* &amp;lbrack;Python&amp;rbrack; No se pueden encontrar efectos en GroupLayerNode

**Problemas conocidos**:

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;brack; Bloqueo al importar algunos ajustes preestablecidos
* &amp;lbrack;Motor&amp;rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &amp;lbrack;Python&amp;rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento
* &amp;lbrack;RedHat&amp;rbrack; Problemas con el selector de color

## Versión 10

### 10.1.2

Fecha de publicación: **2024/12/3** Resumen: **Versión secundaria, correcciones de errores**

**Corregido**:

* &amp;lbrack;Bloqueo&amp;rbrack; Eliminar entrada de imagen
* No se puede agregar una alfombra inteligente mediante el botón de pila de capas
* &amp;lbrack;Python&amp;rbrack; No se pueden encontrar efectos en GroupLayerNode

**Problemas conocidos**:

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;brack; Bloqueo al importar algunos ajustes preestablecidos
* &amp;lbrack;Motor&amp;rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &amp;lbrack;Python&amp;rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento
* &amp;lbrack;RedHat&amp;rbrack; Problemas con el selector de color

### 10.1.1

Fecha de publicación: **2024/11/5** Resumen: **Versión secundaria, correcciones de errores**

**Agregado**:

* &amp;lbrack;Proyecto&amp;rbrack; Mantener abierto el proyecto actual hasta que se valide la nueva selección de proyecto
* &amp;lbrack;Desenvolvimiento automático&amp;rbrack; La densidad del texel permite dividir mejor las Islas de UV en UDIM
* &amp;lbrack;Haciendo un bake&amp;rbrack; Corregir copia ambigua en el menú contextual de Mapas de malla
* &amp;lbrack;Deformar&amp;rbrack; Eliminación de la escala en la ventanilla del eje Z (profundidad)
* &amp;lbrack;Importar/Exportar&amp;rbrack; Eliminar la compatibilidad con formatos de archivo de imagen no utilizados
* Actualizar Substance Engine a 9.1.4

**Corregido**:

* &amp;lbrack;Bloqueo&amp;rbrack; Después de reubicar el recurso en Recursos y guardar el proyecto
* &amp;lbrack;Bloqueo&amp;rbrack; Problemas con la biblioteca de aiserver
* &amp;lbrack;Bloqueo&amp;rbrack; bloqueo de servidor Illustrator en algunos casos excepcionales
* &amp;lbrack;Bloqueo&amp;rbrack; En algunos casos raros, al salir de la aplicación
* No se pueden enviar informes de bloqueo en algunos equipos
* &amp;lbrack;Haciendo un bake&amp;rbrack; El color del vértice no se lee correctamente
* &amp;lbrack;UI&amp;rbrack; La ubicación de las ventanas y las novedades al inicio se cambian
* &amp;lbrack;Assimp&amp;rbrack; No se reconoce la superficie estándar de Maya al hacer un bake ID
* &amp;lbrack;Python&amp;rbrack; La biblioteca SSL que falta genera un error
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Win&amp;rbrack; Error al llamar a QColorConstants.Transparent
* &amp;lbrack;Python&amp;rbrack; Las miniaturas de capas creadas mediante Python no se actualizan hasta que se hace clic dentro de la pila de capas
* &amp;lbrack;Sombreador&amp;rbrack; Vínculo roto en el registro de cambios de API del sombreador
* &amp;lbrack;3D Assets&amp;rbrack; Usar la configuración del proxy del sistema operativo al acceder a recursos 3D

**Problemas conocidos**:

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;brack; Bloqueo al importar algunos ajustes preestablecidos
* &amp;lbrack;Motor&amp;rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &amp;lbrack;Python&amp;rbrack; Widget que parece eliminado a través de script todavía funciona
* &amp;lbrack;RedHat&amp;rbrack; Problemas con el selector de color

### 10.1.0

Fecha de publicación: **17/09/2024** Resumen: **Versión principal, contenido nuevo: Filtro de color/máscara de área de relleno, filtro de pegatinas de bordado y seis filtros de Substance genéricos, USD de importación con propiedades de material y sombreador, mejora del rendimiento, compatibilidad con VFX Platform 2024 y migración a Linux RedHat**

**Agregado**:

* &amp;lbrack;Contenido&amp;rbrack; Añadir nuevo filtro de color/máscara de área de relleno
* &amp;lbrack;Contenido&amp;rbrack; Añadir nuevo filtro de pegatinas de bordado
* &amp;lbrack;Contenido&amp;rbrack; Añade 6 nuevos filtros Substance genéricos (FXAA, pixelado, paso alto, posterizar, paso suave y umbral)
* &amp;lbrack;USD&amp;rbrack; Exportar USD capa con un material de ASM definido
* &amp;lbrack;USD&amp;rbrack; Importar USD con propiedades de materiales y sombreadores
* &amp;lbrack;Rendimiento&amp;rbrack; Habilitar miniaturas de pila de capas optimizadas de forma predeterminada
* &amp;lbrack;Rendimiento&amp;rbrack; Reducir el tiempo de apertura de archivos de proyecto y el consumo de memoria (descodificación de datos)
* Compatible con la plataforma VFX 2024
* &amp;lbrack;VFX Platform 2024&amp;rbrack; Actualizar a Python 3.11
* &amp;lbrack;VFX Platform 2024&amp;rbrack; Actualización a OpenEXR 3.2
* &amp;lbrack;VFX Platform 2024&amp;rbrack; &amp;lbrack;USD&amp;rbrack; Actualizar OpenSubdiv 3.6.0
* &amp;lbrack;Plataforma VFX 2024&amp;rbrack;&amp;lbrack;Administración de color&amp;rbrack; Actualizar a OCIO 2.3.2
* &amp;lbrack;Linux&amp;rbrack; Migración a Linux RedHat
* &amp;lbrack;Linux&amp;rbrack; Actualizar la versión principal del controlador Nvidia a 535.171.04
* &amp;lbrack;Importar&amp;rbrack; Adición de una opción para voltear el mapa de normales al importar una malla GLTF
* &amp;lbrack;UI&amp;rbrack; Usar el valor predeterminado del sistema operativo para la distancia de detección de eventos de arrastre
* &amp;lbrack;Substance Engine&amp;rbrack; Agregar función de tira de llamadas para eliminar los símbolos del ejecutable
* &amp;lbrack;Pantalla de bienvenida&amp;rbrack; Actualizar al nuevo formato de pantalla de bienvenida
* Actualizar Substance Engine a la versión 9.1.3
* &amp;lbrack;Python&amp;rbrack; Mostrar vínculos a ejemplos en el menú de documentación de la pila de capas
* &amp;lbrack;JavaScript&amp;rbrack; Mover complementos de Javascript a la subcarpeta javascript/plugins

**Corregido**:

* &amp;lbrack;Illustrator&amp;rbrack; Bloqueo al exportar un Mosaico de UV con un gráfico .ai en casos específicos
* &amp;lbrack;Trazos dinámicos&amp;rbrack;&amp;lbrack;Path&amp;rbrack; La opción aleatoria por trazo no funciona en un trazado
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Propiedades&amp;rbrack; El bloqueo se activa cuando el mosaico no es uniforme
* El archivo TXT de depuración se crea al hacer doble clic en el proyecto de Painter
* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Es posible que falten algunas texturas
* &amp;lbrack;ASM&amp;rbrack; Dispersión El canal de color ignora los colores metálicos
* &amp;lbrack;Contenido&amp;rbrack; El filtro de desenfoque no funciona en el espacio de color &quot;operativo&quot;
* &amp;lbrack;Contenido&amp;rbrack; Height Ajustar filtro también modifica el alfa de la capa

**Problemas conocidos**:

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;Bloqueo&amp;rbrack; &amp;lbrack;ACE&amp;rbrack; No utilizar el espacio de color sRGB ICE para transformar la visualización
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;brack; Bloqueo al importar algunos ajustes preestablecidos
* &amp;lbrack;Bloqueo&amp;rbrack; Reubicar recurso y guardar proyecto
* &amp;lbrack;Motor&amp;rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &amp;lbrack;Python&amp;rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento
* &amp;lbrack;RedHat&amp;rbrack; Problemas con el selector de color

### 10.0.1

Fecha de publicación: **2024/06/11** Resumen: **Versión secundaria, correcciones de errores**

**Agregado:**

* &amp;lbrack;Biblioteca&amp;rbrack; Conversión de fuentes de Substance en archivos de fuentes normales
* &amp;lbrack;Illustrator&amp;rbrack;&amp;lbrack;SVG&amp;rbrack; Dar a las miniaturas de la selección de ámbito un fondo gris claro
* &amp;lbrack;Python&amp;rbrack; Función Añadir en origen de mapa de bits para enumerar los espacios de color disponibles

**Corregido**:

* &amp;lbrack;Pila de capas&amp;rbrack; La carpeta siempre se cierra al entrar o salir de otras carpetas
* &amp;lbrack;Guardar&amp;rbrack; El archivo de proyecto se pierde cuando se produce un error al guardar como copia o al guardar automáticamente en casos específicos
* &amp;lbrack;Importar&amp;rbrack; Los activos con el mismo nombre pero con diferentes extensiones se anulan
* &amp;lbrack;Propiedades&amp;rbrack; Faltan ajustes al utilizar el punto de anclaje en las entradas de imagen
* &amp;lbrack;Illustrator&amp;rbrack; No se pueden importar archivos de Illustrator después del bloqueo del servidor sin reiniciar Painter
* &amp;lbrack;Python&amp;rbrack; El padre de la instancia no se puede establecer con el tipo &quot;properties&quot;
* &amp;lbrack;Python&amp;rbrack; Al definir el poli alto como parámetro de haga un bake, no se carga el poli alto
* &amp;lbrack;Python&amp;rbrack; El mensaje de error para set_color_space() es demasiado genérico
* &amp;lbrack;Python&amp;rbrack; Las fuentes de referencia permiten crear ciclos

**Problemas conocidos**:

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;brack; Bloqueo al importar algunos ajustes preestablecidos
* &amp;lbrack;Illustrator&amp;rbrack; Bloqueo al exportar un Mosaico de UV con un gráfico .ai en casos específicos
* &amp;lbrack;Trazos dinámicos&amp;rbrack;&amp;lbrack;Path&amp;rbrack; La opción aleatoria por trazo no funciona en un trazado

### 10.0.0

Fecha de publicación: **2024/05/16** Resumen: **Versión principal, edición de la pila de capas con la API de Python, lectura de archivos nativos de Illustrator, integración de recursos 3D y nuevo recurso de texto**

**Agregado**:

* &amp;lbrack;Illustrator&amp;rbrack; Uso de archivos de Illustrator con mesas de trabajo en Painter
* &amp;lbrack;Illustrator&amp;rbrack;&amp;lbrack;SVG&amp;rbrack; Añadir previsualizaciones en la selección de ámbito
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Examine, seleccione y descargue contenidos 3D directamente en Painter
* &amp;lbrack;Substance 3D Assets&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevo panel
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Mapas y materiales del entorno de apoyo
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Permitir volver a cargar, navegar y abrir la carpeta de ubicación en el nuevo panel Substance 3D Assets
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Adición de un gestor de descargas
* &amp;lbrack;Recurso de texto&amp;rbrack; Permitir el uso de fuentes incrustables
* &amp;lbrack;Recurso de texto&amp;rbrack; Permitir procesar una fuente/texto en una malla
* &amp;lbrack;Recurso de texto&amp;rbrack; Visualización de fuentes del usuario y otras rutas compartidas en el panel Activos con una nueva categoría
* &amp;lbrack;Recurso de texto&amp;rbrack;&amp;lbrack;Propiedades&amp;rbrack; Añadir compatibilidad con propiedades de fuentes avanzadas
* &amp;lbrack;Recurso de texto&amp;rbrack; Permitir buscar/ver fuentes en miniestantes
* &amp;lbrack;Recurso de texto&amp;rbrack; Añadir mensaje/cuadro de diálogo de error al importar una fuente incompatible
* Miscelánea
* &amp;lbrack;Rellenar proyección&amp;rbrack; Mejorar el comportamiento del manipulador de escala al utilizar valores pequeños
* &amp;lbrack;Manipuladores&amp;rbrack; Agregar nuevo modo preciso al presionar el método abreviado CTRL
* &amp;lbrack;Manipuladores&amp;rbrack; Mejorar la estabilidad del manipulador de superficie al convertir
* &amp;lbrack;Exportar&amp;rbrack; Añadir nombre de espacio de color en salidas SBSAR
* &amp;lbrack;Rendimiento&amp;rbrack; Mejorar el tiempo de detección de la biblioteca de los activos en el disco
* &amp;lbrack;Substance&amp;rbrack; Actualización al motor de Substance versión 9.1.2
* &amp;lbrack;Arrastrar y soltar&amp;rbrack; Alinear la rotación de pegatinas con la cámara al colocar en la ventana gráfica
* &amp;lbrack;Python&amp;rbrack; Edición de la pila de capas
* &amp;lbrack;Python&amp;rbrack; Permitir seleccionar capa, efecto, máscara o máscara geográfica en la interfaz de usuario
* &amp;lbrack;Python&amp;rbrack; Permitir obtener/definir modos de fusión de capas
* &amp;lbrack;Python&amp;rbrack; Permitir obtener o establecer la configuración de proyección de la capa de relleno
* &amp;lbrack;Python&amp;rbrack; Permitir consultar el color de material del Substance desde una capa de relleno
* &amp;lbrack;Python&amp;rbrack; Permitir consultar y definir colores uniformes y recursos en capas y efectos
* &amp;lbrack;Python&amp;rbrack; Permitir la creación y edición de recursos de texto en pila de capas
* &amp;lbrack;Python&amp;rbrack; Permitir editar canales activos en capas y efectos
* &amp;lbrack;Python&amp;rbrack; Permitir que las acciones por lotes tengan una sola acción de deshacer/rehacer
* &amp;lbrack;Python&amp;rbrack; Permitir cargar o editar parámetros de origen vectorial
* &amp;lbrack;Python&amp;rbrack; Permitir la edición de propiedades de color de capa y efectos con la gestión de color
* &amp;lbrack;Python&amp;rbrack; Permitir consultar y crear capas con instancias
* &amp;lbrack;Python&amp;rbrack; Permitir añadir efecto de selección de color
* &amp;lbrack;Python&amp;rbrack; Permitir el control de la gestión de color de imágenes de mapa de bits
* &amp;lbrack;Python&amp;rbrack; Permitir detener/anular pausa del motor
* &amp;lbrack;Python&amp;rbrack; Permitir navegar a nodos del mismo nivel y principales
* &amp;lbrack;Python&amp;rbrack; Permitir la creación de un efecto de filtro/generador
* &amp;lbrack;Python&amp;rbrack; Permitir añadir efecto de nivel
* &amp;lbrack;Python&amp;rbrack; Permitir añadir máscara inteligente en una capa
* &amp;lbrack;Python&amp;rbrack; Permitir crear o editar puntos de ancla
* &amp;lbrack;Python&amp;rbrack; Permitir obtener/definir máscara en capas
* &amp;lbrack;Python&amp;rbrack; Permitir la creación del efecto de máscara de comparación
* &amp;lbrack;Python&amp;rbrack; Permitir consultar y utilizar ajustes preestablecidos de recursos de Substance
* &amp;lbrack;Python&amp;rbrack; Permitir la lista de ajustes preestablecidos y sus valores mediante la función internal_properties para los recursos del Substance
* &amp;lbrack;Python&amp;rbrack; Permitir la lista de ajustes preestablecidos de exportación predefinidos
* &amp;lbrack;Python&amp;rbrack; Permitir que se muestren los ajustes preestablecidos de exportación disponibles en la biblioteca
* &amp;lbrack;Python&amp;rbrack; Permitir recuperar el contenido de los ajustes preestablecidos de exportación

**Corregido**:

* &amp;lbrack;Bloqueo&amp;rbrack; Deshacer &quot;Quitar instancia del sombreador&quot; con Ctrl-Z
* &amp;lbrack;Bloqueo&amp;rbrack; Crear una capa en una pila vacía si la última selección fue un efecto
* &amp;lbrack;SVG&amp;rbrack; Problema con el valor de área recortada personalizada
* &amp;lbrack;Desenvolvimiento automático&amp;rbrack; Si se vuelve a calcular solo el empaquetado sin ningún cambio en la orientación UV, se producirá un bloqueo
* &amp;lbrack;Arrastrar y soltar&amp;rbrack; El retraso debido a los recursos externos se carga previamente varias veces
* &amp;lbrack;UI&amp;rbrack; La miniatura de un recurso de arrastrar y soltar puede ocultar un mensaje de advertencia en la pila de capas
* &amp;lbrack;Rendimiento&amp;rbrack; Los mosaicos UV enmascarados aún se calculan
* &amp;lbrack;USD&amp;rbrack; Resaltado incorrecto para la selección de ámbito
* &amp;lbrack;Recurso&amp;rbrack; La imagen de mapa de bits se daña después de pintar en el canal normal y guardar el proyecto
* &amp;lbrack;USD&amp;rbrack; Admitir ordenación de mallas de vértices con la mano izquierda
* &amp;lbrack;Substance&amp;rbrack; Restablecer valores predeterminados volver siempre a cero para el widget de ángulo
* &amp;lbrack;Motor&amp;rbrack; Pintar con un SVG en una galería de símbolos no funciona
* &amp;lbrack;Motor&amp;rbrack; Los trazos de pincel de mapa de normales se rompen después de deshacer una acción
* &amp;lbrack;Contenido&amp;rbrack; El gráfico en el Filtro de material tiene una fusión alfa y un espacio de color incorrectos
* &amp;lbrack;Contenido&amp;rbrack; Los modos de fusión del Tile Generator no funcionan
* &amp;lbrack;Contenido&amp;rbrack; El filtro de histograma produce bandas en algunos casos
* &amp;lbrack;Contenido&amp;rbrack; La iluminación hecha un bake estilizada no tiene en cuenta el height pintado
* &amp;lbrack;Python&amp;rbrack; Error inesperado al recuperar información de capas instanciada después de cambiar de sombreador
* &amp;lbrack;Guardar&amp;rbrack; El archivo de proyecto se pierde cuando se produce un error en &quot;Guardar como&quot; en casos específicos

**Problemas conocidos**:

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Arrastre y colocación de recursos en pila de capas en Wayland OS
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent
* &amp;lbrack;Guardar&amp;rbrack; El archivo de proyecto de Spp se pierde cuando &quot;guardar como copia&quot; falla en casos específicos
* &amp;lbrack;MacOS Intel&amp;brack; Bloqueo al importar algunos ajustes preestablecidos
* &amp;lbrack;Illustrator&amp;rbrack; No se pueden importar archivos de Ai después del bloqueo del servidor sin reiniciar Painter
* &amp;lbrack;Importar&amp;rbrack; Los activos con el mismo nombre pero con diferentes extensiones se anulan

## Versión 9

### 9.1.2

Fecha de publicación: **30/01/2024** Resumen: **Versión secundaria, correcciones de errores**

**Agregado**:

* &amp;lbrack;Rendimiento&amp;rbrack; Mejorar el tiempo de creación de la primera capa de relleno en proyectos nuevos
* &amp;lbrack;Rendimiento&amp;rbrack; Reducir el tiempo de carga de los mapas de entorno pesados
* &amp;lbrack;Substance&amp;rbrack; Permitir guardar o cerrar proyectos incluso cuando se generan miniaturas

**Corregido**:

* La acción de guardar falla en proyectos de versiones anteriores cuando se modifica la ventana gráfica
* &amp;lbrack;Bloqueo&amp;rbrack; Reimportación de mallas al utilizar el archivo AO personalizado y la gestión de color
* &amp;lbrack;Rellenar proyección&amp;rbrack; Al hacer clic en el manipulador de escala, aparece el mensaje &quot;no puede pintarse&quot;
* &amp;lbrack;Brush&amp;rbrack; Pintar con alineación UV causa artefactos
* &amp;lbrack;Pila de capas&amp;rbrack; El cambio de nombre de la capa es lento cuando la pila es muy larga
* &amp;lbrack;Pila de capas&amp;rbrack; Mensaje de error incorrecto al utilizar un filtro incompatible en la máscara
* &amp;lbrack;Pila de capas&amp;rbrack; La selección vuelve a la capa superior después de la eliminación
* &amp;lbrack;Exportar&amp;rbrack; La textura normal generada siempre está en el modo de relleno Espacio 3D contiguo
* &amp;lbrack;Exportar&amp;rbrack; La textura alfa no se genera con el ajuste preestablecido de exportación de vista 2D
* &amp;lbrack;Exportar&amp;rbrack; La exportación SBSAR tiene usos incorrectos con mapas convertidos
* &amp;lbrack;Sombreador&amp;rbrack; El registro de cambios de API del sombreador no está actualizado con los últimos cambios de ASM

**Problemas conocidos**:

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Arrastre y colocación de recursos en pila de capas en Wayland OS
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportación USD activada por TextureStateEvent

### 9.1.1

Fecha de publicación: **12/2023/05** Resumen: **Versión secundaria, correcciones de errores y envío a la funcionalidad de After Effects**

**Agregado:**

* &amp;lbrack;Interop&amp;rbrack; Permitir el envío de una malla con textura a After Effects (Ae 24.1)

**Corregido:**

* &amp;lbrack;Rellenar&amp;rbrack; La proyección del conjunto UV en conjunto UV no lee más de 2 conjuntos UV
* &amp;lbrack;Bloqueo&amp;rbrack; Uso del mapa de entorno de 16K
* &amp;lbrack;Bloqueo&amp;rbrack; Exr utilizado como entrada de imagen
* &amp;lbrack;Bloqueo&amp;rbrack; Copiar y pegar trazados en proyectos
* &amp;lbrack;QoL&amp;rbrack; La acción de arrastrar y soltar un recurso del Alpha en el modo de pegatina crea una Proyección de UV en la máscara
* &amp;lbrack;Ruta&amp;rbrack; Copiar vértices de trazado también cambia el nombre de la ruta de destino al volver a abrir el proyecto
* &amp;lbrack;Linux&amp;rbrack; La selección de color se puede romper con varias pantallas
* &amp;lbrack;Auto Unwrap&amp;rbrack; Problema de interfaz de usuario para control de densidad de texto
* &amp;lbrack;Administración de color&amp;rbrack; Los comentarios de la interfaz de usuario son razonables en cada caso, pero el motor no
* &amp;lbrack;Administración de color&amp;rbrack; Selección incorrecta del espacio de color en la máscara con anulación de datos de usuario

**Problemas conocidos:**

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; con Linux Wayland en AMD al arrastrar y soltar el recurso en la Pila de capas
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Cambio del valor de filtrado anisotrópico en el sistema operativo Monterey
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú del botón derecho es demasiado pequeño en la pantalla HD
* &amp;lbrack;Python&amp;rbrack; Bloqueo de USD de exportación activado por TextureStateEvent

### 9.1.0

Fecha de publicación: **2023/11/07** Resumen: **Versión principal con compatibilidad con SVG y transparencia, así como mejoras en la herramienta de arrastrar y soltar y ruta**

**Agregado:**

* &amp;lbrack;SVG&amp;rbrack; Permitir la importación de archivos vectoriales (SVG)
* &amp;lbrack;SVG&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Añadir compatibilidad con propiedades específicas del SVG
* &amp;lbrack;SVG&amp;rbrack; Añada una opción para conservar fácilmente las proporciones de la imagen original
* &amp;lbrack;SVG&amp;rbrack; Permitir el uso automático de alfa de SVG con transparencia
* &amp;lbrack;Interop&amp;rbrack; Permitir el envío de una malla con textura a After Effects (versión beta de Ae 24.1)
* &amp;lbrack;Interop&amp;rbrack; Añadir configuración para Enviar a After Effects
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Assets&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Importar automáticamente el recurso al arrastrar y soltar en la ranura de la interfaz de usuario
* &amp;lbrack;QoL&amp;rbrack; Permitir arrastrar y soltar recursos externos en la pila de capas
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Arrastrar y soltar texturas desde el panel de Recursos en la Pila de capas
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Permitir arrastrar y soltar el generador, filtros en la malla
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Permitir soltar activos externos en la malla
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Proyección&amp;rbrack; Añadir nuevo conjunto UV al modo de proyección conjunto UV
* &amp;lbrack;QoL&amp;rbrack; Arrastrar y soltar Máscaras inteligentes como nuevas capas en la ventana gráfica y la Pila de capas
* &amp;lbrack;QoL&amp;rbrack; Añadir selector para generadores con varias salidas cuando se utiliza en la máscara
* &amp;lbrack;QoL&amp;rbrack; Permitir arrastrar y soltar imágenes de un solo canal sobre un efecto de relleno
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Utilice los modificadores CTRL/ALT con la función de arrastrar y soltar para especificar dónde y cómo crear efectos o capas
* &amp;lbrack;Ruta&amp;rbrack; Cambiar la visibilidad de los trazados individualmente en el panel Trazado
* &amp;lbrack;Ruta&amp;rbrack; Permitir el uso de manipuladores de transformación para puntos de trazado
* &amp;lbrack;Ruta&amp;rbrack; Permitir el control manual de las tangentes por vértice
* &amp;lbrack;Ruta&amp;rbrack; Copiar/pegar propiedades de trazado
* &amp;lbrack;Ruta&amp;rbrack; Introducir un método abreviado vacío para el botón de tangente de rotura
* &amp;lbrack;Sombreador&amp;rbrack; Añadir compatibilidad con Opacidad y Translucidez en sombreador de ASM
* &amp;lbrack;Sombreador&amp;rbrack; Añadir compatibilidad para el canal de Color de absorción con el sombreador de ASM
* &amp;lbrack;Sombreador&amp;rbrack; Mejorar información sobre parámetros de sombreador de ASM
* &amp;lbrack;Sombreador&amp;rbrack; Cambiar el color predeterminado del canal de Translucidez a negro
* &amp;lbrack;Configuración de visualización&amp;rbrack; Habilitar Suavizado temporal de forma predeterminada
* &amp;lbrack;Configuración de visualización&amp;rbrack; Activar configuración de dispersión subsuperficial de forma predeterminada
* &amp;lbrack;Substance&amp;rbrack; Añadir compatibilidad para la propiedad ColorSpace desde la entrada/salida de gráficos
* &amp;lbrack;Substance&amp;rbrack; Actualizar el motor de Substance a la versión 9.0.3
* &amp;lbrack;UI&amp;rbrack; Hacer accesible el botón de la barra de herramientas contextual incluso si la ventana de la aplicación es pequeña
* &amp;lbrack;Auto Unwrap&amp;rbrack; Número de Mosaicos de UV de control con Densidad de texto
* &amp;lbrack;Haciendo un bake&amp;rbrack; Desactivar Trazado de rayos de GPU en GPU AMD de forma predeterminada
* &amp;lbrack;Rendimiento&amp;rbrack; Aplique compresión sin pérdida en imágenes de 16 bits para reducir el espacio del proyecto
* &amp;lbrack;Python&amp;rbrack; Permitir la manipulación de la cámara predeterminada en Vista 3D
* &amp;lbrack;Python&amp;rbrack; Exponer la capacidad de exportar mallas mediante scripts
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Samples&amp;rbrack; Añade un nuevo proyecto de muestra &quot;French Restaurant Table&quot;
* &amp;lbrack;Contenido&amp;rbrack; Actualizar el logotipo de Substance alfa a una nueva versión
* &amp;lbrack;Contenido&amp;rbrack; Añade tres filtros de material enfocados en el SVG (pegatina personalizada, spray personalizado y gráfico al material)

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; Cambio del tamaño del manipulador cuando no se utiliza la herramienta simetría
* &amp;lbrack;Bloqueo&amp;rbrack; &amp;lbrack;Pila de capas&amp;rbrack; Crear capa cuando no hay nada seleccionado
* &amp;lbrack;Proyecto&amp;rbrack; Los mapas de malla se pueden dañar después de eliminar los recursos no utilizados
* &amp;lbrack;Proyecto&amp;rbrack; Daños en los recursos tras volver a importar o hacer un bake la imagen
* &amp;lbrack;Assets&amp;rbrack; Al volver a cargar un activo, se elimina de Favoritos
* &amp;lbrack;Importar&amp;rbrack; No se pueden importar recursos cuando no se encuentra ningún resultado en el panel de recursos
* &amp;lbrack;UI&amp;rbrack; La flecha de la barra de herramientas contextual no aparece en algunos casos
* &amp;lbrack;Substance&amp;rbrack; No se admite el botón en paralelo para valores booleanos
* &amp;lbrack;Nivel&amp;rbrack; Etiqueta de canal incorrecta cuando se utiliza en la máscara
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; Los archivos glTF/GLB exportados desde Painter no tienen una unidad de tamaño físico
* &amp;lbrack;Contenido&amp;rbrack; La intensidad del filtro de desenfoque se fija en 16
* &amp;lbrack;Contenido&amp;rbrack; La entrada de imagen del filtro &quot;color de destino&quot; no está visible

**Problemas conocidos:**

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; con Linux Wayland en AMD al arrastrar y soltar el recurso en la Pila de capas
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Cambio del valor de filtrado anisotrópico en el sistema operativo Monterey
* &amp;lbrack;Bloqueo&amp;rbrack; Exr utilizado como entrada de imagen
* &amp;lbrack;Bloqueo&amp;rbrack; Uso del mapa de entorno de 16K
* &amp;lbrack;Auto Unwrap&amp;rbrack; Problema de interfaz de usuario para control de densidad de texto
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;UI&amp;rbrack; El menú del botón derecho es demasiado pequeño en la pantalla HD
* &amp;lbrack;Python&amp;rbrack; Bloqueo de USD de exportación activado por TextureStateEvent
* &amp;lbrack;QoL&amp;rbrack; La acción de arrastrar y soltar un recurso del Alpha en el modo de pegatina crea una Proyección de UV en la máscara

### 9.0.1

Fecha de publicación: **2023/09/19** Resumen: **Versión menor de corrección de errores con varias mejoras**

**Agregado:**

* &amp;lbrack;Importar&amp;rbrack; Establecer ubicación de importación predeterminada en la ventana de importación
* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Permitir restablecer los parámetros a sus valores predeterminados
* &amp;lbrack;Haciendo un bake&amp;rbrack; Definir hacer un bake a resolución de pintura al crear un proyecto
* &amp;lbrack;Simetría&amp;rbrack; Desvincular manipulador específico de simetría de método abreviado Q
* &amp;lbrack;Menú&amp;rbrack; Añadir la opción &quot;mostrar registro&quot; en el menú de ayuda
* &amp;lbrack;Viewport&amp;rbrack; Mejorar la velocidad de procesamiento de sombras
* &amp;lbrack;Substance&amp;rbrack; Actualizar el motor a la versión 9.0.1
* &amp;lbrack;Administración de color&amp;rbrack; OCIO archivo de configuración puede tener cualquier tipo de extensión
* &amp;lbrack;Assets&amp;rbrack; El recurso Sbsar con uso de &#39;pegatina&#39; debe configurarse automáticamente para deformar la proyección
* &amp;lbrack;Ruta&amp;rbrack; Mostrar un mensaje al intentar interactuar con la herramienta Ruta mientras la interfaz de usuario y los Gizmo están ocultos

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; Alt + Arrastrar en el panel Trazado
* &amp;lbrack;Importar recursos&amp;rbrack; Bloqueo aleatorio al quitar recursos para importar
* Bloqueo al importar un archivo GLB comprimido
* Problema al pintar en mallas que comparten UV
* Parpadeo de malla negro al volver a calcular o cargar la caché
* &amp;lbrack;Propiedades&amp;rbrack; El menú contextual para restablecer parámetros no aparece en los menús desplegables
* &amp;lbrack;Nivel&amp;rbrack; Reguladores de entrada bloqueados por nivel anterior
* &amp;lbrack;AMD&amp;rbrack;&amp;lbrack;Sparse&amp;rbrack; La opción SVT, si está activada, genera artefactos
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Bloqueo al hacer doble clic en los vértices
* &amp;lbrack;Ruta&amp;rbrack; IU y ruta visibles en el modo de hacer un bake
* &amp;lbrack;AMD&amp;rbrack; Textura perdida al jugar con la visibilidad
* &amp;lbrack;Disperso&amp;rbrack; Resolución demasiado baja al girar la malla

**Problemas conocidos:**

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción

### 9.0.0

Fecha de lanzamiento: **2023/06/20** Resumen: **Versión principal con Pintura a lo largo de la ruta que permite curvas 3D, nuevos materiales base y la limpieza de materiales heredados y nuevos ajustes preestablecidos para curvas 3D**

**Agregado:**

* &amp;lbrack;Ruta&amp;rbrack; Herramienta Añadir nueva Pintura a lo largo del trazado
* &amp;lbrack;Ruta&amp;rbrack; Adición de un método abreviado vacío para la herramienta de trazado
* &amp;lbrack;Ruta&amp;rbrack; Permitir la adición de nuevos puntos a un trazado existente
* &amp;lbrack;Ruta&amp;rbrack; Agregar método abreviado para salir de la creación de la ruta actual
* &amp;lbrack;Ruta&amp;rbrack; Permitir la edición de propiedades de pincel para trazados
* &amp;lbrack;Ruta&amp;rbrack; Ajuste automático de tangentes al colocar un punto
* &amp;lbrack;Ruta&amp;rbrack; Calcular tangentes al mover un punto
* &amp;lbrack;Ruta&amp;rbrack; Ajuste de los puntos recién creados a la superficie de una malla
* &amp;lbrack;Ruta&amp;rbrack; Permitir editar la presión por vértice
* &amp;lbrack;Ruta&amp;rbrack; Ajustar la presión de un punto recién creado desde puntos vecinos
* &amp;lbrack;Ruta&amp;rbrack; Permitir la conversión de puntos a suavizado/esquina (salto de tangente)
* &amp;lbrack;Ruta&amp;rbrack; Permitir mover un punto recién añadido inmediatamente
* &amp;lbrack;Ruta&amp;rbrack; Permitir la eliminación de puntos de un trazado existente
* &amp;lbrack;Ruta&amp;rbrack; Permitir invertir la dirección de un trazado
* &amp;lbrack;Ruta&amp;rbrack; Permitir la selección de una ruta en la ventana gráfica
* &amp;lbrack;Ruta&amp;rbrack; Permitir la selección de puntos de trazado con selección de recuadro
* &amp;lbrack;Ruta&amp;rbrack; Introducir métodos abreviados CTRL-A para seleccionar todos los puntos de un trazado
* &amp;lbrack;Ruta&amp;rbrack; Permitir cerrar trazado
* &amp;lbrack;Ruta&amp;rbrack; Permitir especificar el eje ascendente de la ruta en Propiedades
* &amp;lbrack;Ruta&amp;rbrack; Añadir un menú de control de vértices a la barra de herramientas contextual
* &amp;lbrack;Ruta&amp;rbrack; Introducir los modos de pintura/borrado/difuminado en la herramienta de trazado
* &amp;lbrack;Ruta&amp;rbrack; Creación de comentarios visuales para trazados en la ventana gráfica
* &amp;lbrack;Ruta&amp;rbrack; Adición de un indicador visual para la dirección del trazado
* &amp;lbrack;Ruta&amp;rbrack; Añadir thickness de línea a la configuración de visualización de trazado
* &amp;lbrack;Ruta&amp;rbrack; Permitir ocultar la interfaz de usuario de rutas
* &amp;lbrack;Ruta&amp;rbrack; Agregar el panel Trazado a la lista de trazados de la capa seleccionada actualmente
* &amp;lbrack;Ruta&amp;rbrack; Adición de comentarios visuales al pasar el cursor sobre un trazado en el panel Trazado
* &amp;lbrack;Ruta&amp;rbrack; Mostrar el panel Trazado siempre que se seleccione la herramienta Trazado
* &amp;lbrack;Ruta&amp;rbrack; Permitir cambiar el nombre, eliminar, copiar, cortar y duplicar trazado en el panel Trazado
* &amp;lbrack;Ruta&amp;rbrack; Mostrar mensaje al intentar interactuar en la ventana gráfica 2D con la herramienta Trazado
* &amp;lbrack;Biblioteca&amp;rbrack; Integrar nuevo contenido (herramientas de trazado y materiales base)
* &amp;lbrack;Trazos dinámicos&amp;rbrack; Agregar propiedad de distancia para trazos dinámicos
* &amp;lbrack;Trazos dinámicos&amp;rbrack; Añadir propiedades de tamaño y espaciado a los trazos dinámicos
* &amp;lbrack;Trazos dinámicos&amp;rbrack; Agregar propiedad de inicio/medio/fin para trazos dinámicos
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exponer los parámetros de configuración del proyecto para el formato USD
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exponer parámetros de creación de proyectos para el formato USD
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Añadir información de ruta de proyecto dentro del archivo USD exportado
* &amp;lbrack;GLTF&amp;rbrack; Actualización de texturas de la biblioteca al volver a cargar un archivo GLTF
* &amp;lbrack;Sombreador&amp;rbrack; Reducir defectos de costura para Islas de UV con diferentes orientaciones
* &amp;lbrack;Motor&amp;rbrack; Actualizar al motor de Substance versión 9.0

**Corregido:**

* &amp;lbrack;Importar&amp;rbrack; Algunos GLB con texturas no reciben texturas en Painter
* &amp;lbrack;AMD&amp;rbrack; Artefactos en los bordes de todos los rellenos de proyección 3D
* &amp;lbrack;Motor&amp;rbrack; Las texturas se rompen al alternar la visibilidad de las capas
* &amp;lbrack;Motor&amp;rbrack; Las texturas están vacías en algunos lugares al cambiar el modo de fusión
* &amp;lbrack;Motor&amp;rbrack; La textura/proyección está en modo de deformación vacío en algunos casos
* &amp;lbrack;Iray&amp;rbrack; Iteración restablecida a 0 al guardar el procesamiento
* &amp;lbrack;Registro&amp;rbrack; USD mensaje de error al realizar Archivo > Nuevo

**Problemas conocidos:**

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Pila de capas&amp;rbrack; El origen de entrada no se guarda por capa

## Versión 8

### 8.3.1

Fecha de publicación: **2023/04/27**

**Agregado:**

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añadir método abreviado (vacío) para mostrar/ocultar la visualización de la ventana gráfica
* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Mostrar siempre el nivel de poli bajo al utilizar el botón &quot;Ocultar mallas de haga un bake&quot;
* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Mostrar sufijo para Coincidencia por nombre según el conjunto de texturas actual
* &amp;lbrack;Importar&amp;rbrack; Añadir soporte para archivos binarios GLTF (glb)
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Menú Añadir para seleccionar o crear instancias del sombreador
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Permitir cambiar rápidamente el conjunto de texturas y la resolución de Mosaico de UV
* &amp;lbrack;Tamaño físico&amp;rbrack; Mejorar el comportamiento del manipulador al utilizar tamaño físico en Proyección de UV
* &amp;lbrack;UI&amp;rbrack; Volver a &quot;Guardar como&quot; en el menú principal de archivos
* &amp;lbrack;UI&amp;rbrack; Guardar selección de vista (solo 2D, solo 3D, ambos) en diseño de IU
* &amp;lbrack;USD&amp;rbrack; Mensaje de error menos vago al crear un proyecto con formas de USD no compatibles
* &amp;lbrack;Python&amp;rbrack; Añadir eventos de hacer un bake para seguir el progreso de Hacer un bake
* &amp;lbrack;Python&amp;rbrack; Permitir cancelar una hace un bake
* &amp;lbrack;Python&amp;rbrack; Exponer &quot;según plantilla de salida&quot; para el tipo de archivo y la profundidad de bits en la exportación
* &amp;lbrack;Python&amp;rbrack; Exponer el tiempo de actualización para TextureStateEvent.Update

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; Bloqueo raro al cerrar un proyecto
* &amp;lbrack;Bloqueo&amp;rbrack; &amp;lbrack;Haciendo un bake&amp;rbrack; Activar la sincronización del mapa de malla con el Height o la curvatura en un proyecto específico
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Scripting&amp;rbrack; Bloqueo al añadir un material después de crear la instancia del sombreador
* &amp;lbrack;Haciendo un bake modo&amp;rbrack; La intensidad de AO en material neutro no tiene efecto
* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Bloqueo al cambiar al modo de hacer un bake antes de cargar el modelo
* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Mensaje de error que falta en la ficha Hacer un bake proceso
* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Los ajustes de material neutro no tienen efecto después de volver a importar una malla
* &amp;lbrack;Haciendo un bake modo&amp;rbrack; El separador de ventanilla se guarda globalmente y no por modo
* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Problema de visualización: normal promedio no cambia la superficie de la jaula
* &amp;lbrack;Administración de color&amp;rbrack; La opción Detección automática del espacio de color está desactivada cuando OCIO env var está presente
* &amp;lbrack;Contenido&amp;rbrack; El filtro Contorno de máscara tiene un artefacto con entrada de height
* &amp;lbrack;Contenido&amp;rbrack; El regulador de intensidad del filtro de desenfoque de pendiente se fija en 1.0
* &amp;lbrack;Interop&amp;rbrack; No se puede crear el proyecto con GLTF desde Sampler
* &amp;lbrack;Pila de capas&amp;rbrack; El valor del mosaico de proyección no se actualiza correctamente con manipulador
* &amp;lbrack;Linux&amp;rbrack; Desplazamiento entre el lápiz de Tablet PC gráfico y el cursor con HDPI superior al 100 %
* &amp;lbrack;Python&amp;rbrack; Bloqueo al volver a importar una malla después de crear un proyecto
* &amp;lbrack;Substance&amp;rbrack; Los ruidos 3D se rompen después de volver a importar una malla
* &amp;lbrack;Mosaicos de UV&amp;rbrack; El desplazamiento de la Proyección de UV se fija en 1
* &amp;lbrack;Viewport&amp;rbrack; Los comentarios visuales de líneas rectas ya no son visibles
* &amp;lbrack;WhatsNew&amp;rbrack; Retorno de línea incorrecto en títulos de funciones

**Problemas conocidos:**

* &amp;lbrack;Importar&amp;rbrack; Algunos GLB con texturas no reciben texturas en Painter

### 8.3.0

*(Lanzado: 10 de enero de 2023*)Resumen: **Versión principal con nuevo modo de hacer un bake, nueva importación y exportación de archivos USD y compatibilidad de tamaño físico para la Proyección de UV**

**Agregado:**

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Nuevo modo de hacer un bake dedicado al proceso de hacer un bake

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Definir método abreviado para cambiar al modo de hacer un bake a F8

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Botón Añadir Inicio y Cancelar haga un bake en la ventana gráfica

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añadir selección de haga un bake en la lista Conjunto de texturas

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Ventana Añadir nuevos Bakeres de mapa de malla para seleccionar bakeres

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añada una nueva ventana Ajustes de mapa de malla para editar los ajustes de hace un bake

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añada una nueva ventana Haciendo un bake registro para seguir el proceso de hacer un bake

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Agregar parámetros de hacer un bake y acciones de deshacer a la ventana de historial

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Adición de rutas de navegación en Ajustes de mapa de malla

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añadir miniaturas de mapas de malla en la ventana Bakeres de mapas de malla

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añadir menú contraíble de ajustes de visualización en la ventana gráfica 3D

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añadir configuración de visualización para mostrar/ocultar la malla de alta densidad

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añadir configuración de visualización para mostrar/ocultar la malla de la jaula y la malla metálica

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añadir configuración de visualización para mostrar/ocultar la malla de baja densidad

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añada un ajuste de visualización para mostrar los bordes duros sin costuras UV como errores

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Informar en la ventana gráfica sobre los errores de malla y hacer un bake si Hacer un bake registro no es visible

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Agregar acción para sincronizar la configuración del baker en todos los conjuntos de texturas

  En la ventana Bakeres de mapa de malla, cada baker (así como los ajustes comunes) se pueden sincronizar en los conjuntos de texturas haciendo clic en el icono de enlace junto a su nombre. Esta acción abrirá una ventana que permite seleccionar qué conjuntos de texturas compartirán los mismos parámetros.

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Agregar acciones para copiar y pegar ajustes de baker

  En la ventana Bakeres de mapa de malla hay acciones disponibles para copiar y pegar cada configuración de baker en los conjuntos de texturas, ya sea a través del menú específico en la parte superior de la ventana o el menú contextual del botón derecho.

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; El botón Añadir en Hacer un bake registro para saltar del error a la configuración correcta

  Cuando un baker falla o una malla no se carga correctamente, aparece un mensaje de error en el registro de Hace un bake. Un botón junto al mensaje permite cambiar la ventana Bakeres de mapa de malla y ajustes de mapa de malla para mostrar los ajustes relacionados. Esto ayuda a aislar con mayor facilidad el origen de un problema para poder solucionarlo.

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añadir menús para gestionar conjuntos de texturas y selecciones de Bakeres

  En las ventanas &quot;Lista de conjuntos de texturas&quot; y &quot;Bakeres de mapa de malla&quot; se ha añadido un pequeño menú de acciones para ayudar a copiar e invertir las selecciones.

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Lista de selección de baker dividida por conjunto de texturas

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Dividir ajustes comunes por conjunto de texturas

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Cargar mallas de alta polietileno y jaula sin congelar la interfaz

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Usar la barra de progreso de la ventanilla para mostrar la carga de malla

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Añadir estado de carga de malla en el registro de Hace un bake

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Permitir girar la malla en la ventana gráfica durante la hace un bake

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Definir el orden de hace un bake en función de la visibilidad actual de la ventana gráfica de la malla

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Visualización de la jaula de haga un bake implícita en la ventana gráfica

  Si no se utiliza un fichero de malla de jaula personalizado, se generará una malla de jaula automática y se mostrará en la ventana gráfica. Su tamaño se basará en el parámetro Distancia frontal máxima de los ajustes comunes que se hacen un bake. La malla de la jaula se utiliza para indicar hasta dónde llegará la coincidencia entre el poli bajo y alto.

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Mostrar la lista de nombres de malla coincidentes por nombre en Registro de Hace un bake

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Usar material neutro para mostrar el modelo 3D en la ventana gráfica

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Desactivar el cálculo del motor mientras está en modo de hacer un bake

* &amp;lbrack;Haciendo un bake modo&amp;rbrack; Mostrar una advertencia al salir de la aplicación mientras hay un haga un bake en curso

* &amp;lbrack;Bakeres&amp;rbrack; Actualizar etiquetas de configuración de suavizado

  Los valores del ajuste de suavizado se han cambiado de nombre a &quot;Supersampling&quot; (Supermuestreo) y con un número multiplicador explícito para aclarar su comportamiento.

* &amp;lbrack;Bakeres&amp;rbrack; Actualice baker a la versión 2.5.7.

* &amp;lbrack;USD&amp;rbrack; Importación y exportación de archivos de Universal Scene Description (USD)

* &amp;lbrack;USD&amp;rbrack; Agregar USD opciones a la ventana Nuevo proyecto al seleccionar un archivo USD

* &amp;lbrack;USD&amp;rbrack; Agregar nueva ventana de selección Ámbito y Variantes

  Al importar un fichero de USD, pulsar en el botón de cambio de la ventana Nuevo proyecto o Configuración del proyecto permite seleccionar qué parte y variantes de un fichero de USD se van a importar.

* &amp;lbrack;USD&amp;rbrack; Opción Añadir niveles de subdivisión

  Al crear un nuevo proyecto con un archivo de malla de USD que contiene subdivisiones, es posible seleccionar el nivel de subdivisiones mediante un regulador. El proyecto se creará con la malla subdividida. El nivel se puede modificar mediante la configuración del proyecto.

* &amp;lbrack;USD&amp;rbrack; Importación USD mallas desolladas en un marco específico

  Al crear un nuevo proyecto con un archivo de malla de USD que contiene animación, es posible seleccionar el marco mediante un regulador que refleje la secuencia de cronología incrustada. El marco se puede modificar mediante la configuración del proyecto.

* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Añadir una opción para exportar archivos USD

  Nueva casilla de verificación Exportar USD añadida a la ventana Exportar texturas. Cuando está activada, permite exportar archivos USD, así como mapas de textura, utilizando cualquier plantilla.

* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Añadir USD formato de archivo a la exportación de malla

* &amp;lbrack;USD&amp;rbrack; Cambie el nombre del ajuste preestablecido de exportación &quot;Rugosidad del metal PBR USD&quot; para que sea más explícito

  Se puede acceder a la plantilla de exportación de USD conocida anteriormente como &quot;Rugosidad del metal de USD PBR&quot; a través de texturas de exportación > Plantilla de salida > USDz (Apple AR).

* &amp;lbrack;Auto Unwrap&amp;rbrack; Añadir orientación de bloqueo para el empaquetado

  Nueva opción para la configuración de desajuste automático que permite conservar la orientación de las Islas de UV existentes al utilizar la función de empaquetado. Se puede acceder a él desde Nuevo proyecto > Opciones de Desenvolvimiento automático > Orientación de la Isla de UV.

* &amp;lbrack;Tamaño físico&amp;rbrack; Añadir configuración para utilizar automáticamente el Tamaño físico en el efecto de relleno/capa

  Se ha añadido una nueva opción para cambiar automáticamente a la escala de tamaño físico al utilizar un material con tamaño físico incorporado. Se puede activar por proyecto a través de Nuevo proyecto o a través de Editar > Configuración del proyecto > Tamaño físico > Cambiar la escala de la capa de relleno a Tamaño físico al asignar materiales.

* &amp;lbrack;Tamaño físico&amp;rbrack; Exponer tamaño físico para Proyección de UV

  La escala de tamaño físico ahora está disponible para las Proyecciones de UV: permite el cambio de tamaño automático para un material en función del tamaño físico de una malla. Se puede seleccionar a través de Escala > Tamaño físico en la ventana Propiedades de la capa de relleno o del efecto.

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir consultar la versión de la aplicación

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Actualizar API para que coincida con los nuevos parámetros de haga un bake

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Haciendo un bake módulo: editar hacer un bake parámetros

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Haciendo un bake módulo: iniciar/cancelar hacer un bake

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Haciendo un bake módulo: seleccionar método de curvatura

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Haciendo un bake módulo: selección de bakeres/mosaicos uv

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Haciendo un bake módulo: sincronizar la configuración del baker en todos los conjuntos de texturas

* &amp;lbrack;SVT&amp;rbrack; Habilitar la compatibilidad de hardware disperso en las GPU AMD

  La aceleración de hardware para el sistema de texturas virtuales dispersas ahora se puede activar con las GPU AMD. Este ajuste se activa automáticamente en las preferencias generales.

* &amp;lbrack;Proyección&amp;rbrack; Cambiar nombre de parámetros de proyección cilíndrica

  El parámetro &quot;Cylinder Cap Culling&quot; ha pasado a denominarse &quot;Backface Culling&quot; para representar mejor su acción. La información sobre herramientas asociada se ha ajustado en consecuencia.

* &amp;lbrack;Proyecto&amp;rbrack; Guardar la versión de la aplicación en el proyecto y recuperarla mediante scripts

  Desde la versión 8.2, la versión de la aplicación se almacena ahora dentro del archivo spp al guardar. Este número de versión se puede recuperar con la función last_saved_substance_painter_version() en el módulo de proyecto de la API de Python. Para un proyecto realizado antes de la versión 8.2, el valor devuelto será nulo.

* &amp;lbrack;Importar&amp;rbrack; Mejorar el tiempo de importación general de modelos 3D

  Mejoramos el tiempo general de importación de mallas. Por ejemplo, reducir el tiempo de espera al cargar mallas de alta densidad para hacer un bake. Esta optimización se aplica en particular a la carga de archivos OBJ.

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; Cambio de canales en un filtro con una pila específica

* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;M1&amp;rbrack; Bloqueo al crear una capa de relleno y salir de la pila de capas

  Este problema se puede solucionar actualizando a Mac OS 13 (Ventura).

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Bloqueo al utilizar ui.add_dock_widget() con un tipo incorrecto

* &amp;lbrack;Haciendo un bake&amp;rbrack; Mensaje de error incompleto en el registro cuando falla una hace un bake

* &amp;lbrack;Haciendo un bake&amp;rbrack; La memoria no se libera al finalizar la hace un bake

* &amp;lbrack;Motor&amp;rbrack; La caché de textura no se actualiza al cambiar la visibilidad del efecto

* &amp;lbrack;Exportar&amp;rbrack; vista 2D exporta mapa aleatoriamente uniforme

* &amp;lbrack;Proyecto&amp;rbrack; Error de asignación de memoria al guardar el proyecto con malla grande

* &amp;lbrack;Viewport&amp;rbrack; TAA causa defectos al pintar en algunos casos

**Problemas conocidos:**

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Pila de capas&amp;rbrack; El origen de entrada no se guarda por capa

### 8.2.0

*(Lanzado: 6 de octubre de 2022*)Resumen: **Versión principal con nuevos paneles de incorporación (nuevo panel de bienvenida y nuevo panel), exportación a SBSAR, efectos para carpetas, varias mejoras para la calidad de vida y correcciones de errores.**

**Agregado:**

* &amp;lbrack;Incorporación&amp;rbrack; Panel de bienvenida para nuevos usuarios

  Se ha añadido una nueva pantalla de bienvenida cuando los nuevos usuarios de CC abren Painter por primera vez.

* &amp;lbrack;Incorporación&amp;rbrack; Panel Novedades para mejorar la capacidad de detección de las nuevas funciones

  Se ha añadido una nueva pantalla Novedades que muestra las principales funciones nuevas. Se muestra automáticamente la primera vez que se abre Painter después de una actualización importante, y se puede volver a acceder a él a través de Ayuda > Novedades.

* &amp;lbrack;Incorporación&amp;rbrack; Cambiar nombre de usuario anterior Bienvenido a &quot;Pantalla de inicio&quot;

  Se ha cambiado el nombre de la pantalla de bienvenida para evitar confusiones con la nueva pantalla de bienvenida.

* &amp;lbrack;UI&amp;rbrack; Resolver problemas de escala para pantallas de alta resolución

  Se ha mejorado la adaptación de la interfaz de usuario de Painter en pantallas de alta definición con escala de visualización personalizada.

* &amp;lbrack;UI&amp;rbrack; Evitar mensajes de error persistentes en la interfaz de usuario

  Los mensajes de error de proyectos anteriores ahora se eliminan de la barra de estado inferior.

* &amp;lbrack;UI&amp;rbrack; Menú Guardar retrabajo

  Las opciones de guardado adicionales ahora se agrupan en un submenú y se cambia el nombre de algunas de ellas por coherencia.

* &amp;lbrack;UI&amp;rbrack; Guardar y exportar/compartir diseños de IU

  En el menú Ventana hay nuevas acciones para guardar el diseño de interfaz de usuario en archivos y volver a cargarlos. Los diseños de pintura y procesamiento se guardan por separado. Se han añadido varias funciones a &quot;substance_painter.ui&quot; para guardar, restablecer y cargar diseños de interfaz de usuario.

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

* &amp;lbrack;Panel Activos&amp;rbrack; Los recursos favoritos de los &quot;Pin&quot; aparecerán en la parte superior del panel de recursos

  Se ha añadido una nueva opción de clic con el botón derecho en los recursos de la biblioteca que permite pin como favoritos en la parte superior del panel. También puede ver todos sus activos favoritos a través de Búsquedas guardadas.

* &amp;lbrack;Panel Activos&amp;rbrack; Eliminar, volver a cargar y cambiar el nombre de activos

  Se han añadido opciones de menú contextual para eliminar, volver a cargar y cambiar el nombre de los activos en la biblioteca del usuario. Se eliminan directamente de la ubicación de su biblioteca en el disco y se vuelven a cargar desde la ubicación original. Los activos que forman parte de un paquete como .abr o .sbsar no se pueden editar individualmente.

* &amp;lbrack;Selección de color&amp;rbrack; Adición de modos de fusión al efecto Selección de color

* &amp;lbrack;Pila de capas&amp;rbrack; Añadir modo de fusión y opacidad en los filtros

* &amp;lbrack;Pila de capas&amp;rbrack; Permitir valores de mosaico mayores que 128 para capas/efectos de relleno

* &amp;lbrack;Pila de capas&amp;rbrack; Tapones cilíndricos para proyección cilíndrica en capa/efecto de relleno

  La proyección cilíndrica en Propiedades de capa de relleno ahora tiene la opción de eliminar tapas de cilindro.

* &amp;lbrack;Registro&amp;rbrack; Mostrar un mensaje de error si los elementos de malla están en espacio negativo al intentar crear un proyecto de Mosaico de UV

  Se ha añadido un mensaje de error más claro al no crear un proyecto de Mosaico de UV porque las partes UV se encuentran en espacios negativos.

* &amp;lbrack;Proyecto&amp;rbrack; Indicar la versión en el mensaje de error &quot;Datos demasiado recientes&quot; al abrir un proyecto

  Al abrir un proyecto que es demasiado reciente para la aplicación, el mensaje de error indicará ahora la versión del proyecto para que sea más fácil identificar la versión correcta de la aplicación.

* &amp;lbrack;Viewport&amp;rbrack; Permita que se ilumine la malla desde abajo

  Se ha añadido un nuevo parámetro Alineación del entorno en Configuración de la pantalla > Cámara > Configuración del entorno para alinear la iluminación del mapa de entorno con la cámara cuando se establece en &quot;Local&quot;.

* &amp;lbrack;Viewport&amp;rbrack; Ver R, G, B y Alpha en la ventana gráfica (modo de visualización individual)

  En Configuración de visualización > Configuración de ventana gráfica > Visualización de canal , hay un nuevo ajuste de Canales de color que solo permite mostrar el componente R, G, B o Alpha de un canal en el modo de visualización única.

* &amp;lbrack;Sombreador&amp;rbrack; Permitir la configuración de canales de usuario como RGBA en sombreadores de capas de material

  Al definir la configuración de canales del conjunto de texturas dentro de un sombreador para la capa de material, ahora es posible especificar el formato del canal que se va a desviar del valor predeterminado. Esto permite en particular solicitar canales de usuario de color en lugar de solo escala de grises.

* &amp;lbrack;Exportar&amp;rbrack; Permitir exportar texturas como SBSAR

  Al exportar texturas a través de la ventana Archivo > Exportar Texturas, se puede elegir el formato de archivo SBSAR (Archivo de Substance) para reagruparlas. El contenido de la SBSAR depende de la plantilla de salida utilizada. El formato de archivo SBSAR también se puede establecer en los ajustes preestablecidos de exportación. Cuando se utiliza una configuración híbrida (SBSAR + otro formato), las texturas que tienen como destino un SBSAR se agrupan mientras que el resto se exporta junto a ellas.

* &amp;lbrack;Exportar&amp;rbrack; Opción Exponer 16 bits para EXR formato de archivo

  Al exportar archivos de textura de EXR, ahora es posible elegir 16f bit (medio Flotante) o 32f bit (Flotante) en la ventana Exportar Texturas (tanto para ajustes de exportación como para ajustes preestablecidos de exportación). Los proyectos antiguos y los ajustes preestablecidos de exportación antiguos se establecerán de forma predeterminada en 16f bit para reflejar el comportamiento antiguo.

* &amp;lbrack;Python&amp;rbrack; Agregar evento para saber cuándo se modifican los conjuntos de texturas

  El nuevo &quot;substance_painter.event.TextureStateEvent&quot; permite saber cuándo se ha modificado un conjunto de texturas debido a un trazo de pintura, un nuevo canal añadido o un canal eliminado.

* &amp;lbrack;Python&amp;rbrack; Permitir obtener y definir recursos de mapa de malla en los ajustes de Conjunto de texturas

  Se han añadido nuevas funciones en el módulo &quot;substance_painter.project&quot; para obtener y definir recursos de mapas de malla. Estas funciones se pueden utilizar para actualizar los mapas de malla a los que hace referencia la configuración de Conjunto de texturas.

* &amp;lbrack;Complementos&amp;rbrack; Opción Quitar para obtener otros complementos de JS

  Se ha eliminado la opción para obtener los complementos de JavaScript, ya que se alojaban en el sitio web obsoleto Compartir .

* &amp;lbrack;Contenido&amp;rbrack; Añadir nueva plantilla Roblox y exportar ajuste preestablecido

  Se han añadido una nueva plantilla de proyecto &quot;Material Variant&quot; y &quot;Surface Appearance&quot; de Roblox y un ajuste preestablecido de exportación para facilitar la exportación de texturas PBR a Roblox. Se puede acceder a la plantilla desde la ventana Archivo > Nuevo proyecto.

* Actualizar Substance Engine a la última versión (8.6.3)

* &amp;lbrack;Vapor&amp;rbrack; Compilación optimizada para chipset Apple Silicon (Apple M1 / M2)

**Corregido:**

* Bloqueo al utilizar 16k exr

* &amp;lbrack;Bloqueo&amp;rbrack; Ctrl Z Después de eliminar una instancia del sombreador

* &amp;lbrack;Iray&amp;rbrack; IoR está bloqueado en 1 para algunos sombreadores

* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;Haciendo un bake&amp;rbrack; Algunos High-Poly no se cargan

* &amp;lbrack;Administración de color&amp;rbrack; Nombre de espacio de color incorrecto en la IU con filtros

* &amp;lbrack;Python&amp;rbrack; Los objetos de recursos devueltos por la función import no tienen un tipo

  Al importar un paquete de Substance en Python, la función devolvía el paquete en lugar de sus gráficos. El módulo de recursos ahora proporciona funciones y parámetros para recuperar los gráficos de un paquete de Substance.

**Problemas conocidos:**

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Pila de capas&amp;rbrack; El origen de entrada no se guarda por capa
* &amp;lbrack;Pintura&amp;rbrack; El suavizado temporal provoca defectos al pintar en algunos casos
* &amp;lbrack;Exportar&amp;rbrack; vista 2D exporta mapa aleatoriamente uniforme

### 8.1.3

*(Lanzado: 25 de agosto de 2022*)Resumen: **Versión secundaria de corrección de errores**

**Agregado:**

* Actualizar a Iray SDK 1.6

**Corregido:**

* &amp;lbrack;Sombreador&amp;rbrack; Bloqueo con sombreador defectuoso antiguo
* &amp;lbrack;Material Layering&amp;rbrack; Los materiales pueden desaparecer al volver a abrir un proyecto

**Problemas conocidos:**

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Pila de capas&amp;rbrack; El origen de entrada no se guarda por capa
* &amp;lbrack;Bloqueo&amp;rbrack; Ctrl Z Después de eliminar una instancia del sombreador
* &amp;lbrack;Iray&amp;rbrack; IoR está bloqueado en 1 para algunos sombreadores

### 8.1.2

*(Lanzado: 19 de julio de 2022*)Resumen: **Versión secundaria de corrección de errores**

**Agregado:**

* &amp;lbrack;Auto Unwrap&amp;rbrack; Nueva opción &quot;Optimizar para mallas orgánicas&quot; para seleccionar el algoritmo de segmentación
* &amp;lbrack;Tamaño físico&amp;rbrack; Opciones de unidad de exposición en Nueva configuración de proyecto y proyecto
* &amp;lbrack;Administración de color&amp;rbrack; Usar la pantalla del monitor de forma predeterminada al utilizar ACE
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Tenga en cuenta ACE archivo de ajustes preestablecidos env-var al crear el proyecto
* &amp;lbrack;Administración de color&amp;rbrack; Restablecer la configuración de gestión de color en la ventana Nuevo proyecto cuando cambie la configuración
* &amp;lbrack;Administración de color&amp;rbrack; Deshabilitar el acceso a la configuración de OCIO cuando está presente env-var
* &amp;lbrack;Administración de color&amp;rbrack; Actualice de forma segura ACE configuración cuando ya no exista un parámetro
* Actualizar Substance Engine a la versión 8.6.0
* &amp;lbrack;Exportar&amp;rbrack; Añadir nuevo ajuste preestablecido de exportación GLTF compatible con el Desplazamiento
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Recuperar información de recursos (incluidos metadatos personalizados)
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Agregar función a la lista de consulta de nombres de malla por conjunto de texturas
* &amp;lbrack;Contenido&amp;rbrack; Añadir una nueva plantilla de mezclador y exportar un ajuste preestablecido

**Corregido:**

* &amp;lbrack;MacOS&amp;rbrack; Bloqueo al lanzar a Irak en algunos casos
* &amp;lbrack;Miniaturas&amp;rbrack; Las miniaturas de estante no se cargan correctamente
* Se omiten varios canales UV
* &amp;lbrack;Auto Unwrap&amp;rbrack; Cálculo innecesario al dividir islas largas
* &amp;lbrack;Auto Unwrap&amp;rbrack; Opción de evitar las islas alargadas no tenidas en cuenta
* &amp;lbrack;Auto Unwrap&amp;rbrack; Pérdida de datos adicionales (colores de vértice) al reempaquetar UV
* &amp;lbrack;UI&amp;rbrack; Barra de desplazamiento horizontal en la ventana de propiedades cuando la gestión de color está activada
* &amp;lbrack;Administración de color&amp;rbrack; OCIO configuraciones no tienen la función substance_3d_painter_standard_srgb
* &amp;lbrack;Generador&amp;rbrack; Uso incorrecto de los datos de usuario &quot;deshabilitado&quot;
* &amp;lbrack;Administración de color&amp;rbrack; No se debe hacer clic en el menú desplegable Espacio de color &quot;No compatible&quot;
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Sombreador&amp;rbrack; La anulación de definición de sRGB ya no funciona
* &amp;lbrack;Generador&amp;rbrack; Uso incorrecto de los datos de usuario &quot;desactivar&quot;
* &amp;lbrack;Pila de capas&amp;rbrack; Previsualizaciones rotas con proyectos de Mosaicos de UV
* &amp;lbrack;Sombreador&amp;rbrack; La documentación de la API no está completamente actualizada con Normales dobladas
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Interoperability&amp;rbrack; No se puede enviar a Stager con caracteres especiales
* &amp;lbrack;Contenido&amp;rbrack; Algunas miniaturas de pinceles preestablecidos están vacías o son demasiado oscuras

**Problemas conocidos:**

* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &amp;lbrack;Pila de capas&amp;rbrack; Las fuentes de entrada no se guardan por capa
* &amp;lbrack;Bloqueo&amp;rbrack; Ctrl Z Después de eliminar una instancia del sombreador
* &amp;lbrack;Iray&amp;rbrack; IoR está bloqueado en 1 para algunos sombreadores
* &amp;lbrack;Sombreador&amp;rbrack; Bloqueo con sombreador defectuoso antiguo

### 8.1.1

*(Lanzado: 28 de junio de 2022*)Resumen: **Revisión de versión secundaria**

**Agregado:**

* &amp;lbrack;Pila de capas&amp;rbrack; Al pulsar Alt en la máscara ya no se deseleccionan los efectos

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack; Abrir proyecto antiguo guardado en el modo de vista en solitario
* &amp;lbrack;Bloqueo&amp;rbrack; Eliminar un generador en propiedades
* &amp;lbrack;Configuración del conjunto de texturas&amp;rbrack; La mezcla normal/de Oclusión ambiental y el height a los métodos normales se rompen
* &amp;lbrack;Exportar&amp;rbrack; La exportación de texturas mediante relleno de difusión produce mapas negros

**Problemas conocidos:**

* &amp;lbrack;MacOS&amp;rbrack; Bloqueo al lanzar Iray en Monterey
* &amp;lbrack;Vista previa de miniaturas&amp;rbrack; Las miniaturas simplificadas no se actualizan cuando se utiliza un anclaje
* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción

### 8.1.0

*(Lanzado: 07 de junio de 2022*)Resumen: **Versión principal compatible con ICC, escalado de materiales basado en datos de tamaño físico, nuevos bakeres, mejoras en el cuentagotas de color y una amplia gama de contenido adicional**

**Agregado:**

* &amp;lbrack;Administración de color&amp;rbrack; Añadir compatibilidad con perfiles ICC con Adobe Color Engine (ACE)
* &amp;lbrack;Administración de color&amp;rbrack; Añada compatibilidad para &quot;RGB de Adobe 98&quot; como espacio de color de trabajo para ICC
* &amp;lbrack;Administración de color&amp;rbrack; Permitir la configuración de ACE/ICC mediante un archivo de configuración
* &amp;lbrack;Administración de color&amp;rbrack; Permitir la entrada de valores de color lineal en el Selector de color con el modo Heredado
* &amp;lbrack;Administración de color&amp;rbrack; Permitir especificar el perfil de color utilizado para seleccionar color fuera de la interfaz de usuario
* &amp;lbrack;Administración de color&amp;rbrack; Recordar el último valor de visualización elegido en la ventana gráfica
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Hacer que los generadores/filtros funcionen correctamente con la gestión de color
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Añadir nuevas palabras clave de anulación de espacio de color $working y $standardsrgb
* &amp;lbrack;Tamaño físico&amp;rbrack;&amp;lbrack;Motor&amp;rbrack; Extraer información del tamaño físico de la malla
* &amp;lbrack;Tamaño físico&amp;rbrack;&amp;lbrack;Motor&amp;rbrack; cálculo del tamaño físico
* &amp;lbrack;Tamaño físico&amp;rbrack; Opciones de exposición para utilizar el tamaño físico en la interfaz de usuario
* &amp;lbrack;Tamaño físico&amp;rbrack; Añadir ayudantes visuales en la ventana gráfica
* &amp;lbrack;Haciendo un bake&amp;rbrack; Añadir baker de Height
* &amp;lbrack;Haciendo un bake&amp;rbrack; Baker Añadir Normales dobladas
* &amp;lbrack;Haciendo un bake&amp;rbrack; Añadir baker de opacidad
* &amp;lbrack;Cuentagotas; Nueva previsualización del cuentagotas de color junto al ratón y el color gestionado
* &amp;lbrack;Cuentagotas; El panel del selector de color vuelve a aparecer en su última posición cuando se vuelve a abrir
* &amp;lbrack;Cuentagotas; Un nuevo icono para el Selector de material
* &amp;lbrack;Cuentagotas; Gestión de color de la previsualización del canal del selector de color
* &amp;lbrack;Cuentagotas; Añadir la funcionalidad de hacer clic para seleccionar al cuentagotas
* &amp;lbrack;Cuentagotas; El selector de material ya no activa canales no activos
* &amp;lbrack;Cuentagotas; Permitir el uso del cuentagotas con un método abreviado
* &amp;lbrack;Cuentagotas; El cuentagotas selecciona el canal correspondiente, cuando corresponde
* &amp;lbrack;Cuentagotas; Al entrar en el modo del selector de color se desactivan todos los métodos abreviados
* &amp;lbrack;Cuentagotas; Eliminación de la selección automática del campo hexadecimal
* &amp;lbrack;Cuentagotas; No cerrar el panel al utilizar el selector de materiales
* &amp;lbrack;Cuentagotas; Nuevo estado deshabilitado cuando el canal no está disponible para seleccionar
* &amp;lbrack;Exportar&amp;rbrack; Añadir atributo de tangente a la exportación glTF
* Actualizar Substance Engine a v8.4
* Actualizar Auto Unwrap a 0.9.0
* Actualizar a Qt 5.15.8
* Actualizar a Python 3.9
* &amp;lbrack;Sombreador&amp;rbrack; Añadir compatibilidad con el sombreado de Normales dobladas
* &amp;lbrack;MacOS&amp;rbrack; Compatibilidad con SpaceMouse 3DConnection
* &amp;lbrack;Python&amp;rbrack; Documentar la versión de Python utilizada en la API
* &amp;lbrack;Contenido&amp;rbrack; Añade 6 nuevos sonidos 3D con 105 ajustes preestablecidos
* &amp;lbrack;Contenido&amp;rbrack; 20 nuevos mapas de suciedad y 2 patrones de pliegues de tela
* &amp;lbrack;Contenido&amp;rbrack; Actualizar el ajuste preestablecido de exportación &quot;Mapas de malla&quot; para utilizar nuevos bakeres
* &amp;lbrack;Contenido&amp;rbrack; La Pendiente de desenfoque y el filtro de deformación dependen de la resolución del conjunto de texturas
* &amp;lbrack;Contenido&amp;rbrack; Actualizar proyectos de ejemplo para utilizar los 3 nuevos bakeres

**Corregido:**

* &amp;lbrack;glTF&amp;rbrack; No se puede abrir glTF con un carácter especial
* &amp;lbrack;Motor&amp;rbrack; Artefactos con anisotropía y SVT desactivados
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;M1&amp;rbrack; Los materiales inteligentes no se muestran correctamente
* &amp;lbrack;Procesamiento de malla&amp;rbrack; No se pueden importar mallas desde Modeler
* &amp;lbrack;UI&amp;rbrack; Barra de desplazamiento horizontal en la ventana de nuevo proyecto con la gestión de color activada
* &amp;lbrack;Administración de color&amp;rbrack; Falta el valor del espacio de trabajo en el selector de color con algunas configuraciones de OCIO
* &amp;lbrack;Administración de color&amp;rbrack; La previsualización del pincel en la ventana gráfica no tiene gestión de color
* &amp;lbrack;SpaceMouse&amp;rbrack; La tabla dinámica no se actualiza inmediatamente con el cambio de enfoque y, a veces, se sale del modelo
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Los archivos USD exportados tienen una estructura incorrecta
* &amp;lbrack;USD&amp;rbrack; Problema de oclusión ambiental al exportar
* &amp;lbrack;Contenido&amp;rbrack; Actualizar la malla de la miniatura para que coincida con el proyecto de muestra Previsualizar esfera

**Problemas conocidos:**

* La exportación de texturas mediante relleno de difusión produce mapas negros
* La mezcla normal o de Oclusión ambiental no funciona
* &amp;lbrack;MacOS&amp;rbrack; Bloqueo al lanzar a Irak en algunos casos raros
* &amp;lbrack;Vista previa de miniaturas&amp;rbrack; Las miniaturas simplificadas no se actualizan cuando se utiliza un anclaje
* &amp;lbrack;Administración de color&amp;rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción

## Versión 7

### 7.4.3

*(Lanzado: 11 de abril de 2022*)Resumen: **Corrección de error compatible con SpaceMouse de conexión 3D en la ventana gráfica 2D**

**Agregado:**

* &amp;lbrack;SpaceMouse&amp;rbrack; Compatibilidad con SpaceMouse de conexión 3D en la ventana gráfica 2D

**Corregido:**

* &amp;lbrack;Selector de color&amp;rbrack; No se puede escribir en campos hexadecimales
* &amp;lbrack;Administración de color&amp;rbrack; Los recursos utilizados en el modo de proyección no tienen gestión de color en la superposición
* &amp;lbrack;Administración de color&amp;rbrack; Los errores no se notifican en el registro
* &amp;lbrack;SpaceMouse&amp;rbrack; Quitar mensaje de error genérico si el usuario no tiene un SpaceMouse
* &amp;lbrack;SpaceMouse&amp;rbrack; Al cargar un proyecto, el punto de giro siempre está oculto
* &amp;lbrack;Bakeres&amp;rbrack; El ajuste &quot;Normales medias&quot; no tiene efecto en los proyectos de Mosaico de UV
* &amp;lbrack;Mosaico de UV&amp;rbrack; Las superposiciones de mosaicos uv inactivos desaparecen al volver a cargar la malla con diferentes mosaicos
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; La secuencia de comandos remota no funciona
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; No se pueden consultar varios canales desde la API y se produce un error
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Bloqueo al utilizar el evento ProjectEditionEntered
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Bloqueo al llamar a get_active_stack()

**Problemas conocidos:**

* Conexión 3D con SpaceMouse no compatible en MacOS
* &amp;lbrack;UI&amp;rbrack; Barra de desplazamiento horizontal con gestión de color que aparece en algunos casos en la ventana de nuevo proyecto
* &amp;lbrack;Mac M1&amp;rbrack; Los materiales inteligentes no se muestran correctamente

### 7.4.2

*(Lanzado: 8 de marzo de 2022*)Resumen: **Corrección de error compatible con SpaceMouse de conexión 3D y mejoras en la administración de color (OCIO)**

**Agregado:**

* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Compatibilidad con la conexión 3D de SpaceMouse en la ventana gráfica 3D para la navegación
* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Métodos abreviados/teclas básicos para los modelos Pro y Enterprise SpaceMouse en el área de visualización 3D
* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Icono del centro de rotación dedicado en la ventana gráfica 3D
* &amp;lbrack;Administración de color&amp;rbrack; Utilizar funciones de OCIO configuración para cambiar la configuración predeterminada
* &amp;lbrack;Administración de color&amp;rbrack; Gestión de color de la ventana de propiedades para widgets de color
* &amp;lbrack;Administración de color&amp;rbrack; Gestión de color de la ventana de propiedades para la previsualización de material
* &amp;lbrack;Administración de color&amp;rbrack; Gestión de color de muestras en el selector de color
* &amp;lbrack;Administración de color&amp;rbrack; Añadir un ajuste para definir el espacio de color sRGB estándar
* &amp;lbrack;Administración de color&amp;rbrack; Añadir el espacio de color sRGB estándar desde OCIO configuración en el selector de color Lista de selectores de visualización
* &amp;lbrack;Administración de color&amp;rbrack; Mejoras en el menú de anulación del espacio de color
* &amp;lbrack;Administración de color&amp;rbrack; Permitir anular el espacio de color del mapa de entorno en Configuración de visualización
* &amp;lbrack;Administración de color&amp;rbrack; Dibujar degradados del selector de color según la visualización actual
* &amp;lbrack;Administración de color&amp;rbrack; Ajustar valores HDR. de forma predeterminada en el editor de color
* &amp;lbrack;Administración de color&amp;rbrack; Usar el paso a través (sin espacio de color) para filtros en el modo Heredado
* &amp;lbrack;Administración de color&amp;rbrack; Limitar la visualización de degradados en el editor de color para que coincida con &amp;lbrack;0-1&amp;rbrack; gama
* &amp;lbrack;Administración de color&amp;rbrack; Ocultar el selector de visualización en el selector de color en el modo Heredado
* &amp;lbrack;Administración de color&amp;rbrack; Hacer que el campo hexadecimal del selector de color esté siempre en el espacio de color sRGB
* &amp;lbrack;Administración de color&amp;rbrack; Desactivar menú desplegable de visualización del selector de color para canales de datos
* &amp;lbrack;Optimización&amp;rbrack; La cuadrícula de deformación vuelve a calcular únicamente los mosaicos UV cubiertos
* &amp;lbrack;Exportar&amp;rbrack; Permitir exportar proyectos de Mosaico de UV para Sketchfab, USD y glTF
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir cambiar la función de asignación de tonos

**Corregido:**

* &amp;lbrack;Sketchfab&amp;rbrack; La actualización de un modelo existente termina creando un nuevo modelo
* &amp;lbrack;Sketchfab&amp;rbrack; Bloqueo al buscar un modelo actualizado anteriormente
* Bloqueo al exportar a USD
* Bloqueo al crear una nueva instancia del sombreador en Máscara de geometría o cuando la geometría está oculta
* &amp;lbrack;Importar ventana de recursos&amp;rbrack; Bloqueo al cambiar el tipo de recursos importados
* Los mapas de malla normales se invierten cuando se utilizan en la pila de capas
* &amp;lbrack;Substance&amp;rbrack; El modo de fusión de datos de usuario no se tiene en cuenta
* &amp;lbrack;Administración de color&amp;rbrack; Los mapas de bits con espacio de color en el nombre de archivo se importan como secuencias de Mosaico de UV
* &amp;lbrack;Administración de color&amp;rbrack; Las salidas de gestión de color del gráfico del Substance están en un espacio de color incorrecto
* &amp;lbrack;Administración de color&amp;rbrack; La herramienta Relleno poligonal muestra un color incorrecto
* &amp;lbrack;Administración de color&amp;rbrack; ACE asignador de tonos se aplica a los canales en modo solo
* &amp;lbrack;Administración de color&amp;rbrack; La iluminación de la esfera de previsualización de herramientas no se gestiona por el color
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Los mapas convertidos aplican una conversión incorrecta
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack;&amp;lbrack;Administración de color&amp;rbrack; Los proyectos creados con plantillas y OCIO variables de entorno están en modo Heredado
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; No se puede utilizar la función de evaluación de JavaScript al inicio
* &amp;lbrack;Oferta de Adobe 3D&amp;rbrack; No se puede iniciar Painter al utilizar la configuración regional con idiomas no admitidos de forma predeterminada

**Problemas conocidos:**

* Conexión 3D con SpaceMouse no compatible en MacOS
* &amp;lbrack;UI&amp;rbrack; Barra de desplazamiento horizontal con gestión de color que aparece en algunos casos en la ventana de nuevo proyecto
* &amp;lbrack;Bakeres&amp;rbrack; El ajuste &quot;Normales medias&quot; no tiene efecto en los proyectos de Mosaico de UV
* &amp;lbrack;Mac M1&amp;rbrack; Los materiales inteligentes no se muestran correctamente
* &amp;lbrack;Administración de color&amp;rbrack; Los recursos utilizados en el modo de proyección no tienen gestión de color en la superposición
* &amp;lbrack;Selector de color&amp;rbrack; No se puede escribir en campos hexadecimales

### 7.4.1

*(Lanzado: 14 de diciembre de 2021*)Resumen: **Corrección de errores con mejoras en la administración de color**

**Agregado:**

* &amp;lbrack;Administración de color&amp;rbrack; Usar función de datos en nombres de archivo exportados
* &amp;lbrack;Administración de color&amp;rbrack; Expanda la sección Administración de color de forma predeterminada cuando se selecciona OCIO en las nuevas ventanas de proyecto y configuración del proyecto
* &amp;lbrack;Administración de color&amp;rbrack; Añadir ACE asignador de tonos en modo heredado
* &amp;lbrack;Administración de color&amp;rbrack; Ajustar la configuración predeterminada
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Rellenar $colorEspacio en nombres de archivo para canales de datos
* &amp;lbrack;Exportar&amp;rbrack; Exportar proyecto de Mosaico de UV a Stager
* &amp;lbrack;Interoperabilidad&amp;rbrack; No disponible para las ediciones Steam y Substance
* &amp;lbrack;Interoperabilidad&amp;rbrack; Permitir enviar un proyecto de Mosaico de UV a Stager

**Corregido:**

* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Bloqueo&amp;rbrack; Painter no empieza con Catalina
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Bloqueo&amp;rbrack; Bloqueo aleatorio al jugar con la gestión de color/tipo de datos en el canal del usuario
* &amp;lbrack;Administración de color&amp;rbrack; Recursos utilizados como escala de grises en el espacio de color de visualización de máscara nuevo menú
* &amp;lbrack;Administración de color&amp;rbrack; El canal de usuario es más oscuro en la ventana gráfica en el modo heredado + vista solo
* &amp;lbrack;Administración de color&amp;rbrack; El mapa Env siempre es lineal cuando se utiliza en iRay
* &amp;lbrack;Administración de color&amp;rbrack; El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
* &amp;lbrack;Administración de color&amp;rbrack; El selector de color se interrumpe en el interior de un Substance en modo heredado
* &amp;lbrack;Administración de color&amp;rbrack; El cambio entre vistas de canal solo en la ventana gráfica no se muestra con el espacio de color correcto al utilizar el menú desplegable
* &amp;lbrack;Administración de color&amp;rbrack; La exportación aplica una conversión incorrecta en los canales de usuario con gestión de color en el modo heredado
* Los trazos realizados en la máscara de vista solo no se muestran al volver a la vista de material
* &amp;lbrack;Exportar&amp;rbrack; Los mapas convertidos no se exportan como canales con gestión de color
* &amp;lbrack;Conjunto de texturas&amp;rbrack; Falta la información sobre herramientas con el nombre original en los canales de usuario renombrados
* &amp;lbrack;Vapor&amp;rbrack; Faltan archivos al comprobar su integridad con Steam

**Problemas conocidos:**

* &amp;lbrack;Mac M1&amp;rbrack; Los materiales inteligentes no se muestran correctamente

### 7.4.0

*(Lanzado: 24 de noviembre de 2021*)Resumen: **Versión principal. Introducción de la primera versión de la administración de color, desacoplar vista 2D o 3D, nueva opción de desempaquetado UV automático para evitar islas alargadas, llamar a funciones de JavaScript desde la API de Python y nuevo contenido**

**Agregado:**

* &amp;lbrack;Administración de color&amp;rbrack; Compatibilidad con la gestión de color OpenColorIO versión 2
* &amp;lbrack;Administración de color&amp;rbrack; Añadir ajustes de gestión de color a los ajustes del proyecto
* &amp;lbrack;Administración de color&amp;rbrack; Ventana de advertencia sobre los cambios de configuración de la gestión de color al abrir un proyecto
* &amp;lbrack;Administración de color&amp;rbrack; Mostrar un mensaje de error si se ha seleccionado un archivo de configuración de OCIO no válido
* &amp;lbrack;Administración de color&amp;rbrack; Permitir anular la configuración con OCIO variable de entorno
* &amp;lbrack;Administración de color&amp;rbrack; Varias configuraciones de OCIO integradas de forma predeterminada con la aplicación
* &amp;lbrack;Administración de color&amp;rbrack; Extraer nombre de espacio de color del nombre de archivo de mapa de bits importado
* &amp;lbrack;Administración de color&amp;rbrack; Permitir anular el espacio de color con un espacio de color desde la configuración de la ventana Propiedades
* &amp;lbrack;Administración de color&amp;rbrack; Añadir opciones de gestión de color en Configuración del conjunto de texturas
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Permitir la gestión de color de vistas 2D y 3D por separado
* &amp;lbrack;Administración de color&amp;rbrack; Cargar y convertir mapa de entorno en el espacio de color de trabajo
* &amp;lbrack;Administración de color&amp;rbrack; Ajustar el selector de color y el editor con el espacio de color actual
* &amp;lbrack;Administración de color&amp;rbrack; Permitir seleccionar la visualización transformar espacio de color en la ventana gráfica con un nuevo menú desplegable
* &amp;lbrack;Administración de color&amp;rbrack; Aplicar visualización transformar con resultados de procesamiento de Iray
* &amp;lbrack;Administración de color&amp;rbrack; Exportar texturas con diferentes espacios de color
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Aplicación de ajustes de gestión de color de la variable de entorno (OCIO) a proyectos nuevos
* &amp;lbrack;Viewport&amp;rbrack; Permitir desacoplar la ventana gráfica 2D o 3D
* &amp;lbrack;Auto Unwrap&amp;rbrack; Nueva opción para evitar islas alargadas
* &amp;lbrack;Secuencia de comandos Python&amp;rbrack; Llamar a funciones de JavaScript desde la API de Python
* &amp;lbrack;Nueva ventana de proyecto&amp;rbrack; Hacer que la sección de mapas importados sea contraíble
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Permitir ocultar normales como una opción en la configuración de Deformación
* &amp;lbrack;Contenido&amp;rbrack; 11 nuevos mapas de suciedades
* &amp;lbrack;Contenido&amp;rbrack; 8 nuevos ajustes preestablecidos de herramientas (cremallera, cable de apriete, brillo)
* &amp;lbrack;Contenido&amp;rbrack; 8 materiales nuevos (cicatriz, bolsillo, ...)
* &amp;lbrack;Contenido&amp;rbrack; 1 generador nuevo (inflar encogimiento)

**Problemas conocidos:**

* &amp;lbrack;Mac M1&amp;rbrack; Los materiales inteligentes no se muestran correctamente
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Bloqueo&amp;rbrack; Bloqueo aleatorio al jugar con la gestión de color/tipo de datos en el canal del usuario
* &amp;lbrack;Administración de color&amp;rbrack; El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Si se guarda el procesamiento en EXR o TIFF mientras la gestión de color está activada en la ventana gráfica, el guardado siempre será lineal
* &amp;lbrack;Administración de color&amp;rbrack; Los recursos utilizados como escala de grises en la máscara muestran el menú Espacio de color incorrecto
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; El mapa Env siempre es lineal cuando se usa en Irak
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Los mapas convertidos no se exportan como canales con gestión de color
* &amp;lbrack;Administración de color&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; La exportación ignora si el canal del usuario tiene gestión de color o no está en modo heredado

### 7.3.1

*(Lanzado: 24 de noviembre de 2021*)Resumen: **Corrección de error**

**Agregado:**

* &amp;lbrack;Proyección&amp;rbrack; La escala solo debería funcionar en el espacio de objetos

**Corregido:**

* &amp;lbrack;Mac M1&amp;rbrack; La capa de material no funciona
* &amp;lbrack;Mac M1&amp;rbrack;&amp;lbrack;Proyección&amp;rbrack; La deformación no funciona
* Los detalles del micro no se muestran correctamente
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Bloqueo&amp;rbrack; Cambio al modo de deformación con una capa creada con una versión anterior
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Voltear no funciona cuando la transformación se establece en el espacio de entorno
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; La opción Dividir permanece seleccionada después de realizar la división
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;UV&amp;rbrack; El punto de giro se restablece al voltear la proyección
* &amp;lbrack;Filtro&amp;rbrack; Hacer un bake El entorno de iluminación cambia al volver a cargar o cambiar un parámetro
* &amp;lbrack;Interoperabilidad&amp;rbrack; No disponible para las ediciones Steam y Substance
* &amp;lbrack;Interoperabilidad&amp;rbrack; El botón &quot;Examinar contenidos 3D en el mercado&quot; siempre debe abrir el CCD en la pestaña 3D de Stock y Mercado

**Problemas conocidos:**

* &amp;lbrack;Mac M1&amp;rbrack; Los materiales inteligentes no se muestran correctamente

### 7.3.0

*(Lanzado: 13 de octubre de 2021*)Resumen: **Versión principal. Contiene una nueva proyección de deformación 3D, una nueva proyección cilíndrica, mejoras del selector de color, nuevas funciones en la API de Python y correcciones de errores**

**Agregado:**

* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Exponer deformación 3D como un nuevo modo de proyección
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Permitir el modo de pegatina para Alpha, Texturas y procedimientos con la función de arrastrar y soltar en la ventana gráfica
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Usar proyección de deformación con método abreviado de pegatina (ALT)
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack;&amp;lbrack;Barra de herramientas&amp;brack; Transformar deformación como completa o por vértices
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack;&amp;lbrack;Barra de herramientas&amp;brack; Añadir puntos de rejilla con las opciones de deformación dividida en sentido cruzado, horizontal o vertical
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack;&amp;lbrack;Barra de herramientas&amp;brack; Menú dedicado para acciones de restablecimiento
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack;&amp;lbrack;Barra de herramientas&amp;brack; Opción para ajustar automáticamente las tangentes al mover puntos
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack;&amp;lbrack;Barra de herramientas&amp;brack; Menú dedicado para la edición de cuadrícula (tamaño, restablecimiento, color y tamaño de control)
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Nuevo método abreviado de teclado para cambiar el modo de edición de deformación de vértices completos (MAYÚS+V)
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Clic+Ctrl permite cambiar entre la herramienta Superficie y otras herramientas
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Cilíndrico&amp;rbrack; Exponer el modo de proyección cilíndrica
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Barra de herramientas&amp;rbrack; Configuración del manipulador de grupo (tamaño, pasos de cuadrícula, pasos de ángulo)
* &amp;lbrack;Selector de color&amp;rbrack; Nueva interfaz de usuario del selector de color
* &amp;lbrack;Selector de color&amp;rbrack; Uso de valores sRGB en widgets de selector de color
* &amp;lbrack;Selector de color&amp;rbrack; Permitir guardar y eliminar muestras de color
* &amp;lbrack;Selector de color&amp;rbrack; Cuentagotas accesible desde las ranuras de color y normales
* &amp;lbrack;Selector de color&amp;rbrack; Permitir la edición de color dinámico entre 0 y 255 valores
* &amp;lbrack;Selector de color&amp;rbrack; Hacer común el estado de HSV/RGB en toda la aplicación
* &amp;lbrack;Selector de color&amp;rbrack; La ventana del selector de color es semipersistente
* &amp;lbrack;Selector de color&amp;rbrack; Al pulsar Esc se cierra la ventana del selector de color
* Mejora del rendimiento para la interacción de la interfaz de usuario y la pintura
* &amp;lbrack;Motor&amp;rbrack; Actualizar a la nueva versión del motor de Substance (8.3.0)
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir volver a cargar la malla del proyecto actual
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir la actualización de recursos en proyectos
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir establecer y consultar la resolución de Mosaicos de UV
* &amp;lbrack;Interoperabilidad&amp;rbrack; No disponible para las ediciones Steam y Substance
* &amp;lbrack;Interoperabilidad&amp;rbrack; Recibir varios recursos de Bridge

**Corregido:**

* El selector de color no muestra el color correcto
* &amp;lbrack;Haciendo un bake&amp;rbrack; La lista de conjuntos de texturas no está ordenada correctamente
* &amp;lbrack;FBX import&amp;rbrack; No se tienen en cuenta las transformaciones de pivote de grupo 3ds Max
* &amp;lbrack;Substance Engine&amp;rbrack; Bloqueo con la importación de SBSAR dañado
* &amp;lbrack;MacOS&amp;rbrack; La opción de configuración del proyecto en diferentes idiomas no está presente
* El guardado automático puede congelar Painter durante procesos largos

**Problemas conocidos:**

* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; La opción Dividir permanece seleccionada después de realizar la división
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Voltear no funciona cuando la transformación se establece en el espacio de entorno
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;Deformar&amp;rbrack; Líneas de artefacto entre parches en algunos casos raros
* &amp;lbrack;Proyección&amp;rbrack;&amp;lbrack;UV&amp;rbrack; El punto de giro se restablece al voltear la proyección
* &amp;lbrack;Mac M1&amp;rbrack; Los materiales inteligentes no se muestran correctamente
* &amp;lbrack;M1&amp;rbrack;&amp;lbrack;Regresión&amp;rbrack; La capa de material no funciona

### 7.2.3

*(Lanzado: 24 de agosto de 2021*)Resumen: **Versión secundaria, corrección de errores**

**Agregado:**

* &amp;lbrack;Bibliotecas&amp;rbrack; Agregar una forma de excluir archivos no deseados del rastreo

**Corregido:**

* &amp;lbrack;Win&amp;rbrack; Problemas de suspensión y varias pantallas
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Bloqueo&amp;rbrack; Cambio de sombreador al utilizar efectos
* &amp;lbrack;Viewport&amp;rbrack; El modo de previsualización completa ya no muestra el cursor del pincel sin alfa
* &amp;lbrack;UI&amp;rbrack; El widget de ángulo gira en la dirección equivocada
* &amp;lbrack;Pila de capas&amp;rbrack; Muchas subcarpetas crean bloqueos muy largos
* &amp;lbrack;Iray&amp;rbrack; Diferentes vistas en Iray y OpenGL: Visible si no funciona
* &amp;lbrack;Iray&amp;rbrack; El índice de refracción no se tiene en cuenta y no aparece en las propiedades de mdl
* &amp;lbrack;JavaScript&amp;rbrack; ShowExportDialog() nunca devuelve true
* No se puede leer mtl desde Adobe Stock

### 7.2.2

*(Lanzado: 27 de julio de 2021*)Resumen: **Versión secundaria, corrección de errores**

**Agregado:**

* Actualizar la versión de requisitos de controlador AMD

**Corregido:**

* &amp;lbrack;Mac M1&amp;rbrack; Detección de memoria incorrecta
* &amp;lbrack;Exportar&amp;rbrack; Los trazados muy largos no se muestran correctamente

**Problemas conocidos:**

* &amp;lbrack;Contenido&amp;rbrack; Sombreadores obsoletos de las muestras

### 7.2.1

*(Lanzado: 02 de julio de 2021*)Resumen: **Versión secundaria, revisión**

**Agregado:**

* &amp;lbrack;Interop&amp;rbrack; Añada información sobre herramientas para indicar que el envío de proyectos de Mosaico de UV a Stager aún no se admite
* &amp;lbrack;Complemento&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Actualización del icono de Livelink

**Corregido:**

* &amp;lbrack;Nvidia&amp;rbrack; La versión del controlador que comienza por 30 se considera obsoleta
* &amp;lbrack;Bibliotecas&amp;rbrack; El estado del panel Activos no se guarda a menos que esté abierto un proyecto
* &amp;lbrack;Bibliotecas&amp;rbrack; La nueva búsqueda guardada conserva la palabra clave de la antigua búsqueda guardada
* &amp;lbrack;Bakeres&amp;rbrack;&amp;lbrack;UVTiles&amp;rbrack; Los mapas de ID por meshID también tienen en cuenta los Mosaicos de UV
* &amp;lbrack;Exportar&amp;rbrack; Los archivos gLTF no importan el color del vértice
* &amp;lbrack;Iray&amp;rbrack; Faltan algunas sugerencias
* &amp;lbrack;Interop&amp;rbrack; Enviar a Stager no siempre está desactivado cuando no se detecta Stager
* &amp;lbrack;Actualizador de recursos&amp;rbrack; No se puede actualizar Photoshop Brushmaker
* &amp;lbrack;Contenido&amp;rbrack; El generador de desgaste de borde de fibra de vidrio está roto

### 7.2.0

*(Lanzado: 23 de junio de 2021*)Resumen: **Versión principal: proporciona una actualización del panel de recursos, un nuevo sombreador con acceso a nuevos canales y parámetros, una actualización general de la interfaz de usuario, algunas mejoras de rendimiento muy solicitadas, compatibilidad con más idiomas y mucho más.**

**Agregado:**

* &amp;lbrack;Bibliotecas&amp;rbrack; Nuevo panel Activos para sustituir el estante
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevo diseño del panel Activos
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Cambiar la orientación y la interfaz de usuario predeterminadas del panel Activos
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Introducir una opción de vista de lista en la biblioteca
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nueva navegación de rutas de navegación en el panel Activos
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Seleccionar &quot;Todas las bibliotecas&quot; al seleccionar una búsqueda guardada
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Seleccionar &quot;Todas las bibliotecas&quot; cuando se anula la selección de todas las carpetas
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nueva etiqueta para pinceles de partículas
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Se ha reemplazado &quot;estantería&quot; por &quot;Todas las bibliotecas&quot; en la aplicación.
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Permitir ocultar carpetas vacías
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; La biblioteca de usuario predeterminada debe estar visible aunque esté vacía
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevo método de filtrado mediante iconos de tipo de activo
* &amp;lbrack;Bibliotecas&amp;rbrack; Método abreviado &quot;CTRL&quot; para seleccionar varios tipos de recursos
* &amp;lbrack;Bibliotecas&amp;rbrack; Nueva variable de entorno para controlar el presupuesto de memoria de previsualización de recursos
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Nuevos mapas de entorno
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Content&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Procesar desplazamiento en materiales predeterminados
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Definir sombreador de Adobe Standard Material (ASM) como predeterminado para la generación de vistas previas
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Contenido&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Nuevas plantillas de proyecto para el nuevo sombreador de ASM
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Miniatura&amp;rbrack; Utilizar nuevo mapa de entorno de Studio 6
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Miniatura&amp;rbrack; Leer miniatura en el recurso en lugar de generarla
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Miniatura&amp;rbrack; Añadir desplazamiento a la generación de miniaturas
* &amp;lbrack;Configuración del conjunto de texturas&amp;rbrack;
* &amp;lbrack;Configuración del conjunto de texturas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Exponer el nuevo height al método de conversión normal
* &amp;lbrack;Configuración del conjunto de texturas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Repaso de la organización de la interfaz de usuario de los canales
* &amp;lbrack;Configuración del conjunto de texturas&amp;rbrack; Límite de canales de usuario aumentado a 16 canales
* &amp;lbrack;Configuración del conjunto de texturas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Indicar qué canales son compatibles con el sombreador seleccionado actualmente
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Nuevo sombreador de Adobe Standard Material
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Se ha agregado la compatibilidad con Anisotropía, capa transparente, dispersión subsuperficial, Specular edge color y brillo
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Cambiar los valores de color de los canales predeterminados
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Plantilla de exportación actualizada de Adobe Dimension a Adobe Substance 3D Stager
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Se han añadido rótulos y descripciones emergentes para los parámetros de sombreador y MDL
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Hacer visible el color de la Dispersión en vista 2D aunque no se admita SSS
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Apoya al sombreador de ASM en Irak con el nuevo MDL
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Dispersión subsuperficial actualizada en brillo y revestimiento de especificaciones PBR heredadas
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Se ha cambiado el tipo de SSS predeterminado para las muestras.
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Documentación añadida para la API de ASM
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Optimizar sombreadores para ignorar los canales no utilizados
* &amp;lbrack;Sombreador&amp;rbrack; Exponer nuevos canales de Conjunto de texturas
* &amp;lbrack;Sombreador&amp;rbrack; Dispersión subsuperficial mejorada
* &amp;lbrack;Sombreador&amp;rbrack; Parámetros de sombreador nuevos ocultos para algunos sombreadores
* &amp;lbrack;Sombreador&amp;rbrack; Visible si para los parámetros de sombreador
* &amp;lbrack;Rendimiento&amp;rbrack;
* &amp;lbrack;Bibliotecas&amp;rbrack; Mejoras en el tiempo de carga y el rendimiento del cálculo de la previsualización de recursos
* &amp;lbrack;Motor&amp;rbrack; Mejoras de rendimiento de pintura
* &amp;lbrack;Auto Unwrap&amp;rbrack;
* &amp;lbrack;Auto Unwrap&amp;rbrack; Mejoras de rendimiento de empaquetado
* &amp;lbrack;Auto Unwrap&amp;rbrack; Ajuste automático compatible con el flujo de trabajo de Mosaico de UV
* &amp;lbrack;Desenvolvimiento automático&amp;rbrack; Nueva opción para colocar las coordenadas UV según la orientación de la malla
* &amp;lbrack;Otro&amp;rbrack;
* &amp;lbrack;Configuración&amp;rbrack; Dirección de zoom predeterminada cambiada
* &amp;lbrack;UI&amp;rbrack; Actualización general de la IU
* &amp;lbrack;UI&amp;rbrack; Repaso del menú Ayuda
* &amp;lbrack;UI&amp;rbrack; Reemplazar icono de inversión
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Complemento&amp;rbrack; Icono Reemplazar para el vínculo del complemento dcc
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Actualizar la versión mínima requerida y el mensaje emergente
* &amp;lbrack;Pila de capas&amp;rbrack; Crear una nueva capa dentro de la carpeta vacía seleccionada
* Actualizar documentación de Python
* &amp;lbrack;Marca&amp;rbrack;
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nombre de la aplicación actualizado a Adobe Substance 3D Painter
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Se ha actualizado la versión independiente a &#39;Edición de Substance&#39;.
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nombre del ejecutable de la aplicación, ruta de instalación, paquete e iconos actualizados
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Ruta y biblioteca predeterminadas renombradas
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Ventana Acerca de Actualizada
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Pantalla de bienvenida actualizada
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Se ha eliminado el número de versión basado en años
* &amp;lbrack;Localización&amp;rbrack; Nuevas traducciones al alemán, francés y chino simplificado
* &amp;lbrack;Interoperabilidad&amp;rbrack; No disponible para las ediciones Steam y Substance
* &amp;lbrack;Interoperabilidad&amp;rbrack; Interoperabilidad con el ecosistema de Adobe: Designer, Sampler, Stager y Bridge
* &amp;lbrack;Interoperabilidad&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Recibir y actualizar recursos de Designer
* &amp;lbrack;Interoperabilidad&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Recibir recursos de Sampler
* &amp;lbrack;Interoperabilidad&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Enviar contenido a Stager
* &amp;lbrack;Interoperabilidad&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Mostrar en Adobe Bridge
* &amp;lbrack;Interoperabilidad&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Permitir el acceso rápido a Adobe 3D Assets
* &amp;lbrack;Interoperabilidad&amp;rbrack; Nuevas etiquetas de uso de sbsar
* &amp;lbrack;Interoperabilidad&amp;rbrack; Gestionar tipos de activos recibidos
* &amp;lbrack;Interoperabilidad&amp;rbrack; Los activos recibidos de Adobe Substance 3D Designer o Adobe Substance 3D Sampler se almacenan en la biblioteca seleccionada de forma predeterminada por el usuario
* &amp;lbrack;Interoperabilidad&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevo icono en la barra de herramientas de la izquierda para enviarlo a Stager o Photoshop

**Corregido:**

* &amp;lbrack;Tablet&amp;rbrack; Bajo rendimiento al pintar con presión
* &amp;lbrack;Tablet&amp;rbrack; Problema en tabletas con controles deslizantes
* &amp;lbrack;Bloqueo&amp;rbrack; El nombre no coincide entre la lista Conjunto de texturas y el Exportador
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Bibliotecas&amp;rbrack; Doble clic en una subbiblioteca
* &amp;lbrack;Bibliotecas&amp;rbrack; Problema al rastrear directorios de la biblioteca
* &amp;lbrack;Bibliotecas&amp;rbrack; La línea de comandos de generación de previsualización forzada no funciona del modo esperado
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Content&amp;rbrack; El filtro Entorno de luz hecho un bake es negro de forma predeterminada
* &amp;lbrack;Linux&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Exportar malla&amp;rbrack; No se puede importar glTF creado en Linux/MacOS
* &amp;lbrack;Linux&amp;rbrack; Arrastrar y soltar un archivo en el panel Recursos puede provocar un bloqueo
* &amp;lbrack;Desenvolvimiento automático&amp;rbrack; El Desenvolvimiento automático está disponible incluso si no se ha seleccionado una malla para la recarga
* &amp;lbrack;Partículas&amp;rbrack; Comportamiento incorrecto de las partículas con la gravedad
* &amp;lbrack;Pila de capas&amp;rbrack; El histograma de niveles solo puede utilizar Luminancia con algunos canales
* &amp;lbrack;Máscara de geometría&amp;rbrack; El menú del botón derecho del ratón en una carpeta al editar la máscara de geometría no funciona
* &amp;lbrack;Proyección&amp;rbrack; Costura con proyección esférica y filtrado bilineal
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Exportar máscara a archivo solo exporta el mosaico 0, 0
* &amp;lbrack;Exportar malla&amp;rbrack; FBX exportación de malla está vacía
* &amp;lbrack;Iray&amp;rbrack; El mapa de normales no se tiene en cuenta en los nuevos proyectos al procesar
* &amp;lbrack;Guardar&amp;rbrack; Guardar problemas en unidades compartidas
* &amp;lbrack;Haciendo un bake&amp;rbrack; Al volver a hornear una malla con parámetros modificados, se muestra una advertencia
* &amp;lbrack;Haciendo un bake&amp;rbrack;&amp;lbrack;Regresión&amp;rbrack; Resultado incorrecto cuando el cuadro delimitador global de mallas de poli altas no incluye el origen de la escena
* &amp;lbrack;Python&amp;rbrack; Las bibliotecas de usuario personalizadas no se tienen en cuenta

**Problemas conocidos:**

* &amp;lbrack;Bibliotecas&amp;rbrack; Las búsquedas guardadas no se guardan si no hay ningún proyecto abierto
* &amp;lbrack;NVIDIA&amp;rbrack; Mensaje para el controlador obsoleto incluso si el controlador está actualizado

### 7.1.1 (2021.1.1)

*(Lanzado: 23 de marzo de 2021*)Resumen: **Versión secundaria, corrección de errores con posibilidad de introducir valores hexadecimales en el selector de color**

**Agregado:**

* &amp;lbrack;Registro&amp;rbrack; Advertencia a los usuarios sobre los controladores de GPU AMD incompatibles
* &amp;lbrack;Selector de color&amp;rbrack; Permitir escribir valores hexadecimales

**Corregido:**

* &amp;lbrack;Baker&amp;rbrack; Disminución del rendimiento
* &amp;lbrack;Máscara de geometría&amp;rbrack; Alt clic en el nombre de la malla puede llevar a un bloqueo
* &amp;lbrack;Motor&amp;rbrack; La pintura no actualiza toda la vista cuando es necesario
* &amp;lbrack;Pila de capas&amp;rbrack; La selección se bloquea después de cambiar el sombreador
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Selector de color&amp;rbrack; El color es ligeramente diferente del que se ha elegido
* &amp;lbrack;Exportar&amp;rbrack; El uso del formato de archivo PSD no genera un archivo por Mosaico de UV
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Javascript&amp;rbrack; alg.mapexport.getPathsExportDocumentMaps() no devuelve todos los valores
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Los complementos deshabilitados se vuelven a habilitar al volver a abrir Painter

### 7.1.0 (2021.1.0)

*(Lanzado: 28 de enero de 2021*)Resumen: **Versión principal, nueva máscara de geometría que permite seleccionar y pintura partes de la geometría, copiar y pegar efectos en la pila de capas, mejorar el flujo de trabajo de Mosaico de UV, actualizar Iray, Bakeres, Substance Engine y nuevo contenido**

**Agregado:**

* Nueva máscara de geometría y pintura las partes seleccionadas de la geometría
* &amp;lbrack;Máscara de geometría&amp;rbrack; Permitir la pintura de las partes seleccionadas de la geometría por nombres de malla
* &amp;lbrack;Máscara de geometría&amp;rbrack; Selección rectangular en ambas ventanas gráficas
* &amp;lbrack;Máscara de geometría&amp;rbrack; Permitir ocultar/ignorar la geometría excluida en cualquier capa
* &amp;lbrack;Máscara de geometría&amp;rbrack;&amp;lbrack;Propiedades&amp;rbrack; Selección rápida de casillas de verificación al hacer clic y arrastrar
* &amp;lbrack;Geometry Mask&amp;rbrack;&amp;lbrack;Properties&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Incluir/excluir todo con un menú desplegable en la ventana Propiedades
* &amp;lbrack;Máscara de geometría&amp;rbrack;&amp;lbrack;Propiedades&amp;rbrack; Permitir seleccionar rápidamente un elemento de una lista con ALT+CLIC IZQUIERDO
* &amp;lbrack;Máscara de geometría&amp;rbrack;&amp;lbrack;Propiedades&amp;rbrack; Superposición en las ventanas gráficas al pasar el cursor por los nombres/Mosaicos de UV de malla en la ventana Propiedades
* &amp;lbrack;Máscara de geometría&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Añadir opciones de Copiar/Pegar a la máscara de geometría
* &amp;lbrack;Máscara de geometría&amp;rbrack; Icono Nuevo para el botón Ocultar/ignorar geometría excluida
* &amp;lbrack;Máscara de geometría&amp;rbrack; Nueva información sobre herramientas para Ocultar/ignorar geometría excluida
* &amp;lbrack;Máscara de geometría&amp;rbrack; Pulse el método abreviado del teclado ALT+H para activar o desactivar el botón &quot;ocultar y omitir geometría excluida&quot;
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Nueva miniatura de vista previa de la esfera de capa de relleno para Mosaicos de UV y modo simplificado
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Permitir salir fácilmente de la máscara de Mosaico de UV
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Permitir dar una descripción por Mosaico de UV
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Configuración del conjunto de texturas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Dos nuevos títulos de sección en el menú desplegable para cambiar la resolución de Mosaico de UV
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Salir de la máscara de Mosaico de UV al arrastrar un material a la ventana gráfica
* &amp;lbrack;Pila de capas&amp;rbrack; Añadir opciones de Copiar/Pegar para efectos
* &amp;lbrack;Pila de capas&amp;rbrack; Permitir copiar y pegar efectos de un conjunto de texturas a otro
* &amp;lbrack;Pila de capas&amp;rbrack; Permitir selección múltiple de efectos
* &amp;lbrack;Pila de capas&amp;rbrack; Añadir opciones de copiar/pegar como métodos abreviados para efectos de capa
* &amp;lbrack;Pila de capas&amp;rbrack; Cambiar automáticamente entre máscara y contenido al arrastrar efectos a otra capa
* &amp;lbrack;Pila de capas&amp;rbrack; Crear automáticamente una máscara al pegar una máscara de otra capa
* &amp;lbrack;Pila de capas&amp;rbrack; Añada acciones de mover efectos dentro del menú contextual del botón derecho de los efectos
* &amp;lbrack;Pila de capas&amp;rbrack; Permitir arrastrar y soltar efectos de una capa a otra
* &amp;lbrack;Pila de capas&amp;rbrack; Al arrastrar elementos a una carpeta, se colocan en la parte superior de la carpeta
* Actualizar Iray a la versión 2020.1.0
* &amp;lbrack;Bakeres&amp;rbrack; Actualizar Bakeres a la versión 2.5.4
* &amp;lbrack;Bakeres&amp;rbrack; Mostrar Mosaicos de UV individuales en la ventana de progreso de hacer un bake
* &amp;lbrack;Bakeres&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Permite hacer un bake rápidamente el conjunto de texturas actual con un nuevo botón
* &amp;lbrack;Bakeres&amp;rbrack; Permitir al usuario seleccionar rápidamente uno de los bakeres con ALT+CLIC IZQUIERDO
* Actualizar Substance Engine a la versión 8.0.8
* &amp;lbrack;Substance Engine&amp;rbrack; Compatibilidad con el color predeterminado en los nuevos archivos .sbsar
* &amp;lbrack;Auto Unwrap&amp;rbrack; Mejora del rendimiento
* &amp;lbrack;Exportar&amp;rbrack; Agregue comentarios visuales para indicar qué resolución de Mosaico de UV difiere de la predeterminada del proyecto
* &amp;lbrack;Exportar&amp;rbrack; Añadir un factor de tamaño de escena al archivo json de sombreador exportado
* &amp;lbrack;Idioma&amp;rbrack; Añadir traducción al japonés
* &amp;lbrack;UI&amp;rbrack; Ventana Actualizar Acerca de con control de versiones de dependencias internas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir la administración de recursos de Shelf
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir saber cuándo un proyecto está listo para hacer un bake y exportar
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir saber cuándo un recurso de plataforma ha terminado de rastrear recursos en el disco
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir consultar la lista de mosaicos UV por conjuntos de texturas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir la asignación de previsualizaciones personalizadas a recursos de estante
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir la gestión de estantes personalizados
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Agregue un índice de método en cada submódulo de la documentación
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Nuevo estilo para la documentación
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Mejora de los recursos y documentación de la estantería
* &amp;lbrack;Contenido&amp;rbrack; Tres nuevos ajustes preestablecidos de herramientas para realizar puntos de sutura
* &amp;lbrack;Shelf&amp;rbrack; Eliminar temporalmente &quot;Exportar a Substance share&quot; al realizar la transición a la nueva plataforma de Substance share

**Corregido:**

* Bloqueo al utilizar monitores con diferentes resoluciones
* Bloqueo en Substance Engine con algunos proyectos raros
* La actualización de la ventana gráfica falla con Ocultar/Ignorar geometría excluida al cambiar de capa
* &amp;lbrack;vista 2D&amp;rbrack; La ventana gráfica 2D puede faltar en algunos proyectos
* &amp;lbrack;Haciendo un bake&amp;rbrack; &quot;Coincidir por nombre de malla&quot; ignora partes del objeto
* &amp;lbrack;Pila de capas&amp;rbrack; Hacer clic en un efecto de capa abre una carpeta
* &amp;lbrack;Máscara de geometría&amp;rbrack; El Mosaico de UV se sigue contando en la máscara incluso al volver a importar la malla sin ella
* &amp;lbrack;Máscara de geometría&amp;rbrack; El menú del botón derecho del ratón en la ventana gráfica no proporciona las herramientas correctas
* &amp;lbrack;Motor&amp;rbrack; Grandes retrasos en proyectos concretos
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Alta latencia con solicitudes de POST JSON remoto en Windows
* &amp;lbrack;Linux&amp;rbrack; La cantidad de Vram no se detecta correctamente con GPU integradas específicas
* &amp;lbrack;Auto Unwrap&amp;rbrack; Bloqueos o desajuste prolongado en algunos proyectos

## Versión 6

### 6.2.2 (2020.2.2)

*(Lanzado: 28 de septiembre de 2020*)Resumen: **Versión secundaria, corrección de errores con algunas funciones en la API de Python**

**Agregado:**

* &amp;lbrack;Rendimiento&amp;rbrack; No compute todos los Mosaicos de UV cuando utilice la selección de ID de color
* &amp;lbrack;Bakeres&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Visualización de descripciones de conjuntos de texturas
* &amp;lbrack;Bakeres&amp;rbrack; Permitir guardar hacer un bake configuración
* &amp;lbrack;Bakeres&amp;rbrack; Añadir opciones de contraer todo/expandir todo a la pestaña Selección
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Ocultar descripción cuando esté vacía
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Hacer clic en el Mosaico de UV debe expandir/contraer la lista
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Permitir cambiar el tamaño horizontal del panel Lista de conjuntos de texturas
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Texto de información sobre herramientas coherente para el flujo de trabajo de Mosaicos de UV y Conjunto de texturas con texturas no seleccionadas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir el uso de ajustes preestablecidos de exportación para exportar texturas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Añadir un registro de cambios en la documentación
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir consultar todos los canales disponibles en una pila determinada
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Mejoras de IU de consola

**Corregido:**

* &amp;lbrack;AMD&amp;rbrack; Detección incorrecta de una versión obsoleta del controlador
* Bloqueo al volver a importar una malla con un diseño de Mosaicos de UV diferente en algunos casos
* Bloqueo al utilizar partículas con UDIM en mallas muy pesadas
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Bloqueo al exportar una malla con información de desplazamiento en algunos casos
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Bloqueo&amp;rbrack; Exportar Vista 2D en formato psd puede causar un bloqueo
* Importar imágenes como secuencias al crear un proyecto no funciona
* Motor atascado en un bucle infinito
* &amp;lbrack;Método abreviado&amp;rbrack; La cámara gira siempre en modo de ajuste al cambiar los métodos abreviados de modo de ajuste
* Las mallas siempre se desenvuelven automáticamente cuando se vuelven a importar aunque la opción esté desactivada
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; El campo de texto de descripción a veces no está completamente visible durante la edición
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; El menú desplegable para ocultar/mostrar conjuntos de texturas no está completamente visible
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Al hacer clic en el icono del ojo no se debe introducir el nombre &quot;Editar conjunto de texturas&quot;
* &amp;lbrack;Configuración del conjunto de texturas&amp;rbrack; Al quitar un canal, también se elimina el canal siguiente
* &amp;lbrack;Exportar&amp;rbrack; Incluir todo y Restablecer todo no tiene en cuenta los Mosaicos de UV
* &amp;lbrack;Bakeres&amp;rbrack; Aparecen bakeres no seleccionados durante el proceso de hacer un bake
* La actualización de la resolución no se tiene en cuenta para los mapas con bake utilizados como entrada
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Bloqueo de la ventana gráfica 3D al añadir Material inteligente tras carpeta con la máscara de Mosaico de UV seleccionada
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; La malla metálica sigue siendo visible para los mosaicos ocultos con el modo de pintura directa
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Sketchfab&amp;rbrack; Problemas con el tipo de suscripción &quot;más&quot;
* &amp;lbrack;Sketchfab&amp;rbrack; La casilla &quot;Este recurso es privado&quot; no se muestra después de cambiar de cuenta
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Los ajustes preestablecidos de pincel &quot;ondulado&quot; pueden provocar problemas de rendimiento
* &amp;lbrack;Complemento Photoshop&amp;rbrack; Mensaje en el registro: no compatible con el flujo de trabajo de Mosaico de UV
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; PYTHONPATH env var impide que se inicie la aplicación
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Error tipográfico en la documentación de Python

### 6.2.1 (2020.2.1)

*(Lanzado: 29 de julio de 2020*)Resumen: **Versión secundaria, revisión**

**Agregado:**

* Añada la variable de entorno &quot;SUBSTANCE_PAINTER_VRAM_BUDGET&quot; para anular la cantidad de RVam de la GPU
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Rendimiento&amp;rbrack; No calcular todos los mosaicos UV al utilizar la herramienta Relleno poligonal

**Corregido:**

* &amp;lbrack;Iray&amp;rbrack; Guardar renderizado devuelve un error que produce una imagen en negro
* &amp;lbrack;Linux&amp;rbrack; Bloqueo después de la pantalla de bienvenida en CentOS 7.3
* &amp;lbrack;Linux&amp;rbrack; La cantidad de Vram no se detecta correctamente con configuraciones específicas
* &amp;lbrack;Bloqueo&amp;rbrack; Apertura de un proyecto con el nombre de un conjunto de texturas duplicado
* &amp;lbrack;Motor&amp;rbrack; Problema de invalidación de caché al modificar una máscara
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Efecto de fuente incorrecto cuando el conjunto de texturas está desactivado

**Problemas conocidos:**

* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; No se puede ocultar la descripción
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Problemas de IU
* &amp;lbrack;Iray&amp;rbrack; El procesamiento del PSD no se abre
* &amp;lbrack;Complemento Photoshop&amp;rbrack; No compatible con el flujo de trabajo de Mosaicos de UV

### 6.2.0 (2020.2.0)

*(Lanzado: 23 de julio de 2020*)Resumen: **Versión principal con nuevo flujo de trabajo de Mosaicos de UV, pintura entre Mosaicos de UV y mejora del rendimiento**

**Agregado:**

* Mosaicos de UV (UDIM)
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Pintura en mosaicos UV
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Permitir elegir entre el flujo de trabajo nuevo y el heredado para Mosaicos de UV
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Importación de secuencias de imágenes de UDIM/Mosaicos de UV como recurso
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Añadir lista de Mosaicos de UV por conjunto de texturas en la ventana Lista de conjuntos de texturas
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Permita editar la resolución de varios Mosaicos de UV a la vez en Configuración del conjunto de texturas
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;vista 2D&amp;rbrack; Visualización de Mosaicos de UV como una cuadrícula
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;vista 2D&amp;rbrack; Nuevo botón de ventanilla para mostrar u ocultar información de Mosaicos de UV
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Cambiar la herramienta de pintura a un solo canal de forma predeterminada para proyectos de Mosaico de UV
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Botón Nuevo en la barra de herramientas contextual para ignorar los Mosaicos de UV enmascarados mientras se pinta
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Nuevos iconos de pila de capas para mejorar el rendimiento
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Mejorar los iconos de Pintura y relleno en la barra de herramientas
* &amp;lbrack;Máscara de Mosaico de UV&amp;rbrack;&amp;lbrack;vista 2D&amp;rbrack; Permitir incluir o excluir varios Mosaicos de UV a la vez (clic izquierdo, CTRL+clic izquierdo)
* &amp;lbrack;Máscara de Mosaico de UV&amp;rbrack; Nueva máscara de Mosaico de UV para incluir, excluir azulejos por capa con un nuevo icono
* &amp;lbrack;Máscara de Mosaico de UV&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Mostrar el número de Mosaicos de UV en el icono de máscara de Mosaicos de UV cuando no se incluyen todos
* &amp;lbrack;Máscara de Mosaico de UV&amp;rbrack;&amp;lbrack;2D/Vista 3D&amp;rbrack; Añade el efecto de pasar el cursor para visualizar los Mosaicos de UV bajo el cursor
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Bakeres&amp;rbrack; Permitir seleccionar y hacer un bake Mosaicos de UV específicos
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Bakeres&amp;rbrack; Añadir opciones de selección para conjuntos de texturas/Mosaicos de UV
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Bakeres&amp;rbrack; Opción de menú del botón derecho para seleccionar Mosaicos de UV dentro de un conjunto de texturas
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Bakeres&amp;rbrack; Permitir una selección rápida en el conjunto de texturas/Mosaicos de UV arrastrando
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Bakeres&amp;rbrack; Reemplace los botones &quot;Todo&quot; y &quot;Ninguno&quot; en Mapas de malla por opciones de selección más explícitas
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Bakeres&amp;rbrack; Mostrar el número de texturas que se harán un bake
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Permitir la selección y exportación de Mosaicos de UV específicos
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Permitir una selección rápida de Mosaicos de UV arrastrando
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Añadir opciones del menú desplegable para Mosaicos de UV
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Hacer que algunos ajustes preestablecidos de exportación no estén disponibles si no funcionan con Mosaicos de UV (Adobe Dimension, Sketchfab, glTF, USD)
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Contenido&amp;rbrack; Actualice los ajustes preestablecidos de exportación para utilizar la nueva etiqueta $udim
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Mejora de los informes de errores al importar mallas con Islas de UV superpuestas
* &amp;lbrack;Mosaicos de UV&amp;rbrack; Mosaicos de UV compatibles en Irak
* &amp;lbrack;Mosaicos de UV&amp;rbrack;&amp;lbrack;Scripting&amp;rbrack; Añadir documentación de exportación de Mosaico de UV a la documentación de Python
* Rendimiento
* &amp;lbrack;Rendimiento&amp;rbrack; Botón Nuevo en la barra de herramientas contextual para pausar el cálculo del motor al trabajar (MAYÚS+ESC)
* &amp;lbrack;Rendimiento&amp;rbrack; Apertura de proyectos más rápida al retrasar el cálculo de la caché del conjunto de texturas
* &amp;lbrack;Rendimiento&amp;rbrack; No espere a que se carguen los mapas de malla al abrir el proyecto
* &amp;lbrack;Rendimiento&amp;rbrack;&amp;lbrack;2D/Vista 3D&amp;rbrack; No calcular el canal de máscara en la ventana gráfica cuando no se utiliza
* &amp;lbrack;Rendimiento&amp;rbrack; No bloquee la aplicación al cargar los mapas de malla mostrados en las ventanas gráficas
* &amp;lbrack;Rendimiento&amp;rbrack; Mejorar la velocidad de guardado incremental al guardar un proyecto
* &amp;lbrack;Rendimiento&amp;rbrack;&amp;lbrack;Bakeres&amp;rbrack; Cambiar la configuración de dilatación predeterminada para mejorar el ahorro de tiempo y el tamaño del proyecto
* &amp;lbrack;Rendimiento&amp;rbrack;&amp;lbrack;Bakeres&amp;rbrack; Cambiar a escala de grises en Bakeres específicos para mejorar el ahorro de tiempo y el tamaño del proyecto
* &amp;lbrack;Rendimiento&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Mejorar el rendimiento del motor para exportar texturas más rápido
* &amp;lbrack;Rendimiento&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Mejorar la capacidad de respuesta al abrir el cuadro de diálogo de exportación con muchos conjuntos de texturas
* &amp;lbrack;Rendimiento&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Mejorar el rendimiento al cambiar a la pestaña &quot;Lista de exportaciones&quot;
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Reducir el tiempo de arranque de Iray
* Otro
* &amp;lbrack;Bakeres&amp;rbrack; Añadir opciones de selección para conjuntos de texturas
* Mover la administración de instancias del sombreador a la configuración del conjunto de texturas
* &amp;lbrack;2D/Vista 3D&amp;rbrack; Añada un mensaje en la parte inferior de la ventana gráfica para indicar qué tipo de máscara se ha editado
* &amp;lbrack;Pila de capas&amp;rbrack; Nueva opción en la configuración para cambiar entre las miniaturas antiguas y nuevas
* &amp;lbrack;Pila de capas&amp;rbrack; Añada comentarios visuales para indicar el estado de carga de las miniaturas
* &amp;lbrack;Proj&amp;rbrack; Nuevo modo de proyección &quot;Fill (Match Per UV-Tile)&quot; para cargar secuencias de imágenes
* &amp;lbrack;Proj&amp;rbrack; Cambie el modo de proyección de capas de relleno a &quot;Rellenar (coincidencia por azulejo UV)&quot; en casos específicos
* &amp;lbrack;Contenido&amp;rbrack; Optimizar ajustes preestablecidos de pincel de carboncillo para mejorar el rendimiento
* Actualizar Iray a la versión 2020.0.0
* &amp;lbrack;Exportar&amp;rbrack; Desactivar la ficha Lista de exportaciones cuando no hay nada seleccionado
* Desempaquetado automático
* &amp;lbrack;Auto Unwrap&amp;rbrack; Mejorar la tasa de éxito del proceso de desempaquetado automático
* &amp;lbrack;Auto Unwrap&amp;rbrack; Parametrización mejorada para aumentar la velocidad y la estabilidad

**Corregido:**

* &amp;lbrack;Alembic&amp;rbrack; Las facetas se omiten al importar archivos
* &amp;lbrack;Alembic&amp;rbrack; Tiempo de carga infinito con archivos específicos
* &amp;lbrack;Importar&amp;rbrack; La secuencia de imágenes de UDIM incorrecta se importa cuando solo difiere la extensión del archivo
* &amp;lbrack;Bloqueo&amp;rbrack; Al intentar abrir un proyecto bloqueado por otro proceso, se produce un bloqueo
* &amp;lbrack;Proyección&amp;rbrack; Artefactos en malla duplicada al utilizar proyección triplanar
* &amp;lbrack;Exportar&amp;rbrack; El canal de emisivo no se exporta con USD formato
* &amp;lbrack;Contenido&amp;rbrack; Material inteligente &quot;Carboncillo&quot; contiene trazos de pintura

**Problemas conocidos:**

* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; No se puede ocultar la descripción
* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Problemas de IU

### 6.1.3 (2020.1.3)

*(Lanzado: 16 de junio de 2020*)Resumen: **Corrección de error**

**Agregado:**

* &amp;lbrack;Exportar&amp;rbrack; Agregar configuración de desplazamiento en el archivo json de parámetros de Sombreador

**Corregido:**

* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Motor&amp;rbrack; Bloqueo al intentar borrar y reemplazar canales existentes
* &amp;lbrack;Bloqueo&amp;rbrack; Cambio del sombreador después de pintar una máscara en capas de material
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Motor&amp;rbrack; Bloqueos con algunos proyectos pesados
* &amp;lbrack;Bakeres&amp;rbrack; La coincidencia por nombre no funciona con OBJ exportadas desde zBrush
* &amp;lbrack;Desplazamiento&amp;rbrack;&amp;lbrack;SVT&amp;rbrack; Las texturas no se muestran al abrir el proyecto cuando el desplazamiento está activado
* &amp;lbrack;Exportar&amp;rbrack; Algunas texturas se exportan en gris uniforme
* &amp;lbrack;Exportar&amp;rbrack; Los conjuntos de texturas desactivados no se deben exportar para los ajustes preestablecidos de exportación de Dimension y Sketchfab
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Bloqueo al utilizar la API JavaScript para acceder a la configuración de exportación en el evento onProjectOpened
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Javascript&amp;rbrack; no se llama a onExportFinished() después de una exportación

### 6.1.2 (2020.1.2)

*(Lanzado: 28 de mayo de 2020*)Resumen: **Corrección de error con Substance Engine y actualización de Bakeres**

**Agregado:**

* &amp;lbrack;Bakeres&amp;rbrack; Actualizar a la versión más reciente
* &amp;lbrack;Bakeres&amp;rbrack; Nuevo método de muestreo en bakeres de Oclusión ambiental, curvatura y Thickness
* Actualizar a la versión más reciente de Substance Engine
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir la creación de ResourceID para los recursos del proyecto
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir consultar información del canal
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Añadir funciones de ejecución en seco y devolución de llamada para simular la exportación de textura

**Corregido:**

* &amp;lbrack;Bakeres&amp;rbrack; Normales incorrectas en el baker World Space Normals utilizando un Mapa de normales tangente en casos específicos
* &amp;lbrack;Bakeres&amp;rbrack; Error al hacer un bake la Oclusión ambiental con Optix cuando no hay poli alta
* &amp;lbrack;Trazos dinámicos&amp;rbrack; Retraso al cargar un conjunto de texturas específico
* &amp;lbrack;Exportar&amp;rbrack; No se deben exportar los conjuntos de texturas desactivados para USD, glTF
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; No se puede editar la nueva configuración del baker de curvatura
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; alg.texturesets.addChannel() no devuelve un error en algunos casos
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Error tipográfico en la documentación de la API de Javascript para setProjectExportOptions()
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Exporta siempre todos los conjuntos de texturas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; sys.ejecutable devuelve una ruta de acceso a python.exe en lugar de a Substance Painter
* La caché de textura no es compatible en los sistemas operativos Mac y Windows/Linux
* &amp;lbrack;Livelink UE4&amp;rbrack; Solo se utiliza el último material para todos los conjuntos de texturas en una malla combinada

**Problemas conocidos:**

* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Dimension&amp;rbrack;&amp;lbrack;Skecthfab&amp;rbrack; No se deben exportar los conjuntos de texturas desactivados
* &amp;lbrack;Bloqueo&amp;rbrack; Cambiar el sombreador después de haber pintado una máscara en capas de material

### 6.1.1 (2020.1.1)

*(Lanzado: 5 de mayo de 2020*)Resumen: **Revisión**

**Agregado:**

* &amp;lbrack;Exportar&amp;rbrack; Comentarios visuales de estado anulado en TextureSet

**Corregido:**

* &amp;lbrack;Exportar&amp;rbrack; El tamaño de la ventana del exportador es demasiado grande en un monitor con resolución especial y no se puede cambiar de tamaño
* &amp;lbrack;Exportar&amp;rbrack; Las opciones no se guardan después de la exportación
* &amp;lbrack;Exportar&amp;rbrack; Bloqueo o no se puede exportar con el ajuste preestablecido exportar &quot;desde caché&quot;
* &amp;lbrack;Exportar&amp;rbrack; Cancelar la exportación genera un mapa vacío adicional inesperado
* &amp;lbrack;Exportar&amp;rbrack; Corregir ajustes preestablecidos de exportación virtual
* &amp;lbrack;Python&amp;rbrack; PYTHONPATH env var no se tiene en cuenta
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Si se cancela la exportación mediante Python, se devuelve un error de excepción
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; export_project_texturas resultado incorrecto con formato de archivo psd
* &amp;lbrack;Bakeres&amp;rbrack; Bloqueo en Linux con Trazado de rayos de GPU

**Problemas conocidos:**

* &amp;lbrack;JavaScript&amp;rbrack; No se puede editar la nueva configuración del baker de curvatura
* &amp;lbrack;JavaScript&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Exporta siempre todos los conjuntos de texturas
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; No se deben exportar los conjuntos de texturas desactivados
* &amp;lbrack;Bloqueo&amp;rbrack; Cambiar el sombreador después de haber pintado una máscara en capas de material

### 6.1.0 (2020.1.0)

*(Lanzado: 22 de abril de 2020*)Resumen: **Versión principal con nueva textura y exportador de malla (con desplazamiento y teselación), desempaquetado UV actualizado con más controles, nuevos bakeres, nueva API python de scripts, mejor experiencia de usuario para la proyección de pegatinas y nuevo contenido**

**Agregado:**

* Nueva textura y exportador de malla
* &amp;lbrack;Exportar&amp;rbrack; Nueva interfaz de exportador
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Permitir la selección de los canales de mapas que se exportan por conjunto de texturas
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Permitir la modificación del tamaño del conjunto de texturas para todos los conjuntos de texturas en una sola acción
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Permitir una plantilla diferente por conjunto de texturas (excepto para USD, glTF, Sketchfab y Dimension)
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Activación y desactivación rápidas de mapas y conjuntos de texturas
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; La resolución de exportación 8192x8192 ya no es experimental
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Permitir la modificación del formato de archivo y la profundidad de bits por mapa
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Permitir restablecer los valores de los parámetros predeterminados
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Permitir que la configuración se guarde sin exportar
* &amp;lbrack;Exportar&amp;rbrack;&amp;lbrack;Plantillas de salida tab&amp;rbrack; Cambie el nombre de la pestaña &quot;Configuración&quot; a la pestaña &quot;Plantillas de salida&quot;
* &amp;lbrack;Exportar&amp;rbrack;&amp;lbrack;Plantillas de salida tab&amp;rbrack; Permitir la definición del formato de archivo y la profundidad de bits por mapa preestablecido
* &amp;lbrack;Exportar&amp;rbrack;&amp;lbrack;Lista de pestañas de exportaciones&amp;rbrack; Nueva pestaña de vista previa para resumir y ver el proceso de exportación
* &amp;lbrack;Importar/Exportar malla&amp;rbrack; Optimización del rendimiento de tiempo de importación/exportación
* &amp;lbrack;Exportar malla&amp;rbrack; Exportar malla en FBX
* &amp;lbrack;Exportar malla&amp;rbrack; Exportar malla con desplazamiento y teselación
* &amp;lbrack;Exportar malla&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevos ajustes para volver a calcular el vértice normal, aplicar triangulación
* &amp;lbrack;Exportar malla&amp;rbrack; Exportar topología de malla original con nuevas UV generadas por el desajuste automático
* Se ha actualizado el desajuste automático de UV con más controles
* &amp;lbrack;Desempaquetado UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Añadir configuración para activar el desajuste automático de UV en la ventana de nuevo proyecto
* &amp;lbrack;Desempaquetado UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevas opciones para controlar los pasos de desenvolvimiento (costuras, desenvolvimiento, empaquetado)
* &amp;lbrack;Desempaquetado UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Permitir la conservación de las costuras de desenrollado/desenrollado/empaquetado existentes
* &amp;lbrack;Desempaquetado UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevas opciones para volver a calcular por completo los pasos de desajuste
* &amp;lbrack;Desempaquetado UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nueva opción para controlar el tamaño del margen (ninguno, pequeño, mediano y grande)
* Nuevos Bakeres
* &amp;lbrack;Bakeres&amp;rbrack; Sustituir la curvatura antigua por la nueva curvatura de la malla
* &amp;lbrack;Bakeres&amp;rbrack; Opción Añadir coincidencia por nombre para ignorar la cara posterior en el baker &quot;Oclusión ambiental&quot;
* &amp;lbrack;Bakeres&amp;rbrack; Opción Añadir plano de tierra en el baker &quot;Oclusión ambiental&quot;
* Nueva API de Python de scripts (3.7.6)
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevo menú de scripts para Python
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nueva documentación de Python en el menú Ayuda
* &amp;lbrack;Python&amp;rbrack; Exponga los módulos python de Substance Painter: substance_painter, alg, display, project.setting, project, texturesets, ui
* &amp;lbrack;Python&amp;rbrack; Exponer el nuevo módulo Python &quot;substance_painter&quot;
* &amp;lbrack;Python&amp;rbrack; Exponer nuevo submódulo de Python: alg, display, log, project, resource, texturesets, ui
* &amp;lbrack;Python&amp;rbrack; Listener para cambios de proyecto
* &amp;lbrack;Python&amp;rbrack; Nuevos ejemplos en la documentación de Python
* &amp;lbrack;JavaScript&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Menú de complementos reemplazado por JavaScript
* &amp;lbrack;Viewport&amp;rbrack; Permitir la creación de una proyección de pegatinas &quot;arrastrando/soltando + ALT&quot; de un recurso desde la estantería
* Nuevo contenido
* &amp;lbrack;Contenido&amp;rbrack; 5 nuevos materiales de pegatina de Substance Source
* &amp;lbrack;Contenido&amp;rbrack; Añadir nuevas plantillas de proyecto y exportar ajustes preestablecidos para el procesador de Maxwell
* &amp;lbrack;Contenido&amp;rbrack; Agregar plantilla de proyecto para la exportación de Keyshot 9
* &amp;lbrack;Contenido&amp;rbrack; Actualizar el ajuste preestablecido de exportación de Keyshot 9 para admitir desplazamiento y emisivo
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Exportador&amp;rbrack; Actualización de todos los ajustes preestablecidos de exportación para que coincidan con las últimas versiones de motores de juegos y procesadores
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Exportador&amp;rbrack; Actualice los archivos de ajustes preestablecidos de exportación para utilizar nuevos ajustes de tramado y formato
* &amp;lbrack;Contenido&amp;rbrack; Nuevas plantillas y sombreadores para admitir material de VRay (VRayMtl)
* &amp;lbrack;Pila de capas&amp;rbrack; Permitir la eliminación de efectos de capa mediante el icono de la papelera o el método abreviado del teclado Eliminar
* Eliminar el Substance Source de plugins (utilizar el iniciador con la funcionalidad &quot;enviar a&quot;)
* &amp;lbrack;Windows&amp;rbrack; No mostrar la advertencia de TDR en las GPU de gama alta

**Corregido:**

* Problemas de traducción en el cuadro de diálogo Nuevo archivo de proyecto
* &amp;lbrack;Bakeres&amp;rbrack; La opción &quot;Guardar archivo de escena preprocesado&quot; ya no funciona
* &amp;lbrack;Proyección Plana&amp;rbrack; La proyección no funciona en mallas con UV repetidos
* &amp;lbrack;Decal&amp;rbrack; Diferencia de comportamiento en el canal normal al utilizar distintos modos de proyección de la capa de relleno
* &amp;lbrack;Difuminado&amp;rbrack;&amp;lbrack;Clonar&amp;rbrack; Pueden aparecer artefactos al pintar con máscaras
* &amp;lbrack;Motor&amp;rbrack; Bloqueo con contenido de capas específico
* &amp;lbrack;Motor&amp;rbrack; Bloqueo aleatorio al pintar en algunos casos
* &amp;lbrack;Punto de ancla&amp;rbrack; La referencia a una máscara vacía siempre devuelve blanco
* &amp;lbrack;Exportar&amp;rbrack; Capa que no se tiene en cuenta en algunas configuraciones de pila concretas
* &amp;lbrack;Exportar malla&amp;rbrack; No se puede exportar con una ruta que contiene caracteres especiales
* &amp;lbrack;Exportar malla&amp;rbrack; No se pueden leer archivos glTF cuando se exportan desde Linux o MacOS
* &amp;lbrack;Importar mesh&amp;rbrack; La reimportación de DAE, PLY o glTF no funciona según lo previsto

**Problemas conocidos:**

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; No se puede editar la nueva configuración del baker de curvatura
* &amp;lbrack;Bakeres&amp;rbrack; Bloqueo en Linux con Trazado de rayos de GPU
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; No se deben exportar los conjuntos de texturas desactivados
* &amp;lbrack;Bloqueo&amp;rbrack; Cambiar el sombreador después de haber pintado una máscara en capas de material

## Versión 5

### 5.3.3 (2019.3.3)

*(Lanzado: 06 de febrero de 2020*)Resumen: **Corrección de error con actualización a Iray 2019.3**

**Agregado:**

* Actualización a Irak 2019.3
* &amp;lbrack;Registro&amp;rbrack; Indicar bios obsoletos para la CPU Ryzen que conducen al bloqueo durante el hago un bake
* &amp;lbrack;ABR&amp;rbrack; Extraer alfa ABR a la estantería

**Corregido:**

* &amp;lbrack;Baker&amp;rbrack; Hacer un bake error si la malla de alta densidad no tiene UV
* &amp;lbrack;Linux&amp;rbrack; Los métodos abreviados de ratón personalizados no se guardan
* &amp;lbrack;Brush&amp;rbrack; El contorno desaparece con algunas formas alfa
* &amp;lbrack;Tablet&amp;rbrack; Detección incorrecta al mover los reguladores
* &amp;lbrack;Atajos&amp;rbrack; No se puede configurar ningún método abreviado con &quot;Ctrl+Alt+MouseClick&quot;
* &amp;lbrack;Shelf&amp;rbrack; No se puede ver información sobre herramientas de recursos al utilizar una tableta con lápiz
* &amp;lbrack;vista 2D&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; El ajuste preestablecido de vista 2D no tiene en cuenta la información normal
* Bloqueo al pintar en alineación UV con determinados pinceles
* Pintar bajo un filtro crea artefactos en el trazo en curso
* &amp;lbrack;Viewport&amp;rbrack; Caché de textura incorrecta en la ventana gráfica después de volver a importar una malla
* &amp;lbrack;Bloqueo&amp;rbrack; Error al guardar después de exportar a Photoshop
* &amp;lbrack;Bloqueo&amp;rbrack; Escribir símbolos especiales en el prefijo al importar recursos
* &amp;lbrack;Bloqueo&amp;rbrack; Haga clic en la referencia en Propiedades del punto de ancla
* &amp;lbrack;Puntos de ancla&amp;rbrack; El canal no se actualiza cuando hay un filtro entre el punto de anclaje y la referencia
* El vínculo de la URL de Iray en el menú Ayuda no funciona

**Problemas conocidos:**

* &amp;lbrack;Desempaquetado UV&amp;rbrack; El procesamiento de mallas de alta polietileno puede tardar mucho tiempo
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Los vértices en las mismas coordenadas exactas se combinan
* &amp;lbrack;Desempaquetado UV&amp;rbrack; La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Proporción de texel no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Proporción de textura no uniforme entre conjuntos de texturas
* &amp;lbrack;Desempaquetado UV&amp;rbrack; La isla de UV generada puede ser muy alargada y no encajar en el espacio UV en algunos casos
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Es posible que las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no se desenvuelvan con UV

### 5.3.2 (2019.3.2)

*(Lanzado: 21 de enero de 2020*)Resumen: **Corrección de error**

**Corregido:**

* Al abrir un proyecto guardado en el modo de canal solo, no se muestra la malla
* La ventana gráfica no siempre se actualiza al pintar en una capa con la herramienta de clonación

**Problemas conocidos:**

* &amp;lbrack;Bakeres&amp;rbrack; Bloqueo relacionado con el subprocesamiento múltiple en CPU Ryzen
* &amp;lbrack;Desempaquetado UV&amp;rbrack; El procesamiento de mallas de alta polietileno puede tardar mucho tiempo
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Los vértices en las mismas coordenadas exactas se combinan
* &amp;lbrack;Desempaquetado UV&amp;rbrack; La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Proporción de texel no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Proporción de textura no uniforme entre conjuntos de texturas
* &amp;lbrack;Desempaquetado UV&amp;rbrack; La isla de UV generada puede ser muy alargada y no encajar en el espacio UV en algunos casos
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Es posible que las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no se desenvuelvan con UV

### 5.3.1 (2019.3.1)

*(Lanzado: 20 de diciembre de 2019*)Resumen: **Revisión**

**Corregido:**

* Bloqueo al trabajar en mallas con Proyecciones de UV específicas
* &amp;lbrack;ABR&amp;rbrack; Bloqueo al cambiar entre ajustes preestablecidos de Photoshop
* &amp;lbrack;Linux&amp;rbrack; No se puede iniciar el Substance Painter en CentOS 7.4 debido a un problema de dependencia de libGLX
* &amp;lbrack;Bakeres&amp;rbrack; Bloqueo al hacer un bake después de utilizar Archivo > Limpiar
* &amp;lbrack;Bakeres&amp;rbrack; Hacer un bake el cuadro de diálogo de progreso inmovilizar después de cancelar
* &amp;lbrack;Bakeres&amp;rbrack; Hacer un bake malla después de exportar texturas no funciona
* &amp;lbrack;Bakeres&amp;rbrack; El uso de resultados &quot;Coincidir por nombre&quot; con mapas de malla negros
* &amp;lbrack;Bakeres&amp;rbrack; La jaula no se tiene en cuenta
* &amp;lbrack;Shelf&amp;rbrack; La importación de archivos de PSD genera imágenes rotas
* &amp;lbrack;Ejemplo&amp;rbrack; El proyecto de muestra &quot;Mat&quot; tiene cámaras rotas y un ajuste preestablecido de exportación incorrecto

**Problemas conocidos:**

* &amp;lbrack;Bakeres&amp;rbrack; Bloqueo relacionado con el subprocesamiento múltiple en CPU Ryzen
* &amp;lbrack;Desempaquetado UV&amp;rbrack; El procesamiento de mallas de alta polietileno puede tardar mucho tiempo
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Los vértices en las mismas coordenadas exactas se combinan
* &amp;lbrack;Desempaquetado UV&amp;rbrack; La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Proporción de texel no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Proporción de textura no uniforme entre conjuntos de texturas
* &amp;lbrack;Desempaquetado UV&amp;rbrack; La isla de UV generada puede ser muy alargada y no encajar en el espacio UV en algunos casos
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Es posible que las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no se desenvuelvan con UV

### 5.3.0 (2019.3.0)

*(Lanzado: 17 de diciembre de 2019*)Resumen: **Versión principal con mejora de la experiencia del usuario al pintar a mano, trabajar con tabletas, desempaquetado automático de UV en versión beta (0.3.0) y nuevo contenido diverso para pintar a mano**

**Agregado:**

* Integrar la versión 0.3.0 del desempaquetado automático de UV en Substance Painter
* &amp;lbrack;desempaquetado UV&amp;rbrack; Desempaquetado automático de UV en el Substance Painter cuando no hay UV o UV parciales
* &amp;lbrack;desempaquetado UV&amp;rbrack; Una configuración global para activarla y desactivarla
* &amp;lbrack;desempaquetado UV&amp;rbrack; Versión registrada en el archivo de registro
* &amp;lbrack;desempaquetado UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Indicar progreso de desajuste de UV
* &amp;lbrack;UI&amp;rbrack; Nuevos ajustes en la barra de herramientas contextual para seleccionar la vista previa del pincel: Vista previa completa, contorno de pincel y forma de cruz
* &amp;lbrack;Herramienta&amp;rbrack; Nuevo modo de fusión avanzado en la sección alfa: Aclarar (máxima) además de Normal
* &amp;lbrack;Pila de capas&amp;rbrack; Opción de corrección de gamma por capa para alfa o máscara (menú del botón derecho)
* &amp;lbrack;Pila de capas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Añada el icono &quot;i&quot; cuando se corrija la gamma de una capa alfa
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;Herramienta&amp;rbrack; Exponer presión mínima para tamaño y flujo
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevo ajuste en la barra de herramientas contextual para seleccionar la presión de curva: lineal, fácil de entrar, fácil de salir
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Agregar Ctrl+Alt+clic para desplazarse
* Importar ajustes preestablecidos de pincel de Photoshop (formato ABR)
* &amp;lbrack;ABR&amp;rbrack; Admitir parámetros de forma
* &amp;lbrack;ABR&amp;rbrack; Compatibilidad con parámetros de dinámica de forma
* &amp;lbrack;ABR&amp;rbrack; Parámetros de transferencia de soporte
* &amp;lbrack;ABR&amp;rbrack; Compatibilidad con parámetros de dispersión
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Trazos dinámicos&amp;rbrack; Compatibilidad con redondez y volteo
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Exponer la estructura de carpetas del pincel en el Editor de filtros
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Añadir icono de Photoshop en miniaturas
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Añada una lista de parámetros no compatibles en la miniatura detallada de ABR
* &amp;lbrack;Herramienta&amp;rbrack;&amp;lbrack;Trazos dinámicos&amp;rbrack; Nuevo ajuste de trazo dinámico para controlar cuántas semillas aleatorias se van a generar
* &amp;lbrack;Herramienta&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Añadir nueva configuración de distribución y eje para la variación de dispersión
* &amp;lbrack;Método abreviado&amp;rbrack; Agregue Ctrl+Mayús+B para abrir la ventana de Hacer un bake
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Menú&amp;rbrack; Añada la entrada en el menú &quot;Editar&quot; para abrir la ventana de Haga un bake
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Settings&amp;rbrack; Mejora de la alineación de la lista de métodos abreviados
* &amp;lbrack;UI&amp;rbrack; Sustitución de los iconos de los controles de presión (tamaño y flujo) por botones de encendido/apagado
* &amp;lbrack;Viewport&amp;rbrack; Permitir enfocar la ventana gráfica 2D y 3D por separado
* Actualización a QT 5.12.5
* &amp;lbrack;UI&amp;rbrack; Indicar el progreso de carga de malla
* &amp;lbrack;Substance&amp;rbrack; Añade compatibilidad con rangos suaves y sin sujeción con reguladores
* &amp;lbrack;Substance&amp;rbrack; Aumentar la precisión de los parámetros del Substance hasta 6 decimales
* &amp;lbrack;Substance&amp;rbrack; Tenga en cuenta el paso definido por un parámetro
* &amp;lbrack;Substance&amp;rbrack; Optimizar la generación de trazos dinámicos con compatibilidad con condiciones en los datos de usuario
* &amp;lbrack;Substance&amp;rbrack; Permite designar una salida de gráfico como una máscara para todos los canales a través de los datos de usuario
* &amp;lbrack;Contenido&amp;rbrack; Actualizar proyecto de muestra &quot;Mat&quot; con topología compatible con desplazamientos, nuevo mapa de ID y nuevas cámaras
* &amp;lbrack;Contenido&amp;rbrack; Integrar 3 filtros nuevos (MatFx): Comic Book, Acuarela, Pintura al óleo (inspirado en la obra de Emrecan Cubukcu)
* &amp;lbrack;Contenido&amp;rbrack; Integrar 102 ajustes preestablecidos de pincel de Photoshop de los paquetes de Kyle T. Webster
* &amp;lbrack;Contenido&amp;rbrack; Integrar 18 nuevos ajustes preestablecidos de pincel: Flecha de rodillo de pintura, texto de advertencia de rodillo de Pintura, carboncillo fino y más
* &amp;lbrack;Contenido&amp;rbrack; Integrar 9 nuevas alfas: Rodillo de Pintura del creador de pinceles, Photoshop del creador de pinceles, patrones de pinceles y mucho más
* &amp;lbrack;Contenido&amp;rbrack; Integrar 2 nuevos ajustes preestablecidos de herramientas: Gouache denso y Gouache descolorido
* &amp;lbrack;Contenido&amp;rbrack; Integrar 1 nuevo generador: Comprobador UV (Islas de UV de realce y costuras)
* &amp;lbrack;Contenido&amp;rbrack; Integrar 2 nuevos ajustes preestablecidos de exportación: Keyshot 9+ y Spark AR Studio
* &amp;lbrack;Contenido&amp;rbrack; Integrar 1 nueva plantilla de proyecto : Spark AR Studio (Facebook)

**Corregido:**

* &amp;lbrack;Tablet&amp;rbrack; Deshacer trazos de puntero (Ctrl+Z) retrasa más que deshacer trazos del ratón
* &amp;lbrack;Tablet&amp;rbrack; Presión de inicio y fin no tenida en cuenta al trazar una línea recta
* &amp;lbrack;Tablet&amp;rbrack; El primer sello se dibuja dos veces al utilizar una línea recta
* &amp;lbrack;Tablet&amp;rbrack; Mejorar la compatibilidad con los métodos abreviados de la tableta Huion
* &amp;lbrack;Tablet&amp;rbrack; Mejorar la compatibilidad con los botones del lápiz de Huion
* &amp;lbrack;Tablet&amp;rbrack; Desplazamiento entre la vista previa del pincel y el sello dibujado
* &amp;lbrack;Tablet&amp;rbrack; Los métodos abreviados para modificar pinceles con lápiz suelen dar lugar a un rendimiento bajo en casos excepcionales
* &amp;lbrack;Tablet&amp;rbrack; Retraso al pintar en una capa específica
* En raras ocasiones, pueden producirse texturas borrosas al cambiar la ventanilla
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Las entradas de imagen no siempre se muestran
* Limpiar no elimina los ajustes preestablecidos del estante que se hayan importado en un proyecto
* &amp;lbrack;Herramienta&amp;rbrack;&amp;lbrack;Trazo dinámico&amp;rbrack; Problema de rendimiento al ajustar el recuento cíclico de sello
* Problemas de actualización al pintar en modo de ventanilla 3D/2D en casos excepcionales
* Pintar un trazo muy largo puede provocar un congelamiento
* &amp;lbrack;Herramienta&amp;rbrack; Problema de rendimiento al pintar con trazos dinámicos específicos
* &amp;lbrack;UI&amp;rbrack; La barra de herramientas contextual sigue mostrando las propiedades del pincel al seleccionar una carpeta
* Los valores del eje de simetría no se restablecen
* La importación de texturas EXR con valores de coma flotante es totalmente negra
* Pulsar Alt+clic en un canal para aislar no funciona para el filtro y el generador
* &amp;lbrack;Exportar&amp;rbrack; Bloqueos específicos del proyecto en la exportación
* &amp;lbrack;Substance&amp;rbrack; Valor predeterminado incorrecto en el menú desplegable si el parámetro está oculto por Visible If
* &amp;lbrack;Sombreador&amp;rbrack; Los canales definidos mediante Material Layering no se ordenan del mismo modo en la interfaz de usuario
* &amp;lbrack;Shelf&amp;rbrack; Los metadatos de ajustes preestablecidos no se guardan en el disco

**Problemas conocidos:**

* &amp;lbrack;Desempaquetado UV&amp;rbrack; El procesamiento de mallas de alta polietileno puede tardar mucho tiempo
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Los vértices en las mismas coordenadas exactas se combinan
* &amp;lbrack;Desempaquetado UV&amp;rbrack; La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Proporción de texel no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Proporción de textura no uniforme entre conjuntos de texturas
* &amp;lbrack;Desempaquetado UV&amp;rbrack; La isla de UV generada puede ser muy alargada y no encajar en el espacio UV en algunos casos
* &amp;lbrack;Desempaquetado UV&amp;rbrack; Es posible que las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no se desenvuelvan con UV
* El ejemplo de reunión tiene algunos problemas con cámaras importadas

### 5.2.3 (2019.2.3)

*(Lanzado: 23 de octubre de 2019*)Resumen: **Versión de corrección de errores**

**Agregado:**

* &amp;lbrack;Lista de conjuntos de texturas&amp;rbrack; Botón Añadir para activar o desactivar rápidamente el modo de enfoque
* &amp;lbrack;Registro&amp;rbrack; Añadir el número de versión de Windows 10 en el archivo de registro
* Actualizar a la versión más reciente de Substance Engine
* &amp;lbrack;MacOS&amp;rbrack; Se ha certificado el software para seguir los nuevos requisitos de distribución de MacOS Catalina

**Corregido:**

* &amp;lbrack;Complemento&amp;rbrack; El complemento de origen no funciona
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Sombreador&amp;rbrack; Mac OS 10.14.5 y AMD: la colocación de los materiales en capas no funciona como se pretende

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.2 (2019.2.2)

*(Lanzado: 20 de septiembre de 2019*)Resumen: **Versión de corrección de errores**

**Corregido:**

* La importación de recursos mediante secuencias de comandos puede provocar un bloqueo
* &amp;lbrack;Complemento&amp;rbrack; Descargar material desde el origen puede provocar un bloqueo

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.1 (2019.2.1)

*(Lanzado: 17 de septiembre de 2019*)Resumen: **Versión de corrección de errores**

**Corregido:**

* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Los archivos USDZ exportados de MacOS no se pueden abrir
* &amp;lbrack;Conjunto de texturas&amp;rbrack; No es posible aislar un conjunto de texturas con el modificador ALT
* &amp;lbrack;Shelf&amp;rbrack; Los ajustes preestablecidos, Materiales inteligentes y Máscaras inteligentes siempre se modifican al salir de la aplicación
* &amp;lbrack;Pila de capas&amp;rbrack; No se puede seleccionar el efecto después de eliminar otro efecto
* Parpadeo al utilizar un regulador dentro del panel de propiedades de la herramienta
* Bloqueo al exportar ajustes preestablecidos a la estantería
* Bloqueo al exportar un ajuste preestablecido con espacio insuficiente
* Bloqueo al crear un ajuste preestablecido con espacio insuficiente

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.0 (2019.2.0)

*(Lanzado: 25 de julio de 2019*)Resumen: **Versión principal con actualizaciones de los bakeres en términos de rendimiento y un nuevo modo de previsualización + nuevo contenido**

**Agregado:**

* &amp;lbrack;Bakeres&amp;rbrack; Se ha agregado compatibilidad para Trazado de rayos de GPU con DXR y OptiX (Oclusión ambiental, Thickness)
* &amp;lbrack;Bakeres&amp;rbrack; Optimizaciones y aceleraciones para el Trazado de rayos de CPU
* &amp;lbrack;Bakeres&amp;rbrack;&amp;lbrack;Modo Vis&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevo modo de visualización de hace un bake en la ventana gráfica
* &amp;lbrack;Bakeres&amp;rbrack;&amp;lbrack;Preferences&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nueva opción de hacer un bake para activar y desactivar el Trazado de rayos de GPU
* &amp;lbrack;Bakeres&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Repaso del cuadro de diálogo de la barra de progreso
* &amp;lbrack;Bakeres&amp;rbrack; Mejora de los mensajes de advertencia y error
* &amp;lbrack;Bakeres&amp;rbrack; Permitir una cancelación más receptiva del proceso de hacer un bake
* &amp;lbrack;Bakeres&amp;rbrack; Volver a abrir la ventana hacer un bake después de hacer clic en Cancelar
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Mejora de la usabilidad del manipulador de rotación
* &amp;lbrack;Configuración&amp;rbrack; Opción para mejorar el rendimiento mediante la reducción de la resolución de la ventanilla para pantallas HDPI
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Cambiar la resolución del conjunto de texturas
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Obtener conjunto de texturas seleccionado
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir al usuario seleccionar un conjunto de texturas
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Función para saber cuándo se ha cambiado la selección del conjunto de texturas
* &amp;lbrack;Shelf&amp;rbrack; Se han añadido 40 nuevos materiales inteligentes
* &amp;lbrack;Shelf&amp;rbrack; Se han añadido 20 máscaras inteligentes nuevas

**Corregido:**

* &amp;lbrack;Pila de capas&amp;rbrack; Bloqueo de la interfaz de usuario al seleccionar varias capas
* &amp;lbrack;Pila de capas&amp;rbrack; Agrupar muchas capas bloquea la interfaz de usuario más tiempo de lo habitual
* &amp;lbrack;Pila de capas&amp;rbrack; En algunos casos, se pueden seleccionar una capa y un efecto al mismo tiempo
* Los gráficos de Substance utilizados dentro de las herramientas de pintura no se generan con la resolución adecuada
* &amp;lbrack;Baker&amp;rbrack; El botón &quot;Hacer un bake todos los conjuntos de texturas&quot; no se desactiva si no se selecciona ningún baker
* &amp;lbrack;MacOS&amp;rbrack; Desactivar el mensaje de advertencia sobre teselación
* La herramienta Proyección no tiene previsualización cuando se utiliza con una máscara
* Bloqueos y proyectos dañados al intentar ahorrar con espacio en disco insuficiente
* &amp;lbrack;Shelf&amp;rbrack; Bloqueo al importar un recurso a través de la estantería con espacio insuficiente
* &amp;lbrack;Shelf&amp;rbrack; Bloqueo al restaurar el ajuste preestablecido de sesión
* &amp;lbrack;Shelf&amp;rbrack; Importar un ajuste preestablecido con un nombre que termine con un espacio provoca un bloqueo
* &amp;lbrack;Shelf&amp;rbrack; Importar un recurso con un prefijo que termina en un espacio vacío genera un bloqueo

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.1.3 (2019.1.3)

*(Lanzado: 01 de julio de 2019*)Resumen: **Corrección de error con 2 nuevas características**

**Agregado:**

* Permite especificar el presupuesto de VRam con una línea de comandos (p. ej. —vram-budget 4096)
* &amp;lbrack;QML&amp;rbrack; Exponer las propiedades wrapMode y elide de los botones QML y las casillas de verificación

**Corregido:**

* &quot;Seguir ruta&quot; no funciona todo el tiempo
* La asignación de canales no funciona con SBSAR utilizado en ranuras de un solo canal
* &amp;lbrack;Pila de capas&amp;rbrack; Bajo rendimiento al desplazarse con capas ocultas
* &amp;lbrack;TextureSet&amp;rbrack; Bloqueo al hacer clic entre máscaras
* &amp;lbrack;SVT&amp;rbrack; El desplazamiento no se muestra correctamente y parpadea en algunos casos
* &amp;lbrack;Alembic&amp;rbrack; Bloqueo con malla usando normales de punto en lugar de normales de vértice
* &amp;lbrack;Alembic&amp;rbrack;&amp;lbrack;Log&amp;rbrack; Informar de un error en el registro si no se admite el archivo Alembic durante la importación

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic

### 5.1.2 (2019.1.2)

*(Lanzado: 21 de mayo de 2019*)Resumen: **Revisión**

**Corregido:**

* Bloqueo al seleccionar dos recursos con una entrada de imagen

### 5.1.1 (2019.1.1)

*(Lanzado: 20 de mayo de 2019*)Resumen: **Revisión**

**Agregado:**

* Actualización a la versión más reciente de Substance Engine con la última versión de Substance Designer 2019.1

**Corregido:**

* &amp;lbrack;Substance&amp;rbrack; Visible Si no se tiene en cuenta para las imágenes de entrada
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Motor&amp;rbrack; El cambio de la resolución del conjunto de texturas provoca un bloqueo en algunos casos
* &amp;lbrack;Motor&amp;rbrack; En algunos casos aparecen texturas negras aleatorias
* &amp;lbrack;Pila de capas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Al alternar una máscara con MAYÚS, se pueden seleccionar varias capas al mismo tiempo
* &amp;lbrack;Pila de capas&amp;rbrack; La opacidad no afecta al efecto de Pintura con el modo de fusión PassThrough
* &amp;lbrack;Pila de capas&amp;rbrack; La entrada de height a filtro normal no se actualiza correctamente con el trazo del pincel del borrador
* &amp;lbrack;LayersStack&amp;rbrack; Bloqueo al deshacer la caída de una máscara inteligente
* Malla metálica parpadeando con sombras y anti-aliasing temporal activado
* &amp;lbrack;Desplazamiento&amp;rbrack; Retraso en AMD con algunas mallas pesadas
* &amp;lbrack;Windows&amp;rbrack; Bloqueo al abrir algunos proyectos mediante el explorador de archivos
* &amp;lbrack;Histograma&amp;rbrack; Bloqueo al eliminar la máscara con el punto de anclaje en algunos casos
* Bloqueo en la generación de vistas previas en algunos casos raros
* &amp;lbrack;Bloqueo&amp;rbrack; No se puede volver a abrir un proyecto con demasiadas herramientas de clonación y difuminado
* No se muestra ninguna malla en el modo de material después de guardarla en algunos casos
* &amp;lbrack;Secuencias de comandos&amp;rbrack; alg.mapexport.documentStructure() devuelve valores incorrectos para carpetas

**Problemas conocidos:**

* Al hacer doble clic en el nombre del conjunto de texturas, se seleccionará antes de entrar en el modo de cambio de nombre

### 5.1.0 (2019.1.0)

*(Lanzado: 23 de abril de 2019*)Resumen: **Trazo dinámico con nuevo contenido, Desplazamiento y teselación en tiempo real e Iray, efecto Máscara de comparación, simetría radial, Plano y Proyección esférica**

**Agregado:**

* &amp;lbrack;Herramienta&amp;rbrack; Trazo dinámico: Variación Substance junto a un trazo de pincel
* &amp;lbrack;Trazo dinámico&amp;rbrack; Exponer nuevo parámetro de índice de sello con opciones
* &amp;lbrack;Trazo dinámico&amp;rbrack; Tenga en cuenta el parámetro $time
* &amp;lbrack;Trazo dinámico&amp;rbrack; Generar nuevo parámetro $randomseed por trazo y por sello
* &amp;lbrack;Trazo dinámico&amp;rbrack; Iniciar un índice de trazo dinámico desde un número aleatorio
* &amp;lbrack;Trazo dinámico&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Ayuda para encontrar un recurso de trazo dinámico con un icono nuevo dedicado
* Desplazamiento y teselación en la ventana gráfica en tiempo real
* Desplazamiento y teselado en Iray
* &amp;lbrack;configuración de Sombreador&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nueva pestaña para controlar el desplazamiento y la teselación
* &amp;lbrack;Pila de capas&amp;rbrack; Nuevo efecto CompararMáscara: generar una máscara comparando dos canales
* &amp;lbrack;Pila de capas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nueva entrada en el menú contextual &quot;Añadir máscara con combinación de height&quot; para insertar un efecto Comparar máscara
* &amp;lbrack;Simetría&amp;rbrack; Nuevo modo de simetría: pintura radial
* &amp;lbrack;configuración de Simetría&amp;rbrack; Expanda ambas secciones &quot;Configuración&quot; y &quot;Pantalla&quot;
* &amp;lbrack;configuración de Simetría&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Vista previa para pintura radial
* Exponga dos nuevos modos de proyección: plano y esférico
* &amp;lbrack;Proj&amp;rbrack; Nuevo modo de recorte de forma para todas las proyecciones
* &amp;lbrack;Proj&amp;rbrack; Modo plano con nuevo manipulador: Herramienta Superficie
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;Método abreviado&amp;rbrack; Método abreviado MAYÚS+W para la herramienta Superficie
* &amp;lbrack;Proj&amp;rbrack; Enmascaramiento de proyección plana con selección de profundidad y sacrificio de la cara posterior
* &amp;lbrack;Manipulador&amp;rbrack; Mejora del manipulador de rotación en los tres ejes para triplanar
* &amp;lbrack;Herramienta&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Al pulsar Alt y hacer clic en un canal, se selecciona ese canal (lo activa o desactiva todos los demás)
* &amp;lbrack;Motor&amp;rbrack; Actualizar a la versión más reciente de Substance Engine
* &amp;lbrack;Conjunto de texturas&amp;rbrack; Selección múltiple y cambio de resolución
* &amp;lbrack;Conjunto de texturas&amp;rbrack; Activación y desactivación rápidas de los conjuntos de texturas
* &amp;lbrack;Conjunto de texturas&amp;rbrack; Combinar solo y todas las opciones en un nuevo menú
* &amp;lbrack;Conjunto de texturas&amp;rbrack;&amp;lbrack;Pila de capas&amp;rbrack; Nuevo icono para la activación y desactivación
* &amp;lbrack;Pila de capas&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Inserta efectos por encima de los que ya están seleccionados
* &amp;lbrack;Pila de capas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Estilo de selección de vista de pila de capas de retrabajo
* &amp;lbrack;Pila de capas&amp;rbrack; El modo de fusión para capas con instancias ahora está en modo Pass Through de forma predeterminada
* &amp;lbrack;Exportar&amp;rbrack; Opción para activar y desactivar el tramado
* &amp;lbrack;Complemento&amp;rbrack; Modificador de precisión de soporte para reguladores (MAYÚS)
* &amp;lbrack;Complemento&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevo icono para autoguardar
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Mostrar el contenido de una carpeta
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir la eliminación de archivos
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Leer toda la información de la pila, incluidos los recursos utilizados
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Dynamic stroke&amp;brack; Nuevas herramientas y ajustes preestablecidos de pincel
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Dynamic stroke&amp;brack; Dos nuevos degradados procedimientos: Tono de degradado y Generador de degradado
* &amp;lbrack;Contenido&amp;rbrack; 11 nuevos filtros: Pintura de pelado MatFx, gotas de agua MatFx y más
* &amp;lbrack;Contenido&amp;rbrack; 7 nuevos generadores: Stitcher automático, UV Random Color, UV Texel Density y más
* &amp;lbrack;Contenido&amp;rbrack; 93 alfas nuevas: nuevos textos, flechas y otras formas
* &amp;lbrack;Contenido&amp;rbrack; 2 nuevos procedimientos: Tono de degradado, Generador de degradados y mucho más
* &amp;lbrack;Contenido&amp;rbrack; 21 nuevos ajustes preestablecidos de herramienta y pincel para Trazos dinámicos : Guijarros, Huellas, Spray y más
* &amp;lbrack;Contenido&amp;rbrack; 2 Nuevos HDR: Canopus Ground y Autumn Forest
* &amp;lbrack;Contenido&amp;rbrack; Actualizar el contenido con la selección aleatoria de semillas en el estante
* &amp;lbrack;Contenido&amp;rbrack; Nuevo icono con parámetro de semilla aleatoria expuesto en la estantería

**Corregido:**

* &amp;lbrack;Pila de capas&amp;rbrack; La pila de capas sigue arrastrando para siempre
* &amp;lbrack;Mac&amp;rbrack; &quot;Mostrar en Finder&quot; puede provocar la congelación
* &amp;lbrack;Secuencias de comandos&amp;rbrack; La configuración guardada mediante la interfaz de usuario personalizada se pierde si se mueve el archivo de sombreador
* &amp;lbrack;Secuencias de comandos&amp;rbrack; El número de versión de la API es incorrecto y no está actualizado
* &amp;lbrack;Efecto&amp;rbrack; El contenido del histograma no se muestra correctamente
* &amp;lbrack;Efecto&amp;rbrack; El efecto del histograma no se actualiza en algunos casos
* &amp;lbrack;Shelf&amp;rbrack; Los puntos no están correctamente alineados en el material &quot;Pirámide de tela de plástico&quot;

**Problemas conocidos:**

* Al hacer doble clic en el nombre del conjunto de texturas, se seleccionará antes de entrar en el modo de cambio de nombre
* &amp;lbrack;Pila de capas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Al alternar una máscara con MAYÚS, se pueden seleccionar varias capas al mismo tiempo

## Versión 4

### 4.3.3 (2018.3.3)

*(Lanzado: 7 de marzo de 2019*)Resumen: **corrección de errores**

**Agregado:**

* &amp;lbrack;Contenido&amp;rbrack; Integrar nueva plantilla de proyecto: &quot;PBR - Rugosidad metálica Alpha-blend&quot;
* El orden de búsqueda de la biblioteca dinámica de Linux ha cambiado para priorizar las bibliotecas en el directorio de instalación antes de lo que está instalado en el sistema

**Corregido:**

* La malla desaparece a veces de la ventana gráfica 3D (presione F para restablecer la cámara)
* Actualizar el cargador de Substance Painter de Sketchfab con los nuevos tipos de licencia de Sketchfab
* &amp;lbrack;Import&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; Control incorrecto de la modulación de la textura de entrada como se define en los archivos glTF
* &amp;lbrack;Import&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; El plano de tierra se muestra incorrectamente con la importación glTF en algunos casos
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; La opacidad no funciona en Arkit
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; BLOQUEOS de exportación de USDz en algunos casos
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exportar a USD sin guardar los posibles clientes en el bloqueo
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Modo de mosaico incorrecto para texturas, modo de subdivisión para mallas y tipos de salida para sombreadores
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exportaciones dispersas de solo algunos conjuntos de texturas con toda la geometría
* &amp;lbrack;Instancia&amp;rbrack; Bloqueo al intentar eliminar una capa de instancia rota
* &amp;lbrack;Regresión&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Algunos mapas no se exportan en la profundidad de bits elegida
* &amp;lbrack;Linux&amp;rbrack; Problema con library libtbb.so.2

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.3.2 (2018.3.2)

*(Lanzado: 24 de enero de 2019*)Resumen: **Revisión con nuevas características (exportación USDZ y filtrado de Texturas en el puerto de visualización)**

**Agregado:**

* &amp;lbrack;Exportar&amp;rbrack; Permitir exportación a USDZ
* &amp;lbrack;Viewport&amp;rbrack; Permita controlar la calidad de la textura en los Ajustes de visualización
* &amp;lbrack;Viewport&amp;rbrack; Se ha añadido el ajuste de sesgo mip en Ajustes de visualización
* &amp;lbrack;Viewport&amp;rbrack; Se ha añadido un filtrado anisotrópico en Configuración de visualización
* &amp;lbrack;plugins&amp;rbrack; Actualizar los complementos oficiales para usar el estilo de Substance Painter 2018
* &amp;lbrack;Licencia&amp;rbrack; Instalar la licencia de forma predeterminada en una carpeta de usuario

**Corregido:**

* Bloqueo vinculado a la descompresión
* Añadir TAA en material solo
* Ruido con sombra, TAA y sombreador de prueba alfa con tramado
* Eliminar el tramado de specular para todos los sombreadores PBR clásicos
* Bloqueo en la configuración del sombreador en algunos casos
* La activación de la dispersión no está sincronizada entre los procesamientos de OpenGL e Iray
* Las herramientas de difuminado y clonación ya no funcionan en mallas específicas
* Algunos conjuntos de texturas no pueden aparecer en el procesamiento de Iray
* Los conjuntos de texturas renombrados no se guardan después de cerrar el proyecto
* Artefactos de malla metálica al arrastrar y soltar materiales en mapas de ID
* &amp;lbrack;Secuencias de comandos&amp;rbrack; La creación de la ruta de archivo no se fuerza al guardar un proyecto
* &amp;lbrack;Secuencias de comandos&amp;rbrack; La devolución de llamada &quot;onProjectAboutToSave()&quot; ya no funciona
* Vínculos de foro rotos en la ventana de informe de errores

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.3.1 (2018.3.1)

*(Lanzado: 06 de diciembre de 2018*)Resumen: **Revisión**

**Agregado:**

* &amp;lbrack;Simetría&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; La simetría pintada en la Vista 2D ha vuelto y ahora presenta una vista previa del pincel clónico corregida

**Corregido:**

* &amp;lbrack;Exportar&amp;rbrack; La exportación de vista 2D genera una textura negra en algunos casos
* &amp;lbrack;Iray&amp;rbrack; La información normal se vuelve incorrecta en Iray después de crear instancias de una capa de material
* Los conjuntos de texturas no cuadrados pueden provocar en algunos casos bloqueos
* &amp;lbrack;Deshacer&amp;rbrack; Varias teclas Ctrl+Z pueden llevar aleatoriamente en algunos casos al bloqueo
* &amp;lbrack;QML&amp;rbrack; AlgScrollView puede crear una advertencia en el registro en algunos casos (bucles de enlace)

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows
* El suavizado y las sombras cuando están activos juntos pueden dar resultados inesperados

### 4.3.0 (2018.3.0)

*(Lanzado: 20 de noviembre de 2018*)Resumen: **Actualizaciones de la ventana gráfica, exportación adecuada de Vista 2D, nuevos ayudantes de interfaz de usuario, una herramienta de simetría mejorada, nuevo contenido y un gran aumento en el rendimiento**

**Agregado:**

* &amp;lbrack;Suavizado&amp;rbrack;&amp;lbrack;Ventana&amp;rbrack; Nuevo filtrado de suavizado temporal para la ventana gráfica 3D (mediante Configuración de visualización)
* &amp;lbrack;Exportar&amp;rbrack; Exportar el contenido de la ventana gráfica 2D como una sola textura
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Tramado&amp;rbrack; Mostrar tramado en la exportación
* &amp;lbrack;Pila de capas&amp;rbrack; Colores en capas y carpetas
* &amp;lbrack;Pila de capas&amp;rbrack; Activación y desactivación rápidas de varias capas y efectos
* &amp;lbrack;Pila de capas&amp;rbrack; Navegación más sencilla para los modos de fusión con las teclas de flecha arriba y desplazamiento del ratón
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Manipulador de rotación adicional en los tres ejes para triplanar
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;Accesos directos&amp;rbrack; - y + para cambiar el tamaño del manipulador de Proyección de UV
* &amp;lbrack;Sombreador&amp;rbrack; Controlar los parámetros de las capas recubiertas con canales en el sombreador recubierto de PBR
* &amp;lbrack;Substance&amp;rbrack; Exponer nuevas entradas de textura basadas en malla para filtros y generadores
* &amp;lbrack;Simetría&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Control del desplazamiento de simetría con manipuladores
* &amp;lbrack;Simetría&amp;rbrack;&amp;lbrack;Barra de herramientas contextual&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nuevo panel simetría con opciones
* &amp;lbrack;Simetría&amp;rbrack; Nuevo modo de intersección de línea de simetría
* &amp;lbrack;Simetría&amp;rbrack; Nuevo cursor de clonación de simetría
* &amp;lbrack;Simetría&amp;rbrack;&amp;lbrack;Atajos&amp;rbrack; Q para ocultar y -, + para cambiar el tamaño y cambiar para ajustar
* &amp;lbrack;Registro&amp;rbrack; Mejore los mensajes de error cuando no se pueden exportar texturas
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir cambiar o actualizar los recursos en Configuración de visualización
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir la creación o eliminación de canales en conjuntos de texturas
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shaders&amp;brack; Añada compatibilidad con la anisotropía con un sombreador específico (pbr-metal-rough-anisotropía-angle)
* &amp;lbrack;Contenido&amp;rbrack; Actualización de la esfera de previsualización con la anisotropía y el ángulo modificado
* &amp;lbrack;Contenido&amp;rbrack; Línea de obturación matFx actualizada
* &amp;lbrack;Contenido&amp;rbrack; Nueva digitalización de caras sin problemas Texturing.XYZ
* &amp;lbrack;Contenido&amp;rbrack; Nuevos procedimientos anisotrópicos
* &amp;lbrack;Contenido&amp;rbrack; Nuevo filtro: entorno de iluminación generado
* &amp;lbrack;Contenido&amp;rbrack; Nuevo mapa de entorno: studio automotive neutral
* &amp;lbrack;Contenido&amp;rbrack; Nueva plantilla de proyecto: PBR - Ángulo de anisotropía de rugosidad metálica (con canales de anisotropía)
* &amp;lbrack;Contenido&amp;rbrack; Nueva plantilla de proyecto: PBR - rugosidad metálica recubierta
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Motor&amp;rbrack; Texturas virtuales dispersas (SVT)
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Preferences&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Opción de aceleración de compatibilidad de hardware SVT
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Log&amp;rbrack; Información adicional para la función de texturas virtuales dispersas (por ejemplo, disco de tamaño)
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Ventana de mensaje al inicio si el tamaño del disco es demasiado bajo para la caché
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Preferences&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Ubicación de caché global del Substance Painter
* &amp;lbrack;SVT&amp;rbrack; Nueva variable de entorno para especificar la ruta de acceso de la caché del Substance Painter
* &amp;lbrack;SVT&amp;rbrack; Nueva variable de entorno para activar la aceleración de compatibilidad de hardware SVT
* &amp;lbrack;SVT&amp;rbrack; Detectar compatibilidad dispersa por hardware
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Hardware Sparse&amp;rbrack; Aumentar la versión mínima del controlador para la GPU Nvidia
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Avisar al usuario si hay artefactos con texturas virtuales dispersas al abrir el proyecto

**Corregido:**

* &amp;lbrack;Selector de color&amp;rbrack; Cursor de pintura que aparece al intentar seleccionar un color
* El bloqueo al seleccionar o anular la selección de capas en un orden específico puede provocar bloqueos
* Bloqueo al pegar como instancia una capa con una máscara
* &amp;lbrack;Canal de usuario&amp;rbrack;&amp;lbrack;Regresión&amp;rbrack; Bloqueo al cambiar el nombre del canal de usuario
* &amp;lbrack;Canal de usuario&amp;rbrack; Vista previa de pincel gris
* &amp;lbrack;Alembic&amp;rbrack; Solo un conjunto de texturas de varios materiales tras la importación
* &amp;lbrack;Motor&amp;rbrack; La textura exportada difiere de la ventana gráfica para los sellos de pincel
* &amp;lbrack;Motor&amp;rbrack; La inversión con un efecto de nivel no afecta por completo a una textura
* El selector de material está aplicando un trazo de pincel al seleccionar
* Cambiar la resolución a 128x128px conduce a un bloqueo
* Los vínculos de mapa de malla no se actualizan correctamente al rehornear o crear instancias de capas
* &amp;lbrack;Substance&amp;rbrack; UserData ColorSpace no funciona en la malla Hecha un bake Normal solicitada como entrada
* No coincide la asociación MDL al utilizar varias instancias de sombreado
* &amp;lbrack;Simetría&amp;rbrack;&amp;lbrack;Rellenar capa&amp;rbrack; Plano de simetría y su manipulador activos en Capa de relleno
* &amp;lbrack;Viewport&amp;rbrack; El punto de tabla dinámica para la traducción no siempre se actualiza después de hacer clic
* &amp;lbrack;UI&amp;rbrack; Corrección de iconos y eliminación de marcadores de posición para monitores HDPI

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows
* El suavizado y las sombras cuando están activos juntos pueden dar resultados inesperados

### 4.2.3 (2018.2.3)

*(Lanzado: 25 de septiembre de 2018)*

**Corregido:**

* &amp;lbrack;vista 2D&amp;rbrack; El vista 2D se rompe con algunas mallas al crear un nuevo proyecto
* &amp;lbrack;Bloqueo&amp;rbrack; El cambio de la Proyección de UV a la proyección tri-plana conduce a un bloqueo
* &amp;lbrack;RayCollider&amp;rbrack; Varios bloqueos debido a &quot;RayCollider&quot;
* &amp;lbrack;Herramienta&amp;rbrack; Al cambiar las capas, se pierden las propiedades de pincel modificadas
* La configuración del pincel se restablece al cambiar al borrador

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.2.2 (2018.2.2)

*(Lanzado: 11 de septiembre de 2018*)Resumen: **Revisión con actualización de contenido, nuevas funcionalidades de secuencias de comandos y poder deshabilitar la actualización automática**

**Agregado:**

* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Añadir un ajuste preestablecido de Estante de piel
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;shelf&amp;brack; Conversión de 19 normales de piel en materiales para dispersión subsuperficial
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Crear una plantilla de proyecto desde un proyecto abierto
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Obtener o establecer la configuración de exportación de un proyecto abierto
* &amp;lbrack;Actualizaciones&amp;rbrack; Puede desactivar la ventana emergente de actualización automática de la variable de entorno y configuración
* &amp;lbrack;Actualizaciones&amp;rbrack; No mostrar hasta la próxima versión en el mantenimiento anticuado emergente

**Corregido:**

* &amp;lbrack;Cámara&amp;rbrack; Zoom incorrecto al cambiar de ortográfico a Perspectiva
* &amp;lbrack;Mostrar&amp;rbrack; Algunos mapas se muestran en modo lineal en lugar de sRGB
* &amp;lbrack;Viewports&amp;rbrack; El enfoque de malla no se comporta correctamente
* &amp;lbrack;vista 2D&amp;rbrack; Proyecto con cámara rota ha desaparecido UVs Cáscaras
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Información sobre herramientas&amp;rbrack; aparece información sobre herramientas de dispersión subsuperficial en el registro
* Algunos proyectos no se pueden abrir en 2018.2 y el mensaje de error no puede guardar un paquete de substance nulo
* &amp;lbrack;Máscara&amp;rbrack; El color de la herramienta pintura se puede bloquear en algunos casos al trabajar en una máscara
* &amp;lbrack;Material&amp;rbrack; Los mapas no aparecen en situaciones específicas
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;Herramientas&amp;rbrack; Manipulador activo con un generador
* &amp;lbrack;Substance&amp;rbrack; Faltan grupos de parámetros de Substance
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Nombre de software incorrecto en la documentación
* &amp;lbrack;UDIM&amp;rbrack; No hay información en el registro acerca de los proyectiles UV en múltiples mosaicos UVs

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

*(Lanzado: 02 de agosto de 2018*)Resumen: **Versión de verano, compatibilidad con dispersión subsuperficial, mejoras en la proyección y el relleno, importación y selección de cámaras, compatibilidad con Alembic y glTF, arrastrar y soltar en mapa de ID, compatibilidad de formato de Substance mejorada y nuevo contenido**

**Agregado:**

* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Dispersión subsuperficial genérica
* &amp;lbrack;SSS&amp;rbrack; Sincronizar MDL y parámetros de dispersión subsuperficial
* &amp;lbrack;SSS&amp;rbrack; Se ha añadido un nuevo canal de escala de grises llamado Dispersión
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Configuración de Sombreador&amp;rbrack; Parámetro de tipo de dispersión para la dispersión subsuperficial (cutánea o translúcida)
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Configuración de Sombreador&amp;rbrack; Parámetro de escala de dispersión para dispersión subsuperficial
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Configuración de Sombreador&amp;rbrack; Parámetro de color de dispersión para dispersión subsuperficial
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Configuración de visualización&amp;rbrack; Dispersión Recuento de muestras para dispersión subsuperficial
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Integrar MDL de dispersión subsuperficial para Iray
* &amp;lbrack;Sombreador&amp;rbrack; Actualización de sombreador mediante el actualizador de recursos
* &amp;lbrack;Sombreador&amp;rbrack; Actualizar la documentación y la API del registro de cambios
* &amp;lbrack;Propiedades de herramienta&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Nuevos parámetros para la proyección triplanar
* &amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Controlar las propiedades de la capa de relleno en la vista 3D directamente con los manipuladores (proyección triplanar)
* &amp;lbrack;Atajos&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Nuevos métodos abreviados Q, W, E, R y T para manipuladores de proyección triplanar
* &amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Controlar las propiedades de la capa de relleno en Vista 2D directamente con los manipuladores (Proyección de UV)
* &amp;lbrack;Atajos&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Nuevo método abreviado Q para manipuladores de Proyección de UV
* &amp;lbrack;Barra de herramientas contextual&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Manipuladores de proyección triplanar de control
* &amp;lbrack;Barra de herramientas contextual&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Manipuladores de Proyección de UV de control
* &amp;lbrack;Propiedades de herramienta&amp;rbrack; Desactivación del mosaico de textura con la herramienta Proyección y Galería de símbolos
* &amp;lbrack;Stencil&amp;rbrack; Usar imágenes no cuadradas con la herramienta o galería de símbolos Proyección
* &amp;lbrack;Stencil&amp;rbrack; Permitir el control del modo de mosaico en la ventana Propiedades
* &amp;lbrack;Stencil&amp;rbrack; El zoom no está centrado en una galería de símbolos que no sea de mosaico
* &amp;lbrack;Cámaras&amp;rbrack; Importar cámaras de Maya, Max, Blender, Modo, DAE
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Selección y control de cámaras importadas en la ventana gráfica
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Selección y control de cámaras importadas en Irán
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;UI&amp;rbrack;&amp;lbrack;Nuevo proyecto&amp;rbrack;&amp;lbrack;Configuración del proyecto&amp;rbrack; Importar cámaras está marcado de forma predeterminada
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Accesos directos&amp;rbrack; Añadir métodos abreviados para cambiar de cámara
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Añadir marco en la ventana gráfica
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Ajustes de ventana&amp;rbrack; Control de la opacidad del marco
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Configuración de la cámara&amp;rbrack; Distancia focal máxima a 500 mm
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Configuración de la cámara&amp;rbrack; Proporción de exposición
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Configuración de la cámara&amp;rbrack; Añadir una opción de bloqueo
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Configuración de la cámara&amp;rbrack; Añadir una opción de restauración
* &amp;lbrack;Cámaras&amp;rbrack;&amp;lbrack;Configuración de la cámara&amp;rbrack; Añadir atributo de distancia de enfoque
* &amp;lbrack;glTF&amp;rbrack; Importación de un archivo glTF
* &amp;lbrack;glTF&amp;rbrack; Importar mapa de oclusión ambiental
* &amp;lbrack;Alembic&amp;rbrack; Importar marco Alembic 1 con geometría estática
* &amp;lbrack;Shelf&amp;rbrack; Arrastre y suelte materiales directamente en la malla mediante mapas de ID con un modificador (CTRL/Comando)
* &amp;lbrack;Pila de capas&amp;rbrack; Creación automática de máscaras de ID con arrastrar y soltar materiales en la malla con mapas de ID
* &amp;lbrack;Pila de capas&amp;rbrack; Desplazamiento automático de capas con arrastrar y soltar por la pila de capas
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Propiedades de herramienta&amp;rbrack; Exponer el ajuste preestablecido de Substance
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Menú Ayuda&amp;rbrack; Mejora del menú Ayuda
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Nuevo proyecto&amp;rbrack;&amp;lbrack;Configuración del proyecto&amp;rbrack; Reorganización de la ventana
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Nuevo proyecto&amp;rbrack;&amp;lbrack;Configuración del proyecto&amp;rbrack; Reemplazar término de malla por archivo
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Visualización de atributos del Substance en la IU
* &amp;lbrack;Atajos&amp;rbrack; Conmutadores F4 entre la vista 2D y 3D
* &amp;lbrack;Atajos&amp;rbrack; Nuevos métodos abreviados para alternar la galería de símbolos N y la máscara rápida U
* &amp;lbrack;integración de Substance&amp;rbrack; Tenga en cuenta las instrucciones &#39;visible if&#39; en los parámetros del Substance
* &amp;lbrack;Viewport&amp;rbrack; Las sombras no se ven forzadas a calcularse después del movimiento de la cámara
* &amp;lbrack;Contenido&amp;rbrack; Actualizar MeetMat con cámaras importadas
* &amp;lbrack;Contenido&amp;rbrack; Añadir una muestra con la dispersión subsuperficial activada - JadeToad
* &amp;lbrack;Contenido&amp;rbrack; Añade una nueva plantilla de proyecto PBR con la dispersión subsuperficial activada
* &amp;lbrack;Contenido&amp;rbrack; Ajustes preestablecidos de exportación actualizados para añadir un nuevo canal de dispersión
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Se ha añadido compatibilidad de dispersión subsuperficial para: pbr-metal-rough, pbr-metal-rough-alpha-test, recubierto de pbr, pbr-spec-gloss
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Se ha añadido canal de dispersión a 5 materiales inteligentes (mármoles y pieles)
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; 1 nuevo material de jade
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; 1 cera nueva Material

**Corregido:**

* &amp;lbrack;CMD&amp;rbrack; Diferentes resultados usando la misma línea de comandos con diferentes versiones
* &amp;lbrack;TDR&amp;rbrack; Si TdrLevel está configurado no tiene ningún error en su registro
* &amp;lbrack;Baker&amp;rbrack; El mapa de oclusión ambiental está volteado
* &amp;lbrack;ID Map&amp;rbrack; Bloqueo al seleccionar fuera del rango 0-1
* &amp;lbrack;Iray&amp;rbrack; Bloqueo al cambiar conjuntos de texturas y volver al modo de Pintura
* &amp;lbrack;Viewport&amp;rbrack; Sincronización de áreas de colocación entre puntos de visión para arrastrar y soltar
* &amp;lbrack;Motor&amp;rbrack; Artefacto de Moiré al aplicar mosaico a capas de relleno o pintar pinceles pequeños
* &amp;lbrack;Licencia&amp;rbrack; Comprobación de versión de software errónea del servicio de licencias
* &amp;lbrack;Licencia&amp;rbrack; Rediseña la forma en que gestionamos la autenticación
* &amp;lbrack;API&amp;rbrack; Llame al evento de la API de scripts onNewProjectCreated incluso al crear con una plantilla
* &amp;lbrack;Sombreador&amp;rbrack; El sombreador compilado no se carga de la memoria caché cuando el archivo de sombreador no se compila
* &amp;lbrack;Shelf&amp;rbrack; Al exportar el archivo HDR. de la estantería, se generará un archivo con valores de sujeción
* &amp;lbrack;Exportar&amp;rbrack; EXR exportar abrazaderas RGB valores de color entre 0 y 1
* &amp;lbrack;Contenido&amp;rbrack; Ruido procedimiento El fragmento de ruido de Perlin 3D se pixeló

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.1.3 (2018.1.3)

*(Lanzado: 28 de junio de 2018)*

**Agregado:**

* &amp;lbrack;Preferencias&amp;rbrack; Propuesta de guardar el proyecto cuando se reinicie Painter

**Corregido:**

* &amp;lbrack;Complemento&amp;rbrack; El Substance Source de búsqueda no funciona
* &amp;lbrack;Materiales inteligentes&amp;rbrack; La importación de Materiales inteligentes provoca un bloqueo en algunos casos
* &amp;lbrack;Materiales inteligentes&amp;rbrack; La eliminación de Materiales inteligentes provoca un bloqueo en algunos casos
* &amp;lbrack;Guardar&amp;rbrack; Guardar conduce a un bloqueo en algunos casos raros
* &amp;lbrack;Shelf&amp;rbrack; Invertir no funciona en las Celdas 2 y 3
* &amp;lbrack;Shelf&amp;rbrack; Error tipográfico en algunos Alpha
* &amp;lbrack;Shelf&amp;rbrack; Algunos materiales de Substance no se renderizan correctamente

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.2 (2018.1.2)

*(Lanzado: 12 de junio de 2018*)Resumen: **Mejora en la velocidad de Hace un bake, Sistema de guardado mejorado, Reguladores actualizados, Plugin API actualizado, Traducción al chino, Relleno mejorado ahora Opcional**

**Agregado:**

* &amp;lbrack;Bakeres&amp;rbrack; Mejora del rendimiento con la nueva versión de baker
* Cuadro de diálogo Forzar visualización con GPU no compatible
* &amp;lbrack;Guardar&amp;rbrack; Exponer la nueva funcionalidad de proyecto compacto (modo de guardado completo/compacto)
* &amp;lbrack;Guardar&amp;rbrack; Informar al usuario en caso de error al guardar
* &amp;lbrack;Clean&amp;rbrack; Siguiente guardado en modo completo/compacto
* &amp;lbrack;Reguladores&amp;rbrack; Mejora de la precisión de las barras y los reguladores de color/escala de grises
* &amp;lbrack;Reguladores&amp;rbrack; Adición de controles de flecha arriba/abajo
* &amp;lbrack;Reguladores&amp;rbrack; Misma zona de detección para los reguladores de barras de color y escala de grises
* &amp;lbrack;Complemento&amp;rbrack; Guardado automático siempre en modo incremental
* &amp;lbrack;Complemento&amp;rbrack; Opción para cambiar los complementos al nuevo estilo de interfaz
* &amp;lbrack;Idioma&amp;rbrack; Añadir traducción al chino
* &amp;lbrack;Relleno&amp;rbrack; Opción para cambiar entre el relleno UV y el relleno vecino del espacio 3D por conjunto de texturas en Configuración del conjunto de texturas
* &amp;lbrack;Script&amp;rbrack; Exponer modo de guardado: completo/compacto o incremental
* &amp;lbrack;Script&amp;rbrack; Actualizar documentación de scripts/QML
* &amp;lbrack;Registro&amp;rbrack; Indicar el modo de guardado en el registro (completo/compacto o incremental)

**Corregido:**

* &amp;lbrack;Herramienta&amp;rbrack; La ranura de canal se transforma en una ranura de material en rellenos de un solo canal
* Bloqueo al cargar una malla (FBX) con algunas caras no asignadas por un material
* Bloqueo en Irán con NVIDIA GRID 5.2 en máquina virtual
* Bloqueo al deshacer la eliminación de un ajuste preestablecido de material
* Bloqueo al cargar algunos proyectos
* &amp;lbrack;Línea de comandos&amp;rbrack; Nueva línea de comandos para mallas de UDIM divididas por audio
* &amp;lbrack;Barra de herramientas&amp;rbrack; Reducción de la barra de herramientas
* &amp;lbrack;Instanciando&amp;rbrack; No se pueden crear instancias de mapas de bits en varios conjuntos de texturas
* &amp;lbrack;Viewport&amp;rbrack; La actualización no se completa al pintar en malla con UV en mosaico
* &amp;lbrack;Iray&amp;rbrack; El mapa de normales se aplica dos veces a los dieléctricos
* &amp;lbrack;Shelf&amp;rbrack; Errores tipográficos en algunos parámetros del Substance (alfa, procedimientos y matfx)
* &amp;lbrack;Shelf&amp;rbrack; Error tipográfico del mapa de bits &quot;Solo personal autorizado&quot;
* &amp;lbrack;Script&amp;rbrack; La función alg.shaders.materials() ya no funciona

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.1 (2018.1.1)

*(Lanzado: 3 de abril de 2018)*

**Corregido:**

* &amp;lbrack;Tablet&amp;rbrack; Problema al cambiar las opciones de interacción predeterminadas
* &amp;lbrack;Bakeres&amp;rbrack; Bloqueo con la biblioteca Assimp
* &amp;lbrack;Bakeres&amp;rbrack; Regresión en el rendimiento con el mapa A.O
* &amp;lbrack;Iray&amp;rbrack; La Distorsión de lente no se aplica al canal alfa
* &amp;lbrack;Controladores&amp;rbrack; Actualización de los requisitos mínimos de controladores
* &amp;lbrack;3Dview&amp;rbrack; Las normales no se generan correctamente en mallas de UDIM sin información de normales
* &amp;lbrack;Intel&amp;rbrack; Bloqueo normativo con Substance Painter 2018.1.0
* &amp;lbrack;Intel&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Problema con el relleno (defectos negros)

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.0 (2018.1.0)

*(Lanzado: 15 de marzo de 2018)*

**Agregado:**

* Nuevo estilo general (iconos, color, comportamiento)
* Nuevo diseño predeterminado
* &amp;lbrack;Tablet&amp;rbrack; Mejora de la experiencia del usuario al pintar
* &amp;lbrack;Menú principal&amp;rbrack; Ordenar primero los elementos nativos de las vistas y barras de herramientas
* &amp;lbrack;Menú principal&amp;rbrack; Mover acciones de máscara rápida en la sección de ventanilla
* &amp;lbrack;Menú principal&amp;rbrack; Sección Mover las acciones del botón derecho al área de visualización
* &amp;lbrack;Menú principal&amp;rbrack; Cambiar el nombre del menú &quot;Ver&quot; por &quot;Ventana&quot;
* &amp;lbrack;Menú rápido&amp;rbrack; Nuevas propiedades de la herramienta haciendo clic con el botón derecho en la ventana gráfica
* &amp;lbrack;Widget de acoplamiento&amp;rbrack; Nueva barra de herramientas acoplada para una reducción/recuperación rápida
* &amp;lbrack;Configuración de visualización&amp;rbrack; Combinación de la ventana de configuración de cámara y visor
* &amp;lbrack;Pila de capas&amp;rbrack; Menú contextual del botón derecho
* &amp;lbrack;Pila de capas&amp;rbrack; Arrastra y suelta para mover cualquier efecto dentro de la misma capa
* &amp;lbrack;Barra de herramientas&amp;rbrack; Reorganización de la barra de herramientas y nueva barra de herramientas contextual
* &amp;lbrack;Herramientas barra de herramientas&amp;rbrack; Dividir la herramienta Clonar en dos herramientas independientes
* &amp;lbrack;Herramientas propiedades&amp;rbrack; Valor de escala de grises de fondo más claro en la previsualización
* &amp;lbrack;Herramientas propiedades&amp;rbrack; Organización en fichas (rellenar y herramientas)
* &amp;lbrack;Herramienta&amp;rbrack; El resultado de pintura coincide con la galería de símbolos
* &amp;lbrack;Viewport&amp;rbrack; Cursor nuevo para la capa de relleno
* &amp;lbrack;Viewport&amp;rbrack; Navegación y pintura más fluidas (velocidad de marco más alta)
* &amp;lbrack;Viewport&amp;rbrack; Cuadro combinado Selección de material/canal/mapa en la ventana gráfica
* &amp;lbrack;Viewport&amp;rbrack; Reducir el parpadeo mientras se gira (activar sombra)
* &amp;lbrack;Shelf&amp;rbrack; Mostrar materiales de forma predeterminada al abrir Painter
* &amp;lbrack;Shelf&amp;rbrack; Mejora del tiempo de carga de texturas y materiales Substance (de 2 a 6 veces más rápido)
* &amp;lbrack;Shelf&amp;rbrack; Reorganizar carpetas de materiales para que se ajusten a la estructura del Substance Source
* &amp;lbrack;Shelf&amp;rbrack; Arrastre y suelte materiales directamente en la malla en la ventana gráfica
* &amp;lbrack;Shelf&amp;rbrack; Nuevos ruidos en 3D (Perlin, Perlin Fractal, Simplex y Worley)
* &amp;lbrack;Shelf&amp;rbrack; Nuevo generador de máscaras de 3D linear gradient con posición de malla
* &amp;lbrack;Shelf&amp;rbrack; Ruidos básicos actualizados para admitir la expansión no cuadrada
* &amp;lbrack;Shelf&amp;rbrack; Se ha añadido una nueva plantilla y un ajuste preestablecido de exportación para Lens Studio (aplicación Snap)
* &amp;lbrack;Shelf&amp;rbrack; Materiales inteligentes y Máscaras inteligentes actualizados para utilizar la versión más reciente del Editor de máscaras (microdetalles)
* &amp;lbrack;Shelf&amp;rbrack; Nuevo proyecto de muestra &quot;TilingMaterial&quot; para crear materiales de mosaico sin costuras
* &amp;lbrack;Shelf&amp;rbrack; Nuevos ajustes preestablecidos de pincel (caligrafía, mojado, rayado, etc.)
* &amp;lbrack;Reguladores&amp;rbrack; Nuevo estilo y comportamiento de los reguladores y las barras de escala de grises/color
* &amp;lbrack;Bakeres&amp;rbrack; Permitir el uso del cuadro delimitador de escena completo para calcular el mapa de posición
* &amp;lbrack;Sombreador&amp;rbrack; Quitar el parámetro de fuerza de height de los parámetros de sombreador predeterminados
* &amp;lbrack;Motor&amp;rbrack; Motor del Substance actualizado
* &amp;lbrack;Motor&amp;rbrack; Discontinuidades iguales o inferiores en los fragmentos UV
* &amp;lbrack;Complementos&amp;rbrack; Importar materiales descargados de Substance Source con mayor rapidez
* &amp;lbrack;Complementos&amp;rbrack; Actualizar todos los complementos para que coincidan con el nuevo estilo general
* &amp;lbrack;Preferencias&amp;rbrack; Previsualización de los cambios de color de fondo automáticamente
* &amp;lbrack;Clean&amp;rbrack; Menor riesgo de corrupción de proyectos
* &amp;lbrack;Abrir&amp;rbrack; Mejora del tiempo del proyecto de apertura
* &amp;lbrack;Nuevo proyecto&amp;rbrack; Nuevo proyecto: mejora del tiempo de actualización de malla
* &amp;lbrack;Guardar&amp;rbrack; Ahorro de tiempo del proyecto
* &amp;lbrack;Registro&amp;rbrack; Tipo de licencia registrado en el registro
* &amp;lbrack;TextureSet&amp;rbrack; Cambie el nombre del botón &quot;Hacer un bake Texturas&quot; por &quot;Hacer un bake mapas de malla&quot;
* Cambie el nombre de &quot;Mapas adicionales&quot; por &quot;Mapas de malla&quot;

**Corregido:**

* &amp;lbrack;Viewport&amp;rbrack; Mal rendimiento con mallas que contienen muchos subobjetos
* &amp;lbrack;Herramientas propiedades&amp;rbrack; Canal desactivado al arrastrar y soltar una imagen en la ranura de material
* &amp;lbrack;Herramientas propiedades&amp;rbrack; La vista previa del pincel se rompe con las herramientas de difuminado y clonación
* &amp;lbrack;Conjunto de texturas&amp;rbrack; El orden de los canales es incorrecto al utilizar plantillas
* &amp;lbrack;Shelf&amp;rbrack; Falta icono para el generador de Conversión de escala de grises
* &amp;lbrack;Shelf&amp;rbrack; El número de círculo de Sign alfa está roto (falta la fuente)
* Detección incorrecta de GPU integradas al iniciarse
* &amp;lbrack;Bloqueo&amp;rbrack; Arrastrar y colocar un recurso importado cuyo nombre tenga el carácter #
* &amp;lbrack;Motor&amp;rbrack; Problema de detección de Vram en la GPU integrada
* &amp;lbrack;Motor&amp;rbrack; Se han corregido numerosos bloqueos en Substance Engine Linker
* &amp;lbrack;Motor&amp;rbrack; Artefactos cuadrados al cambiar la resolución
* &amp;lbrack;Efectos de posprocesamiento&amp;rbrack; El cambio de tamaño de la interfaz es lento cuando los efectos de posprocesamiento están activados
* &amp;lbrack;Bakeres&amp;rbrack; La unidad de escena no se respeta correctamente para los valores de distancia de rayos
* &amp;lbrack;Bakeres&amp;rbrack; La distancia AO desde Mesh Occluder se fija a 1 independientemente del valor de entrada
* &amp;lbrack;Bakeres&amp;rbrack; La coincidencia por nombre ignora algunas mallas con nombres específicos
* &amp;lbrack;Bakeres&amp;rbrack; El color de la configuración de Polygroup y Submesh ID siempre devuelve una imagen en negro
* &amp;lbrack;Bakeres&amp;rbrack; La Hace un bake de ID falla con mallas de FBX binarias de Blender
* &amp;lbrack;Sombreador&amp;rbrack; Ruido en el vista 2D con dota-2 y non-pbr-spec-gloss
* &amp;lbrack;Linux&amp;rbrack; Sólo se utiliza un subproceso de CPU al hacer un bake
* &amp;lbrack;MacOS&amp;rbrack; Bloqueo con el cursor del pincel moviéndose sobre la ventana gráfica

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* El proceso posterior de distorsión no se tiene en cuenta al exportar en IRay (alfa)

## Versión 3

### 3.4.2 (2017.4.2)

*(Lanzado: 24 de enero de 2018)*

**Agregado:**

* &amp;lbrack;Exportar&amp;rbrack; Obtener el estado de una exportación con el progreso del paso
* &amp;lbrack;Exportar&amp;rbrack; Permitir cancelar una exportación
* &amp;lbrack;Exportar&amp;rbrack; Exportar texturas a Sketchfab sin perder calidad de mapa de normales
* &amp;lbrack;Exportar&amp;rbrack; Exportar en formato binario glTF (glb)
* &amp;lbrack;Exportar&amp;rbrack; Permitir cambiar el tamaño de las columnas en la ficha de configuración de la ventana de exportación
* &amp;lbrack;Sombreador&amp;rbrack; Agregar un registro de cambios para la API del sombreador
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Agregar funciones de devolución de llamada Antes y Después al exportar texturas
* &amp;lbrack;Iray&amp;rbrack; Actualización a SDK 2017.1 (compatibilidad con las GPU Volta)

**Corregido:**

* Bloqueo al salir de la aplicación antes de mostrar la ventana principal
* &amp;lbrack;MAC&amp;rbrack; Bloqueo al cargar mapas en escala de grises con IRA
* &amp;lbrack;MAC&amp;rbrack; VRAM detección no es correcta con el nuevo sistema operativo High Sierra
* &amp;lbrack;Complemento&amp;rbrack; La descarga de recursos de Substance Source ya no funciona
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Detección de versión mínima de complemento incorrecta
* &amp;lbrack;Exportar&amp;rbrack; Error al guardar el ajuste preestablecido de exportación después de exportar texturas
* &amp;lbrack;Instanciando&amp;rbrack; Problema en generadores instanciados en un TextureSet sin asignaciones adicionales
* &amp;lbrack;Viewport&amp;rbrack; El tramado no funciona con una resolución superior a 4k
* &amp;lbrack;Viewport&amp;rbrack; La visualización de material de vista 2D está cubierta de ruido
* &amp;lbrack;Shelf&amp;rbrack; Mejorar el tiempo de carga de los ajustes preestablecidos de estantería
* &amp;lbrack;Motor&amp;rbrack; Fusión incorrecta al pintar en la selección de color

### 3.4.1 (2017.4.1)

*(Lanzado: 15 de diciembre de 2017)*

**Agregado:**

* &amp;lbrack;Secuencias de comandos&amp;rbrack; Exportar malla mediante la API de scripts
* &amp;lbrack;Importar&amp;rbrack; Desactivar la importación de formatos de archivo de malla no compatibles (permitir solo obj, fbx, dae, ply)
* &amp;lbrack;Registro&amp;rbrack; Indique con mayor precisión el problema de TDR en el archivo de registro

**Corregido:**

* Bloqueo si la aplicación se cierra antes de que finalice el rastreo de recursos
* Bloqueo al abrir proyectos con la herramienta Dedo/Clonar
* Bloqueo al utilizar rehacer después de deshacer un cambio de Sombreador en Configuración del visor
* &amp;lbrack;Motor&amp;rbrack; La texturización difiere entre Painter 2017.2 y 2017.4
* &amp;lbrack;Viewport&amp;rbrack; Al seleccionar un mapa de ID de una instancia, se muestra un color incorrecto
* &amp;lbrack;Exportar&amp;rbrack; Bloqueo al exportar una textura normal o de oclusión no válida
* &amp;lbrack;Exportar&amp;rbrack; Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6
* &amp;lbrack;Complemento&amp;rbrack; El complemento de Photoshop ignora la selección de canales y siempre exporta todo
* &amp;lbrack;Capas&amp;rbrack; Los anclajes se rompen al copiar o pegar entre conjuntos de texturas
* &amp;lbrack;Capas&amp;rbrack; Algunas referencias de anclaje no se pueden restaurar si están rotas
* &amp;lbrack;Sombreador&amp;rbrack; el parámetro de rugosidad secundaria con revestimiento de pbr está roto
* &amp;lbrack;Vapor&amp;rbrack; La ventana emergente del comprobador de versiones no debería estar visible al iniciarse

**Problemas conocidos:**

* &amp;lbrack;AMD&amp;rbrack; Bloqueos y bloqueos al intentar realizar una pintura en una malla. Se puede solucionar con una actualización del controlador de la GPU.

### 3.4.0 (2017.4.0)

*(Lanzado: 23 de noviembre de 2017)*

**Agregado:**

* &amp;lbrack;Instanciando&amp;rbrack; Permitir la creación de instancias de parámetros en capas
* &amp;lbrack;Instanciando&amp;rbrack; Permitir saltar entre una capa de origen y una instancia
* &amp;lbrack;Instanciando&amp;rbrack; Añadir una acción &quot;Crear instancias en conjuntos de texturas&quot;
* &amp;lbrack;Instanciando&amp;rbrack; Indicar en la pila de capas las instancias de reentrada (ciclos)
* &amp;lbrack;Instanciando&amp;rbrack; Eliminar instancias cuando se elimina un origen
* &amp;lbrack;Instanciando&amp;rbrack; No permitir referencias de anclaje desde fuera de una carpeta con instancias
* &amp;lbrack;UI&amp;rbrack; Mueva la pila Deshacer a su propia ventana llamada &quot;Historial&quot;
* &amp;lbrack;Complemento&amp;rbrack; Integrar el plugin Live-Link de DCC
* &amp;lbrack;Motor&amp;rbrack; Mejorar el rendimiento de la pintura con pintura dispersa
* &amp;lbrack;Exportar&amp;rbrack; Añadir opciones de borrador y reexportación al exportador de Sketchfab
* &amp;lbrack;Shelf&amp;rbrack; Añadir el control &quot;voltear&quot; para las sustancias de fuentes
* &amp;lbrack;Shelf&amp;rbrack; Añade 20 nuevos materiales de procedimientos
* &amp;lbrack;Shelf&amp;rbrack; Añadir 40 nuevos mapas grunges (basados en mapa de bits y procedimientos)
* &amp;lbrack;Viewport&amp;rbrack; Activar colisiones de previsualización de pincel en otros conjuntos de texturas visibles
* Requisitos mínimos de actualización de controladores de GPU AMD

**Corregido:**

* Bloqueo Al calcular Substance con resoluciones demasiado grandes
* Bloqueo al pintar con partículas
* &amp;lbrack;Viewport&amp;rbrack; Reflejo de specular incorrecto en el Vista 2D con mallas específicas
* &amp;lbrack;UI&amp;rbrack; Aparecen algunas acciones no deseadas en la ventana Historial

**Problemas conocidos:**

* &amp;lbrack;Capas&amp;rbrack; Algunas referencias de anclaje no se pueden restaurar si están rotas
* Bloqueo al utilizar rehacer después de deshacer un cambio de Sombreador en Configuración del visor

### 3.3.3 (2017.3.3)

*(Lanzado: 01 de diciembre de 2017)*

**Corregido:**

* &amp;lbrack;Vapor&amp;rbrack; La ventana emergente del comprobador de versiones no debería estar visible al iniciarse
* &amp;lbrack;Exportar&amp;rbrack; Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6

### 3.3.2 (2017.3.2)

*(Lanzado: 20 de noviembre de 2017)*

**Agregado:**

* &amp;lbrack;UI&amp;rbrack; Mejorar el diálogo de la nueva versión y añadir changelog
* &amp;lbrack;UI&amp;rbrack; Indicar si el mantenimiento ha caducado en el cuadro de diálogo Nueva versión
* &amp;lbrack;Licencia&amp;rbrack; Actualizar el sistema de licencias para gestionar las fechas de mantenimiento
* &amp;lbrack;Exportar&amp;rbrack; Cambiar nombre de Adobe Standard Material a Adobe Dimension

**Corregido:**

* &amp;lbrack;Mac&amp;rbrack; Pintar conduce a cuadrados negros y corrupciones de textura
* &amp;lbrack;Motor&amp;rbrack; La caché a veces puede desaparecer en la ventana gráfica
* &amp;lbrack;Motor&amp;rbrack; Aparecen artefactos de bloque cuando se activa la compresión de memoria
* &amp;lbrack;Haciendo un bake&amp;rbrack; Mensajes de error extraños al hacer un bake mallas específicas
* &amp;lbrack;Exportar&amp;rbrack; Los PSD se escriben incorrectamente y Photoshop no los reconoce correctamente
* &amp;lbrack;Capas&amp;rbrack; No debería ser posible copiar y pegar capas en varios proyectos
* &amp;lbrack;Substance&amp;rbrack; El espacio de color UserData para la entrada Normal se invierte en algunos casos
* &amp;lbrack;Shelf&amp;rbrack; Micro-normal en generadores genera curvatura invertida
* &amp;lbrack;Shelf&amp;rbrack; HSL filtro también afecta al canal alfa
* &amp;lbrack;Linux&amp;rbrack; La instalación en Centos falla debido a la falta de dependencias
* El instalador no elimina todos los recursos de la instalación anterior en ciertos casos

### 3.3.1 (2017.3.1)

*(Lanzado: 26 de octubre de 2017)*

**Agregado:**

* &amp;lbrack;Exportar&amp;rbrack; Permitir exportar la malla desde un proyecto
* &amp;lbrack;Shelf&amp;rbrack; Quitar &quot;Sub-Shelf&quot; de los títulos de las pestañas
* Guardar la configuración posterior al proceso en plantillas
* Haz que el mensaje TDR sea más comprensible
* Mejorar la ventana Configuración para informar de errores

**Corregido:**

* Bloqueo al borrar varios subestantes
* Bloqueo al cambiar de un nivel a otro durante un cálculo del motor
* &amp;lbrack;Mac&amp;rbrack; Bloqueo en la GPU Intel durante los cálculos del motor
* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Rendimiento incorrecto cuando el tramado está activado
* &amp;lbrack;Mac&amp;rbrack; MacOS 10.13 se reconoce como &quot;Versión desconocida&quot; en el archivo de registro
* &amp;lbrack;Baker&amp;rbrack; Hacer un bake con una jaula ya no funciona
* &amp;lbrack;Capas&amp;rbrack; El método abreviado Ctrl+C (acción de copia) ya no funciona
* &amp;lbrack;Capas&amp;rbrack; Al pegar capas, la interfaz de usuario no se actualiza con las referencias del anclaje
* &amp;lbrack;Anchor&amp;rbrack; Duplicar o copiar y pegar capa con referencias rompe vínculos
* &amp;lbrack;Exportar&amp;rbrack; La exportación en 8K puede bloquear o bloquear la aplicación en algunos casos
* &amp;lbrack;Exportar&amp;rbrack; Varios problemas en el formato de archivo glTF generado
* &amp;lbrack;Importar&amp;rbrack; Volver a importar una malla con el mismo nombre de archivo ya no funciona
* &amp;lbrack;Complemento&amp;rbrack; La ventana de guardado automático siempre aparece encima de todo
* &amp;lbrack;UI&amp;rbrack; Bucle infinito al pulsar &quot;Escape&quot; en el cuadro de diálogo TDR
* &amp;lbrack;UI&amp;rbrack; Restaurar IU muestra una segunda barra de título en la ventana de la estantería

### 3.3.0 (2017.3.0)

*(Lanzado: 28 de septiembre de 2017)*

**Agregado:**

* &amp;lbrack;Exportar&amp;rbrack; Permitir la exportación de mallas y texturas para el proyecto de Adobe Felix
* &amp;lbrack;Exportar&amp;rbrack; Permitir exportar a formato de archivo glTF
* &amp;lbrack;Motor&amp;rbrack; Optimizar el tamaño de las texturas en VRAM mediante la compresión de bloques
* &amp;lbrack;Viewport&amp;rbrack; Posibilidad de arrastrar y soltar una malla o un proyecto en la ventana gráfica
* &amp;lbrack;UI&amp;rbrack; Mejorar el mensaje de advertencia sobre TDR
* &amp;lbrack;UI&amp;rbrack; El registro debe mostrarse sólo si se solicita
* &amp;lbrack;UI&amp;rbrack; Permitir borrar el contenido de la ventana de registro
* &amp;lbrack;UI&amp;rbrack; Mostrar advertencias y errores en la barra de estado
* &amp;lbrack;UI&amp;rbrack; Mostrar pestañas en la parte superior como en los navegadores web
* &amp;lbrack;UI&amp;rbrack; Mejorar el contexto y los mensajes &quot;no puede pintarse&quot;
* &amp;lbrack;UI&amp;rbrack; Añadir una acción &quot;Guardar como copia&quot; en el menú Archivo
* &amp;lbrack;Capa&amp;rbrack; Establecer el valor predeterminado de mosaico en 1 de forma predeterminada
* &amp;lbrack;Shelf&amp;rbrack; Filtro de degradado mejorado para admitir 10 colores dinámicos
* &amp;lbrack;Shelf&amp;rbrack; Agregar un espacio en la consulta predeterminada de la miniestantería
* &amp;lbrack;Shelf&amp;rbrack; Añadir una acción &quot;Abrir en el explorador&quot; para los recursos locales en el estante
* &amp;lbrack;Shelf&amp;rbrack; Agregar plantilla y sombreador para Adobe Material Standard (Proyecto Felix)
* &amp;lbrack;Shelf&amp;rbrack; Aumentar mosaico máximo a 128 en sombreadores de capas de material
* &amp;lbrack;Shelf&amp;rbrack; Se ha añadido curvatura sobel para microdetalles de Generadores de máscaras
* &amp;lbrack;Complemento&amp;rbrack; Añadir complemento de autoguardado con intervalo de tiempo personalizable
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Añadir una función &quot;Guardar como copia&quot;

**Corregido:**

* &amp;lbrack;UI&amp;rbrack; El diseño se interrumpe al iniciarse por primera vez
* &amp;lbrack;Exportar&amp;rbrack; El PSD generado al exportar tiene errores de formato
* &amp;lbrack;Exportar&amp;rbrack; EXR siempre exporta el mapa de altura de 8 bits
* &amp;lbrack;Exportar&amp;rbrack; Bloqueo al exportar mapas adicionales dañados
* &amp;lbrack;Importar&amp;rbrack; Los bordes duros no se conservan en mallas de polietileno bajas en algunos casos
* &amp;lbrack;Importar&amp;rbrack; Mensajes de error mejorados al importar mallas con problemas
* &amp;lbrack;Bakeres&amp;rbrack; Error al Hacer un bake la asignación de ID con la opción Coincidir por nombre activada
* &amp;lbrack;Viewport&amp;rbrack; El espacio tangente no se sincroniza con los bakeres
* &amp;lbrack;Efecto&amp;rbrack; Al retroceder una capa no se restaura la referencia de un anclaje
* &amp;lbrack;Efecto&amp;rbrack; Problema de actualización al crear un vínculo entre dos máscaras con anclajes
* &amp;lbrack;Efecto&amp;rbrack; Los anclajes de máscaras encima de la máscara no deben aparecer en la lista
* &amp;lbrack;Efecto&amp;rbrack; La opción Extraer el Alpha de Anclajes no funciona
* &amp;lbrack;Motor&amp;rbrack; La máscara se invierte sola después del primer trazo de pincel
* &amp;lbrack;Motor&amp;rbrack; Bloqueo al cambiar el conjunto de texturas en un proyecto específico
* &amp;lbrack;Shelf&amp;rbrack; Bloqueo al eliminar un ajuste preestablecido de un proyecto
* &amp;lbrack;Shelf&amp;rbrack; Error tipográfico en el filtro Tri-Plano avanzado
* &amp;lbrack;Shelf&amp;rbrack; La escala de ruido del AO de MG Mask Builder no funciona correctamente
* &amp;lbrack;Shelf&amp;rbrack; MG Mask Builder tiene parámetros de curvatura invertidos
* &amp;lbrack;Shelf&amp;rbrack; Los alfa importados generan una previsualización de esfera de material en lugar de una plana

### 3.2.0 (2017.2.0)

*(Lanzado: 27 de julio de 2017)*

**Agregado:**

* Puntos de anclaje: sistema de referencia de capas y máscaras
* &amp;lbrack;Capas&amp;rbrack; Capacidad para cambiar el nombre de los efectos de relleno y Pintura
* &amp;lbrack;Complemento&amp;rbrack; Complemento de Substance Source actualizado
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir consultar la resolución del conjunto de texturas
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir para obtener el estado del motor de pintura
* &amp;lbrack;Rendimiento&amp;rbrack; Optimizaciones mejoradas de carga de proyectos y estampado de pinceles

**Corregido:**

* &amp;lbrack;Herramienta&amp;rbrack; Problemas de rendimiento al ajustar parámetros de material
* &amp;lbrack;Motor&amp;rbrack; Trazos de pincel que desaparecen al cambiar la resolución (4K>2K)
* &amp;lbrack;Vista 3D&amp;rbrack; El espacio tangente no se sincroniza con los bakeres
* &amp;lbrack;Shelf&amp;rbrack; La ruta de los documentos de usuario no se crea automáticamente
* &amp;lbrack;Shelf&amp;rbrack; Hacer ajustes preestablecidos compatibles con versiones anteriores después de una actualización
* &amp;lbrack;Sombreador&amp;rbrack; El sombreador que no es PBR ya no funciona
* &amp;lbrack;Bakeres&amp;rbrack; Error al Hacer un bake la asignación de ID con la opción Coincidir por nombre activada
* &amp;lbrack;Ejemplo&amp;rbrack; Los nombres de los conjuntos de texturas del proyecto de muestra Meet Mat son incorrectos
* Guardar un proyecto antes de crear una plantilla devuelve errores de permisos de escritura

### 3.1.0 (2017.1.0)

*(Lanzado: 20 de junio de 2017)*

**Agregado:**

* &amp;lbrack;Complemento&amp;rbrack; Nuevo complemento de Substance Source (permite descargar contenidos en el estante)
* &amp;lbrack;Shelf&amp;rbrack; 4 Fuentes nuevas (japonés + chino simplificado, máquina de escribir, segmento)
* &amp;lbrack;Shelf&amp;rbrack; 230 nuevos Alpha (combinación de patrones, pinceles y digitalizaciones de huellas digitales)
* &amp;lbrack;Shelf&amp;rbrack; 50 Nuevos Procedurals (Patrones de tela de la ropa medieval y contemporánea)
* &amp;lbrack;Shelf&amp;rbrack; 2 Nuevos mapas ambientales (Mondarrain y Villa Nova Street)
* &amp;lbrack;Shelf&amp;rbrack; 9 Nuevos filtros (Edge Wear de detalle MatFx, Ajustar, HBAO, etc.)
* &amp;lbrack;Shelf&amp;rbrack; Mapa de entorno de panorama predeterminado mejorado
* &amp;lbrack;Shelf&amp;rbrack; Nuevos ajustes preestablecidos de exportación de Arnold 5
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir la importación de recursos en el estante

**Problemas conocidos:**

* &amp;lbrack;Exportar&amp;rbrack; La edición de un ajuste preestablecido de exportación es muy lenta

## Versión 2

### 2.6.2

*(Lanzado: 20 de octubre de 2017)*

**Agregado:**

* &amp;lbrack;Conjunto de texturas&amp;rbrack; Permitir la eliminación de conjuntos de texturas deshabilitados
* &amp;lbrack;Shelf&amp;rbrack; Permitir que varios usuarios escriban dentro de la misma carpeta de la estantería
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Poder volver a cargar la carpeta de complementos
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Añada una versión mínima de API necesaria en los metadatos del plugin para garantizar la compatibilidad
* &amp;lbrack;IRay&amp;rbrack; Mejoras del cuadro de diálogo Exportar imagen

**Corregido:**

* &amp;lbrack;Motor&amp;rbrack; Problema de desaparición de trazos al cambiar la resolución (4K>2K)
* &amp;lbrack;Bakeres&amp;rbrack; Error al Hacer un bake la asignación de ID con la opción Coincidir por nombre activada
* &amp;lbrack;Bakeres&amp;rbrack; Los mensajes de error no son lo suficientemente explícitos
* &amp;lbrack;Vista 3D&amp;rbrack; El espacio tangente no se sincroniza con los bakeres
* &amp;lbrack;Herramienta&amp;rbrack; Artefactos negros al utilizar la herramienta de difuminado
* &amp;lbrack;Sombreador&amp;rbrack; El sombreador que no es PBR ya no funciona
* &amp;lbrack;Sombreador&amp;rbrack; &quot;recubierto de pbr&quot; está roto
* &amp;lbrack;Sombreador&amp;rbrack; La rugosidad del sombreador &quot;recubierto de pbr&quot; ya no tiene impacto
* &amp;lbrack;Sombreador&amp;rbrack; El sombreador del brillo de la especificación no coincide con Iray y SD
* &amp;lbrack;Shelf&amp;rbrack; Bloqueo al cargar dos archivos con el mismo nombre pero extensiones diferentes
* &amp;lbrack;Shelf&amp;rbrack; Ya no se pueden editar los ajustes preestablecidos en los estantes
* &amp;lbrack;Shelf&amp;rbrack; No se puede establecer una vista previa personalizada para los recursos importados en el estante
* Los recursos cargados desde la caché pierden sus usos
* Guardar un proyecto antes de crear una plantilla devuelve errores de permisos de escritura
* Guardado de proyecto incorrecto si el nombre de archivo contiene dos puntos
* Importación de archivos con varios puntos (.) en el nombre de archivo causa problemas

### 2.6.1

*(Lanzado: 12 de mayo de 2017)*

**Agregado:**

* &amp;lbrack;TextureSet&amp;rbrack; No permitir reasignar materiales de malla a nada

**Corregido:**

* Bloqueo al cambiar de TextureSet después de reemplazar mapa con bake
* Bloqueo al hacer &quot;Deshacer y Rehacer&quot; después de cambiar el modo de fusión de la capa
* Bloqueo o congelación al utilizar el efecto &quot;selección de color&quot; con mapa de ID grande
* &amp;lbrack;Exportar&amp;rbrack; Los conjuntos de texturas cuyo nombre se ha cambiado no se ordenan alfabéticamente en la ventana de exportación
* &amp;lbrack;TextureSet&amp;rbrack; Restablecer el nombre predeterminado no comprueba la unicidad
* &amp;lbrack;TextureSet&amp;rbrack; El conjunto de texturas renombrado se desactiva después de volver a abrir el proyecto
* &amp;lbrack;Shelf&amp;rbrack; Falta contenido de plantillas predeterminadas
* &amp;lbrack;Shelf&amp;rbrack; Las texturas no cuadradas se muestran como cuadradas
* &amp;lbrack;Sombreador&amp;rbrack; Cuando se desactiva un conjunto de texturas, se destruye el sombreador asociado
* &amp;lbrack;Secuencias de comandos&amp;rbrack; alg.haga un bake.setTextureSetBakingParameters() ya no funciona
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Tutorial de error tipográfico en websocket
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Varios problemas en AlgWidgets
* &amp;lbrack;Registro&amp;rbrack; Detección incorrecta de memoria virtual disponible en algunos casos

### 2.6.0

*(Lanzado: 27 de abril de 2017)*

**Agregado:**

* Agregar nuevo proyecto de muestra &quot;Meet Mat&quot;
* &amp;lbrack;Complemento&amp;rbrack; Nuevo plugin &quot;Resources Updater&quot;
* &amp;lbrack;TextureSet&amp;rbrack; Permitir cambiar el nombre y añadir una descripción a los conjuntos de texturas
* &amp;lbrack;TextureSet&amp;rbrack; Permitir reasignar materiales
* &amp;lbrack;TextureSet&amp;rbrack; Añadir un botón de configuración en la ventana de lista de conjuntos de texturas
* &amp;lbrack;TextureSet&amp;rbrack; Mostrar los conjuntos de texturas &quot;desactivados&quot; en la parte inferior de la lista
* &amp;lbrack;Substance&amp;rbrack; Utilice mapas adicionales con la resolución actual del conjunto de texturas para mejorar el rendimiento
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir actualizar un recurso utilizado en un proyecto (material, generador, etc.)
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Añadir una forma de añadir o quitar un estante
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir consultar información de recursos en proyectos
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir la recuperación de una lista de aplazamientos disponibles
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Tutorial de mejora de miniaturas de AlgWidget
* &amp;lbrack;Exportar&amp;rbrack; Desactivar o habilitar la profundidad de bits en función de la compatibilidad con el formato de archivo
* &amp;lbrack;Registro&amp;rbrack; Añadir nombre de complemento para imprimir en la consola
* &amp;lbrack;Registro&amp;rbrack; Quitar error sobre conjuntos de texturas ocultos
* Actualizar la pantalla de bienvenida con nuevos iconos y texto para los ejemplos

**Corregido:**

* Bloqueo al actualizar una malla en proyectos específicos
* &amp;lbrack;Viewport&amp;rbrack; El color interior del plano de simetría ya no es visible
* &amp;lbrack;Viewport&amp;rbrack; Algunos efectos posteriores al proceso se activan al utilizar la vista en solitario
* &amp;lbrack;Shaders&amp;rbrack; La fusión &quot;over_premult&quot; no funciona correctamente
* &amp;lbrack;Shaders&amp;rbrack; Advertencia sobre la prueba alfa con el sombreador predeterminado
* &amp;lbrack;Shelf&amp;rbrack; Análisis incorrecto de etiquetas de Substance
* &amp;lbrack;Shelf&amp;rbrack; El intemperismo del Óxido MatFX no funciona correctamente
* &amp;lbrack;Shelf&amp;rbrack; HSL filtro está activado en canales incorrectos de forma predeterminada
* &amp;lbrack;Shelf&amp;rbrack; El enfoque está activado en el canal Height/Normal de forma predeterminada
* &amp;lbrack;Exportar&amp;rbrack; Los distintos ajustes preestablecidos de exportación no utilizan un mapa de normales de OpenGL
* &amp;lbrack;Herramienta&amp;rbrack; Problemas de imprecisión al crear artefactos con la herramienta clonar/difuminar

### 2.5.3

*(Lanzado: 15 de marzo de 2017)*

**Corregido:**

* &amp;lbrack;Baker&amp;rbrack; Bloqueo al hacer un bake con mallas específicas

**Problemas conocidos:**

* &amp;lbrack;Mac&amp;rbrack; En algunos casos, las partículas pueden dañar la textura

### 2.5.2

*(Lanzado: 14 de marzo de 2017)*

**Corregido:**

* &amp;lbrack;Herramienta&amp;rbrack; Las tabletas Wacom no funcionan en Linux
* &amp;lbrack;Herramienta&amp;rbrack; Artefactos negros al utilizar la herramienta de difuminado
* &amp;lbrack;Bakeres&amp;rbrack; Error al hacer un bake si se utiliza Coincidir por nombre con una jaula
* &amp;lbrack;Bakeres&amp;rbrack; Oclusión ambiental rota al hacer un bake sólo con Mapa de normales
* &amp;lbrack;Shelf&amp;rbrack; Los filtros genéricos no controlan alfa correctamente (contraste/luminosidad, paso alto, etc.)
* &amp;lbrack;Viewport&amp;rbrack; Problema de rendimiento al cargar un proyecto con sombras activadas
* &amp;lbrack;Viewport&amp;rbrack; Problema de tramado en Vista 3D en MacOS
* &amp;lbrack;Viewport&amp;rbrack; Las previsualizaciones de objetos se muestran incorrectamente cuando el perfil de color está activado
* &amp;lbrack;Iray&amp;rbrack; Bloqueo al volver a cambiar el proyecto a OpenGL si Iray no se inicializa
* &amp;lbrack;IRay&amp;rbrack; El brillo se omite al procesar el sombreador SpecGloss/mdl
* &amp;lbrack;Sombreador&amp;rbrack; El sombreador de especificaciones/brillo no coincide con Iray y SD
* &amp;lbrack;Sombreador&amp;rbrack; Conversión de sRGB diferente de la conversión de LUT lineal a sRGB
* &amp;lbrack;Sombreador&amp;rbrack; Procesamiento incorrecto al cargar el proyecto con sombreadores obsoletos
* &amp;lbrack;Sombreador&amp;rbrack; los sombreadores &quot;recubiertos de pbr&quot; ya no funcionan
* &amp;lbrack;Exportar&amp;rbrack; Algunos canales aún se exportan aunque no estén presentes en el conjunto de texturas
* &amp;lbrack;Capas&amp;rbrack; El modo de fusión &quot;mapa de normales de detalles inversos&quot; no funciona en canales en escala de grises
* &amp;lbrack;UI&amp;rbrack; Problema en la &quot;ventana de selección de color&quot; con el monitor HDPI y el zoom de visualización al 150 %

**Problemas conocidos:**

* &amp;lbrack;Mac&amp;rbrack; En algunos casos, las partículas pueden dañar la textura

### 2.5.1

*(Lanzado: 27 de febrero de 2017)*

**Corregido:**

* &amp;lbrack;Mac&amp;rbrack; Entrada de la tableta Wacom rota en 3D y Vista 2D
* &amp;lbrack;Bakeres&amp;rbrack; La coincidencia por nombre ya no funciona
* &amp;lbrack;Bakeres&amp;rbrack; El ajuste &quot;Normales medias&quot; ya no funciona
* &amp;lbrack;Iray&amp;rbrack; Representación incorrecta con falta de mapa de normales hecho un bake
* &amp;lbrack;Iray&amp;rbrack; Los perfiles de color se comportan de forma diferente en comparación con el procesador OpenGL
* &amp;lbrack;Iray&amp;rbrack; Al exportar el procesamiento como mapa de bits no se incluye la corrección del perfil de color
* &amp;lbrack;Substance&amp;rbrack; Los Filtros de material ya no funcionan
* &amp;lbrack;Herramienta&amp;rbrack; La opacidad del trazo no se almacena en los ajustes preestablecidos del pincel
* &amp;lbrack;Herramienta&amp;rbrack; La alineación UV del pincel del Clonar ya no funciona
* &amp;lbrack;Exportar&amp;rbrack; El canal de desplazamiento debe estar centrado en 0,5 al exportar en entero
* &amp;lbrack;Plantilla&amp;rbrack; La ruta de acceso absoluta se almacena en Plantillas
* &amp;lbrack;TextureSet&amp;rbrack; La textura del canal persiste después de quitar el canal

**Problemas conocidos:**

* &amp;lbrack;Linux&amp;rbrack; Las entradas de tabletas Wacom no funcionan en 3D ni en Vista 2D
* &amp;lbrack;Mac&amp;rbrack; En algunos casos, las partículas pueden dañar la textura
* &amp;lbrack;Exportar&amp;rbrack; En casos muy raros, pueden aparecer rectángulos negros en las GPU AMD

### 2.5.0

*(Lanzado: 21 de febrero de 2017)*

**Agregado:**

* Compatibilidad añadida para las GPU AMD Radeon Pro y AMD FirePro
* &amp;lbrack;Herramienta&amp;rbrack; Añadir compatibilidad con la opacidad del trazo
* &amp;lbrack;Herramienta&amp;rbrack; Agregue un modificador que permita continuar con el último trazo de pincel
* &amp;lbrack;Iray&amp;rbrack; Actualización compatible con las GPU Pascal
* &amp;lbrack;Viewport&amp;rbrack; Añadir compatibilidad con perfiles de color (LUT)
* &amp;lbrack;Substance&amp;rbrack; Integrar nuevo marco (motor SD6)
* &amp;lbrack;UI&amp;rbrack; Aumentar la lista de tamaño de &quot;archivo reciente&quot; en el menú Archivo
* &amp;lbrack;Importar&amp;rbrack; Usar categoría de sustancias para rellenar el prefijo en el cuadro de diálogo de importación
* &amp;lbrack;Bakeres&amp;rbrack; Permitir hacer un bake texturas 8K
* &amp;lbrack;Bakeres&amp;rbrack; Permitir hacer un bake resoluciones que no sean cuadradas
* &amp;lbrack;Bakeres&amp;rbrack; Mejorar el consumo de memoria al hacer un bake mallas pesadas de alto contenido de polietileno
* &amp;lbrack;Shelf&amp;rbrack; Bloquear estantes (y proyectos) para prohibir la edición simultánea y evitar daños
* &amp;lbrack;Shelf&amp;rbrack; Leer categorías y palabras clave de sustancias para utilizarlas en el filtrado
* &amp;lbrack;Shelf&amp;rbrack; Permitir excluir recursos del resultado de una consulta de búsqueda
* &amp;lbrack;Shelf&amp;rbrack; Cálculo del tiempo de miniaturas mejorado
* &amp;lbrack;Shelf&amp;rbrack; Permitir insertar ajustes preestablecidos en proyectos
* &amp;lbrack;Shelf&amp;rbrack; Permitir contraer o expandir rápidamente la vista de árbol con MAYÚS
* &amp;lbrack;Shelf&amp;rbrack; Permitir guardar miniaturas cuando los recursos son de solo lectura (caché local)
* &amp;lbrack;Shelf&amp;rbrack; Nuevo contenido : nuevos filtros (transformar, espejo, tri-plana, etc.)
* &amp;lbrack;Shelf&amp;rbrack; Nuevo contenido : nuevos perfiles de LUT (clásicos y artísticos, como Film Noir, Vintage, etc.)
* &amp;lbrack;Shelf&amp;rbrack; Nuevo contenido : 10 nuevos Substance de fuentes para generar rápidamente textos personalizados
* &amp;lbrack;Shelf&amp;rbrack; Nuevas plantillas : Unity 5 y Unreal Engine 4
* &amp;lbrack;Shelf&amp;rbrack; Filtro de HSL mejorado para facilitar la labor de los artistas
* &amp;lbrack;Sombreador&amp;rbrack; Añadir compatibilidad para el canal de specular level en sombreadores PBR
* &amp;lbrack;Sombreador&amp;rbrack; Añadir soporte para tramado en sombreador de prueba de Alpha
* &amp;lbrack;Sombreador&amp;rbrack; Añadir compatibilidad para la asignación de oclusión de paralaje en sombreadores PBR
* &amp;lbrack;Sombreador&amp;rbrack; Permitir definir la interfaz de usuario personalizada para los parámetros de sombreador
* &amp;lbrack;MatLayering&amp;rbrack; Creación de un nuevo canal de máscara para el flujo de trabajo de capas de material
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir escribir metadatos en un proyecto de SP
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir la exportación con un ajuste preestablecido de exportación específico
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir recuperar parámetros de sombreador como JSON
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Agregar compatibilidad para conexiones WebSocket
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Añadir la posibilidad de cargar instancias del sombreador
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Añadir la posibilidad de crear un nuevo proyecto
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir recuperar la dirección URL de la malla importada en un proyecto
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir hagas un bake no cuadrados
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Informar de errores al configurar datos mediante la API de scripts
* &amp;lbrack;Substance&amp;rbrack; Agregar etiqueta de datos de usuario para especificar el formato de mapa de normales

**Corregido:**

* Bloqueo al elegir color con substancias
* Bloqueo al cargar una imagen que no es RGBA32f como mapa de entorno
* Bloqueo relacionado con la pintura en GPU AMD
* &amp;lbrack;Malla&amp;rbrack; OBJ importación no reconoce materiales sin el archivo mtl
* &amp;lbrack;Malla&amp;rbrack; La generación del nombre del conjunto de texturas de UDIM puede ser incorrecta en algunas mallas
* &amp;lbrack;UI&amp;rbrack; El botón Deshacer/Rehacer de la configuración del visor roba el foco y detiene el desplazamiento del ratón
* &amp;lbrack;UI&amp;rbrack; Algunas etiquetas se recortan incorrectamente en High-DPI
* &amp;lbrack;Capa&amp;rbrack; El efecto Reemplazar modo de pintura tiene un comportamiento incorrecto en Máscara
* &amp;lbrack;Capa&amp;rbrack; El modo de fusión de Restar se comporta de forma incorrecta con alfa
* &amp;lbrack;Herramienta&amp;rbrack; El tamaño del pincel se vuelve enorme en vista 2D al pintar sobre bordes UV
* &amp;lbrack;Herramienta&amp;rbrack; La línea recta ajustada tiene un comportamiento errático con High-DPI
* &amp;lbrack;Herramienta&amp;rbrack; La resolución de la galería de símbolos a veces es incorrecta
* &amp;lbrack;Bakeres&amp;rbrack; Los valores de &quot;Distancia máxima del oclusor&quot; se fijan si &quot;relativo al cuadro delimitador&quot; está &quot;Desactivado&quot;
* &amp;lbrack;Sombreador&amp;rbrack; Las definiciones de canal de pilas y parámetros automáticos no coinciden
* &amp;lbrack;Vista 3D&amp;rbrack; Visualización incoherente del canal normal según la configuración del proyecto
* &amp;lbrack;Viewport&amp;rbrack; Algunos mapas de normales tienen valores cerrados que aparecen como artefactos
* &amp;lbrack;Viewport&amp;rbrack; Los efectos posteriores siempre están desactivados de forma predeterminada
* &amp;lbrack;Exportar&amp;rbrack; El ajuste de mezcla normal es incorrecto si falta el canal normal
* &amp;lbrack;Exportar&amp;rbrack; Generación de texturas incorrecta en algunos casos en GPU AMD
* &amp;lbrack;Exportar&amp;rbrack; Los parámetros de sombreador no se exportan correctamente si están ubicados dentro de un grupo
* &amp;lbrack;Exportar&amp;rbrack; La edición de un ajuste preestablecido de exportación en una estantería personalizada genera un error de registro
* &amp;lbrack;Shelf&amp;rbrack; El filtrado de vista de árbol no coincide exactamente con el nombre de la carpeta
* &amp;lbrack;Shelf&amp;rbrack; Cambiar el nombre de un ajuste preestablecido de estantería es difícil de leer
* &amp;lbrack;Shelf&amp;rbrack; El recurso de sombreador importado en la estantería no se conserva después de reiniciar
* &amp;lbrack;Shelf&amp;rbrack; Contenido : Falta el ajuste preestablecido de la herramienta Soldadura
* &amp;lbrack;Shelf&amp;rbrack; Contenido : El Tile Generator no funciona correctamente
* &amp;lbrack;Shelf&amp;rbrack; Contenido : Se ha corregido una máscara incorrecta en el material inteligente sucio del neumático de goma
* &amp;lbrack;Shelf&amp;rbrack; Contenido : Se ha corregido un nombre de grupo incorrecto en el material de la bolsa de cuero
* &amp;lbrack;Iray&amp;rbrack; La mitad de las mallas están desaparecidas en Irán
* &amp;lbrack;Linux&amp;rbrack; Bloqueo al arrastrar un recurso por encima del Vista 3D
* &amp;lbrack;Mac&amp;rbrack; Las preferencias se restablecen en cada inicio en Sierra

**Problemas conocidos:**

* &amp;lbrack;Exportar&amp;rbrack; En casos muy raros, pueden aparecer rectángulos negros en las GPU AMD
* &amp;lbrack;Iray&amp;rbrack; Los perfiles de color pueden comportarse de formas extrañas en ocasiones

### 2.4.1

*(Lanzado: 28 de octubre de 2016)*

**Corregido:**

* Bloqueo al crear un proyecto con una plantilla
* Bloqueo al cerrar el cuadro de diálogo de exportación durante una exportación
* &amp;lbrack;Mac&amp;rbrack; Errores al guardar el proyecto (error al guardar el ajuste preestablecido de exportación)
* &amp;lbrack;Shelf&amp;rbrack; Al crear un nuevo ajuste preestablecido, este se mostrará dos veces
* &amp;lbrack;Shelf&amp;rbrack; Los ajustes preestablecidos no se pueden cargar en modo de solo lectura sin derechos de administrador

### 2.4.0

*(Lanzado: 27 de octubre de 2016)*

**Agregado:**

* &amp;lbrack;Shelf&amp;rbrack; Nueva interfaz para examinar recursos (vista de árbol, filtros, etc.)
* &amp;lbrack;Shelf&amp;rbrack; Permitir guardar una búsqueda como un ajuste preestablecido
* &amp;lbrack;Shelf&amp;rbrack; Permitir la creación de una nueva ventana a partir de un ajuste preestablecido
* &amp;lbrack;Shelf&amp;rbrack; Nueva interfaz para importar recursos
* &amp;lbrack;Shelf&amp;rbrack; No copiar la estantería algorítmica predeterminada en la carpeta Documentos
* &amp;lbrack;Shelf&amp;rbrack; Nuevos ajustes preestablecidos de partículas : Circuito eléctrico, Líneas eléctricas, Rococó, Venas pequeñas
* &amp;lbrack;Shelf&amp;rbrack; Se han mejorado los ajustes preestablecidos de partículas antiguas para que sean más fáciles de usar (como &quot;Lluvia&quot;).
* &amp;lbrack;Shelf&amp;rbrack; Agregar nueva información en el menú contextual de recursos
* &amp;lbrack;Viewport&amp;rbrack; Mejorar el rendimiento al cargar mapas de entorno
* &amp;lbrack;Viewport&amp;rbrack; Agregar compatibilidad con mapas de entorno que no sean potencia de dos

**Corregido:**

* Bloqueo al quitar una máscara
* Bloqueo al pintar después de guardar un ajuste preestablecido
* Bloqueo con el desenfoque de entorno en algunas GPU
* Bloqueo al asignar un recurso incorrecto con el estante mini
* &amp;lbrack;Shelf&amp;rbrack; Limpiar y guardar eliminar etiquetas y metadatos para los recursos del proyecto
* &amp;lbrack;Shelf&amp;rbrack; al importar un ajuste preestablecido, sus recursos se mostrarán en el estante
* &amp;lbrack;Exportar&amp;rbrack; El mapa de normales generado a partir del canal de height tiene una intensidad baja
* &amp;lbrack;Exportar&amp;rbrack; La malla normal no siempre está presente en el mapa de normales final
* &amp;lbrack;Exportar&amp;rbrack; La dilación con la transparencia puede resultar a veces sin transparencia
* &amp;lbrack;Secuencias de comandos&amp;rbrack; &quot;alg.plugin_root_directory&quot; puede devolver una ruta de red truncada
* &amp;lbrack;TextureSet&amp;rbrack; El botón Bloquear se activa al volver a abrir proyectos no cuadrados

### 2.3.1

*(Lanzado: 07 de octubre de 2016)*

**Agregado:**

* &amp;lbrack;Complemento&amp;rbrack;&amp;lbrack;Photoshop&amp;rbrack; Permitir especificar qué material/pila/canales se van a exportar
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Los nombres de función tienen algunas incoherencias

**Corregido:**

* &amp;lbrack;Exportar&amp;rbrack; Alpha se puede descartar en los ajustes preestablecidos de exportación personalizados
* &amp;lbrack;Exportar&amp;rbrack; El Alpha obtiene una conversión de gamma incorrecta en canales sRGB
* &amp;lbrack;Exportar&amp;rbrack; Los documentos no cuadrados se exportan como cuadrados
* &amp;lbrack;Exportar&amp;rbrack; Imposible exportar mapas adicionales si falta uno
* &amp;lbrack;Iray&amp;rbrack; Algunos parámetros (como la intensidad del emisivo) no tienen ningún efecto
* &amp;lbrack;NVIDIA&amp;rbrack; Bloqueo al inicio con NVIDIA Quadro K2200/GTX 750/760
* &amp;lbrack;AMD&amp;rbrack; Conjunto de colores incorrecto para miniaturas y previsualizaciones
* &amp;lbrack;AMD&amp;rbrack; Bloqueos y error del controlador al abrir archivos nuevos y abiertos
* &amp;lbrack;Registro&amp;rbrack; Falta &quot;software-version&quot; en el archivo de registro

### 2.3.0

*(Lanzado: 15 de septiembre de 2016)*

**Agregado:**

* &amp;lbrack;Complemento&amp;rbrack; Nuevo plugin &quot;Exportar a Photoshop&quot; (exportar pila de capas completa)
* &amp;lbrack;Exportar&amp;rbrack; Permitir especificar la anchura del relleno (en píxeles o infinito)
* &amp;lbrack;Exportar&amp;rbrack; Permitir establecer el tipo de fondo fuera de las UV
* &amp;lbrack;Shelf&amp;rbrack; Sombreador de capas de material nuevo para mezclar 10 materiales
* &amp;lbrack;Shelf&amp;rbrack; Nuevo sombreador de arcilla para ver los detalles con el canal height/normal
* &amp;lbrack;Shelf&amp;rbrack; Nuevo filtro de iluminación hecho un bake con entrada de entorno
* &amp;lbrack;Shelf&amp;rbrack; Se han actualizado algunos generadores de máscaras para añadir transformaciones que no son cuadradas
* &amp;lbrack;Viewport&amp;rbrack; Añadir mapa de normales compuesto (normal+height+hacer un bake) al modo solo
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir la exportación de mapas adicionales
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir consultar mapas adicionales disponibles por conjunto de texturas
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir recuperar formato de canal
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Añadir ejemplos en la documentación que hace un bake
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir consultar la visibilidad de una capa
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir consultar el modo de fusión y la opacidad de la capa
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir la exportación de mapas convertidos (mapas de normales finales, archivos AO mixtos, etc.)
* &amp;lbrack;Substance&amp;rbrack; Leer y conectar usos personalizados
* &amp;lbrack;Atajos&amp;rbrack; Agregar tecla modificadora (MAYÚS) para retroceder en el modo solo cíclico
* &amp;lbrack;Exportar&amp;rbrack; Se ha actualizado el ajuste preestablecido de exportación predeterminado para desactivar alfa
* &amp;lbrack;UI&amp;rbrack; Las miniaturas ahora solo se calculan si el motor está disponible
* &amp;lbrack;UI&amp;rbrack; Mostrar una mención cuando las miniaturas se estén calculando

**Corregido:**

* Bloqueo con algunos proyectos antiguos al abrirlos
* Bloqueo con caché de canales de textura dañada
* Bloqueo al mezclar más de 4 materiales con el flujo de trabajo de capas de material
* &amp;lbrack;UI&amp;rbrack; Los métodos abreviados de herramientas no funcionan si la barra de herramientas está oculta
* &amp;lbrack;UI&amp;rbrack; La barra de herramientas de Iray se etiqueta como &quot;Sin título&quot; en el menú Ver
* &amp;lbrack;UI&amp;rbrack; Las barras de herramientas del complemento se denominan &quot;Sin inclinar&quot; en el menú Ver
* &amp;lbrack;Baker&amp;rbrack; Al pulsar Intro mientras se edita un ajuste de hacer un bake, se inicia el proceso de hacer un bake
* &amp;lbrack;Baker&amp;rbrack; Rangos incorrectos para algunos parámetros
* &amp;lbrack;Importar&amp;rbrack; Imposible importar OBJ mallas debido a números muy grandes
* &amp;lbrack;Importar&amp;rbrack; Algunos archivos OBJ se importan con demasiados subobjetos
* &amp;lbrack;Exportar&amp;rbrack; el fondo del canal se rellena con negro en lugar del color predeterminado en la exportación
* &amp;lbrack;Herramienta&amp;rbrack; Las partículas no funcionan correctamente si FOV es demasiado bajo
* &amp;lbrack;Herramienta&amp;rbrack; El color de previsualización del pincel es incorrecto con las máscaras en subpilas
* &amp;lbrack;Viewport&amp;rbrack; Cuando el pincel entra en áreas vacías de la Vista 2D se vuelve gigantesco
* &amp;lbrack;Viewport&amp;rbrack; Vista previa del pincel en blanco al pintar texturas normales
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Documentación incorrecta : &quot;ao&quot; en lugar de &quot;ambientocclusion&quot;
* &amp;lbrack;Secuencias de comandos&amp;rbrack; El proceso iniciado con subprocess() se mata al cerrar Painter
* &amp;lbrack;Shelf&amp;rbrack; El filtro de iluminación hecho un bake utiliza una entrada de AO incorrecta
* &amp;lbrack;MacOS&amp;rbrack; Se ha eliminado el proyecto Fire Hydrant (incompatible)
* El proyecto predeterminado se abre al cargar un archivo \*.spt (en lugar de \*.spp)

**Problemas conocidos:**

* &amp;lbrack;Complemento&amp;rbrack; Debido a Photoshop, el height y el canal normal no se pueden traducir tal cual

### 2.2.0

*(Lanzado: 22 de julio de 2016)*

**Agregado:**

* &amp;lbrack;Shelf&amp;rbrack; Mejorar el sistema de búsqueda y las consultas
* &amp;lbrack;Shelf&amp;rbrack; Añadir campo de búsqueda para miniestantes
* &amp;lbrack;Sombreador&amp;rbrack; Permitir definir la precisión de paso de los reguladores
* &amp;lbrack;Sombreador&amp;rbrack; Añadir un botón Deshacer/Rehacer para parámetros de sombreador
* &amp;lbrack;Sombreador&amp;rbrack; La recarga de un sombreador no debe restablecer sus parámetros
* &amp;lbrack;MatLayering&amp;rbrack; Añadir compatibilidad con Controles dinámicos de capas de materiales y subpilas
* &amp;lbrack;MatLayering&amp;rbrack; Permitir la importación de archivos json para configurar los ajustes de sombreador
* &amp;lbrack;MatLayering&amp;rbrack; Desbloquear límite de muestras de textura (cambiar a texturas sin enlace)
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir definir la configuración de bakeres e iniciar su cálculo
* &amp;lbrack;Substance&amp;rbrack; Usar &quot;uso&quot; para conexiones de entrada/salida además de identificadores
* &amp;lbrack;Herramienta&amp;rbrack; Permitir seleccionar el canal de previsualización en la ventana gráfica para la herramienta Proyección

**Corregido:**

* Bloqueo durante el lanzamiento si las sustancias se encuentran en una carpeta incorrecta
* El informe de bloqueo a veces no funciona debido a un archivo de registro incorrecto
* &amp;lbrack;Iray&amp;rbrack; Los efectos de posprocesamiento no se actualizan cuando Iray está en pausa
* &amp;lbrack;Iray&amp;rbrack; El método abreviado de enfoque automático ya no funciona
* &amp;lbrack;Iray&amp;rbrack; El comportamiento del regulador de apertura cambia en función del tamaño del recurso
* &amp;lbrack;Capas&amp;rbrack; El primer canal de materiales no está activado de forma predeterminada si todos están desactivados
* &amp;lbrack;Sombreador&amp;rbrack; No se imprimen errores si un &quot;param auto&quot; es incorrecto

**Problemas conocidos:**

* &amp;lbrack;Mac&amp;rbrack; El límite de muestras de textura está bloqueado en 16 (problema de controlador de GPU)

### 2.1.1

*(Lanzado: 01 de julio de 2016)*

**Agregado:**

* &amp;lbrack;Licencia&amp;rbrack; Poder cambiar la ubicación del archivo de licencia
* &amp;lbrack;Viewport&amp;rbrack; Añada un método abreviado &quot;B&quot; para desplazarse entre mapas adicionales
* &amp;lbrack;Importar&amp;rbrack; Permitir la importación FBX 2016/2017 correctamente
* &amp;lbrack;Herramienta&amp;rbrack; Quitar fichas al utilizar la máscara rápida
* &amp;lbrack;Iray&amp;rbrack; Añadir información de dimensiones de escena
* &amp;lbrack;Iray&amp;rbrack; Permitir aumentar el número máximo de muestras y el tiempo de procesamiento
* &amp;lbrack;UI&amp;rbrack; Actualizar el resultado inmediatamente al utilizar el botón +/- en los reguladores
* &amp;lbrack;UI&amp;rbrack; Permitir una mayor precisión para los reguladores de escala de grises
* &amp;lbrack;Exportar&amp;rbrack; No exportar un canal alfa para texturas que sean solo RGB
* &amp;lbrack;Exportar&amp;rbrack; Actualizar ajuste preestablecido de exportación de Dota 2
* &amp;lbrack;Shelf&amp;rbrack; Nuevo patrón de &quot;azulejos hexagonales&quot;
* &amp;lbrack;Shelf&amp;rbrack; Nueva herramienta &quot;Soldadura&quot;
* &amp;lbrack;Shelf&amp;rbrack; Filtros de acabado actualizados para proporcionar controles de dirección

**Corregido:**

* &amp;lbrack;Exportar&amp;rbrack; Imposible exportar archivos de PSD en 8 bits
* &amp;lbrack;Exportar&amp;rbrack; La exportación en 8K no está disponible en algunas configuraciones de hardware
* &amp;lbrack;Exportar&amp;rbrack; La ventana de Sketchfab se recorta
* &amp;lbrack;Exportar&amp;rbrack; Mapa de rugosidad incorrecto en el ajuste preestablecido de exportación de especificación/brillo
* &amp;lbrack;UI&amp;rbrack; Escribir en los reguladores de escala de grises ya no funciona
* &amp;lbrack;UI&amp;rbrack; Imposible colocar filtros en entradas de sustancias (como Generadores)
* &amp;lbrack;UI&amp;rbrack; Algunos reguladores tienen comportamientos extraños
* &amp;lbrack;UI&amp;rbrack; El paso DeltaTime +/- para partículas es demasiado grande
* &amp;lbrack;Iray&amp;rbrack; Algunos proyectos bloquean la aplicación al cambiar a Irak
* &amp;lbrack;Iray&amp;rbrack; Bloqueo al detectar hardware
* &amp;lbrack;Herramienta&amp;rbrack; El color de previsualización del pincel es incorrecto en el modo Máscara
* &amp;lbrack;Herramienta&amp;rbrack; El selector de material se puede utilizar con herramientas incompatibles
* &amp;lbrack;Herramienta&amp;rbrack; La previsualización de proyección no cambia a Difuso con el flujo de trabajo de especificación/brillo
* &amp;lbrack;Shelf&amp;rbrack; Al cambiar el sombreador predeterminado, se rompen las previsualizaciones de máscaras inteligentes y alfombras inteligentes
* &amp;lbrack;Shelf&amp;rbrack; Algunos materiales inteligentes tienen nombres incorrectos
* &amp;lbrack;Shelf&amp;rbrack; Las formas alfa adicionales están dañadas y no se cargarán
* &amp;lbrack;Viewport&amp;rbrack; Cambio al modo &quot;Mapa adicional&quot; para mostrar primero &quot;otro&quot;
* &amp;lbrack;Viewport&amp;rbrack; La ventana gráfica vuelve a cambiar a &quot;otro&quot; cuando no existe un mapa adicional
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; El informe de bloqueo no funciona en Ubuntu (Steam)
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; Los vínculos de URL web no funcionan en Ubuntu (Steam)
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Quitar &quot;Crashwatcher&quot; cuando Substance Painter ya no corra
* &amp;lbrack;Bloqueo&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; El sistema de informes de bloqueos no funciona correctamente
* &amp;lbrack;Bloqueo&amp;rbrack; La importación de una malla al importar una malla ya genera un bloqueo
* El conjunto de texturas que recoge el método abreviado se restablece en nada después de reiniciar

### 2.1.0

*(Lanzado: 02 de junio de 2016)*

**Agregado:**

* &amp;lbrack;UDIM&amp;rbrack; Importación de mosaicos UDIM de una malla como conjuntos de texturas
* &amp;lbrack;Linux&amp;rbrack; Se ha agregado la compatibilidad con CentOS 6.6 y Ubuntu 12.4
* &amp;lbrack;Exportar&amp;rbrack; Añadir resolución 8K (experimental)
* &amp;lbrack;Exportar&amp;rbrack; Permitir la selección de la profundidad de bits durante la exportación
* &amp;lbrack;Baker&amp;rbrack; Permitir hacer un bake varios conjuntos de texturas a la vez
* Compatibilidad con monitores de alta resolución (escala de PPP alta)
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Establecer resolución y relleno personalizados por textura en la exportación
* &amp;lbrack;Viewport&amp;rbrack; Permitir cambiar entre el conjunto de texturas haciendo clic en la malla (mediante Ctrl+Alt+Clic)
* &amp;lbrack;Viewport&amp;rbrack; Ir a donde se encuentra el cursor del ratón al hacer zoom con la rueda del ratón
* &amp;lbrack;UI&amp;rbrack; Actualizar el color de fondo predeterminado y la visualización del mapa de entorno
* &amp;lbrack;UI&amp;rbrack; Añadir información sobre herramientas con nombres originales para los canales de usuario
* &amp;lbrack;UI&amp;rbrack; Cambiar el color de fondo de los canales a los que no se puede cambiar el nombre
* &amp;lbrack;Herramienta&amp;rbrack; Quitar fichas al utilizar la máscara rápida
* &amp;lbrack;Sombreador&amp;rbrack; Permitir definir grupos para parámetros de sombreador y materiales/máscaras
* &amp;lbrack;Motor&amp;rbrack; Optimización del estampado de tamaño pequeño
* &amp;lbrack;Stencil&amp;rbrack; Añada &quot;W&quot; como método abreviado para cambiar temporalmente la máscara
* &amp;lbrack;Shelf&amp;rbrack; Agregue un botón de cruz para borrar el campo de búsqueda
* &amp;lbrack;Shelf&amp;rbrack; Cargar el Alpha con un solo clic
* &amp;lbrack;Shelf&amp;rbrack; Nuevo ajuste preestablecido de exportación : UDIM Vray, Arnold UDIM, Especificación/Brillo de Metal/Rugoso
* &amp;lbrack;Shelf&amp;rbrack; Nuevas alfas : formas geométricas, vetas y signos
* Agregar nombre y versión en las propiedades del ejecutable de Substance Painter

**Corregido:**

* &amp;lbrack;Substance&amp;rbrack; Imposible utilizar el canal normal y el mapa adicional al mismo tiempo
* &amp;lbrack;Iray&amp;rbrack; La refracción de MDL y el ajuste de absorción no funcionan
* &amp;lbrack;Iray&amp;rbrack; La escala de escena original no se conserva
* &amp;lbrack;Shelf&amp;rbrack; Plantilla de specular/Brillo que usa un sombreador incorrecto
* &amp;lbrack;Exportar&amp;rbrack; El ajuste preestablecido de exportación predeterminado no exporta algunos mapas (como AO)
* &amp;lbrack;Viewport&amp;rbrack; El punto de tabla dinámica no se actualiza al hacer clic fuera de las coordenadas UV en la vista 2D
* &amp;lbrack;UI&amp;rbrack; Los valores del regulador se redondean
* &amp;lbrack;UI&amp;rbrack; A veces, al editar los valores de los reguladores, hay un espacio libre muy pequeño
* &amp;lbrack;Nuevo proyecto&amp;rbrack; La lista desplegable de plantillas no se ha actualizado correctamente (de 1.x a 2.x)
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Se ha corregido el comportamiento de &quot;pasar cursor&quot; en los botones personalizados
* &amp;lbrack;Mac&amp;rbrack; La acción de deshacer en un proyecto vacío bloquea la cámara

**Problemas conocidos:**

* El informe de bloqueo no está disponible en Ubuntu
* Es posible que algunos botones de URL no funcionen. Consulta nuestras preguntas frecuentes para obtener una solución alternativa

### 2.0.5

*(Lanzado: 29 de abril de 2016)*

**Agregado:**

* &amp;lbrack;Shelf&amp;rbrack; Se ha agregado o actualizado una plantilla que no es de pbr, sombreador y ajuste preestablecido de exportación
* &amp;lbrack;Shelf&amp;rbrack; Se ha actualizado el ajuste preestablecido de exportación UE4 para incluir Oclusión ambiental

**Corregido:**

* Bloqueo al abrir y guardar algunos proyectos con recursos dañados
* &amp;lbrack;Viewport&amp;rbrack; La malla metálica parece rota en la Vista 2D
* &amp;lbrack;Shelf&amp;rbrack; Rendimiento mejorado de algunos mapas de entorno de estudio
* &amp;lbrack;Shelf&amp;rbrack; Se duplican algunos mapas de entorno de estudio
* &amp;lbrack;Shelf&amp;rbrack; Falta &quot;Material de iluminación Hecho un bake&quot;
* &amp;lbrack;Shelf&amp;rbrack; Falta el generador de conversión de escala de grises

### 2.0.4

*(Lanzado: 26 de abril de 2016)*

**Agregado:**

* Mejora de los choques de malla y optimiza la representación de mallas metálicas
* Mejorar el rendimiento y la gestión de la memoria con grandes proyectos
* Mejorar la precisión y el paso del regulador
* &amp;lbrack;UI&amp;rbrack; Actualizar el motor sólo al validar un regulador (no al introducir un valor)
* &amp;lbrack;UI&amp;rbrack; Mover Iray cambiar a un botón dedicado en la barra de herramientas principal (y cambiar su método abreviado)
* &amp;lbrack;Herramienta&amp;rbrack; Añadir configuración para el comportamiento de ubicación de origen de la herramienta de clonación
* &amp;lbrack;Sombreador&amp;rbrack; Permitir la lectura de colores de vértices de malla en sombreadores personalizados
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permite recuperar la lista de conjuntos de texturas, canales y capas
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Añadir funciones auxiliares (url a ruta, obtener ruta de exportación desde proyecto)
* &amp;lbrack;Mac&amp;rbrack; Detectar la versión &quot;El Capitan&quot; de Mac Os en el archivo de registro

**Corregido:**

* Bloqueo después de la segunda exportación a Substance share
* Bloqueo al copiar una capa entre conjuntos de texturas con datos de Máscara rápida.
* Algunos proyectos tienen un actualizador muy largo que consume mucha memoria
* &amp;lbrack;Herramienta&amp;rbrack; Bloqueo al seleccionar un ajuste preestablecido de partículas con la herramienta clonar/difuminar
* &amp;lbrack;Baker&amp;rbrack; La carga de FBX archivos tarda demasiado tiempo en cargar mallas pesadas
* &amp;lbrack;Viewport&amp;rbrack; Mapa de entorno estirado en algunos equipos
* &amp;lbrack;Viewport&amp;rbrack; Conversión de gamma incorrecta del alfa del pincel
* &amp;lbrack;Exportar&amp;rbrack; El Alpha se almacena como transparencia en lugar de un canal independiente con archivos Tiff.
* &amp;lbrack;Exportar&amp;rbrack; El canal normal siempre se exporta como OpenGL
* &amp;lbrack;Iray&amp;rbrack; Faltan nombres de reguladores para la configuración de Iray
* &amp;lbrack;Iray&amp;rbrack; El procesamiento se realiza con una resolución incorrecta en Retina/alta PPP
* &amp;lbrack;Iray&amp;rbrack; Bloqueo al cambiar el tamaño de la interfaz en modo Iray
* &amp;lbrack;Iray&amp;rbrack; Gran ralentización del rendimiento al renderizar en algunas resoluciones bajas
* &amp;lbrack;Iray&amp;rbrack; La pausa no funciona (Iray sigue calculando en segundo plano)
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

* &amp;lbrack;Iray&amp;rbrack; Actualizar la plantilla y el sombreador Spec/Gloss para que sean compatibles con Iray
* &amp;lbrack;Exportar&amp;rbrack; Exportar capturas de pantalla a ArtStation
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Ejecución de soporte desde el directorio de plugins
* &amp;lbrack;Secuencias de comandos&amp;rbrack; Permitir &quot;Guardar como&quot;
* &amp;lbrack;UI&amp;rbrack; Permitir hacer doble clic en un regulador para editar su valor
* Mover muestra de Vela al Substance share
* Nuevo proyecto de muestra : Previsualización de esfera
* Advertencia a los usuarios sobre el conflicto de extensión de shell

**Corregido:**

* El instalador anula la instalación de Substance Painter 1.x
* &amp;lbrack;UI&amp;rbrack; El diseño de la lista de canales se rompe con los filtros
* &amp;lbrack;UI&amp;rbrack; No se muestran los parámetros de sombreador
* &amp;lbrack;UI&amp;rbrack; Al cambiar el tamaño de la ventana de capa se recorta incorrectamente el contenido
* &amp;lbrack;Herramienta&amp;rbrack; El canal de opacidad no siempre se usa correctamente
* &amp;lbrack;Herramienta&amp;rbrack; El difuminado/Clonar no funciona con la Simetría
* &amp;lbrack;Herramienta&amp;rbrack; La opacidad de la vista previa del pincel es incorrecta en algunos canales
* &amp;lbrack;Iray&amp;rbrack; Bloqueo al usar Iray cuando todavía no se ha creado
* &amp;lbrack;Iray&amp;rbrack; No se pueden cargar datos de configuración de iris del proyecto
* &amp;lbrack;Iray&amp;rbrack; Iray no se ocupa de la modificación de la configuración después de haber sido pausado
* &amp;lbrack;Shelf&amp;rbrack; Importar un material al estante no funciona
* La galería de símbolos no funciona con el canal Normal
* Bloqueo al pintar en algunos proyectos
* Bloqueo al pintar con partículas en algunos proyectos
* Bloqueo con el Procesador de píxeles durante algunos cálculos

### 2.0.0

*(Lanzado: 16 de marzo de 2016)*

**Agregado:**

* Método abreviado a Substance Almacén en la barra de herramientas principal
* Procesador Iray con modo de visualización y exportación de capturas de pantalla
* Compatibilidad con la creación y el uso de &quot;Máscaras inteligentes&quot;
* Compatibilidad con el flujo de trabajo de PBR de Specular y glosinas (con el nuevo canal difuso)
* Encadenamiento de Substance (enchufe de sustancias en las entradas de imagen de sustancias)
* Compatibilidad de scripts con complementos personalizados
* Mejorar la conversión de Height a Normal utilizando un filtro Sobel
* Cambiar resolución de previsualización de proyección/galería de símbolos a 2K
* Agregar canal normal de forma predeterminada para proyectos nuevos
* Leer la etiqueta de datos de usuario del nodo de salida para activar o desactivar canales de una sustancia de forma predeterminada
* Exponer fusión Normal/AO en ajustes de TextureSet
* &amp;lbrack;Herramienta&amp;rbrack; Nueva herramienta de difuminado para fusionar y difundir colores
* &amp;lbrack;Herramienta&amp;rbrack; Nueva herramienta de Clonar para copiar parte de las texturas
* &amp;lbrack;Herramienta&amp;rbrack; Permitir la selección de canales para la herramienta de difuminado, Clonar y Borrador
* &amp;lbrack;Capa&amp;rbrack; Añadir nombre de Substance para el nombre del efecto Rellenar
* &amp;lbrack;Capa&amp;rbrack; Permitir exportar la máscara al portapapeles
* &amp;lbrack;Viewport&amp;rbrack; Cambiar entre el modo de Perspectiva y el ortográfico
* &amp;lbrack;Viewport&amp;rbrack; Permitir el control del campo de visión en el modo de Perspectiva
* &amp;lbrack;Viewport&amp;rbrack; Permitir definir la Profundidad de la distancia del campo con CTRL+clic central
* &amp;lbrack;Viewport&amp;rbrack; Permita arrastrar y soltar mapas de entorno en el Vista 3D.
* &amp;lbrack;Viewport&amp;rbrack; Se han mejorado los comentarios cuando el motor realiza cálculos potentes.
* &amp;lbrack;Exportar&amp;rbrack; Permitir la exportación de parámetros de sombreador en un archivo json
* &amp;lbrack;UI&amp;rbrack; Interfaz de actualización con nuevos iconos, colores y diseño
* &amp;lbrack;UI&amp;rbrack; Añadir nombres de recursos a los miniestantes
* &amp;lbrack;UI&amp;rbrack; Contraer &quot;asignación de canales&quot; de forma predeterminada
* &amp;lbrack;Sombreador&amp;rbrack; Selección de un color personalizado para los parámetros de textura de sombreador
* &amp;lbrack;Shelf&amp;rbrack; Preguntar dónde importar archivos al arrastrar y soltar recursos
* &amp;lbrack;Shelf&amp;rbrack; Nueva esfera de previsualización para Materiales inteligentes y generadores
* &amp;lbrack;Shelf&amp;rbrack; Añadir sombreador de Brillo de Specular
* &amp;lbrack;Shelf&amp;rbrack; Nuevas formas de superficie dura
* &amp;lbrack;Shelf&amp;rbrack; Nuevas formas y texturas de Alpha
* &amp;lbrack;Shelf&amp;rbrack; Nuevas texturas de piel
* &amp;lbrack;Shelf&amp;rbrack; Nuevos materiales basados en Scan y materiales inteligentes
* &amp;lbrack;Shelf&amp;rbrack; Nuevos materiales inteligentes y compatibilidad con especificaciones/brillo de los antiguos
* &amp;lbrack;Shelf&amp;rbrack; Nuevos filtros de acabado para la simulación de superficies metálicas
* &amp;lbrack;Shelf&amp;rbrack; Nuevo generador de máscaras potente &quot;Mask Editor&quot;
* &amp;lbrack;Shelf&amp;rbrack; Materiales antiguos retrabajados y limpiados
* Nuevo proyecto de muestra &quot;Vela&quot;

**Corregido:**

* &amp;lbrack;Configuración&amp;rbrack; El proyecto anula la rotación de la cámara y la velocidad de zoom
* &amp;lbrack;Viewport&amp;rbrack; Un problema de precisión en la textura normal predeterminada genera reflejos incorrectos
* &amp;lbrack;Viewport&amp;rbrack; Viñeta está activada de forma predeterminada
* &amp;lbrack;Viewport&amp;rbrack; Aparecen artefactos en los bordes del mapa de entorno (GPU de NVIDIA)
* &amp;lbrack;Viewport&amp;rbrack; La miniatura en modo de proyección/galería de símbolos es muy larga de cargar
* &amp;lbrack;Baker&amp;rbrack; Almacenar texturas hechas un bake en un entero de 16 bits en lugar de 32 bits
* &amp;lbrack;Capa&amp;rbrack; Las sustancias obsoletas se muestran incorrectamente en la pila
* El color predeterminado y la profundidad de bits de algunos canales son incorrectos (p. ej.: Specular, Brillo)
* Se ha corregido el comportamiento del borrador para deshabilitar la fusión en modo de paso a través

**Problemas conocidos:**

* La simetría no funciona con la herramienta de difuminado y Clonar
* Falta la exportación de ArtStation

## Versión 1

### 1.7.3

*(Lanzado: 1 de marzo de 2016)*

**Agregado:**

* &amp;lbrack;Exportar&amp;rbrack; Añadir una opción para desactivar el relleno
* &amp;lbrack;Shelf&amp;rbrack; Admitir jerarquía de subestanterías dentro de una carpeta de estanterías

**Corregido:**

* Bloqueo al guardar sobre un archivo de solo lectura anterior
* Bloqueo al abrir un segundo proyecto
* Bloqueo al cargar algunas miniaturas (estanterías, capas o información sobre herramientas)
* La desactivación de &quot;Conservar posiciones de trazos en la malla&quot; no funciona
* &amp;lbrack;Exportar&amp;rbrack; La ampliación de los mapas de bits se realiza con el filtrado más cercano
* &amp;lbrack;Shelf&amp;rbrack; El descubrimiento de recursos es muy lento
* &amp;lbrack;Shelf&amp;rbrack; Los filtros de desenfoque no son compatibles con 16 bits
* &amp;lbrack;Herramienta&amp;rbrack; La simetría no funciona si carga un ajuste preestablecido antiguo de la herramienta
* El cuadro de diálogo Color del canal de Specular no convierte el espacio de color

### 1.7.2

*(Lanzado: 13 de enero de 2016)*

**Agregado:**

* &amp;lbrack;Capas&amp;rbrack; Permitir especificar el segmentado predeterminado para las capas de relleno

**Corregido:**

* &amp;lbrack;Exportar&amp;rbrack; La exportación de Sketchfab ya no funciona
* &amp;lbrack;Capa&amp;rbrack; El filtrado bilineal se aplica incluso en Rellenar sin ninguna transformación
* &amp;lbrack;Herramienta&amp;rbrack; Rendimiento deficiente al utilizar Substance con entradas de imagen en modo de proyección
* &amp;lbrack;Herramienta&amp;rbrack; El selector de material está roto

### 1.7.1

*(Lanzado: 18 de diciembre de 2015)*

**Corregido:**

* Bloqueo al cambiar el conjunto de texturas
* Reproducciones lentas al pintar

### 1.7.0

*(Lanzado: 17 de diciembre de 2015)*

**Agregado:**

* &amp;lbrack;Performance&amp;rbrack; Calcular el contenido de las capas y sus miniaturas al mismo tiempo
* &amp;lbrack;Exportar&amp;rbrack; Guardar la ruta de exportación como relativa cuando esté al lado del proyecto
* &amp;lbrack;Capas&amp;rbrack; Se ha añadido un nuevo modo de fusión : restar y agregar/sub
* &amp;lbrack;Capas&amp;rbrack; Nuevo filtrado HQ bilineal para capas de relleno
* &amp;lbrack;Sombreador&amp;rbrack; Establezca un sombreador predeterminado para la generación de miniaturas en las preferencias.
* &amp;lbrack;Sombreador&amp;rbrack; Permitir especificar un sombreador por conjunto de texturas
* &amp;lbrack;Sombreador&amp;rbrack; Permitir tomar muestras de texturas de la estantería
* &amp;lbrack;Herramienta&amp;rbrack; Nuevo comportamiento de pincel de &quot;ceñir&quot; para pintar
* &amp;lbrack;Herramienta&amp;rbrack; Filtrado mejorado y suavizado reducido al pintar
* &amp;lbrack;Herramienta&amp;rbrack; Calidad de pintura de subpíxeles mejorada
* &amp;lbrack;Herramienta&amp;rbrack; Se ha eliminado la visualización &quot;básica&quot; de la configuración del pincel y se ha mejorado el icono de apertura/cierre del marco
* &amp;lbrack;Menú&amp;rbrack; Añadir iconos de efectos en el menú contextual
* Creación de plantillas desde Proyectos
* &amp;lbrack;Shelf&amp;rbrack; Nuevas plantillas : PBR, Dota 2
* &amp;lbrack;Shelf&amp;rbrack; Nuevo ajuste preestablecido de exportación : Dota 2
* &amp;lbrack;Shelf&amp;rbrack; Nuevos sombreadores : Dota 2, pintura de coches PBR, revestimiento PBR, terciopelo PBR
* &amp;lbrack;Shelf&amp;rbrack; Nuevo material : Óxido de acero y desgaste, iluminación estilizada
* &amp;lbrack;Shelf&amp;rbrack; Nuevos filtros : Difuminado direccional, iluminación estilizada
* &amp;lbrack;Shelf&amp;rbrack; Nuevo pincel : disco duro por defecto suave y duro por defecto con un nuevo alfa para un mejor control de la dureza
* &amp;lbrack;Shelf&amp;rbrack; Nuevos generadores : Distancia y luz 3D
* &amp;lbrack;Shelf&amp;rbrack; Pinceles actualizados con proyección de ceñido y sacrificio de caras posteriores (activado de forma predeterminada)
* &amp;lbrack;Shelf&amp;rbrack; Se ha actualizado Ruido blanco con la versión de procesador de píxeles para agilizar el cálculo

**Corregido:**

* &amp;lbrack;Pantalla de bienvenida&amp;rbrack; Tutorials vínculo enviar a vídeos antiguos
* &amp;lbrack;Canales&amp;rbrack; Si se indica &quot;no&quot; para rellenar la creación de capas con AO, se sigue creando la capa
* &amp;lbrack;Canales&amp;rbrack; Los nombres de canales UserX no se propagan en la interfaz
* &amp;lbrack;Viewport&amp;rbrack; La entrada de máscara está vacía en la lista de canales solo
* &amp;lbrack;Compartir&amp;rbrack; Exportar un alfa para compartir desde SP crea un archivo .image ilegible
* &amp;lbrack;Licencia&amp;rbrack; Solucionar problemas de activación para nombres de usuario con caracteres que no sean ASCII
* &amp;lbrack;Sombreador&amp;rbrack; El cuadro de diálogo de parámetros de color desaparece al seleccionar un color
* &amp;lbrack;Shelf&amp;rbrack; Las miniaturas no se descargan de la memoria cuando no se utilizan
* &amp;lbrack;Shelf&amp;rbrack; Filtro de degradado fijo
* &amp;lbrack;Herramienta&amp;rbrack; La simetría no funciona con la galería de símbolos o la proyección
* &amp;lbrack;Herramienta&amp;rbrack; Nombre incorrecto al crear un nuevo ajuste preestablecido de pincel
* La opción Conservar trazo permanece desactivada incluso al volver a importar una malla
* Restablecimiento del controlador (TDR) al calcular partículas con un tamaño grande.

### 1.6.1

*(Lanzado: 09 de noviembre de 2015)*

**Corregido:**

* Bloqueo al abrir el proyecto si Vista 2D está visible
* Bloqueo al crear un nuevo ajuste preestablecido de exportación si el estante actual no existe
* &amp;lbrack;Herramienta&amp;rbrack; El icono del selector de material puede permanecer visible
* &amp;lbrack;Herramienta&amp;rbrack; El selector de material oculta el cursor del ratón al pintar al mismo tiempo
* &amp;lbrack;Shelf&amp;rbrack; Los metadatos se escriben en el disco después de cada salida

### 1.6.0

*(Lanzado: 29 de octubre de 2015)*

**Agregado:**

* Compatibilidad oficial con Windows 10
* &amp;lbrack;Substance&amp;rbrack; Contraer grupos de parámetros de sustancia de forma predeterminada
* &amp;lbrack;Substance&amp;rbrack; Añadir nueva estructura (mejorar el rendimiento del Procesador de píxeles)
* &amp;lbrack;Viewport&amp;rbrack; Permita desactivar la visualización del plano de simetría en el modo de simetría.
* &amp;lbrack;Viewport&amp;rbrack; Mejorar el procesamiento y el rendimiento de las sombras
* &amp;lbrack;Viewport&amp;rbrack; Pausar cálculo de sombras al pintar
* &amp;lbrack;Viewport&amp;rbrack; Mejorar el rendimiento de representación de malla metálica
* &amp;lbrack;Motor&amp;rbrack; Mejorar la administración de la memoria Vram para reducir su huella
* &amp;lbrack;Motor&amp;rbrack; Mejore la actualización de la textura en las GPU AMD para obtener un mejor rendimiento
* &amp;lbrack;Motor&amp;rbrack; Deshabilite la configuración de optimización enlazada en GPU NVIDIA para obtener un mejor rendimiento
* &amp;lbrack;Efecto&amp;rbrack; Añada una etiqueta para solicitar la entrada de imagen &quot;acolchada&quot;
* &amp;lbrack;Capa&amp;rbrack; Aumentar la precisión del Desplazamiento de UV/escala en el relleno
* &amp;lbrack;Capa&amp;rbrack; Hacer que el regulador de escala sea exponencial en el relleno
* &amp;lbrack;Capa&amp;rbrack; Permita arrastrar y soltar materiales directamente en la pila de capas.
* &amp;lbrack;Capa&amp;rbrack; Permitir arrastrar y soltar filtros directamente en la pila de capas
* &amp;lbrack;Capa&amp;rbrack; Ajustar el color del pincel de máscara al color de máscara recién creado
* &amp;lbrack;Sombreador&amp;rbrack; Exponer varias texcocords
* &amp;lbrack;Sombreador&amp;rbrack; Función de asignación de gamma y tono para permitir funciones personalizadas
* &amp;lbrack;Bakeres&amp;rbrack; Cambiar la configuración predeterminada del baker de posición para el uso TriPlanar
* &amp;lbrack;Herramienta&amp;rbrack; Cambie el nombre &quot;Geometry Decal&quot; por &quot;Polygon Fill&quot;.
* &amp;lbrack;Shelf&amp;rbrack; Actualice los generadores para que sean compatibles con TriPlanar : MG Desgaste del borde del metal, MG Constructor de la máscara, MG Fibra de vidrio, MG Dirt
* &amp;lbrack;Shelf&amp;rbrack; Actualizar materiales con nuevas configuraciones y eliminar materiales no utilizados
* &amp;lbrack;Shelf&amp;rbrack; 22 materiales inteligentes nuevos (plástico, hierro, tela, acero y más)
* &amp;lbrack;Shelf&amp;rbrack; Actualiza los filtros Enfocar, Desenfocar y Deformar con entrada de imagen acolchada para evitar costuras
* &amp;lbrack;Shelf&amp;rbrack; Mejora de la configuración de deformación para facilitar su uso
* &amp;lbrack;Shelf&amp;rbrack; 2 Nuevos ruidos procedimientos : Ruido de Perlin 3D y ruido de Worley 3D

**Corregido:**

* &amp;lbrack;Motor&amp;rbrack; La detección de la cantidad de Vram para la GPU dedicada es incorrecta en Mac
* &amp;lbrack;Motor&amp;rbrack; Las texturas se convierten en una versión más oscura en la ventana gráfica
* &amp;lbrack;Motor&amp;rbrack; Rendimiento deficiente al pintar debajo de varias capas
* &amp;lbrack;Motor&amp;rbrack; Las capas calculadas al abrir el proyecto difieren de la versión almacenada en caché
* &amp;lbrack;Substance&amp;rbrack; Resultados incorrectos en 4K en Mac
* &amp;lbrack;Substance&amp;rbrack; Los parámetros están en el orden incorrecto
* &amp;lbrack;Sombreador&amp;rbrack; Los sombreadores de tono y pixelado son totalmente negros
* &amp;lbrack;Sombreador&amp;rbrack; Los parámetros desaparecen después de cambiar el mapa de entorno
* &amp;lbrack;Shelf&amp;rbrack; Bloqueo al colocar archivos png en la carpeta generator
* &amp;lbrack;Shelf&amp;rbrack; Las miniaturas se generan con una rugosidad baja
* &amp;lbrack;Herramienta&amp;rbrack; Bloqueo al utilizar un mapa de bits en el pincel alfa en windows
* &amp;lbrack;Exportar&amp;rbrack; El ajuste preestablecido de exportación de mapa adicional ahora exporta un mapa del RGB para Posición

### 1.5.7

*(Lanzado: 24 de septiembre de 2015)*

**Corregido:**

* El informe de bloqueos ya no funciona

### 1.5.6

*(Lanzado: 21 de septiembre de 2015)*

**Agregado:**

* &amp;lbrack;Shelf&amp;rbrack; Mejora la calidad de representación de miniaturas (utiliza texturas 1K)

**Corregido:**

* &amp;lbrack;Compartir&amp;rbrack; Imposible firmar con otra cuenta
* &amp;lbrack;Shelf&amp;rbrack; Las miniaturas pesan demasiado en el disco
* &amp;lbrack;Shelf&amp;rbrack; Los materiales inteligentes son muy lentos de cargar
* &amp;lbrack;Windows&amp;rbrack; Solucionar problemas de instalación del servicio de licencias
* &amp;lbrack;Canales&amp;rbrack; El mapa de transmisivo se crea como G8 de forma predeterminada

### 1.5.5

*(Lanzado: 15 de septiembre de 2015)*

**Agregado:**

* &amp;lbrack;Shelf&amp;rbrack; Exportar contenidos a Substance share
* &amp;lbrack;Shelf&amp;rbrack; Adición de una nueva previsualización de esfera para materiales
* &amp;lbrack;Shelf&amp;rbrack; Utilice el mapa de env &quot;Patio acristalado&quot; para generar miniaturas
* &amp;lbrack;Shelf&amp;rbrack; Aumentar resolución de tamaño de miniatura a 512x512 píxeles
* &amp;lbrack;Vista 3D&amp;rbrack; Exponer valor de rotación de entorno
* &amp;lbrack;Windows&amp;rbrack; Firmar la aplicación

**Corregido:**

* &amp;lbrack;Bakeres&amp;rbrack; Resultados incorrectos al hacer un bake mapas al mismo tiempo
* &amp;lbrack;Vista 3D&amp;rbrack; El mapa de env se muestra cuando no hay ningún proyecto abierto
* &amp;lbrack;Capas&amp;rbrack; Los generadores de máscaras no funcionan en el contenido de capas
* &amp;lbrack;Capas&amp;rbrack; Puede realizar la pintura en capas ocultas
* &amp;lbrack;Shelf&amp;rbrack; El dirt_5 y el Dirt_6 son idénticos
* &amp;lbrack;Shelf&amp;rbrack; Algunos generadores de máscaras están pixelados o son de baja calidad
* &amp;lbrack;Herramienta&amp;rbrack; Rotación de gizmo incorrecta en determinados ángulos.
* &amp;lbrack;Herramienta&amp;rbrack; Si hay demasiados canales, los botones de canal se recortan
* &amp;lbrack;Herramienta&amp;rbrack; El método abreviado de inversión de máscara para Máscara rápida no funciona
* &amp;lbrack;Exportar&amp;rbrack; Bocetos: el botón de cancelación no se ha tenido en cuenta correctamente
* &amp;lbrack;Licencia&amp;rbrack; Error de activación cuando no se puede copiar la licencia
* El limitador de velocidad de fotogramas ya no funciona en la IU

### 1.5.0

*(Lanzado: 20 de agosto de 2015)*

**Agregado:**

* &amp;lbrack;Sombreador&amp;rbrack; Agregar número de línea en Sombreador compilando mensajes de error
* &amp;lbrack;Shelf&amp;rbrack; Mejorar la calidad de las vistas previas en miniaturas
* &amp;lbrack;Shelf&amp;rbrack; Generación automatizada de miniaturas para Materiales inteligentes
* &amp;lbrack;Herramienta&amp;rbrack; Método abreviado para controlar el ajuste de la dureza en la sustancia
* &amp;lbrack;Herramienta&amp;rbrack; Usar el widget de escala de grises para la pegatina geométrica al pasar sobre una máscara
* &amp;lbrack;Herramienta&amp;rbrack; Método abreviado para invertir el color de la pintura mientras se pinta en un mapa en escala de grises
* &amp;lbrack;Viewport&amp;rbrack; Permitir mostrar la malla metálica y cambiar su color
* &amp;lbrack;Viewport&amp;rbrack; Desenfocar el fondo del entorno
* &amp;lbrack;Controles&amp;rbrack; Añadir rotación a los métodos abreviados de pincel del ratón
* &amp;lbrack;Exportar&amp;rbrack; Exportar a Sketchfab
* &amp;lbrack;Exportar&amp;rbrack; Creación de ajustes preestablecidos de exportación para procesadores
* &amp;lbrack;Exportar&amp;rbrack; Añadir reflejo del mapa convertido, F0 y 1/IOR
* &amp;lbrack;UI&amp;rbrack; Pantalla Añadir bienvenida
* &amp;lbrack;UI&amp;rbrack; Actualizar diseño predeterminado
* &amp;lbrack;UI&amp;rbrack; Añadir información sobre herramientas que falta y cambiar el nombre de alguna entrada del menú
* &amp;lbrack;Capas&amp;rbrack; Exportar la máscara seleccionada actualmente como mapa de bits
* &amp;lbrack;Capas&amp;rbrack; Añade la acción &quot;invertir máscara&quot; en el menú del botón derecho

**Corregido:**

* &amp;lbrack;Proyecto&amp;rbrack; Si los pivotes de las mallas son diferentes en el FBX, las mallas se explotan al importar
* &amp;lbrack;Substance&amp;rbrack; Los Substance utilizados en las herramientas de proyección están bloqueados en 256\*256
* &amp;lbrack;Capas&amp;rbrack; Bloqueo al utilizar la opción borrar máscara
* &amp;lbrack;Exportar&amp;rbrack; Conversión de gamma incorrecta en texturas muy oscuras
* &amp;lbrack;Exportar&amp;rbrack; El mapa de posición solo se puede utilizar en los ajustes preestablecidos de exportación como mapa de escala de grises
* &amp;lbrack;Herramienta&amp;rbrack; El color de inicio de la calcomanía geométrica es negro cuando se utiliza en una máscara
* &amp;lbrack;Herramienta&amp;rbrack; El método abreviado de rotación no funciona si no hay dureza en el alfa

### 1.4.2

*(Lanzado: 15 de julio de 2015)*

**Corregido:**

* &amp;lbrack;Herramienta&amp;rbrack; Bloqueo al utilizar la pegatina geométrica con máscara rápida
* La actualización de un proyecto de la versión 1.4.0 a la 1.4.1 consume toda la memoria del equipo
* Importación incorrecta del formato de proyecto antiguo
* Los estantes personalizados analizan toda la jerarquía y duplican activos en todas partes

### 1.4.1

*(Lanzado: 23 de junio de 2015)*

**Agregado:**

* &amp;lbrack;Viewport&amp;rbrack; Permitir acoplar paneles uno al lado del otro
* &amp;lbrack;Efecto&amp;rbrack; Adición de un fondo y una regla para el efecto de nivel
* &amp;lbrack;Efecto&amp;rbrack; Añada un efecto de Pintura que permita trabajar sobre otro efecto

**Corregido:**

* &amp;lbrack;Shelf&amp;rbrack; La generación de miniaturas se interrumpe si no hay ningún proyecto abierto
* &amp;lbrack;Shelf&amp;rbrack; La previsualización de ajustes preestablecidos de material no se genera
* &amp;lbrack;Shelf&amp;rbrack; Las previsualizaciones de material se generan en una malla con normales invertidas
* &amp;lbrack;Shelf&amp;rbrack; Las miniaturas siempre se vuelven a calcular debido a una función hash incorrecta
* &amp;lbrack;Shelf&amp;rbrack; Hacer clic en un material de Substance no conecta mapas adicionales
* &amp;lbrack;Herramienta&amp;rbrack; Valor incorrecto muestreado con el selector de material
* &amp;lbrack;Herramienta&amp;rbrack; Color del cursor de ventanilla de selección del selector de color
* &amp;lbrack;vista 2D&amp;rbrack; Velocidad de fotogramas/rendimiento muy baja
* &amp;lbrack;Exportar&amp;rbrack; Bloqueo al abrir la ventana de exportación con ajustes preestablecidos de exportación demasiado recientes.
* &amp;lbrack;Exportar&amp;rbrack; El canal de height al Mapa de normales se convierte en el espacio incorrecto
* &amp;lbrack;Mac&amp;rbrack; El color base de los efectos de Substance se muestra como lineal
* &amp;lbrack;Mac&amp;rbrack; El widget de líneas rectas se dibuja incorrectamente en Retina
* Las líneas rectas pueden permanecer activadas incluso con el método abreviado liberado.
* Las líneas rectas del guizmo desaparecen después de rotar el mapa de entorno
* Las salidas de oclusión ambiental de sustancias no se conectan automáticamente al canal AO
* Solucionar el problema de copia de licencia en Windows con un carácter especial en el nombre de usuario

### 1.4.0

*(Lanzado: 10 de junio de 2015)*

**Agregado:**

* &amp;lbrack;Exportar&amp;rbrack; Añadir mapas adicionales en la lista de los mapas de entrada disponibles
* &amp;lbrack;Shelf&amp;rbrack; Usar materiales sbsar como ajustes preestablecidos de materiales
* &amp;lbrack;Shelf&amp;rbrack; Permitir el uso de rutas de biblioteca personalizadas
* &amp;lbrack;Shelf&amp;rbrack; Cambiar el tamaño mínimo
* &amp;lbrack;Shelf&amp;rbrack; Nuevo contenido : 20 materiales inteligentes nuevos
* &amp;lbrack;Shelf&amp;rbrack; Nuevo contenido : nueva sustancia procedimienta (tejido, malla)
* &amp;lbrack;Shelf&amp;rbrack; Filtro de desenfoque actualizado
* Dibujo de líneas rectas mediante una tecla modificadora
* Adición de un canal de Oclusión ambiental y modificación del comportamiento AO/Normal en la pila de capas
* Leer el color predeterminado de la entrada de imagen definida en los datos de usuario del Substance
* Permitir la exportación del registro desde el menú de ayuda

**Corregido:**

* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Bloqueo con baker Normal desde malla
* &amp;lbrack;Baker&amp;rbrack; Bloqueo si no hay UV en el archivo de la jaula
* &amp;lbrack;Baker&amp;rbrack; La coincidencia por nombres no funciona con OBJ exportados desde zBrush
* &amp;lbrack;Baker&amp;rbrack; Hacer un bake con una jaula sobrescribe hacer un bake si se utilizan varios conjuntos de texturas y UV superpuestos
* &amp;lbrack;Baker&amp;rbrack; Los archivos OBJ específicos dan como resultado texturas negras
* &amp;lbrack;Shelf&amp;rbrack; No se pueden leer los recursos si se establece como de sólo lectura
* &amp;lbrack;Shelf&amp;rbrack; Los archivos de recursos se escriben en Painter si se han utilizado en el proyecto.
* &amp;lbrack;Shelf&amp;rbrack; La recarga de sustancias también actualiza la capa
* &amp;lbrack;Exportar&amp;rbrack; Tiff exporta imágenes de 32 bits que Photoshop o los motores de juegos no pueden leer correctamente
* &amp;lbrack;Exportar&amp;rbrack; El ajuste preestablecido de canales predeterminados siempre exporta como RGB
* &amp;lbrack;Material&amp;rbrack; Asignación de BaseColor con substancias en anulación de canal de Difuso
* &amp;lbrack;Vista 3D&amp;rbrack; Iluminación de Difuso incorrecta con mapas de entorno específicos
* &amp;lbrack;Herramienta&amp;rbrack; No se puede rotar un pincel a un ángulo específico
* La ventana gráfica se enfoca al pasar el cursor por encima mientras se escribe en un campo de texto
* Bloqueo con ajustes preestablecidos demasiado recientes para la versión actual del estante
* Bloqueo después de reemplazar la malla
* Bloqueo al volver a cargar una sustancia con un número diferente de entradas
* FBX mallas de la importación de Cinema4D con nombres de material incorrectos

### 1.3.5

*(Lanzado: 29 de mayo de 2015)*

**Agregado:**

* &amp;lbrack;Licencia&amp;rbrack; Problema de activación cuando ya hay un archivo de licencia
* &amp;lbrack;Mac&amp;rbrack; Bloqueo al cargar archivos FBX específicos
* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;Vista 3D&amp;rbrack; Reflejo incorrecto para la GPU integrada
* &amp;lbrack;Vista 3D&amp;rbrack; La fuente de la máscara rápida está rota
* &amp;lbrack;Vista 3D&amp;rbrack; El selector de material hace que la ventana gráfica sea totalmente negra
* Bloqueo después de abrir proyectos creados en 1.3.3
* La previsualización de material está vacía al utilizar sombreadores con alfa
* La pintura deja de funcionar en mallas específicas
* Las prestaciones disminuyen mucho con mallas OBJ específicas
* Los canales de usuario no se asignan al utilizar efectos
* Las carpetas temporales no se limpian al inicio

**Corregido:**

* Mejoras de tiempo de cálculo en el proyecto extremadamente largo de carga
* Cambie la ventana &quot;Solución de problemas de GPU&quot; para que sea más comprensible
* &amp;lbrack;Capas&amp;rbrack; Guarde el estado del bloqueo de proporción para las capas de relleno y active esta opción de forma predeterminada
* &amp;lbrack;Bakeres&amp;rbrack; La coincidencia por nombre ahora usa el sufijo como separador

### 1.3.4

*(Lanzado: 27 de abril de 2015)*

**Agregado:**

* &amp;lbrack;Mac&amp;rbrack; Bloqueo con Mac OS X Yosemite (10.10)
* &amp;lbrack;Mac&amp;rbrack; Imposible salir del modo de pantalla completa
* &amp;lbrack;Bakeres&amp;rbrack; La opción de hacer un bake coincidencia por nombre no funciona
* &amp;lbrack;Bakeres&amp;rbrack; El espacio de tangente de tinta utilizado en SP no funciona con UE4
* &amp;lbrack;Bakeres&amp;rbrack; El baker de ID. no puede hacer un bake colores de ID. de material
* &amp;lbrack;vista 2D&amp;rbrack; La malla metálica no aparece al utilizar la herramienta Calcomanía geométrica
* &amp;lbrack;Herramienta&amp;rbrack; El canal alfa del pincel se muestra como verificador en lugar de como transparencia con los materiales
* &amp;lbrack;Herramienta&amp;rbrack; Bloqueo con pegatina geométrica
* &amp;lbrack;Capas&amp;rbrack; La ranura de material se contrae de forma predeterminada en la capa Relleno
* &amp;lbrack;Exportar&amp;rbrack; Bloqueo al exportar a un tamaño mayor que la resolución del conjunto de texturas
* El canal de specular no se reconoce en los filtros.
* Limpiar y guardar no quita correctamente los recursos del archivo spp
* No almacenar la transformación de bajo contenido de poli en el archivo de asignación de alto contenido de poli
* FBX archivo se importa con demasiados conjuntos de texturas

**Corregido:**

* Efectos: Los niveles Ajustados deben estar activados de forma predeterminada para imitar los niveles &quot;clásicos&quot;
* Capas: Cambio del nivel mínimo y máximo en la acción Rellenar
* Capas: Guardar y restaurar el estado de la pila
* Bakeres: BAKER AO tener en cuenta el mapa de normales si no se especifica ningún HP
* Bakeres: Se ha añadido información sobre herramientas e información adicional en la ventana hacer un bake
* Crear un archivo de copia de seguridad al guardar un proyecto

### 1.3.3

*(Lanzado: 01 de abril de 2015)*

**Agregado:**

* Añadir la versión de software y el nombre del proyecto en la barra de título
* Corregir nombres de TextureSet y nombres de Materiales inteligentes
* Actualizar el motor del Substance a V5
* &amp;lbrack;Shelf&amp;rbrack; Añadir nuevos mapas de entorno : Corsica beach, studio 05, Tornoco studio y más
* &amp;lbrack;Shelf&amp;rbrack; Actualizar MG Mask Builder con nuevos parámetros
* &amp;lbrack;Shelf&amp;rbrack; Actualización y calibración de mapas de entorno antiguos

**Corregido:**

* Bloqueo al abrir la ventana de exportación
* No es posible arrastrar y soltar en el widget de interfaz de usuario cuando no está acoplado
* &quot;Buscar actualizaciones&quot; no funciona
* &amp;lbrack;Capas&amp;rbrack; No seleccionar la máscara al pulsar ALT + clic en ella
* &amp;lbrack;Herramienta&amp;rbrack; Tri-plana no funciona con el canal Normal
* &amp;lbrack;Vista 3D&amp;rbrack; La iluminación del mapa de env es incorrecta
* &amp;lbrack;Vista 3D&amp;rbrack; El cálculo de la exposición es diferente de Designer
* &amp;lbrack;Vista 3D&amp;rbrack; Las sombras no deben ser visibles en superficies 100 % metálicas
* &amp;lbrack;Vista 3D&amp;rbrack; La malla con UV reflejados tiene tangentes/binomales volteados
* &amp;lbrack;Vista 3D&amp;rbrack; Las sombras producen resultados incorrectos en determinadas mallas
* &amp;lbrack;Bakeres&amp;rbrack; Eliminar la carpeta &quot;.alg_meta&quot; creada por los archivos de asignación
* &amp;lbrack;Bakeres&amp;rbrack; Bloqueo al hacer un bake si Painter vuelve a calcular un TextureSet al mismo tiempo
* &amp;lbrack;Mac&amp;rbrack; Error de IU de White Box al iniciar la aplicación

### 1.3.2

*(Lanzado: 6 de marzo de 2015)*

**Corregido:**

* &amp;lbrack;Vista 3D&amp;rbrack; No es posible volver a cargar un mapa env guardado con el proyecto

### 1.3.1

*(Lanzado: 5 de marzo de 2015)*

**Agregado:**

* &amp;lbrack;Bakeres&amp;rbrack; Agregar una versión en caché de mallas de alta densidad de poli para acelerar el cálculo
* &amp;lbrack;Bakeres&amp;rbrack; Añada un icono de advertencia si no se ha cargado ninguna malla de alta densidad
* &amp;lbrack;Bakeres&amp;rbrack; Si no se carga ninguna malla de alta densidad, utilice en su lugar la malla del proyecto

**Corregido:**

* &amp;lbrack;Bakeres&amp;rbrack; Al pulsar &quot;Intro&quot; al editar el valor de un regulador, cierre la ventana
* &amp;lbrack;Bakeres&amp;rbrack; La activación/desactivación de un baker también activará el botón
* &amp;lbrack;Bakeres&amp;rbrack; Imposible de hacer un bake si utiliza el botón &quot;all/none&quot;
* &amp;lbrack;Bakeres&amp;rbrack; La ordenación de los botones del baker no está en el orden correcto
* &amp;lbrack;Bakeres&amp;rbrack; Las casillas se omiten y todos los bakeres siempre se procesan
* &amp;lbrack;Bakeres&amp;rbrack; Progreso de la barra de progreso fijo

### 1.3.0

*(Lanzado: 4 de marzo de 2015)*

**Agregado:**

* &amp;lbrack;Bakeres&amp;rbrack;&amp;lbrack;Vista 3D&amp;rbrack; Usar cálculo de espacio de tangente Mikkt si no se encuentran tangentes/binormales
* &amp;lbrack;Bakeres&amp;rbrack; Se han añadido nuevos bakeres : Normal, ID, Oclusión, Curvatura, Thickness, Posición
* &amp;lbrack;Efectos&amp;rbrack; La pila de efectos ahora se invierte y se muestra de arriba abajo (como capas)
* &amp;lbrack;Efectos&amp;rbrack; Añadir nuevos iconos en la pila de efectos
* &amp;lbrack;Efectos&amp;rbrack; Añadir modo de fusión entre acciones de relleno en la pila de efectos
* &amp;lbrack;Efectos&amp;rbrack; Cambiar nombre de efectos (efecto de sustancia = filtro, etc.)
* Añadir un archivo &quot;lock&quot; durante el proceso de guardado
* &amp;lbrack;Efectos&amp;rbrack; Agregar acción de relleno en la pila de efectos
* Se ha añadido un nuevo recurso : Materiales inteligentes
* &amp;lbrack;Capas&amp;rbrack; Permitir reordenar efectos de capa
* &amp;lbrack;Herramienta&amp;rbrack; Agregar proyección Tri-Plana
* &amp;lbrack;Vista 3D&amp;rbrack; Añadir compatibilidad con sombras
* &amp;lbrack;Vista 3D&amp;rbrack; Posibilidad de definir los estados de OpenGL necesarios en sombreadores personalizados
* &amp;lbrack;Vista 3D&amp;rbrack; Compatibilidad con alfa mediante nuevos sombreadores
* &amp;lbrack;Vista 3D&amp;rbrack; Ahora se crean versiones de los sombreadores y se guardan completamente en un proyecto
* &amp;lbrack;Vista 3D&amp;rbrack; Avisar al usuario si el sombreador ya no se compila

**Corregido:**

* &amp;lbrack;Capas&amp;rbrack; corregir colocación en una carpeta contraída
* &amp;lbrack;Shelf&amp;rbrack; Corrección del filtrado de contenido en miniestantes
* &amp;lbrack;Shelf&amp;rbrack; Cambiar el nombre de categorías y reorganizar pestañas

### 1.2.1

*(Lanzado: 12 de febrero de 2015)*

**Agregado:**

* Los archivos \*.spp ahora se pueden abrir haciendo doble clic en el explorador
* &amp;lbrack;Exportar&amp;rbrack; Nueva etiqueta &quot;$project&quot; para los ajustes preestablecidos de exportación
* &amp;lbrack;Exportar&amp;rbrack; Añadir lista de mapas (con nomenclatura) debajo de cada conjunto de texturas
* &amp;lbrack;Exportar&amp;rbrack; Añada un botón Todo/Ninguno para seleccionar los conjuntos de texturas
* &amp;lbrack;Exportar&amp;rbrack; Los mapas vacíos se descartan durante la exportación

**Corregido:**

* &amp;lbrack;Exportar&amp;rbrack; Los ajustes preestablecidos de Unity5 tienen mapas invertidos
* &amp;lbrack;Exportar&amp;rbrack; Si se añade una barra diagonal en un nombre de ajuste preestablecido, se creará una carpeta dañada
* &amp;lbrack;Exportar&amp;rbrack; El canal de height exportado en formatos de 32 bits no está sujeto correctamente
* &amp;lbrack;Exportar&amp;rbrack; La lista de conjuntos de texturas no se ordena como en el proyecto
* &amp;lbrack;Herramienta&amp;rbrack; El sacrificio de la cara posterior ya no funciona
* Guardar no funciona con caracteres especiales en el trazado

### 1.2.0

*(Lanzado: 28 de enero de 2015)*

**Agregado:**

* Nuevo canal Normal que permite la pintura de datos de mapa de normales y combinar los resultados
* &amp;lbrack;Exportar&amp;rbrack; Nueva ventana de exportación con la capacidad de crear empaquetados personalizados y definir nombres personalizados
* El formato del archivo de proyecto ahora es un único archivo en lugar de carpetas
* &amp;lbrack;Exportar&amp;rbrack; Admite diferentes formatos normales (DirectX, OpenGL)
* &amp;lbrack;Exportar&amp;rbrack; Crear un archivo de bloqueo temporal durante la exportación
* &amp;lbrack;Capas&amp;rbrack; Mayús + clic izquierdo del ratón se puede utilizar para cambiar una máscara
* &amp;lbrack;Parámetros&amp;rbrack; Exponer el espacio de color en la parte inferior de una entrada de imagen
* &amp;lbrack;Shelf&amp;rbrack; Efecto &quot;MG Mask Builder&quot; ahora tiene nuevos ajustes
* &amp;lbrack;Vista 3D&amp;rbrack; El mapa de oclusión ambiental ahora oculta el aporte difuso, no el specular

**Corregido:**

* El material de proyección o la previsualización de la galería de símbolos no se muestran correctamente en la ventana gráfica
* &amp;lbrack;Vista 3D&amp;rbrack; La información sobre herramientas de método abreviado no se muestra al utilizar métodos abreviados &quot;S&quot; (esténcil)
* &amp;lbrack;Shelf&amp;rbrack; El efecto &quot;MatFx Skin Scale&quot; tiene ahora mejores prestaciones en baja resolución
* &amp;lbrack;Exportar&amp;rbrack; Las texturas de la exportación solo se aumentan al especificar un tamaño de documento más grande

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

* &amp;lbrack;Capa&amp;rbrack; Seleccionar la capa superior al abrir un proyecto o cambiar un conjunto de texturas
* Se ha mejorado la velocidad de &quot;Guardar&quot; y &quot;Guardar como&quot; con el nuevo algoritmo de compresión
* Mostrar un error al abrir un proyecto demasiado reciente para Painter

**Corregido:**

* &amp;lbrack;Herramienta&amp;rbrack; La calcomanía geométrica produce corrupciones de memoria
* &amp;lbrack;Brush&amp;rbrack; No es posible introducir manualmente valores flotantes por debajo de 1 para el tamaño de pincel
* &amp;lbrack;Capa&amp;rbrack; Crear un efecto de selección de color no lo añade a la pila de capas
* &amp;lbrack;Capa&amp;rbrack; Al mover el ratón sobre las capas, Painter se mueve en la barra de tareas
* &amp;lbrack;Capa&amp;rbrack; Añadir un mapa de bits como máscara puede provocar un bloqueo
* La interfaz gráfica de usuario para el modo solo con el canal de Height es incorrecta
* &quot;Guardar proyecto&quot; puede dar error y dañar un proyecto
* Bloqueo al abrir un proyecto después de cargar otro con un sombreador obsoleto

### 1.1.0

*(Lanzado: 16 de diciembre de 2014)*

**Agregado:**

* &amp;lbrack;Efecto&amp;rbrack; Nuevo creador de máscaras de ID de material
* Nueva línea punteada blanca/negra para el gizmo del pincel
* Nuevo parámetro de seguimiento de ángulo
* Nuevo parámetro de sacrificio de la cara posterior
* Nuevo parámetro de Ratón perezoso
* &amp;lbrack;Capas&amp;rbrack; Compatibilidad con varias selecciones y administración
* &amp;lbrack;Capas&amp;rbrack; Copiar y pegar de un conjunto de texturas entre sí
* &amp;lbrack;Exportar&amp;rbrack; Formato de PSD de Adobe Photoshop
* &amp;lbrack;Shelf&amp;rbrack; Nueva herramienta : piel, puntadas metálicas y cremallera
* &amp;lbrack;Shelf&amp;rbrack; Nuevo pincel : molde, lápiz, línea afilada y puntada
* &amp;lbrack;Shelf&amp;rbrack; Nuevo alfa : Ruido gaussiano, línea afilada, molde, pluma, salpicadura, puntada, cremallera
* Se han mejorado las prestaciones de pintura actualizando solo partes de las texturas necesarias

**Corregido:**

* &amp;lbrack;Shelf&amp;rbrack; Imposible cargar una sustancia con un gráfico que tiene etiquetas idénticas
* &amp;lbrack;Capas&amp;rbrack; El modo de fusión Pass Through no funciona con máscaras
* &amp;lbrack;Stencil&amp;rbrack; La escala se rompe en el Vista 2D
* Problemas y bloqueo en el sistema operativo Mac Yosemite

### 1.0.2

*(Lanzado: 09 de noviembre de 2014)*

**Agregado:**

* Rendimiento mejorado en la previsualización de materiales con sustancias
* Se han mejorado las prestaciones con la vista previa del trazo de pincel al actualizar el documento
* Rendimiento mejorado en la ventana gráfica con una velocidad de actualización más baja para el área no operativa
* &amp;lbrack;Efectos de posprocesamiento&amp;rbrack; Interfaz de usuario mejorada para administrar la configuración
* &amp;lbrack;Efectos de posprocesamiento&amp;rbrack; Restablecer los valores predeterminados
* Operaciones de capas y efectos de Substance en el menú contextual
* Apoyo a los insumos/productos premultiplicados en sustancias

**Corregido:**

* &amp;lbrack;Vista 3D&amp;rbrack; Los parámetros de sombreador personalizados están separados por un espacio grande
* &amp;lbrack;Exportar&amp;rbrack; Falta la conversión sRGB para el ajuste preestablecido Unity4
* Posible Bloqueo al cargar mallas fbx
* Bloqueo a veces al cargar mallas obj simples
* La barra de cálculo permanece bloqueada al 100% al cargarse
* Volver a cargar una sustancia la coloca en todas las categorías
* Interruptor DirectX/OpenGL roto

### 1.0.1

*(Lanzado: 27 de octubre de 2014)*

**Agregado:**

* &amp;lbrack;Herramienta&amp;rbrack; Uso de parámetros de material mejorado
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
* &amp;lbrack;Exportar&amp;rbrack; Añadir un pase de dilatación antes del postproceso de difusión
* Argumentos de la línea de comandos en SP para operaciones simples
* Nuevos materiales y efectos
* Previsualización de herramientas (área separada de previsualización de materiales en tiempo real y prueba de trazos)
* No crear un documento predeterminado al iniciar Painter
* &amp;lbrack;Herramienta&amp;rbrack; Añadir la posibilidad de editar manualmente un valor de escala de grises
* Varias mejoras para los patrones (Ajustar, Restablecer)
* Las partículas son ahora subherramientas de las herramientas Pincel, Borrador y Proyección
* &amp;lbrack;Vista 3D&amp;rbrack; Usar AO hecho un bake en el procesamiento de la ventana gráfica
* División de los controles de galerías de símbolos entre la vista 2D y 3D
* Ajuste de tamaño de pulgar pequeño en la biblioteca
* Los campos de búsqueda son específicos de cada ventana
* Ajuste de IU

**Corregido:**

* &amp;lbrack;Substance&amp;brack; El conmutador no funciona
* &amp;lbrack;Diálogo de color&amp;rbrack; Degradado de tono no actualizado
* No es posible actualizar una malla si el nombre del archivo es idéntico
* La herramienta no está visible en las vistas cuando es demasiado pequeña
* La herramienta de pegatina de la pantalla Retina no funciona correctamente
* &amp;lbrack;Substance&amp;rbrack; Int1 se muestran como float1
* &amp;lbrack;Substance&amp;rbrack; no se reconoce la entrada/salida basecolor
* &amp;lbrack;Substance&amp;rbrack; los filtros no se pueden volver a cargar
* &amp;lbrack;Herramienta&amp;rbrack; el widget de escala de grises siempre está contraído

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

* El dibujo del mapa de altura no pintura valores negativos.
* La visualización del Selector de material no debe tener en cuenta el mapa de normales muestreado
* Determinismo de partículas roto
* Matriz de esténcil en Vista 2D
* Nombres en archivos obj
* Varios bloqueos

### 0.6.0-beta

*(Lanzado: 04 de junio de 2014)*

**Agregado:**

* Nueva opción de exportación para exportar un mapa de Speculares desde una composición de canales de rugosidad y metálicos

**Corregido:**

* Compatibilidad con Windows Vista
* El mapa de altura no pintura valores negativos

### 0.5.0-beta

*(Lanzado: 7 de mayo de 2014)*

**Agregado:**

* Interruptores 3D/Vista 2D
* Herramienta Selección de fragmentos UV
* La herramienta cambia automáticamente al pintar sobre máscaras.
* La resolución de los Substance depende de la

**Corregido:**

* Bloqueo al iniciar
* Bloqueo con mallas ASCII
* Matriz de galería de símbolos fija en Vista 2D
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
* &amp;lbrack; y &amp;brack; Métodos abreviados de teclado para Tamaño de pincel
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
