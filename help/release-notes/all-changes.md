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
* &lbrack;Pintura de jaula&rbrack; Crear interfaz de usuario básica de Pintura de jaula
* &lbrack;Pintura de jaula&rbrack; Nuevas opciones de visualización de jaulas
* &lbrack;Pintura de jaula&rbrack; Herramienta Selección/Relleno editable
* &lbrack;Pintura de jaula&rbrack; Mostrar modo de Fusión en la barra de herramientas
* &lbrack;Pintura de jaula&rbrack; HDR. cambios de IU del regulador
* &lbrack;Pintura de jaula&rbrack; Sombreador de visualización
* &lbrack;Pintura de jaula&rbrack; Restablecer opciones de pila
* Mejoras de la herramienta Relleno poligonal
* &lbrack;Relleno poligonal&rbrack; Añadir parche de polígono
* &lbrack;Relleno poligonal&rbrack; Añadir bucle de polígono
* &lbrack;Relleno poligonal&rbrack; Compatibilidad de simetría con Bucle/Parche
* &lbrack;Relleno poligonal&rbrack; Vista previa de borde de simetría
* &lbrack;Relleno poligonal&rbrack; Eliminar triángulos con bucles y bucles parciales
* &lbrack;Relleno poligonal&rbrack; Malla metálica visible solo para el conjunto de texturas activo
* &lbrack;Relleno poligonal&rbrack; Resaltado de borde rojo en triángulos que no se pueden hacer clic
* &lbrack;Relleno poligonal&rbrack; No desactive las opciones del modo de relleno
* &lbrack;Relleno poligonal&rbrack; Permitir definir todas las propiedades de canal con Relleno poligonal
* &lbrack;Relleno poligonal&rbrack; El trazo anterior de la reanudación funciona con el relleno poligonal
* &lbrack;Relleno poligonal&rbrack; Mostrar el cursor prohibido en conjuntos de texturas no activos
* &lbrack;Relleno poligonal&rbrack; Previsualización instantánea ALT
* &lbrack;Relleno poligonal&rbrack; Método abreviado para cambiar temporalmente a Polyloop (MAYÚS+A)
* &lbrack;Viewport&rbrack; Mostrar conjunto de texturas/resaltado de selección de Mosaico de UV
* &lbrack;Viewport&rbrack; Añadir soporte para Transparencia Independiente de Pedidos en la ventana gráfica en tiempo real
* &lbrack;Configuración de visualización&rbrack; Reorganizar la configuración de visualización en nuevos grupos
* &lbrack;Herramienta&rbrack; Añadir compatibilidad con la fusión aditiva con trazos de pincel
* &lbrack;Herramienta&rbrack; Añadir compatibilidad con la fusión aditiva con relleno poligonal
* &lbrack;USD&rbrack; Las USD exportadas con mapa de opacidad se vuelven transparentes en Arnold
* &lbrack;Nvidia&rbrack; Agregar advertencia sobre los controladores más recientes de NVIDIA (616.56 a 617.14)
* Añadir nueva entrada de mapa del motor &quot;mesh_uv_next&quot;
* Actualizar bakeres a la versión 3.23.0
* Actualizar el motor de Substance a la versión 9.6.1

**Corregido:**

* &lbrack;Haciendo un bake&rbrack; La oclusión ambiental Ignorar cara posterior por nombre de malla no funciona
* &lbrack;Haciendo un bake&rbrack; &lbrack;AMD&rbrack; Dispositivo perdido al hacer un bake con mallas de polietileno altas y pesadas
* &lbrack;Performance&rbrack; Uso de cerdos VRAM Painter
* &lbrack;Viewport&rbrack; Faltan texturas al abrir proyectos en pantallas HDPI
* &lbrack;Herramienta&rbrack; El modo de fusión aparece atenuado al pintar en una máscara
* Carpetas temporales no eliminadas después de la exportación en la red
* &lbrack;USD&rbrack; La geometría de USD exportada se divide a lo largo de los bordes UV
* &lbrack;USD&rbrack; Bloqueo al cargar USDz mal formado

### 12.1.5

Fecha de publicación: **2026/09/15**

Resumen: **Versión secundaria**

**Corregido:**

* La exportación de imágenes de un estante a una red ya no funciona
* &lbrack;Generador&rbrack; Si se establece &quot;usar textura&quot; en false, no se desactiva el uso de la entrada de textura
* Bloqueo de la ventana gráfica al guardar mientras se edita la proyección 3d
* La resolución de capas de material es demasiado baja

### 12.1.4

Fecha de publicación: **2026/09/04**

Resumen: **Versión secundaria**

**Corregido:**

* &lbrack;Bloqueo&rbrack; Bloqueo al importar o exportar archivos cuyo nombre de archivo contiene caracteres no ASCII

### 12.1.3

Fecha de publicación: **2026/08/26**

Resumen: **Versión secundaria**

**Agregado:**

* Actualizar el motor de Substance a la versión 9.4.6

**Corregido:**

* &lbrack;Selector de escala de grises&rbrack; El selector permanece abierto después de cambiar la herramienta
* &lbrack;Sesgar Hacer un bake&rbrack; La corrección de sesgo se rompe al pintar y deshacer
* &lbrack;Herramienta de proyección&rbrack; La herramienta de proyección bloquea la interacción Ventana gráfica
* &lbrack;Trazo dinámico&rbrack; Faltan parámetros de trazo dinámico en las propiedades del pincel
* La exportación a una red ya no funciona

### 12.1.2

Fecha de publicación: **2026/08/03**

Resumen: **Versión secundaria**

**Corregido:**

* &lbrack;Bloqueo&rbrack; Algunos Substance pueden provocar un bloqueo cuando se procesan
* &lbrack;Bloqueo&rbrack; Volver a importar malla en modo hacer un bake
* &lbrack;Bloqueo&rbrack; Si no se inicializa la visualización de gráficos, se puede producir un bloqueo
* &lbrack;Bloqueo&rbrack; La exportación de texturas puede producir bloqueos en algunos casos al actualizar el registro
* &lbrack;Bloqueo&rbrack; Bloqueo en el modo de hacer un bake en algunos casos al cargar/actualizar el mapa de entorno
* &lbrack;Haciendo un bake&rbrack; Si se vuelve a iniciar hacer un bake después de modificar el archivo de alta poly, se puede producir un bloqueo
* &lbrack;Enviar a Photoshop&rbrack; No se puede exportar la máscara de la capa
* &lbrack;Motor&rbrack; El resultado del punto de anclaje no se procesa entre una máscara y un canal de color

### 12.1.1

Fecha de publicación: **2026/07/09**

Resumen: Versión secundaria

Añadido:

* &lbrack;Sesgar Hacer un bake&rbrack; Exponer sesgo base modo normal: malla o por triángulo
* &lbrack;Propiedades&rbrack; Hacer que los colores uniformes siempre se restablezcan al valor predeterminado de su canal
* &lbrack;OpenPBR&rbrack; Reagrupar canales por categorías en la ventana Exportar Texturas para crear plantillas de salida
* Actualizar el motor de Substance a la versión 9.4.5

Corregido:

* &lbrack;Proyecto&rbrack; Abrir y guardar algunos proyectos puede tardar más de lo habitual
* &lbrack;Bloqueo&rbrack; La recarga de varias mallas puede provocar un bloqueo
* &lbrack;Bloqueo&rbrack; Eliminar un canal mientras está en el modo de vista de máscara provoca un bloqueo
* &lbrack;Bloqueo&rbrack; Algunos Substance pueden provocar un bloqueo cuando se procesan
* &lbrack;Pintura Skew&rbrack; La herramienta Seleccionado en el sesgo de pintura permanece seleccionada después de cambiar al modo de pintura
* &lbrack;Haciendo un bake configuración común&rbrack; La configuración de la distancia de la jaula no actualiza la visualización de la malla metálica de la jaula y el sombreador
* &lbrack;Motor&rbrack; El relleno UV del modo &quot;3D Space Neighbor&quot; no funciona bien en triángulos finos
* &lbrack;Motor&rbrack; El resultado del punto de anclaje no se procesa entre una máscara y un canal de color

### 12.1.0

Fecha de publicación: **2026/06/23**

Resumen: **Esta actualización es una versión importante, contiene mejoras de bakeres con el nuevo estado de IU predeterminado de hace un bake, mapa de sesgo de pintura, reprocesamiento automático, nueva opción para el desajuste UV automático para mallas de superficie dura y OpenPBRs. Para obtener más detalles, vea las notas de la versión completas.**

**Agregado**:

* &lbrack;Sesgar hacer un bake&rbrack; Herramientas de pintura de sesgo
* &lbrack;Sesgar Hacer un bake&rbrack; Adición de sombreadores de previsualización de sesgo y elementos visuales vectoriales de dirección de sesgo al pintar un mapa de sesgo
* &lbrack;Sesgar Hacer un bake&rbrack; Opción Añadir protección de bordes
* &lbrack;Sesgar hacer un bake&rbrack; Reprocesamiento automático
* &lbrack;Sesgar Hacer un bake&rbrack; Interfaz de lista de mapa de malla de reprocesamiento
* &lbrack;Sesgar Hacer un bake&rbrack; Dividir mapa de malla / Configuración de Haga un bake común + Mover configuración común fuera de la lista de mapas de malla solo para colores o máscaras
* &lbrack;Sesgar Hacer un bake&rbrack; Cambiar botones de la barra de herramientas
* &lbrack;Sesgar Hacer un bake&rbrack; Mostrar el conmutador de Simetría para el pincel en la barra de herramientas superior
* &lbrack;Sesgar Hacer un bake&rbrack; Opciones de cambio de nombre en el menú Sincronización de lista de mapa de malla
* &lbrack;Sesgar Hacer un bake&rbrack; Cuadros de diálogo Actualizar estado de sincronización y activado
* &lbrack;Sesgar Hacer un bake&rbrack; Crear variante del selector de color de escala de grises
* &lbrack;Sesgar Hacer un bake&rbrack; Icono Actualizar modo de hacer un bake
* &lbrack;Auto Unwrap&rbrack; Opción Integrar superficie dura
* &lbrack;OpenPBR&rbrack; Añadir soporte para OpenPBR 1.1
* &lbrack;OpenPBR&rbrack; Convertir OpenPBR en el flujo de trabajo y sombreador predeterminados
* &lbrack;OpenPBR&rbrack; Importar materiales y texturas de OpenPBR mediante USD
* &lbrack;OpenPBR&rbrack; Exportar materiales y texturas de OpenPBR mediante USD
* &lbrack;OpenPBR&rbrack; Actualizar la ventana Exportar Texturas para mostrar la convención de nomenclatura del OpenPBR
* &lbrack;OpenPBR&rbrack; Añadir documentación sobre los cambios al OpenPBR de asistencia
* &lbrack;OpenPBR&rbrack;&lbrack;Iray&rbrack; Añada un nuevo MDL para apoyar al OpenPBR 1.1 en Israel
* Varias mejoras menores de las exportaciones USD
* &lbrack;UI&rbrack; Adición de una advertencia en la ventana gráfica al intentar realizar una pintura en otro conjunto de texturas
* &lbrack;Aplanar&rbrack; Permitir acoplar todas las capas con instancias en los conjuntos de texturas
* &lbrack;Configuración del conjunto de texturas&rbrack; Permitir seleccionar varios canales a la vez a través de una nueva ventana
* &lbrack;Historial&rbrack; Actualizar &quot;valor&quot; Deshacer el texto de la entrada para reflejar el nombre del parámetro
* &lbrack;Pila de capas&rbrack; Hacer que los efectos de relleno de las máscaras se vean en blanco de forma predeterminada (1.0)
* &lbrack;Substance&rbrack; Añadir nueva entrada de mapa del motor &quot;mesh_hard_edges_triangle&quot;
* &lbrack;Substance&rbrack; Añadir nueva entrada de mapa del motor &quot;mesh_hard_edges&quot;
* &lbrack;Sombreador&rbrack; Impedir que las instancias del sombreador compartan los mismos nombres
* &lbrack;Sombreador&rbrack; Utilice el sombreador de la plantilla de proyecto al importar un archivo USD o GLTF
* Actualizar Adobe Color Engine a la versión 7.0
* Actualizar la versión mínima de MacOSX a 13.0 (Ventura)
* &lbrack;Contenido&rbrack; Nuevas plantillas de proyecto para el OpenPBR
* &lbrack;Contenido&rbrack; Actualizar proyectos de muestra para utilizar el nuevo sombreador de OpenPBR
* &lbrack;Python&rbrack; Expanda la API de máscara de geometría para permitir modos de inclusión y exclusión como en la interfaz de usuario

**Corregido**:

* &lbrack;Bloqueo&rbrack;&lbrack;Configuración de mapas de malla&rbrack; Aplicación de ajustes a otros conjuntos de texturas
* &lbrack;Bloqueo&rbrack; Al hacer un bake la curvatura del mapa sin el espacio del mundo normal
* &lbrack;Bloqueo&rbrack;&lbrack;Hacer un bake&rbrack; Hacer un bake con jaula personalizada activada pero sin bloqueos de archivo seleccionados
* &lbrack;Bloqueo&rbrack; Cancelación de hace un bake de AO
* &lbrack;Auto-Cage&rbrack; Carga infinita cuando la ruta del archivo de poli alto no es válida
* &lbrack;Linux&rbrack;&lbrack;Windows&rbrack; El selector de color a veces puede ser completamente negro o no aparecer
* &lbrack;Herramienta Relleno poligonal&rbrack; La herramienta no funciona con sistemas que no sean PBR
* &lbrack;&lbrack;Pintura&rbrack; Al eliminar el canal de color base no se elimina el color pintado anteriormente
* &lbrack;USD&rbrack; No se detectan correctamente todas las instancias del sombreador
* &lbrack;Substance&rbrack; Solo se tiene en cuenta el primer uso de un nodo de entrada/salida
* &lbrack;Sombreador&rbrack; La oclusión ambiental se aplica dos veces con conjuntos de texturas utilizando diferentes métodos de mezcla
* &lbrack;Motor&rbrack; Las texturas normales con un canal azul vacío (negro) pueden producir resultados de mezclas incorrectos
* &lbrack;GLTF Import&rbrack; La fusión alfa está activada en todos los conjuntos de texturas
* &lbrack;GLTF Export&rbrack; La fusión alfa siempre está activada en la exportación
* &lbrack;Exportar&rbrack; La geometría de doble cara siempre está desactivada al importar un fichero GLTF
* &lbrack;Javascript&rbrack; La modificación de la configuración de sombreadores no contribuye al historial de deshacer
* &lbrack;Muestras&rbrack; La dispersión subsuperficial no está activada en la configuración de visualización para Meet Mat

### 12.0.3

Fecha de publicación: **2026/05/05**

Resumen: **Versión secundaria**

**Agregado:**

* Actualizar bakeres a la versión 3.2.2
* Actualizar el motor de Substance a la versión 9.4.3
* &lbrack;Python&rbrack; Guardar un material inteligente en una ubicación específica

**Corregido:**

* &lbrack;Ubuntu&rbrack; Bloqueo al seleccionar material
* &lbrack;Mac&rbrack; Aparece una ventana emergente recurrente para solicitar acceso a los datos de otras aplicaciones
* &lbrack;Haciendo un bake&rbrack; Pueden aparecer defectos en el mapa de curvatura
* &lbrack;Haciendo un bake&rbrack; Hacer un bake es más lento en algunos casos
* &lbrack;Deformar a geometría&rbrack; La deformación de la geometría se desactiva en algunos casos
* &lbrack;Mosaico de UV&rbrack; El alfa extraído del punto de anclaje es ignorado por otros mosaicos
* &lbrack;Python&rbrack;&lbrack;Mac&rbrack; Excepciones en la consola de Python con SSL
* &lbrack;Python&rbrack; bloqueo de Painter a la salida con widgets Qt sobrantes

### 12.0.2

Fecha de publicación: **2026/04/07**

Resumen: **Versión secundaria**

**Agregado:**

* &lbrack;Administración de color&rbrack; Añada nuevos OCIO para especificar el espacio de color predeterminado del selector de color
* &lbrack;Python&rbrack; Exponer la configuración de desajuste automático en la API de Python

**Corregido:**

* &lbrack;Bloqueo&rbrack; Si no hay suficiente espacio en disco, los proyectos se pueden dañar o almacenar en bloqueo
* &lbrack;Bloqueo&rbrack; &lbrack;Cinta&rbrack; El uso de la cinta puede causar bloqueos en algunos proyectos
* &lbrack;Bloqueo&rbrack; &lbrack;Haciendo un bake&rbrack; bloqueo cuando el archivo .assbin no se puede escribir en la carpeta
* &lbrack;Importar&rbrack; OBJ mallas de Stager pueden fallar en la creación del proyecto
* &lbrack;Importar&rbrack; OBJ ha perdido la cara en algunos casos
* &lbrack;Importar&rbrack; USD malla sin ningún material asignado puede generar bloqueo al importarla
* &lbrack;Ruta de acceso rellena&rbrack; No se ve afectado por la simetría
* &lbrack;Stencil&rbrack; La previsualización tiene una resolución inferior a la del resultado pintado
* &lbrack;UI&rbrack; &#39;uv island&#39; sigue apareciendo en la información sobre herramientas de origen de color del mapa de ID
* &lbrack;Mostrar&rbrack; Las sombras aparecen invertidas
* &lbrack;Viewport&rbrack; La proyección de deformación transforma los restos después de cambiar al modo de hacer un bake
* &lbrack;Deformar&rbrack; La cuadrícula desaparece cuando la escala se establece en 0 en el eje Z con la opción Deformar en geometría activada
* &lbrack;Python&rbrack; Error inesperado al agregar un canal con modificación de ámbito

### 12.0.1

Fecha de publicación: **2026/03/18**

Resumen: **Versión secundaria**

**Corregido:**

* &lbrack;Bloqueo&rbrack;&lbrack;Congelar&rbrack; Exportación desde proyectos específicos

### 12.0.0

Fecha de publicación: **2026/03/09** Resumen: **Esta es una versión importante. Esta versión contiene las funciones de acoplar capas, deformar en geometría, nuevos efectos de posprocesamiento, mejoras en la nueva ventana de proyecto y otras mejoras.**

**Agregado**:

* &lbrack;Acoplar capas&rbrack; Acoplamiento de capas dentro de la pila de capas
* &lbrack;Acoplar capas&rbrack; Exportar capas acopladas al disco
* &lbrack;Deformar a geometría&rbrack; Adición de una nueva función de deformación automática a las proyecciones de deformación
* &lbrack;Post-effects&rbrack; Sustituya los efectos de posprocesamiento por otros nuevos
* &lbrack;Post-effects&rbrack; Actualizar asignador de tonos
* &lbrack;Post-effects&rbrack; Añadir nuevo uso para recursos posteriores a los efectos
* &lbrack;Content&rbrack;&lbrack;Post-effects&rbrack; Integrar activos predeterminados posteriores a los efectos en la biblioteca
* &lbrack;Nuevo proyecto&rbrack; Mejorar la interfaz de usuario para la creación de proyectos
* &lbrack;Nuevo proyecto&rbrack; Cambios en la función de reimportación de malla
* &lbrack;Nuevo proyecto&rbrack; Permitir la apertura de archivos \*.geo.usd
* &lbrack;Configuración del proyecto&rbrack; Mejorar la interfaz de usuario para la configuración del proyecto
* Actualizar USD biblioteca a la versión 25.05
* Actualizar Substance Engine a la versión 9.3.4
* Aumentar controladores mínimos a 25.3.1/25.Q2 para las GPU AMD
* Actualizar Qt a 6.8.6
* &lbrack;Secuencias de comandos&rbrack; Actualizar la API de JavaScript a la versión 1.1.20
* Actualizar Python a 3.13

**Corregido:**

* &lbrack;Bloqueo&rbrack; El cambio de una salida de canal de material en una máscara puede provocar un bloqueo
* &lbrack;Importar&rbrack; Las texturas de EXR se fuerzan en sRGB en lugar de lineales al importar archivos USD
* &lbrack;Mosaicos de UV&rbrack; La secuencia de imágenes con una sola imagen también llena otros Mosaicos de UV
* &lbrack;Haciendo un bake&rbrack; El AO es diferente entre la CPU y la GPU al hacer un bake
* &lbrack;Administración de color&rbrack;&lbrack;MacOS&rbrack; El color base de la ventana gráfica no coincide con el selector de color
* &lbrack;USD&rbrack; Los valores uniformes no se importan en algunos casos

## Versión 11

### 11.1.3

Fecha de publicación: **2026/02/12** Resumen: **Versión secundaria**

**Corregido**:

* &lbrack;Pintura&rbrack; La plantilla y la simetría no funcionan en algunos casos
* &lbrack;Ruta&rbrack; No hay actualizaciones al cambiar el regulador de opacidad del trazo de difuminado
* &lbrack;Proyecto&rbrack; No se puede realizar la pintura en alguna geometría
* &lbrack;Cinta&rbrack; El trazado instanciado desaparece al cambiar la resolución del conjunto de texturas
* &lbrack;UI&rbrack; El selector de color se puede reducir y desaparecer en algunos casos

### 11.1.2

Fecha de publicación: **2026/01/13** Resumen: **Versión secundaria**

**Agregado**:

* &lbrack;Haciendo un bake&rbrack; Mejorar el tiempo de hace un bake del proyecto de Mosaicos de UV con el guardado asíncrono
* &lbrack;Shaders&rbrack; Mención en cambios de registro de API del sombreador tras migración de Vulkan
* Actualizar OpenEXR a la versión 3.4.4

**Corregido**:

* &lbrack;Bloqueo&rbrack; Bloqueo durante el inicio en la serie Nvidia GTX 10xx
* &lbrack;Bloqueo&rbrack; El uso del selector de color en diferentes conjuntos de texturas puede provocar un bloqueo al salir de la aplicación
* &lbrack;Rendimiento&rbrack; Problema de rendimiento al pintar en un proyecto con muchas capas
* &lbrack;Rendimiento&rbrack; Retraso al pintar con un lápiz de Tablet PC gráfico
* &lbrack;UI&rbrack; Los ajustes de la cámara permanecen desactivados en el modo de procesamiento (Iray)
* &lbrack;Cinta&rbrack; El trazado puede superponerse inesperadamente después de una esquina en algunos casos
* &lbrack;Cinta&rbrack; Problema de rendimiento con Mosaicos de UV
* &lbrack;Substance&rbrack;&lbrack;UI&rbrack; Las entradas de imagen desaparecen al contraerse
* &lbrack;Substance&rbrack;&lbrack;UI&rbrack; Los grupos anidados pueden permanecer aunque Visible si los oculte
* &lbrack;Haciendo un bake&rbrack;&lbrack;UI&rbrack; No se puede establecer el radio de muestreo de curvatura más allá de 0,01
* &lbrack;Haciendo un bake&rbrack;&lbrack;UI&rbrack; No se puede establecer la distancia máxima del oclusor más allá de 1
* &lbrack;Haciendo un bake&rbrack; El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y hago un bake bajo como alto
* &lbrack;Haciendo un bake&rbrack; El mapa de ID no hace un bake los colores de vértice de FBX en modo Bajo como Alto
* &lbrack;Contenido&rbrack; El filtro Paso alto genera colores atenuados en canales con gestión de color

### 11.1.1

Fecha de publicación: **2025/12/09** Resumen: **Versión secundaria**

**Agregado**:

* &lbrack;Rendimiento&rbrack; Mejorar el rendimiento de los Mosaicos de UV al calcular texturas parciales
* &lbrack;Bakeres&rbrack; Actualizar a la versión 3.15.4

**Corregido**:

* &lbrack;Bloqueo&rbrack;&lbrack;MacOS&rbrack; Bloqueo de guardar siempre el proyecto de la versión anterior
* &lbrack;Bloqueo&rbrack; El cierre de un proyecto a veces puede provocar un bloqueo
* &lbrack;Proyecto&rbrack; Error &quot;los miembros no coinciden en el recuento&quot; al abrir el proyecto realizado en la versión anterior
* &lbrack;Haciendo un bake&rbrack; Los Mosaicos de UV no se combinan con los resultados hechos un bake anteriores, si los hay
* &lbrack;Haciendo un bake&rbrack; Dispositivo perdido incluso con el trazado de rayos desactivado en la serie Nvidia GTX 10XX
* &lbrack;Haciendo un bake&rbrack; El AO con normal tiene defectos en los bordes porque no hay relleno
* &lbrack;Haciendo un bake&rbrack; El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y &quot;coincidencia por nombre&quot; en
* &lbrack;Haciendo un bake&rbrack; El mapa de ID es totalmente negro si a alguna malla de alta densidad le faltan colores de vértice
* &lbrack;Cinta&rbrack; La información sobre herramientas del modo de fusión Alfa menciona el modo de fusión de pantalla en lugar de Sobreexposición lineal
* &lbrack;Ruta&rbrack; Las tangentes crean un bucle inesperado cuando el punto se mueve de cerca a los extremos del trazado
* &lbrack;Herramienta&rbrack; La previsualización de material no funciona cuando se utiliza la proyección en una máscara
* &lbrack;Motor&rbrack; Pintar trazos pequeños puede dar como resultado artefactos de bloque
* &lbrack;Sombreador&rbrack; Al deshacer la creación de la instancia del sombreador, no se elimina correctamente
* &lbrack;Exportar&rbrack; El modo de Alpha para la exportación GLTF siempre está establecido en MASK
* &lbrack;Python&rbrack; Error inesperado al editar la pila de capas fuera del bloque de modificación del ámbito

**Problemas conocidos**:

* &lbrack;Cinta&rbrack; Problema de rendimiento con Mosaicos de UV
* &lbrack;Cinta&rbrack; El trazado puede superponerse inesperadamente después de una esquina en algunos casos
* &lbrack;Bloqueo&rbrack;&lbrack;Cinta&rbrack; La creación de textos muy largos en la cinta de opciones puede causar bloqueo
* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;Motor&rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &lbrack;Python&rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.1.0

Fecha de lanzamiento: **18/11/2025** Resumen: **Esta actualización es una versión importante, contiene la nueva herramienta Cinta de opciones con contenido nuevo dedicado, compatibilidad de simetría para capas de relleno, parámetro de tamaño físico para desplazamiento, rendimiento mejorado a través de los bakeres actualizados, compatibilidad total con Vulkan para Windows y Linux y otras mejoras.**

**Agregado**:

* Nueva herramienta de cinta
* &lbrack;Herramienta&rbrack; Agregar nueva herramienta Cinta para crear trazados perfectos
* &lbrack;Cinta&rbrack; Añadir métodos abreviados de cinta preestablecidos en la ventana Propiedades
* &lbrack;Cinta&rbrack; Permitir cambiar la opacidad de la cinta de opciones por vértice en el trazado
* &lbrack;Cinta&rbrack; Permitir cambiar el tamaño de la cinta de opciones por vértice en el trazado
* &lbrack;Cinta&rbrack; Quitar el inicio/fin definido en un Substance cuando las rutas están cerradas
* &lbrack;Cinta&rbrack; Vista previa de Eliminar trazado/material en la ventana de propiedades para las herramientas Pintura/Borrador/Dedo de trazado
* &lbrack;Cinta&rbrack; Añada modos de fusión para el alfa y algunos canales cuando se superpongan automáticamente
* Rellenar simetría
* &lbrack;Rellenar&rbrack; Añadir compatibilidad con la simetría en capas y efectos de relleno
* &lbrack;Fill&rbrack;&lbrack;UI&rbrack; Mostrar la configuración de simetría en la ventana de propiedades para capas y efectos de relleno
* &lbrack;Rellenar&rbrack; Interfaz de usuario de reprocesamiento de la configuración de simetría tanto en el menú Ventana como en la ventana Propiedades
* &lbrack;Rellenar&rbrack; Reorientar correctamente las texturas normales al proyectar en modo de deformación
* desplazamiento tamaño físico
* &lbrack;Desplazamiento&rbrack; Usar tamaño físico como unidad de desplazamiento
* Mejora del rendimiento
* &lbrack;Rendimiento&rbrack; Mejorar la representación de trazos de pincel pequeños en triángulos grandes
* &lbrack;Rendimiento&rbrack; Mejorar el tiempo de compilación del Sombreador
* &lbrack;Rendimiento&rbrack; Compatibilidad total con Vulkan para Windows y Linux
* &lbrack;Rendimiento&rbrack; Bakeres actualizados con procesamiento de GPU más rápido y compatibilidad con trazados de rayos AMD
* &lbrack;UI&rbrack; Reorganizar las propiedades de las herramientas en grupos y contraer algunos de forma predeterminada
* &lbrack;Motor&rbrack; Actualizar Substance Engine a la versión 9.2.5
* &lbrack;Substance&rbrack; Anulación de resolución de exposición para recursos de Substance en Herramientas y rellenos
* &lbrack;Exportar&rbrack; Actualizar ajuste preestablecido de exportación de Mapas de malla para exportar texturas en escala de grises
* Python
* &lbrack;Haciendo un bake&rbrack;&lbrack;Python&rbrack; Indicar en el registro de cambios los cambios después de actualizar bakeres
* &lbrack;Python&rbrack; Exponer la configuración de simetría de relleno en Python
* Contenido y nuevo contenido
* &lbrack;Contenido&rbrack; Añadir 75 nuevos ajustes preestablecidos de herramientas para la herramienta Cinta de opciones
* &lbrack;Contenido&rbrack; Actualizar el recurso generador de degradados para que sea compatible con la cinta de opciones

**Corregido**:

* &lbrack;Bloqueo&rbrack; La carga de otro proyecto mientras el ajuste de ruta está activado puede causar bloqueos
* &lbrack;Bloqueo&rbrack; Al hacer clic con el botón derecho en el panel Trazado con información de otra sesión del portapapeles, se puede crear un bloqueo
* &lbrack;UI&rbrack; La interfaz se desplaza hacia arriba en las propiedades de la herramienta al crear un trazado
* &lbrack;UI&rbrack; El cursor del ratón desaparece cuando la visualización de la ventanilla de trazado está oculta
* &lbrack;Ruta&rbrack; Copiar/pegar diferentes propiedades de herramienta en el panel Trazado genera propiedades inestables
* &lbrack;Herramienta&rbrack; Los ajustes preestablecidos de las herramientas Borrador y Difuminado no siempre actualizan la selección de canales
* &lbrack;Herramienta&rbrack; El valor pintado es gris, pero la interfaz de usuario muestra blanco después de cargar el ajuste preestablecido de herramientas de color en la máscara
* &lbrack;Herramienta&rbrack; El ajuste preestablecido creado a partir de la máscara conserva los valores de canales cargados de otro ajuste preestablecido
* &lbrack;Substance&rbrack; No se tiene en cuenta la anulación del espacio de color normal definido en el gráfico
* &lbrack;Contenido&rbrack; El recurso de forma de pincel predeterminado utiliza un Substance obsoleto

**Problemas conocidos**:

* El historial de instancias del sombreador no se rastrea correctamente
* &lbrack;Cinta&rbrack; Problema de rendimiento con Mosaicos de UV
* &lbrack;Cinta&rbrack; El trazado puede superponerse inesperadamente después de una esquina en algunos casos
* &lbrack;Cinta&rbrack; Las tangentes crean bucles no deseados cuando el punto se mueve de cerca a los extremos del trazado
* &lbrack;Bloqueo&rbrack;&lbrack;Cinta&rbrack; La creación de textos muy largos en la cinta de opciones puede causar bloqueo
* &lbrack;Herramienta&rbrack; La previsualización de material no funciona cuando se utiliza la proyección en una máscara
* &lbrack;Haciendo un bake&rbrack; El ajuste de AO &quot;Oclusión automática&quot; se ignora con varios conjuntos de texturas y &quot;coincidencia por nombre&quot; activado
* &lbrack;Haciendo un bake&rbrack; El AO con normal tiene defectos en los bordes debido a la falta de relleno
* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;Motor&rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &lbrack;Python&rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.0.3

Fecha de publicación: **2025/08/05** Resumen: **Versión secundaria**

**Agregado**:

* &lbrack;Substance 3D Assets&rbrack; Adición de un punto de notificación al panel Activos 3D
* &lbrack;VFX Platform 2025&rbrack; Añadir ACE configuración 2.0 en la configuración de gestión de color
* &lbrack;VFX Platform 2025&rbrack; Actualice OCIO a la versión 2.4.2
* Actualizar Iray a la versión 2024.10
* &lbrack;Motor&rbrack; Actualizar a Substance Engine v.9.2.3
* &lbrack;Nvidia&rbrack; Aumentar la versión mínima de controladores de NVIDIA a 572.60 (Windows) y 570.169 (Linux)

**Corregido**:

* &lbrack;Python&rbrack; La modificación de ámbito no aparece en la ventana Historial

**Problemas conocidos**:

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;Motor&rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &lbrack;Python&rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.0.2

Fecha de publicación: **2025/06/10** Resumen: **Versión secundaria**

**Agregado**:

* &lbrack;Mac&rbrack; Agregar advertencia sobre versiones específicas del sistema operativo que producen artefactos
* &lbrack;Actualización automática&rbrack; Mejoras menores de UX en el registro de errores de Activos
* &lbrack;Desenvolvimiento automático&rbrack; Actualice a la versión 1.3.2 con mejoras de unión
* &lbrack;USD&rbrack;&lbrack;FBX&rbrack; Añade compatibilidad con varios conjuntos UV con datos dispersos
* &lbrack;Exportar&rbrack; Las mallas exportadas como FBX no tienen sus conjuntos UV adicionales si los hay durante la importación

**Corregido**:

* &lbrack;MacOS&rbrack;&lbrack;Linux&rbrack; Bloqueo al guardar en la unidad de red
* &lbrack;Win&rbrack;&lbrack;Tablet&rbrack; Parpadeo al realizar una panorámica
* &lbrack;SpaceMouse&rbrack; Problema al trabajar con la herramienta Trazado
* &lbrack;Auto-cage&rbrack; No se puede hacer un bake después de una recarga de malla
* &lbrack;Actualización automática&rbrack; La secuencia de imágenes no se vuelve a cargar cuando falta el primer mosaico
* &lbrack;Ruta&rbrack; La tangente personalizada puede afectar a otras tangentes
* &lbrack;Ruta&rbrack; El trazado no aparece en el conjunto de texturas si el primer punto está en otro conjunto de texturas
* &lbrack;UI&rbrack; Algunos menús siempre se desactivan después de abrir un proyecto (por ejemplo: simetría)
* &lbrack;Propiedades&rbrack; No es posible utilizar/cargar ajustes preestablecidos de herramientas con la herramienta Trazado relleno
* &lbrack;USD&rbrack; No se reconocen varios conjuntos UV en el sombreador personalizado al utilizar archivos USD
* &lbrack;USD&rbrack; Las cámaras con los mismos nombres se anulan
* &lbrack;Exportar&rbrack; Enviar a Photoshop genera un espacio de color incorrecto para los resultados de color y escala de grises
* &lbrack;Exportar&rbrack; Los canales de escala de grises con alfa se exportan como color en lugar de como escala de grises con formato PNG
* &lbrack;Exportar&rbrack; La exportación de un canal de escala de grises como PSD genera un archivo no válido o truncado
* &lbrack;Contenido&rbrack; El filtro de deformación en modo multidireccional no funciona
* &lbrack;Python&rbrack; No se puede asignar el error de lista al rastrear nodos de pila de capas

**Problemas conocidos**:

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;Motor&rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &lbrack;Python&rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.0.1

Fecha de publicación: **2025/04/10** Resumen: **Versión secundaria**

Nota: La versión de **Linux CCD se retrasará hasta el 29 de abril**

**Agregado:**

* Actualizar a Qt 6.5.8
* &lbrack;Substance&rbrack; Agregar mensaje de registro para filtros cuando varias entradas de imagen comparten el mismo uso
* &lbrack;Nvidia&rbrack; Agregar advertencia sobre los controladores más recientes de NVIDIA (572.47)

**Corregido:**

* &lbrack;Bloqueo&rbrack; Al arrastrar y soltar una barra lateral con un uso en ranuras de un solo canal
* &lbrack;Bloqueo&rbrack;&lbrack;Path&rbrack; La opción Cambiar tipo de trazado no está atenuada al no hacer clic en un trazado específico
* &lbrack;Rellenar ruta&rbrack; No debería poder seleccionar material de la sustancia
* &lbrack;Motor&rbrack; Artefactos a lo largo de trazos de pincel
* &lbrack;Motor&rbrack; Los trazados se pueden romper con ajustes específicos
* Problema con el menú desplegable para el espacio de color del cuentagotas
* &lbrack;Actualización automática&rbrack; &lbrack;Python&rbrack; Mensaje de error incorrecto al utilizar ResourceID sin versión
* &lbrack;Sombreador&rbrack; Bloqueo al abrir algunos proyectos

**Problemas conocidos:**

* &lbrack;SpaceMouse&rbrack; Problema al trabajar con la herramienta Trazado
* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;Motor&rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &lbrack;Python&rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento

### 11.0.0

Fecha de lanzamiento: **2025/03/11** Resumen: **Versión principal, nueva función de actualización automática, herramienta Ruta de acceso rellena y otras mejoras en la ruta, así como nuevos filtros y una generación experimental de Jaula automática para hacer un bake**

**Agregado**:

* Actualización automática
* &lbrack;Actualización automática&rbrack; Actualización automática de activos modificados en el panel Activos
* &lbrack;Actualización automática&rbrack; Actualización automática de activos modificados en todo el proyecto
* &lbrack;Actualización automática&rbrack; Mantener desactivada la actualización automática de forma predeterminada
* &lbrack;Actualización automática&rbrack; Hacer que la actualización sea opcional si los parámetros del recurso no coinciden (.sbsar, .glsl, .ai, .svg)
* &lbrack;Actualización automática&rbrack; Añadir variable de entorno para desactivar la función de actualización automática
* &lbrack;Actualización automática&rbrack;&lbrack;SBSAR&rbrack; Convertir la actualización en opcional si los parámetros del recurso no coinciden
* Trazado relleno
* &lbrack;Ruta&rbrack;&lbrack;Rellenar&rbrack; Añadir una nueva herramienta para crear trazados rellenos
* Mejoras de ruta
* &lbrack;Ruta&rbrack; Crear trazado que se ajusta a polígonos
* &lbrack;Ruta&rbrack; Permitir cambiar los tipos de ruta
* &lbrack;Ruta&rbrack; Permitir copiar y pegar datos de vértices de trazado entre contenido y máscara
* &lbrack;Ruta&rbrack; Permitir para restringir el ángulo al crear un nuevo punto
* &lbrack;Ruta&rbrack; Permitir la creación de puntos de restricción en una línea
* &lbrack;Ruta&rbrack; Cerrar forma con un solo clic
* &lbrack;Ruta&rbrack; Mostrar información de ruta
* &lbrack;Ruta&rbrack; Permitir escalar y rotar vértices de trazado
* &lbrack;Path&rbrack;&lbrack;UX&rbrack; Facilita el acceso a las herramientas de transformación
* &lbrack;Ruta&rbrack; Añadir previsualización de trazado
* &lbrack;Ruta&rbrack; Desactivar la previsualización de trazado con Mayús + P
* &lbrack;Ruta&rbrack; Mejorar la edición de tangentes desde la vista lateral
* &lbrack;Ruta&rbrack; Permitir el enfoque en una ruta 3D
* &lbrack;Ruta&rbrack; Los vértices deben conservar el estado de selección al activar o desactivar la IU de nuevo
* &lbrack;Ruta&rbrack; Permitir la eliminación de la ruta mediante Retroceso
* &lbrack;Ruta&rbrack; Mantener lista de rutas abierta si el usuario la expande
* &lbrack;Ruta&rbrack;&lbrack;Pila de capas&rbrack; Cambiar el nombre de los duplicados al copiar y pegar correctamente
* &lbrack;Ruta&rbrack; Mejoras en la IU y la información sobre herramientas
* Rendimiento
* &lbrack;Rendimiento&rbrack; Mejorar el rendimiento de la ventanilla al utilizar un nivel de teselación alto
* &lbrack;Rendimiento&rbrack; Habilitar solo el primer canal en nuevas capas/efectos de relleno
* &lbrack;Rendimiento&rbrack; Paralelizar cálculo de trazo de pincel
* Baking
* &lbrack;Haciendo un bake&rbrack; Añadir nueva opción de generación de jaulas totalmente automática para hacer un bake con mallas de alto contenido de polietileno (experimental)
* Contenido
* &lbrack;Contenido&rbrack; Añade 6 filtros nuevos: estilización, cuantificar, anisotrópico kuwahara, suavizado de bisel, distancia direccional, conversión de escala de grises
* &lbrack;Contenido&rbrack; Actualizar Noises y Grunges a la última versión de Designer (con el nuevo 2D Voronoi)
* &lbrack;Contenido&rbrack; Añadir 3 nuevos generadores de textura (Azulejo Aleatorio, Triangle Grid, Generador de Scratches)
* &lbrack;Contenido&rbrack; Cambiar nombre de plantilla de Unreal Engine y exportar ajustes preestablecidos
* Python
* &lbrack;Shelf&rbrack;&lbrack;Python&rbrack; Guardar material inteligente o máscara inteligente en disco desde Python
* &lbrack;Python&rbrack; Añadir la jaula automática de hace un bake a la API de Python
* &lbrack;Python&rbrack; Permitir editar nombres y descripciones de conjuntos de texturas/Mosaicos de UV
* &lbrack;Python&rbrack; Compartir la configuración de resolución en fuentes vectoriales y de fuentes
* &lbrack;Actualización automática&rbrack;&lbrack;Python&rbrack; Exponer las funcionalidades de actualización automática del proyecto en Python
* Varios
* &lbrack;Exportar&rbrack; Facilitar el acceso a las opciones Enviar a con un nuevo panel
* &lbrack;Nvidia&rbrack; Agregar advertencia sobre los controladores más recientes de NVIDIA (572.16)
* El ajuste de ángulo debe verse afectado por la selección de espacio Objeto/Mundo
* &lbrack;Lista de conjuntos de texturas&rbrack; Permitir agregar nombres personalizados a los Mosaicos de UV y utilizarlos en la exportación
* Mac
* &lbrack;Mac&rbrack; Uso de Metal en lugar de OpenGL para el procesamiento de gráficos
* &lbrack;Mac&rbrack; Retirar la asistencia de Mac Intel

**Corregido**:

* &lbrack;Bloqueo&rbrack; Eliminar entrada de imagen
* No se puede agregar una alfombra inteligente mediante el botón de pila de capas
* &lbrack;Python&rbrack; No se pueden encontrar efectos en GroupLayerNode

**Problemas conocidos**:

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;MacOS Intel&brack; Bloqueo al importar algunos ajustes preestablecidos
* &lbrack;Motor&rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &lbrack;Python&rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento
* &lbrack;RedHat&rbrack; Problemas con el selector de color

## Versión 10

### 10.1.2

Fecha de publicación: **2024/12/3** Resumen: **Versión secundaria, correcciones de errores**

**Corregido**:

* &lbrack;Bloqueo&rbrack; Eliminar entrada de imagen
* No se puede agregar una alfombra inteligente mediante el botón de pila de capas
* &lbrack;Python&rbrack; No se pueden encontrar efectos en GroupLayerNode

**Problemas conocidos**:

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;MacOS Intel&brack; Bloqueo al importar algunos ajustes preestablecidos
* &lbrack;Motor&rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &lbrack;Python&rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento
* &lbrack;RedHat&rbrack; Problemas con el selector de color

### 10.1.1

Fecha de publicación: **2024/11/5** Resumen: **Versión secundaria, correcciones de errores**

**Agregado**:

* &lbrack;Proyecto&rbrack; Mantener abierto el proyecto actual hasta que se valide la nueva selección de proyecto
* &lbrack;Desenvolvimiento automático&rbrack; La densidad del texel permite dividir mejor las Islas de UV en UDIM
* &lbrack;Haciendo un bake&rbrack; Corregir copia ambigua en el menú contextual de Mapas de malla
* &lbrack;Deformar&rbrack; Eliminación de la escala en la ventanilla del eje Z (profundidad)
* &lbrack;Importar/Exportar&rbrack; Eliminar la compatibilidad con formatos de archivo de imagen no utilizados
* Actualizar Substance Engine a 9.1.4

**Corregido**:

* &lbrack;Bloqueo&rbrack; Después de reubicar el recurso en Recursos y guardar el proyecto
* &lbrack;Bloqueo&rbrack; Problemas con la biblioteca de aiserver
* &lbrack;Bloqueo&rbrack; bloqueo de servidor Illustrator en algunos casos excepcionales
* &lbrack;Bloqueo&rbrack; En algunos casos raros, al salir de la aplicación
* No se pueden enviar informes de bloqueo en algunos equipos
* &lbrack;Haciendo un bake&rbrack; El color del vértice no se lee correctamente
* &lbrack;UI&rbrack; La ubicación de las ventanas y las novedades al inicio se cambian
* &lbrack;Assimp&rbrack; No se reconoce la superficie estándar de Maya al hacer un bake ID
* &lbrack;Python&rbrack; La biblioteca SSL que falta genera un error
* &lbrack;Python&rbrack;&lbrack;Win&rbrack; Error al llamar a QColorConstants.Transparent
* &lbrack;Python&rbrack; Las miniaturas de capas creadas mediante Python no se actualizan hasta que se hace clic dentro de la pila de capas
* &lbrack;Sombreador&rbrack; Vínculo roto en el registro de cambios de API del sombreador
* &lbrack;3D Assets&rbrack; Usar la configuración del proxy del sistema operativo al acceder a recursos 3D

**Problemas conocidos**:

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;MacOS Intel&brack; Bloqueo al importar algunos ajustes preestablecidos
* &lbrack;Motor&rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &lbrack;Python&rbrack; Widget que parece eliminado a través de script todavía funciona
* &lbrack;RedHat&rbrack; Problemas con el selector de color

### 10.1.0

Fecha de publicación: **17/09/2024** Resumen: **Versión principal, contenido nuevo: Filtro de color/máscara de área de relleno, filtro de pegatinas de bordado y seis filtros de Substance genéricos, USD de importación con propiedades de material y sombreador, mejora del rendimiento, compatibilidad con VFX Platform 2024 y migración a Linux RedHat**

**Agregado**:

* &lbrack;Contenido&rbrack; Añadir nuevo filtro de color/máscara de área de relleno
* &lbrack;Contenido&rbrack; Añadir nuevo filtro de pegatinas de bordado
* &lbrack;Contenido&rbrack; Añade 6 nuevos filtros Substance genéricos (FXAA, pixelado, paso alto, posterizar, paso suave y umbral)
* &lbrack;USD&rbrack; Exportar USD capa con un material de ASM definido
* &lbrack;USD&rbrack; Importar USD con propiedades de materiales y sombreadores
* &lbrack;Rendimiento&rbrack; Habilitar miniaturas de pila de capas optimizadas de forma predeterminada
* &lbrack;Rendimiento&rbrack; Reducir el tiempo de apertura de archivos de proyecto y el consumo de memoria (descodificación de datos)
* Compatible con la plataforma VFX 2024
* &lbrack;VFX Platform 2024&rbrack; Actualizar a Python 3.11
* &lbrack;VFX Platform 2024&rbrack; Actualización a OpenEXR 3.2
* &lbrack;VFX Platform 2024&rbrack; &lbrack;USD&rbrack; Actualizar OpenSubdiv 3.6.0
* &lbrack;Plataforma VFX 2024&rbrack;&lbrack;Administración de color&rbrack; Actualizar a OCIO 2.3.2
* &lbrack;Linux&rbrack; Migración a Linux RedHat
* &lbrack;Linux&rbrack; Actualizar la versión principal del controlador Nvidia a 535.171.04
* &lbrack;Importar&rbrack; Adición de una opción para voltear el mapa de normales al importar una malla GLTF
* &lbrack;UI&rbrack; Usar el valor predeterminado del sistema operativo para la distancia de detección de eventos de arrastre
* &lbrack;Substance Engine&rbrack; Agregar función de tira de llamadas para eliminar los símbolos del ejecutable
* &lbrack;Pantalla de bienvenida&rbrack; Actualizar al nuevo formato de pantalla de bienvenida
* Actualizar Substance Engine a la versión 9.1.3
* &lbrack;Python&rbrack; Mostrar vínculos a ejemplos en el menú de documentación de la pila de capas
* &lbrack;JavaScript&rbrack; Mover complementos de Javascript a la subcarpeta javascript/plugins

**Corregido**:

* &lbrack;Illustrator&rbrack; Bloqueo al exportar un Mosaico de UV con un gráfico .ai en casos específicos
* &lbrack;Trazos dinámicos&rbrack;&lbrack;Path&rbrack; La opción aleatoria por trazo no funciona en un trazado
* &lbrack;UI&rbrack;&lbrack;Propiedades&rbrack; El bloqueo se activa cuando el mosaico no es uniforme
* El archivo TXT de depuración se crea al hacer doble clic en el proyecto de Painter
* &lbrack;USD&rbrack;&lbrack;Export&rbrack; Es posible que falten algunas texturas
* &lbrack;ASM&rbrack; Dispersión El canal de color ignora los colores metálicos
* &lbrack;Contenido&rbrack; El filtro de desenfoque no funciona en el espacio de color &quot;operativo&quot;
* &lbrack;Contenido&rbrack; Height Ajustar filtro también modifica el alfa de la capa

**Problemas conocidos**:

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Win&rbrack;&lbrack;Bloqueo&rbrack; &lbrack;ACE&rbrack; No utilizar el espacio de color sRGB ICE para transformar la visualización
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;MacOS Intel&brack; Bloqueo al importar algunos ajustes preestablecidos
* &lbrack;Bloqueo&rbrack; Reubicar recurso y guardar proyecto
* &lbrack;Motor&rbrack; Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* &lbrack;Python&rbrack; El widget fantasma aparece eliminado por el script todavía en funcionamiento
* &lbrack;RedHat&rbrack; Problemas con el selector de color

### 10.0.1

Fecha de publicación: **2024/06/11** Resumen: **Versión secundaria, correcciones de errores**

**Agregado:**

* &lbrack;Biblioteca&rbrack; Conversión de fuentes de Substance en archivos de fuentes normales
* &lbrack;Illustrator&rbrack;&lbrack;SVG&rbrack; Dar a las miniaturas de la selección de ámbito un fondo gris claro
* &lbrack;Python&rbrack; Función Añadir en origen de mapa de bits para enumerar los espacios de color disponibles

**Corregido**:

* &lbrack;Pila de capas&rbrack; La carpeta siempre se cierra al entrar o salir de otras carpetas
* &lbrack;Guardar&rbrack; El archivo de proyecto se pierde cuando se produce un error al guardar como copia o al guardar automáticamente en casos específicos
* &lbrack;Importar&rbrack; Los activos con el mismo nombre pero con diferentes extensiones se anulan
* &lbrack;Propiedades&rbrack; Faltan ajustes al utilizar el punto de anclaje en las entradas de imagen
* &lbrack;Illustrator&rbrack; No se pueden importar archivos de Illustrator después del bloqueo del servidor sin reiniciar Painter
* &lbrack;Python&rbrack; El padre de la instancia no se puede establecer con el tipo &quot;properties&quot;
* &lbrack;Python&rbrack; Al definir el poli alto como parámetro de haga un bake, no se carga el poli alto
* &lbrack;Python&rbrack; El mensaje de error para set_color_space() es demasiado genérico
* &lbrack;Python&rbrack; Las fuentes de referencia permiten crear ciclos

**Problemas conocidos**:

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;MacOS Intel&brack; Bloqueo al importar algunos ajustes preestablecidos
* &lbrack;Illustrator&rbrack; Bloqueo al exportar un Mosaico de UV con un gráfico .ai en casos específicos
* &lbrack;Trazos dinámicos&rbrack;&lbrack;Path&rbrack; La opción aleatoria por trazo no funciona en un trazado

### 10.0.0

Fecha de publicación: **2024/05/16** Resumen: **Versión principal, edición de la pila de capas con la API de Python, lectura de archivos nativos de Illustrator, integración de recursos 3D y nuevo recurso de texto**

**Agregado**:

* &lbrack;Illustrator&rbrack; Uso de archivos de Illustrator con mesas de trabajo en Painter
* &lbrack;Illustrator&rbrack;&lbrack;SVG&rbrack; Añadir previsualizaciones en la selección de ámbito
* &lbrack;Substance 3D Assets&rbrack; Examine, seleccione y descargue contenidos 3D directamente en Painter
* &lbrack;Substance 3D Assets&rbrack;&lbrack;UI&rbrack; Nuevo panel
* &lbrack;Substance 3D Assets&rbrack; Mapas y materiales del entorno de apoyo
* &lbrack;Substance 3D Assets&rbrack; Permitir volver a cargar, navegar y abrir la carpeta de ubicación en el nuevo panel Substance 3D Assets
* &lbrack;Substance 3D Assets&rbrack; Adición de un gestor de descargas
* &lbrack;Recurso de texto&rbrack; Permitir el uso de fuentes incrustables
* &lbrack;Recurso de texto&rbrack; Permitir procesar una fuente/texto en una malla
* &lbrack;Recurso de texto&rbrack; Visualización de fuentes del usuario y otras rutas compartidas en el panel Activos con una nueva categoría
* &lbrack;Recurso de texto&rbrack;&lbrack;Propiedades&rbrack; Añadir compatibilidad con propiedades de fuentes avanzadas
* &lbrack;Recurso de texto&rbrack; Permitir buscar/ver fuentes en miniestantes
* &lbrack;Recurso de texto&rbrack; Añadir mensaje/cuadro de diálogo de error al importar una fuente incompatible
* Miscelánea
* &lbrack;Rellenar proyección&rbrack; Mejorar el comportamiento del manipulador de escala al utilizar valores pequeños
* &lbrack;Manipuladores&rbrack; Agregar nuevo modo preciso al presionar el método abreviado CTRL
* &lbrack;Manipuladores&rbrack; Mejorar la estabilidad del manipulador de superficie al convertir
* &lbrack;Exportar&rbrack; Añadir nombre de espacio de color en salidas SBSAR
* &lbrack;Rendimiento&rbrack; Mejorar el tiempo de detección de la biblioteca de los activos en el disco
* &lbrack;Substance&rbrack; Actualización al motor de Substance versión 9.1.2
* &lbrack;Arrastrar y soltar&rbrack; Alinear la rotación de pegatinas con la cámara al colocar en la ventana gráfica
* &lbrack;Python&rbrack; Edición de la pila de capas
* &lbrack;Python&rbrack; Permitir seleccionar capa, efecto, máscara o máscara geográfica en la interfaz de usuario
* &lbrack;Python&rbrack; Permitir obtener/definir modos de fusión de capas
* &lbrack;Python&rbrack; Permitir obtener o establecer la configuración de proyección de la capa de relleno
* &lbrack;Python&rbrack; Permitir consultar el color de material del Substance desde una capa de relleno
* &lbrack;Python&rbrack; Permitir consultar y definir colores uniformes y recursos en capas y efectos
* &lbrack;Python&rbrack; Permitir la creación y edición de recursos de texto en pila de capas
* &lbrack;Python&rbrack; Permitir editar canales activos en capas y efectos
* &lbrack;Python&rbrack; Permitir que las acciones por lotes tengan una sola acción de deshacer/rehacer
* &lbrack;Python&rbrack; Permitir cargar o editar parámetros de origen vectorial
* &lbrack;Python&rbrack; Permitir la edición de propiedades de color de capa y efectos con la gestión de color
* &lbrack;Python&rbrack; Permitir consultar y crear capas con instancias
* &lbrack;Python&rbrack; Permitir añadir efecto de selección de color
* &lbrack;Python&rbrack; Permitir el control de la gestión de color de imágenes de mapa de bits
* &lbrack;Python&rbrack; Permitir detener/anular pausa del motor
* &lbrack;Python&rbrack; Permitir navegar a nodos del mismo nivel y principales
* &lbrack;Python&rbrack; Permitir la creación de un efecto de filtro/generador
* &lbrack;Python&rbrack; Permitir añadir efecto de nivel
* &lbrack;Python&rbrack; Permitir añadir máscara inteligente en una capa
* &lbrack;Python&rbrack; Permitir crear o editar puntos de ancla
* &lbrack;Python&rbrack; Permitir obtener/definir máscara en capas
* &lbrack;Python&rbrack; Permitir la creación del efecto de máscara de comparación
* &lbrack;Python&rbrack; Permitir consultar y utilizar ajustes preestablecidos de recursos de Substance
* &lbrack;Python&rbrack; Permitir la lista de ajustes preestablecidos y sus valores mediante la función internal_properties para los recursos del Substance
* &lbrack;Python&rbrack; Permitir la lista de ajustes preestablecidos de exportación predefinidos
* &lbrack;Python&rbrack; Permitir que se muestren los ajustes preestablecidos de exportación disponibles en la biblioteca
* &lbrack;Python&rbrack; Permitir recuperar el contenido de los ajustes preestablecidos de exportación

**Corregido**:

* &lbrack;Bloqueo&rbrack; Deshacer &quot;Quitar instancia del sombreador&quot; con Ctrl-Z
* &lbrack;Bloqueo&rbrack; Crear una capa en una pila vacía si la última selección fue un efecto
* &lbrack;SVG&rbrack; Problema con el valor de área recortada personalizada
* &lbrack;Desenvolvimiento automático&rbrack; Si se vuelve a calcular solo el empaquetado sin ningún cambio en la orientación UV, se producirá un bloqueo
* &lbrack;Arrastrar y soltar&rbrack; El retraso debido a los recursos externos se carga previamente varias veces
* &lbrack;UI&rbrack; La miniatura de un recurso de arrastrar y soltar puede ocultar un mensaje de advertencia en la pila de capas
* &lbrack;Rendimiento&rbrack; Los mosaicos UV enmascarados aún se calculan
* &lbrack;USD&rbrack; Resaltado incorrecto para la selección de ámbito
* &lbrack;Recurso&rbrack; La imagen de mapa de bits se daña después de pintar en el canal normal y guardar el proyecto
* &lbrack;USD&rbrack; Admitir ordenación de mallas de vértices con la mano izquierda
* &lbrack;Substance&rbrack; Restablecer valores predeterminados volver siempre a cero para el widget de ángulo
* &lbrack;Motor&rbrack; Pintar con un SVG en una galería de símbolos no funciona
* &lbrack;Motor&rbrack; Los trazos de pincel de mapa de normales se rompen después de deshacer una acción
* &lbrack;Contenido&rbrack; El gráfico en el Filtro de material tiene una fusión alfa y un espacio de color incorrectos
* &lbrack;Contenido&rbrack; Los modos de fusión del Tile Generator no funcionan
* &lbrack;Contenido&rbrack; El filtro de histograma produce bandas en algunos casos
* &lbrack;Contenido&rbrack; La iluminación hecha un bake estilizada no tiene en cuenta el height pintado
* &lbrack;Python&rbrack; Error inesperado al recuperar información de capas instanciada después de cambiar de sombreador
* &lbrack;Guardar&rbrack; El archivo de proyecto se pierde cuando se produce un error en &quot;Guardar como&quot; en casos específicos

**Problemas conocidos**:

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Bloqueo&rbrack;&lbrack;Linux&rbrack;&lbrack;AMD&rbrack; Arrastre y colocación de recursos en pila de capas en Wayland OS
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent
* &lbrack;Guardar&rbrack; El archivo de proyecto de Spp se pierde cuando &quot;guardar como copia&quot; falla en casos específicos
* &lbrack;MacOS Intel&brack; Bloqueo al importar algunos ajustes preestablecidos
* &lbrack;Illustrator&rbrack; No se pueden importar archivos de Ai después del bloqueo del servidor sin reiniciar Painter
* &lbrack;Importar&rbrack; Los activos con el mismo nombre pero con diferentes extensiones se anulan

## Versión 9

### 9.1.2

Fecha de publicación: **30/01/2024** Resumen: **Versión secundaria, correcciones de errores**

**Agregado**:

* &lbrack;Rendimiento&rbrack; Mejorar el tiempo de creación de la primera capa de relleno en proyectos nuevos
* &lbrack;Rendimiento&rbrack; Reducir el tiempo de carga de los mapas de entorno pesados
* &lbrack;Substance&rbrack; Permitir guardar o cerrar proyectos incluso cuando se generan miniaturas

**Corregido**:

* La acción de guardar falla en proyectos de versiones anteriores cuando se modifica la ventana gráfica
* &lbrack;Bloqueo&rbrack; Reimportación de mallas al utilizar el archivo AO personalizado y la gestión de color
* &lbrack;Rellenar proyección&rbrack; Al hacer clic en el manipulador de escala, aparece el mensaje &quot;no puede pintarse&quot;
* &lbrack;Brush&rbrack; Pintar con alineación UV causa artefactos
* &lbrack;Pila de capas&rbrack; El cambio de nombre de la capa es lento cuando la pila es muy larga
* &lbrack;Pila de capas&rbrack; Mensaje de error incorrecto al utilizar un filtro incompatible en la máscara
* &lbrack;Pila de capas&rbrack; La selección vuelve a la capa superior después de la eliminación
* &lbrack;Exportar&rbrack; La textura normal generada siempre está en el modo de relleno Espacio 3D contiguo
* &lbrack;Exportar&rbrack; La textura alfa no se genera con el ajuste preestablecido de exportación de vista 2D
* &lbrack;Exportar&rbrack; La exportación SBSAR tiene usos incorrectos con mapas convertidos
* &lbrack;Sombreador&rbrack; El registro de cambios de API del sombreador no está actualizado con los últimos cambios de ASM

**Problemas conocidos**:

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Bloqueo&rbrack;&lbrack;Linux&rbrack;&lbrack;AMD&rbrack; Arrastre y colocación de recursos en pila de capas en Wayland OS
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú contextual es demasiado pequeño en pantallas HD
* &lbrack;Bloqueo&rbrack;&lbrack;Python&rbrack; Exportación USD activada por TextureStateEvent

### 9.1.1

Fecha de publicación: **12/2023/05** Resumen: **Versión secundaria, correcciones de errores y envío a la funcionalidad de After Effects**

**Agregado:**

* &lbrack;Interop&rbrack; Permitir el envío de una malla con textura a After Effects (Ae 24.1)

**Corregido:**

* &lbrack;Rellenar&rbrack; La proyección del conjunto UV en conjunto UV no lee más de 2 conjuntos UV
* &lbrack;Bloqueo&rbrack; Uso del mapa de entorno de 16K
* &lbrack;Bloqueo&rbrack; Exr utilizado como entrada de imagen
* &lbrack;Bloqueo&rbrack; Copiar y pegar trazados en proyectos
* &lbrack;QoL&rbrack; La acción de arrastrar y soltar un recurso del Alpha en el modo de pegatina crea una Proyección de UV en la máscara
* &lbrack;Ruta&rbrack; Copiar vértices de trazado también cambia el nombre de la ruta de destino al volver a abrir el proyecto
* &lbrack;Linux&rbrack; La selección de color se puede romper con varias pantallas
* &lbrack;Auto Unwrap&rbrack; Problema de interfaz de usuario para control de densidad de texto
* &lbrack;Administración de color&rbrack; Los comentarios de la interfaz de usuario son razonables en cada caso, pero el motor no
* &lbrack;Administración de color&rbrack; Selección incorrecta del espacio de color en la máscara con anulación de datos de usuario

**Problemas conocidos:**

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Bloqueo&rbrack;&lbrack;Linux&rbrack; con Linux Wayland en AMD al arrastrar y soltar el recurso en la Pila de capas
* &lbrack;Bloqueo&rbrack;&lbrack;Mac&rbrack; Cambio del valor de filtrado anisotrópico en el sistema operativo Monterey
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú del botón derecho es demasiado pequeño en la pantalla HD
* &lbrack;Python&rbrack; Bloqueo de USD de exportación activado por TextureStateEvent

### 9.1.0

Fecha de publicación: **2023/11/07** Resumen: **Versión principal con compatibilidad con SVG y transparencia, así como mejoras en la herramienta de arrastrar y soltar y ruta**

**Agregado:**

* &lbrack;SVG&rbrack; Permitir la importación de archivos vectoriales (SVG)
* &lbrack;SVG&rbrack;&lbrack;UI&rbrack; Añadir compatibilidad con propiedades específicas del SVG
* &lbrack;SVG&rbrack; Añada una opción para conservar fácilmente las proporciones de la imagen original
* &lbrack;SVG&rbrack; Permitir el uso automático de alfa de SVG con transparencia
* &lbrack;Interop&rbrack; Permitir el envío de una malla con textura a After Effects (versión beta de Ae 24.1)
* &lbrack;Interop&rbrack; Añadir configuración para Enviar a After Effects
* &lbrack;QoL&rbrack;&lbrack;Assets&rbrack;&lbrack;UI&rbrack; Importar automáticamente el recurso al arrastrar y soltar en la ranura de la interfaz de usuario
* &lbrack;QoL&rbrack; Permitir arrastrar y soltar recursos externos en la pila de capas
* &lbrack;QoL&rbrack;&lbrack;Pila de capas&rbrack; Arrastrar y soltar texturas desde el panel de Recursos en la Pila de capas
* &lbrack;QoL&rbrack;&lbrack;Viewport&rbrack; Permitir arrastrar y soltar el generador, filtros en la malla
* &lbrack;QoL&rbrack;&lbrack;Viewport&rbrack; Permitir soltar activos externos en la malla
* &lbrack;QoL&rbrack;&lbrack;Proyección&rbrack; Añadir nuevo conjunto UV al modo de proyección conjunto UV
* &lbrack;QoL&rbrack; Arrastrar y soltar Máscaras inteligentes como nuevas capas en la ventana gráfica y la Pila de capas
* &lbrack;QoL&rbrack; Añadir selector para generadores con varias salidas cuando se utiliza en la máscara
* &lbrack;QoL&rbrack; Permitir arrastrar y soltar imágenes de un solo canal sobre un efecto de relleno
* &lbrack;QoL&rbrack;&lbrack;Pila de capas&rbrack; Utilice los modificadores CTRL/ALT con la función de arrastrar y soltar para especificar dónde y cómo crear efectos o capas
* &lbrack;Ruta&rbrack; Cambiar la visibilidad de los trazados individualmente en el panel Trazado
* &lbrack;Ruta&rbrack; Permitir el uso de manipuladores de transformación para puntos de trazado
* &lbrack;Ruta&rbrack; Permitir el control manual de las tangentes por vértice
* &lbrack;Ruta&rbrack; Copiar/pegar propiedades de trazado
* &lbrack;Ruta&rbrack; Introducir un método abreviado vacío para el botón de tangente de rotura
* &lbrack;Sombreador&rbrack; Añadir compatibilidad con Opacidad y Translucidez en sombreador de ASM
* &lbrack;Sombreador&rbrack; Añadir compatibilidad para el canal de Color de absorción con el sombreador de ASM
* &lbrack;Sombreador&rbrack; Mejorar información sobre parámetros de sombreador de ASM
* &lbrack;Sombreador&rbrack; Cambiar el color predeterminado del canal de Translucidez a negro
* &lbrack;Configuración de visualización&rbrack; Habilitar Suavizado temporal de forma predeterminada
* &lbrack;Configuración de visualización&rbrack; Activar configuración de dispersión subsuperficial de forma predeterminada
* &lbrack;Substance&rbrack; Añadir compatibilidad para la propiedad ColorSpace desde la entrada/salida de gráficos
* &lbrack;Substance&rbrack; Actualizar el motor de Substance a la versión 9.0.3
* &lbrack;UI&rbrack; Hacer accesible el botón de la barra de herramientas contextual incluso si la ventana de la aplicación es pequeña
* &lbrack;Auto Unwrap&rbrack; Número de Mosaicos de UV de control con Densidad de texto
* &lbrack;Haciendo un bake&rbrack; Desactivar Trazado de rayos de GPU en GPU AMD de forma predeterminada
* &lbrack;Rendimiento&rbrack; Aplique compresión sin pérdida en imágenes de 16 bits para reducir el espacio del proyecto
* &lbrack;Python&rbrack; Permitir la manipulación de la cámara predeterminada en Vista 3D
* &lbrack;Python&rbrack; Exponer la capacidad de exportar mallas mediante scripts
* &lbrack;Content&rbrack;&lbrack;Samples&rbrack; Añade un nuevo proyecto de muestra &quot;French Restaurant Table&quot;
* &lbrack;Contenido&rbrack; Actualizar el logotipo de Substance alfa a una nueva versión
* &lbrack;Contenido&rbrack; Añade tres filtros de material enfocados en el SVG (pegatina personalizada, spray personalizado y gráfico al material)

**Corregido:**

* &lbrack;Bloqueo&rbrack; Cambio del tamaño del manipulador cuando no se utiliza la herramienta simetría
* &lbrack;Bloqueo&rbrack; &lbrack;Pila de capas&rbrack; Crear capa cuando no hay nada seleccionado
* &lbrack;Proyecto&rbrack; Los mapas de malla se pueden dañar después de eliminar los recursos no utilizados
* &lbrack;Proyecto&rbrack; Daños en los recursos tras volver a importar o hacer un bake la imagen
* &lbrack;Assets&rbrack; Al volver a cargar un activo, se elimina de Favoritos
* &lbrack;Importar&rbrack; No se pueden importar recursos cuando no se encuentra ningún resultado en el panel de recursos
* &lbrack;UI&rbrack; La flecha de la barra de herramientas contextual no aparece en algunos casos
* &lbrack;Substance&rbrack; No se admite el botón en paralelo para valores booleanos
* &lbrack;Nivel&rbrack; Etiqueta de canal incorrecta cuando se utiliza en la máscara
* &lbrack;Export&rbrack;&lbrack;glTF&rbrack; Los archivos glTF/GLB exportados desde Painter no tienen una unidad de tamaño físico
* &lbrack;Contenido&rbrack; La intensidad del filtro de desenfoque se fija en 16
* &lbrack;Contenido&rbrack; La entrada de imagen del filtro &quot;color de destino&quot; no está visible

**Problemas conocidos:**

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Bloqueo&rbrack;&lbrack;Linux&rbrack; con Linux Wayland en AMD al arrastrar y soltar el recurso en la Pila de capas
* &lbrack;Bloqueo&rbrack;&lbrack;Mac&rbrack; Cambio del valor de filtrado anisotrópico en el sistema operativo Monterey
* &lbrack;Bloqueo&rbrack; Exr utilizado como entrada de imagen
* &lbrack;Bloqueo&rbrack; Uso del mapa de entorno de 16K
* &lbrack;Auto Unwrap&rbrack; Problema de interfaz de usuario para control de densidad de texto
* &lbrack;Regresión&rbrack;&lbrack;UI&rbrack; El menú del botón derecho es demasiado pequeño en la pantalla HD
* &lbrack;Python&rbrack; Bloqueo de USD de exportación activado por TextureStateEvent
* &lbrack;QoL&rbrack; La acción de arrastrar y soltar un recurso del Alpha en el modo de pegatina crea una Proyección de UV en la máscara

### 9.0.1

Fecha de publicación: **2023/09/19** Resumen: **Versión menor de corrección de errores con varias mejoras**

**Agregado:**

* &lbrack;Importar&rbrack; Establecer ubicación de importación predeterminada en la ventana de importación
* &lbrack;Haciendo un bake modo&rbrack; Permitir restablecer los parámetros a sus valores predeterminados
* &lbrack;Haciendo un bake&rbrack; Definir hacer un bake a resolución de pintura al crear un proyecto
* &lbrack;Simetría&rbrack; Desvincular manipulador específico de simetría de método abreviado Q
* &lbrack;Menú&rbrack; Añadir la opción &quot;mostrar registro&quot; en el menú de ayuda
* &lbrack;Viewport&rbrack; Mejorar la velocidad de procesamiento de sombras
* &lbrack;Substance&rbrack; Actualizar el motor a la versión 9.0.1
* &lbrack;Administración de color&rbrack; OCIO archivo de configuración puede tener cualquier tipo de extensión
* &lbrack;Assets&rbrack; El recurso Sbsar con uso de &#39;pegatina&#39; debe configurarse automáticamente para deformar la proyección
* &lbrack;Ruta&rbrack; Mostrar un mensaje al intentar interactuar con la herramienta Ruta mientras la interfaz de usuario y los Gizmo están ocultos

**Corregido:**

* &lbrack;Bloqueo&rbrack; Alt + Arrastrar en el panel Trazado
* &lbrack;Importar recursos&rbrack; Bloqueo aleatorio al quitar recursos para importar
* Bloqueo al importar un archivo GLB comprimido
* Problema al pintar en mallas que comparten UV
* Parpadeo de malla negro al volver a calcular o cargar la caché
* &lbrack;Propiedades&rbrack; El menú contextual para restablecer parámetros no aparece en los menús desplegables
* &lbrack;Nivel&rbrack; Reguladores de entrada bloqueados por nivel anterior
* &lbrack;AMD&rbrack;&lbrack;Sparse&rbrack; La opción SVT, si está activada, genera artefactos
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Bloqueo al hacer doble clic en los vértices
* &lbrack;Ruta&rbrack; IU y ruta visibles en el modo de hacer un bake
* &lbrack;AMD&rbrack; Textura perdida al jugar con la visibilidad
* &lbrack;Disperso&rbrack; Resolución demasiado baja al girar la malla

**Problemas conocidos:**

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción

### 9.0.0

Fecha de lanzamiento: **2023/06/20** Resumen: **Versión principal con Pintura a lo largo de la ruta que permite curvas 3D, nuevos materiales base y la limpieza de materiales heredados y nuevos ajustes preestablecidos para curvas 3D**

**Agregado:**

* &lbrack;Ruta&rbrack; Herramienta Añadir nueva Pintura a lo largo del trazado
* &lbrack;Ruta&rbrack; Adición de un método abreviado vacío para la herramienta de trazado
* &lbrack;Ruta&rbrack; Permitir la adición de nuevos puntos a un trazado existente
* &lbrack;Ruta&rbrack; Agregar método abreviado para salir de la creación de la ruta actual
* &lbrack;Ruta&rbrack; Permitir la edición de propiedades de pincel para trazados
* &lbrack;Ruta&rbrack; Ajuste automático de tangentes al colocar un punto
* &lbrack;Ruta&rbrack; Calcular tangentes al mover un punto
* &lbrack;Ruta&rbrack; Ajuste de los puntos recién creados a la superficie de una malla
* &lbrack;Ruta&rbrack; Permitir editar la presión por vértice
* &lbrack;Ruta&rbrack; Ajustar la presión de un punto recién creado desde puntos vecinos
* &lbrack;Ruta&rbrack; Permitir la conversión de puntos a suavizado/esquina (salto de tangente)
* &lbrack;Ruta&rbrack; Permitir mover un punto recién añadido inmediatamente
* &lbrack;Ruta&rbrack; Permitir la eliminación de puntos de un trazado existente
* &lbrack;Ruta&rbrack; Permitir invertir la dirección de un trazado
* &lbrack;Ruta&rbrack; Permitir la selección de una ruta en la ventana gráfica
* &lbrack;Ruta&rbrack; Permitir la selección de puntos de trazado con selección de recuadro
* &lbrack;Ruta&rbrack; Introducir métodos abreviados CTRL-A para seleccionar todos los puntos de un trazado
* &lbrack;Ruta&rbrack; Permitir cerrar trazado
* &lbrack;Ruta&rbrack; Permitir especificar el eje ascendente de la ruta en Propiedades
* &lbrack;Ruta&rbrack; Añadir un menú de control de vértices a la barra de herramientas contextual
* &lbrack;Ruta&rbrack; Introducir los modos de pintura/borrado/difuminado en la herramienta de trazado
* &lbrack;Ruta&rbrack; Creación de comentarios visuales para trazados en la ventana gráfica
* &lbrack;Ruta&rbrack; Adición de un indicador visual para la dirección del trazado
* &lbrack;Ruta&rbrack; Añadir thickness de línea a la configuración de visualización de trazado
* &lbrack;Ruta&rbrack; Permitir ocultar la interfaz de usuario de rutas
* &lbrack;Ruta&rbrack; Agregar el panel Trazado a la lista de trazados de la capa seleccionada actualmente
* &lbrack;Ruta&rbrack; Adición de comentarios visuales al pasar el cursor sobre un trazado en el panel Trazado
* &lbrack;Ruta&rbrack; Mostrar el panel Trazado siempre que se seleccione la herramienta Trazado
* &lbrack;Ruta&rbrack; Permitir cambiar el nombre, eliminar, copiar, cortar y duplicar trazado en el panel Trazado
* &lbrack;Ruta&rbrack; Mostrar mensaje al intentar interactuar en la ventana gráfica 2D con la herramienta Trazado
* &lbrack;Biblioteca&rbrack; Integrar nuevo contenido (herramientas de trazado y materiales base)
* &lbrack;Trazos dinámicos&rbrack; Agregar propiedad de distancia para trazos dinámicos
* &lbrack;Trazos dinámicos&rbrack; Añadir propiedades de tamaño y espaciado a los trazos dinámicos
* &lbrack;Trazos dinámicos&rbrack; Agregar propiedad de inicio/medio/fin para trazos dinámicos
* &lbrack;Python&rbrack;&lbrack;USD&rbrack; Exponer los parámetros de configuración del proyecto para el formato USD
* &lbrack;Python&rbrack;&lbrack;USD&rbrack; Exponer parámetros de creación de proyectos para el formato USD
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Añadir información de ruta de proyecto dentro del archivo USD exportado
* &lbrack;GLTF&rbrack; Actualización de texturas de la biblioteca al volver a cargar un archivo GLTF
* &lbrack;Sombreador&rbrack; Reducir defectos de costura para Islas de UV con diferentes orientaciones
* &lbrack;Motor&rbrack; Actualizar al motor de Substance versión 9.0

**Corregido:**

* &lbrack;Importar&rbrack; Algunos GLB con texturas no reciben texturas en Painter
* &lbrack;AMD&rbrack; Artefactos en los bordes de todos los rellenos de proyección 3D
* &lbrack;Motor&rbrack; Las texturas se rompen al alternar la visibilidad de las capas
* &lbrack;Motor&rbrack; Las texturas están vacías en algunos lugares al cambiar el modo de fusión
* &lbrack;Motor&rbrack; La textura/proyección está en modo de deformación vacío en algunos casos
* &lbrack;Iray&rbrack; Iteración restablecida a 0 al guardar el procesamiento
* &lbrack;Registro&rbrack; USD mensaje de error al realizar Archivo > Nuevo

**Problemas conocidos:**

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Pila de capas&rbrack; El origen de entrada no se guarda por capa

## Versión 8

### 8.3.1

Fecha de publicación: **2023/04/27**

**Agregado:**

* &lbrack;Haciendo un bake modo&rbrack; Añadir método abreviado (vacío) para mostrar/ocultar la visualización de la ventana gráfica
* &lbrack;Haciendo un bake modo&rbrack; Mostrar siempre el nivel de poli bajo al utilizar el botón &quot;Ocultar mallas de haga un bake&quot;
* &lbrack;Haciendo un bake modo&rbrack; Mostrar sufijo para Coincidencia por nombre según el conjunto de texturas actual
* &lbrack;Importar&rbrack; Añadir soporte para archivos binarios GLTF (glb)
* &lbrack;Lista de conjuntos de texturas&rbrack; Menú Añadir para seleccionar o crear instancias del sombreador
* &lbrack;Lista de conjuntos de texturas&rbrack; Permitir cambiar rápidamente el conjunto de texturas y la resolución de Mosaico de UV
* &lbrack;Tamaño físico&rbrack; Mejorar el comportamiento del manipulador al utilizar tamaño físico en Proyección de UV
* &lbrack;UI&rbrack; Volver a &quot;Guardar como&quot; en el menú principal de archivos
* &lbrack;UI&rbrack; Guardar selección de vista (solo 2D, solo 3D, ambos) en diseño de IU
* &lbrack;USD&rbrack; Mensaje de error menos vago al crear un proyecto con formas de USD no compatibles
* &lbrack;Python&rbrack; Añadir eventos de hacer un bake para seguir el progreso de Hacer un bake
* &lbrack;Python&rbrack; Permitir cancelar una hace un bake
* &lbrack;Python&rbrack; Exponer &quot;según plantilla de salida&quot; para el tipo de archivo y la profundidad de bits en la exportación
* &lbrack;Python&rbrack; Exponer el tiempo de actualización para TextureStateEvent.Update

**Corregido:**

* &lbrack;Bloqueo&rbrack; Bloqueo raro al cerrar un proyecto
* &lbrack;Bloqueo&rbrack; &lbrack;Haciendo un bake&rbrack; Activar la sincronización del mapa de malla con el Height o la curvatura en un proyecto específico
* &lbrack;Bloqueo&rbrack;&lbrack;Scripting&rbrack; Bloqueo al añadir un material después de crear la instancia del sombreador
* &lbrack;Haciendo un bake modo&rbrack; La intensidad de AO en material neutro no tiene efecto
* &lbrack;Haciendo un bake modo&rbrack; Bloqueo al cambiar al modo de hacer un bake antes de cargar el modelo
* &lbrack;Haciendo un bake modo&rbrack; Mensaje de error que falta en la ficha Hacer un bake proceso
* &lbrack;Haciendo un bake modo&rbrack; Los ajustes de material neutro no tienen efecto después de volver a importar una malla
* &lbrack;Haciendo un bake modo&rbrack; El separador de ventanilla se guarda globalmente y no por modo
* &lbrack;Haciendo un bake modo&rbrack; Problema de visualización: normal promedio no cambia la superficie de la jaula
* &lbrack;Administración de color&rbrack; La opción Detección automática del espacio de color está desactivada cuando OCIO env var está presente
* &lbrack;Contenido&rbrack; El filtro Contorno de máscara tiene un artefacto con entrada de height
* &lbrack;Contenido&rbrack; El regulador de intensidad del filtro de desenfoque de pendiente se fija en 1.0
* &lbrack;Interop&rbrack; No se puede crear el proyecto con GLTF desde Sampler
* &lbrack;Pila de capas&rbrack; El valor del mosaico de proyección no se actualiza correctamente con manipulador
* &lbrack;Linux&rbrack; Desplazamiento entre el lápiz de Tablet PC gráfico y el cursor con HDPI superior al 100 %
* &lbrack;Python&rbrack; Bloqueo al volver a importar una malla después de crear un proyecto
* &lbrack;Substance&rbrack; Los ruidos 3D se rompen después de volver a importar una malla
* &lbrack;Mosaicos de UV&rbrack; El desplazamiento de la Proyección de UV se fija en 1
* &lbrack;Viewport&rbrack; Los comentarios visuales de líneas rectas ya no son visibles
* &lbrack;WhatsNew&rbrack; Retorno de línea incorrecto en títulos de funciones

**Problemas conocidos:**

* &lbrack;Importar&rbrack; Algunos GLB con texturas no reciben texturas en Painter

### 8.3.0

*(Lanzado: 10 de enero de 2023*)Resumen: **Versión principal con nuevo modo de hacer un bake, nueva importación y exportación de archivos USD y compatibilidad de tamaño físico para la Proyección de UV**

**Agregado:**

* &lbrack;Haciendo un bake modo&rbrack; Nuevo modo de hacer un bake dedicado al proceso de hacer un bake

* &lbrack;Haciendo un bake modo&rbrack; Definir método abreviado para cambiar al modo de hacer un bake a F8

* &lbrack;Haciendo un bake modo&rbrack; Botón Añadir Inicio y Cancelar haga un bake en la ventana gráfica

* &lbrack;Haciendo un bake modo&rbrack; Añadir selección de haga un bake en la lista Conjunto de texturas

* &lbrack;Haciendo un bake modo&rbrack; Ventana Añadir nuevos Bakeres de mapa de malla para seleccionar bakeres

* &lbrack;Haciendo un bake modo&rbrack; Añada una nueva ventana Ajustes de mapa de malla para editar los ajustes de hace un bake

* &lbrack;Haciendo un bake modo&rbrack; Añada una nueva ventana Haciendo un bake registro para seguir el proceso de hacer un bake

* &lbrack;Haciendo un bake modo&rbrack; Agregar parámetros de hacer un bake y acciones de deshacer a la ventana de historial

* &lbrack;Haciendo un bake modo&rbrack; Adición de rutas de navegación en Ajustes de mapa de malla

* &lbrack;Haciendo un bake modo&rbrack; Añadir miniaturas de mapas de malla en la ventana Bakeres de mapas de malla

* &lbrack;Haciendo un bake modo&rbrack; Añadir menú contraíble de ajustes de visualización en la ventana gráfica 3D

* &lbrack;Haciendo un bake modo&rbrack; Añadir configuración de visualización para mostrar/ocultar la malla de alta densidad

* &lbrack;Haciendo un bake modo&rbrack; Añadir configuración de visualización para mostrar/ocultar la malla de la jaula y la malla metálica

* &lbrack;Haciendo un bake modo&rbrack; Añadir configuración de visualización para mostrar/ocultar la malla de baja densidad

* &lbrack;Haciendo un bake modo&rbrack; Añada un ajuste de visualización para mostrar los bordes duros sin costuras UV como errores

* &lbrack;Haciendo un bake modo&rbrack; Informar en la ventana gráfica sobre los errores de malla y hacer un bake si Hacer un bake registro no es visible

* &lbrack;Haciendo un bake modo&rbrack; Agregar acción para sincronizar la configuración del baker en todos los conjuntos de texturas

  En la ventana Bakeres de mapa de malla, cada baker (así como los ajustes comunes) se pueden sincronizar en los conjuntos de texturas haciendo clic en el icono de enlace junto a su nombre. Esta acción abrirá una ventana que permite seleccionar qué conjuntos de texturas compartirán los mismos parámetros.

* &lbrack;Haciendo un bake modo&rbrack; Agregar acciones para copiar y pegar ajustes de baker

  En la ventana Bakeres de mapa de malla hay acciones disponibles para copiar y pegar cada configuración de baker en los conjuntos de texturas, ya sea a través del menú específico en la parte superior de la ventana o el menú contextual del botón derecho.

* &lbrack;Haciendo un bake modo&rbrack; El botón Añadir en Hacer un bake registro para saltar del error a la configuración correcta

  Cuando un baker falla o una malla no se carga correctamente, aparece un mensaje de error en el registro de Hace un bake. Un botón junto al mensaje permite cambiar la ventana Bakeres de mapa de malla y ajustes de mapa de malla para mostrar los ajustes relacionados. Esto ayuda a aislar con mayor facilidad el origen de un problema para poder solucionarlo.

* &lbrack;Haciendo un bake modo&rbrack; Añadir menús para gestionar conjuntos de texturas y selecciones de Bakeres

  En las ventanas &quot;Lista de conjuntos de texturas&quot; y &quot;Bakeres de mapa de malla&quot; se ha añadido un pequeño menú de acciones para ayudar a copiar e invertir las selecciones.

* &lbrack;Haciendo un bake modo&rbrack; Lista de selección de baker dividida por conjunto de texturas

* &lbrack;Haciendo un bake modo&rbrack; Dividir ajustes comunes por conjunto de texturas

* &lbrack;Haciendo un bake modo&rbrack; Cargar mallas de alta polietileno y jaula sin congelar la interfaz

* &lbrack;Haciendo un bake modo&rbrack; Usar la barra de progreso de la ventanilla para mostrar la carga de malla

* &lbrack;Haciendo un bake modo&rbrack; Añadir estado de carga de malla en el registro de Hace un bake

* &lbrack;Haciendo un bake modo&rbrack; Permitir girar la malla en la ventana gráfica durante la hace un bake

* &lbrack;Haciendo un bake modo&rbrack; Definir el orden de hace un bake en función de la visibilidad actual de la ventana gráfica de la malla

* &lbrack;Haciendo un bake modo&rbrack; Visualización de la jaula de haga un bake implícita en la ventana gráfica

  Si no se utiliza un fichero de malla de jaula personalizado, se generará una malla de jaula automática y se mostrará en la ventana gráfica. Su tamaño se basará en el parámetro Distancia frontal máxima de los ajustes comunes que se hacen un bake. La malla de la jaula se utiliza para indicar hasta dónde llegará la coincidencia entre el poli bajo y alto.

* &lbrack;Haciendo un bake modo&rbrack; Mostrar la lista de nombres de malla coincidentes por nombre en Registro de Hace un bake

* &lbrack;Haciendo un bake modo&rbrack; Usar material neutro para mostrar el modelo 3D en la ventana gráfica

* &lbrack;Haciendo un bake modo&rbrack; Desactivar el cálculo del motor mientras está en modo de hacer un bake

* &lbrack;Haciendo un bake modo&rbrack; Mostrar una advertencia al salir de la aplicación mientras hay un haga un bake en curso

* &lbrack;Bakeres&rbrack; Actualizar etiquetas de configuración de suavizado

  Los valores del ajuste de suavizado se han cambiado de nombre a &quot;Supersampling&quot; (Supermuestreo) y con un número multiplicador explícito para aclarar su comportamiento.

* &lbrack;Bakeres&rbrack; Actualice baker a la versión 2.5.7.

* &lbrack;USD&rbrack; Importación y exportación de archivos de Universal Scene Description (USD)

* &lbrack;USD&rbrack; Agregar USD opciones a la ventana Nuevo proyecto al seleccionar un archivo USD

* &lbrack;USD&rbrack; Agregar nueva ventana de selección Ámbito y Variantes

  Al importar un fichero de USD, pulsar en el botón de cambio de la ventana Nuevo proyecto o Configuración del proyecto permite seleccionar qué parte y variantes de un fichero de USD se van a importar.

* &lbrack;USD&rbrack; Opción Añadir niveles de subdivisión

  Al crear un nuevo proyecto con un archivo de malla de USD que contiene subdivisiones, es posible seleccionar el nivel de subdivisiones mediante un regulador. El proyecto se creará con la malla subdividida. El nivel se puede modificar mediante la configuración del proyecto.

* &lbrack;USD&rbrack; Importación USD mallas desolladas en un marco específico

  Al crear un nuevo proyecto con un archivo de malla de USD que contiene animación, es posible seleccionar el marco mediante un regulador que refleje la secuencia de cronología incrustada. El marco se puede modificar mediante la configuración del proyecto.

* &lbrack;USD&rbrack;&lbrack;Export&rbrack; Añadir una opción para exportar archivos USD

  Nueva casilla de verificación Exportar USD añadida a la ventana Exportar texturas. Cuando está activada, permite exportar archivos USD, así como mapas de textura, utilizando cualquier plantilla.

* &lbrack;USD&rbrack;&lbrack;Export&rbrack; Añadir USD formato de archivo a la exportación de malla

* &lbrack;USD&rbrack; Cambie el nombre del ajuste preestablecido de exportación &quot;Rugosidad del metal PBR USD&quot; para que sea más explícito

  Se puede acceder a la plantilla de exportación de USD conocida anteriormente como &quot;Rugosidad del metal de USD PBR&quot; a través de texturas de exportación > Plantilla de salida > USDz (Apple AR).

* &lbrack;Auto Unwrap&rbrack; Añadir orientación de bloqueo para el empaquetado

  Nueva opción para la configuración de desajuste automático que permite conservar la orientación de las Islas de UV existentes al utilizar la función de empaquetado. Se puede acceder a él desde Nuevo proyecto > Opciones de Desenvolvimiento automático > Orientación de la Isla de UV.

* &lbrack;Tamaño físico&rbrack; Añadir configuración para utilizar automáticamente el Tamaño físico en el efecto de relleno/capa

  Se ha añadido una nueva opción para cambiar automáticamente a la escala de tamaño físico al utilizar un material con tamaño físico incorporado. Se puede activar por proyecto a través de Nuevo proyecto o a través de Editar > Configuración del proyecto > Tamaño físico > Cambiar la escala de la capa de relleno a Tamaño físico al asignar materiales.

* &lbrack;Tamaño físico&rbrack; Exponer tamaño físico para Proyección de UV

  La escala de tamaño físico ahora está disponible para las Proyecciones de UV: permite el cambio de tamaño automático para un material en función del tamaño físico de una malla. Se puede seleccionar a través de Escala > Tamaño físico en la ventana Propiedades de la capa de relleno o del efecto.

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir consultar la versión de la aplicación

* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Actualizar API para que coincida con los nuevos parámetros de haga un bake

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Haciendo un bake módulo: editar hacer un bake parámetros

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Haciendo un bake módulo: iniciar/cancelar hacer un bake

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Haciendo un bake módulo: seleccionar método de curvatura

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Haciendo un bake módulo: selección de bakeres/mosaicos uv

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Haciendo un bake módulo: sincronizar la configuración del baker en todos los conjuntos de texturas

* &lbrack;SVT&rbrack; Habilitar la compatibilidad de hardware disperso en las GPU AMD

  La aceleración de hardware para el sistema de texturas virtuales dispersas ahora se puede activar con las GPU AMD. Este ajuste se activa automáticamente en las preferencias generales.

* &lbrack;Proyección&rbrack; Cambiar nombre de parámetros de proyección cilíndrica

  El parámetro &quot;Cylinder Cap Culling&quot; ha pasado a denominarse &quot;Backface Culling&quot; para representar mejor su acción. La información sobre herramientas asociada se ha ajustado en consecuencia.

* &lbrack;Proyecto&rbrack; Guardar la versión de la aplicación en el proyecto y recuperarla mediante scripts

  Desde la versión 8.2, la versión de la aplicación se almacena ahora dentro del archivo spp al guardar. Este número de versión se puede recuperar con la función last_saved_substance_painter_version() en el módulo de proyecto de la API de Python. Para un proyecto realizado antes de la versión 8.2, el valor devuelto será nulo.

* &lbrack;Importar&rbrack; Mejorar el tiempo de importación general de modelos 3D

  Mejoramos el tiempo general de importación de mallas. Por ejemplo, reducir el tiempo de espera al cargar mallas de alta densidad para hacer un bake. Esta optimización se aplica en particular a la carga de archivos OBJ.

**Corregido:**

* &lbrack;Bloqueo&rbrack; Cambio de canales en un filtro con una pila específica

* &lbrack;Mac&rbrack;&lbrack;M1&rbrack; Bloqueo al crear una capa de relleno y salir de la pila de capas

  Este problema se puede solucionar actualizando a Mac OS 13 (Ventura).

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Bloqueo al utilizar ui.add_dock_widget() con un tipo incorrecto

* &lbrack;Haciendo un bake&rbrack; Mensaje de error incompleto en el registro cuando falla una hace un bake

* &lbrack;Haciendo un bake&rbrack; La memoria no se libera al finalizar la hace un bake

* &lbrack;Motor&rbrack; La caché de textura no se actualiza al cambiar la visibilidad del efecto

* &lbrack;Exportar&rbrack; vista 2D exporta mapa aleatoriamente uniforme

* &lbrack;Proyecto&rbrack; Error de asignación de memoria al guardar el proyecto con malla grande

* &lbrack;Viewport&rbrack; TAA causa defectos al pintar en algunos casos

**Problemas conocidos:**

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Pila de capas&rbrack; El origen de entrada no se guarda por capa

### 8.2.0

*(Lanzado: 6 de octubre de 2022*)Resumen: **Versión principal con nuevos paneles de incorporación (nuevo panel de bienvenida y nuevo panel), exportación a SBSAR, efectos para carpetas, varias mejoras para la calidad de vida y correcciones de errores.**

**Agregado:**

* &lbrack;Incorporación&rbrack; Panel de bienvenida para nuevos usuarios

  Se ha añadido una nueva pantalla de bienvenida cuando los nuevos usuarios de CC abren Painter por primera vez.

* &lbrack;Incorporación&rbrack; Panel Novedades para mejorar la capacidad de detección de las nuevas funciones

  Se ha añadido una nueva pantalla Novedades que muestra las principales funciones nuevas. Se muestra automáticamente la primera vez que se abre Painter después de una actualización importante, y se puede volver a acceder a él a través de Ayuda > Novedades.

* &lbrack;Incorporación&rbrack; Cambiar nombre de usuario anterior Bienvenido a &quot;Pantalla de inicio&quot;

  Se ha cambiado el nombre de la pantalla de bienvenida para evitar confusiones con la nueva pantalla de bienvenida.

* &lbrack;UI&rbrack; Resolver problemas de escala para pantallas de alta resolución

  Se ha mejorado la adaptación de la interfaz de usuario de Painter en pantallas de alta definición con escala de visualización personalizada.

* &lbrack;UI&rbrack; Evitar mensajes de error persistentes en la interfaz de usuario

  Los mensajes de error de proyectos anteriores ahora se eliminan de la barra de estado inferior.

* &lbrack;UI&rbrack; Menú Guardar retrabajo

  Las opciones de guardado adicionales ahora se agrupan en un submenú y se cambia el nombre de algunas de ellas por coherencia.

* &lbrack;UI&rbrack; Guardar y exportar/compartir diseños de IU

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

* &lbrack;Panel Activos&rbrack; Los recursos favoritos de los &quot;Pin&quot; aparecerán en la parte superior del panel de recursos

  Se ha añadido una nueva opción de clic con el botón derecho en los recursos de la biblioteca que permite pin como favoritos en la parte superior del panel. También puede ver todos sus activos favoritos a través de Búsquedas guardadas.

* &lbrack;Panel Activos&rbrack; Eliminar, volver a cargar y cambiar el nombre de activos

  Se han añadido opciones de menú contextual para eliminar, volver a cargar y cambiar el nombre de los activos en la biblioteca del usuario. Se eliminan directamente de la ubicación de su biblioteca en el disco y se vuelven a cargar desde la ubicación original. Los activos que forman parte de un paquete como .abr o .sbsar no se pueden editar individualmente.

* &lbrack;Selección de color&rbrack; Adición de modos de fusión al efecto Selección de color

* &lbrack;Pila de capas&rbrack; Añadir modo de fusión y opacidad en los filtros

* &lbrack;Pila de capas&rbrack; Permitir valores de mosaico mayores que 128 para capas/efectos de relleno

* &lbrack;Pila de capas&rbrack; Tapones cilíndricos para proyección cilíndrica en capa/efecto de relleno

  La proyección cilíndrica en Propiedades de capa de relleno ahora tiene la opción de eliminar tapas de cilindro.

* &lbrack;Registro&rbrack; Mostrar un mensaje de error si los elementos de malla están en espacio negativo al intentar crear un proyecto de Mosaico de UV

  Se ha añadido un mensaje de error más claro al no crear un proyecto de Mosaico de UV porque las partes UV se encuentran en espacios negativos.

* &lbrack;Proyecto&rbrack; Indicar la versión en el mensaje de error &quot;Datos demasiado recientes&quot; al abrir un proyecto

  Al abrir un proyecto que es demasiado reciente para la aplicación, el mensaje de error indicará ahora la versión del proyecto para que sea más fácil identificar la versión correcta de la aplicación.

* &lbrack;Viewport&rbrack; Permita que se ilumine la malla desde abajo

  Se ha añadido un nuevo parámetro Alineación del entorno en Configuración de la pantalla > Cámara > Configuración del entorno para alinear la iluminación del mapa de entorno con la cámara cuando se establece en &quot;Local&quot;.

* &lbrack;Viewport&rbrack; Ver R, G, B y Alpha en la ventana gráfica (modo de visualización individual)

  En Configuración de visualización > Configuración de ventana gráfica > Visualización de canal , hay un nuevo ajuste de Canales de color que solo permite mostrar el componente R, G, B o Alpha de un canal en el modo de visualización única.

* &lbrack;Sombreador&rbrack; Permitir la configuración de canales de usuario como RGBA en sombreadores de capas de material

  Al definir la configuración de canales del conjunto de texturas dentro de un sombreador para la capa de material, ahora es posible especificar el formato del canal que se va a desviar del valor predeterminado. Esto permite en particular solicitar canales de usuario de color en lugar de solo escala de grises.

* &lbrack;Exportar&rbrack; Permitir exportar texturas como SBSAR

  Al exportar texturas a través de la ventana Archivo > Exportar Texturas, se puede elegir el formato de archivo SBSAR (Archivo de Substance) para reagruparlas. El contenido de la SBSAR depende de la plantilla de salida utilizada. El formato de archivo SBSAR también se puede establecer en los ajustes preestablecidos de exportación. Cuando se utiliza una configuración híbrida (SBSAR + otro formato), las texturas que tienen como destino un SBSAR se agrupan mientras que el resto se exporta junto a ellas.

* &lbrack;Exportar&rbrack; Opción Exponer 16 bits para EXR formato de archivo

  Al exportar archivos de textura de EXR, ahora es posible elegir 16f bit (medio Flotante) o 32f bit (Flotante) en la ventana Exportar Texturas (tanto para ajustes de exportación como para ajustes preestablecidos de exportación). Los proyectos antiguos y los ajustes preestablecidos de exportación antiguos se establecerán de forma predeterminada en 16f bit para reflejar el comportamiento antiguo.

* &lbrack;Python&rbrack; Agregar evento para saber cuándo se modifican los conjuntos de texturas

  El nuevo &quot;substance_painter.event.TextureStateEvent&quot; permite saber cuándo se ha modificado un conjunto de texturas debido a un trazo de pintura, un nuevo canal añadido o un canal eliminado.

* &lbrack;Python&rbrack; Permitir obtener y definir recursos de mapa de malla en los ajustes de Conjunto de texturas

  Se han añadido nuevas funciones en el módulo &quot;substance_painter.project&quot; para obtener y definir recursos de mapas de malla. Estas funciones se pueden utilizar para actualizar los mapas de malla a los que hace referencia la configuración de Conjunto de texturas.

* &lbrack;Complementos&rbrack; Opción Quitar para obtener otros complementos de JS

  Se ha eliminado la opción para obtener los complementos de JavaScript, ya que se alojaban en el sitio web obsoleto Compartir .

* &lbrack;Contenido&rbrack; Añadir nueva plantilla Roblox y exportar ajuste preestablecido

  Se han añadido una nueva plantilla de proyecto &quot;Material Variant&quot; y &quot;Surface Appearance&quot; de Roblox y un ajuste preestablecido de exportación para facilitar la exportación de texturas PBR a Roblox. Se puede acceder a la plantilla desde la ventana Archivo > Nuevo proyecto.

* Actualizar Substance Engine a la última versión (8.6.3)

* &lbrack;Vapor&rbrack; Compilación optimizada para chipset Apple Silicon (Apple M1 / M2)

**Corregido:**

* Bloqueo al utilizar 16k exr

* &lbrack;Bloqueo&rbrack; Ctrl Z Después de eliminar una instancia del sombreador

* &lbrack;Iray&rbrack; IoR está bloqueado en 1 para algunos sombreadores

* &lbrack;Win&rbrack;&lbrack;Haciendo un bake&rbrack; Algunos High-Poly no se cargan

* &lbrack;Administración de color&rbrack; Nombre de espacio de color incorrecto en la IU con filtros

* &lbrack;Python&rbrack; Los objetos de recursos devueltos por la función import no tienen un tipo

  Al importar un paquete de Substance en Python, la función devolvía el paquete en lugar de sus gráficos. El módulo de recursos ahora proporciona funciones y parámetros para recuperar los gráficos de un paquete de Substance.

**Problemas conocidos:**

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Pila de capas&rbrack; El origen de entrada no se guarda por capa
* &lbrack;Pintura&rbrack; El suavizado temporal provoca defectos al pintar en algunos casos
* &lbrack;Exportar&rbrack; vista 2D exporta mapa aleatoriamente uniforme

### 8.1.3

*(Lanzado: 25 de agosto de 2022*)Resumen: **Versión secundaria de corrección de errores**

**Agregado:**

* Actualizar a Iray SDK 1.6

**Corregido:**

* &lbrack;Sombreador&rbrack; Bloqueo con sombreador defectuoso antiguo
* &lbrack;Material Layering&rbrack; Los materiales pueden desaparecer al volver a abrir un proyecto

**Problemas conocidos:**

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Pila de capas&rbrack; El origen de entrada no se guarda por capa
* &lbrack;Bloqueo&rbrack; Ctrl Z Después de eliminar una instancia del sombreador
* &lbrack;Iray&rbrack; IoR está bloqueado en 1 para algunos sombreadores

### 8.1.2

*(Lanzado: 19 de julio de 2022*)Resumen: **Versión secundaria de corrección de errores**

**Agregado:**

* &lbrack;Auto Unwrap&rbrack; Nueva opción &quot;Optimizar para mallas orgánicas&quot; para seleccionar el algoritmo de segmentación
* &lbrack;Tamaño físico&rbrack; Opciones de unidad de exposición en Nueva configuración de proyecto y proyecto
* &lbrack;Administración de color&rbrack; Usar la pantalla del monitor de forma predeterminada al utilizar ACE
* &lbrack;Administración de color&rbrack;&lbrack;Python&rbrack; Tenga en cuenta ACE archivo de ajustes preestablecidos env-var al crear el proyecto
* &lbrack;Administración de color&rbrack; Restablecer la configuración de gestión de color en la ventana Nuevo proyecto cuando cambie la configuración
* &lbrack;Administración de color&rbrack; Deshabilitar el acceso a la configuración de OCIO cuando está presente env-var
* &lbrack;Administración de color&rbrack; Actualice de forma segura ACE configuración cuando ya no exista un parámetro
* Actualizar Substance Engine a la versión 8.6.0
* &lbrack;Exportar&rbrack; Añadir nuevo ajuste preestablecido de exportación GLTF compatible con el Desplazamiento
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Recuperar información de recursos (incluidos metadatos personalizados)
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Agregar función a la lista de consulta de nombres de malla por conjunto de texturas
* &lbrack;Contenido&rbrack; Añadir una nueva plantilla de mezclador y exportar un ajuste preestablecido

**Corregido:**

* &lbrack;MacOS&rbrack; Bloqueo al lanzar a Irak en algunos casos
* &lbrack;Miniaturas&rbrack; Las miniaturas de estante no se cargan correctamente
* Se omiten varios canales UV
* &lbrack;Auto Unwrap&rbrack; Cálculo innecesario al dividir islas largas
* &lbrack;Auto Unwrap&rbrack; Opción de evitar las islas alargadas no tenidas en cuenta
* &lbrack;Auto Unwrap&rbrack; Pérdida de datos adicionales (colores de vértice) al reempaquetar UV
* &lbrack;UI&rbrack; Barra de desplazamiento horizontal en la ventana de propiedades cuando la gestión de color está activada
* &lbrack;Administración de color&rbrack; OCIO configuraciones no tienen la función substance_3d_painter_standard_srgb
* &lbrack;Generador&rbrack; Uso incorrecto de los datos de usuario &quot;deshabilitado&quot;
* &lbrack;Administración de color&rbrack; No se debe hacer clic en el menú desplegable Espacio de color &quot;No compatible&quot;
* &lbrack;Administración de color&rbrack;&lbrack;Sombreador&rbrack; La anulación de definición de sRGB ya no funciona
* &lbrack;Generador&rbrack; Uso incorrecto de los datos de usuario &quot;desactivar&quot;
* &lbrack;Pila de capas&rbrack; Previsualizaciones rotas con proyectos de Mosaicos de UV
* &lbrack;Sombreador&rbrack; La documentación de la API no está completamente actualizada con Normales dobladas
* &lbrack;Export&rbrack;&lbrack;Interoperability&rbrack; No se puede enviar a Stager con caracteres especiales
* &lbrack;Contenido&rbrack; Algunas miniaturas de pinceles preestablecidos están vacías o son demasiado oscuras

**Problemas conocidos:**

* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción
* &lbrack;Pila de capas&rbrack; Las fuentes de entrada no se guardan por capa
* &lbrack;Bloqueo&rbrack; Ctrl Z Después de eliminar una instancia del sombreador
* &lbrack;Iray&rbrack; IoR está bloqueado en 1 para algunos sombreadores
* &lbrack;Sombreador&rbrack; Bloqueo con sombreador defectuoso antiguo

### 8.1.1

*(Lanzado: 28 de junio de 2022*)Resumen: **Revisión de versión secundaria**

**Agregado:**

* &lbrack;Pila de capas&rbrack; Al pulsar Alt en la máscara ya no se deseleccionan los efectos

**Corregido:**

* &lbrack;Bloqueo&rbrack; Abrir proyecto antiguo guardado en el modo de vista en solitario
* &lbrack;Bloqueo&rbrack; Eliminar un generador en propiedades
* &lbrack;Configuración del conjunto de texturas&rbrack; La mezcla normal/de Oclusión ambiental y el height a los métodos normales se rompen
* &lbrack;Exportar&rbrack; La exportación de texturas mediante relleno de difusión produce mapas negros

**Problemas conocidos:**

* &lbrack;MacOS&rbrack; Bloqueo al lanzar Iray en Monterey
* &lbrack;Vista previa de miniaturas&rbrack; Las miniaturas simplificadas no se actualizan cuando se utiliza un anclaje
* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción

### 8.1.0

*(Lanzado: 07 de junio de 2022*)Resumen: **Versión principal compatible con ICC, escalado de materiales basado en datos de tamaño físico, nuevos bakeres, mejoras en el cuentagotas de color y una amplia gama de contenido adicional**

**Agregado:**

* &lbrack;Administración de color&rbrack; Añadir compatibilidad con perfiles ICC con Adobe Color Engine (ACE)
* &lbrack;Administración de color&rbrack; Añada compatibilidad para &quot;RGB de Adobe 98&quot; como espacio de color de trabajo para ICC
* &lbrack;Administración de color&rbrack; Permitir la configuración de ACE/ICC mediante un archivo de configuración
* &lbrack;Administración de color&rbrack; Permitir la entrada de valores de color lineal en el Selector de color con el modo Heredado
* &lbrack;Administración de color&rbrack; Permitir especificar el perfil de color utilizado para seleccionar color fuera de la interfaz de usuario
* &lbrack;Administración de color&rbrack; Recordar el último valor de visualización elegido en la ventana gráfica
* &lbrack;Administración de color&rbrack;&lbrack;Substance&rbrack; Hacer que los generadores/filtros funcionen correctamente con la gestión de color
* &lbrack;Administración de color&rbrack;&lbrack;Substance&rbrack; Añadir nuevas palabras clave de anulación de espacio de color $working y $standardsrgb
* &lbrack;Tamaño físico&rbrack;&lbrack;Motor&rbrack; Extraer información del tamaño físico de la malla
* &lbrack;Tamaño físico&rbrack;&lbrack;Motor&rbrack; cálculo del tamaño físico
* &lbrack;Tamaño físico&rbrack; Opciones de exposición para utilizar el tamaño físico en la interfaz de usuario
* &lbrack;Tamaño físico&rbrack; Añadir ayudantes visuales en la ventana gráfica
* &lbrack;Haciendo un bake&rbrack; Añadir baker de Height
* &lbrack;Haciendo un bake&rbrack; Baker Añadir Normales dobladas
* &lbrack;Haciendo un bake&rbrack; Añadir baker de opacidad
* &lbrack;Cuentagotas; Nueva previsualización del cuentagotas de color junto al ratón y el color gestionado
* &lbrack;Cuentagotas; El panel del selector de color vuelve a aparecer en su última posición cuando se vuelve a abrir
* &lbrack;Cuentagotas; Un nuevo icono para el Selector de material
* &lbrack;Cuentagotas; Gestión de color de la previsualización del canal del selector de color
* &lbrack;Cuentagotas; Añadir la funcionalidad de hacer clic para seleccionar al cuentagotas
* &lbrack;Cuentagotas; El selector de material ya no activa canales no activos
* &lbrack;Cuentagotas; Permitir el uso del cuentagotas con un método abreviado
* &lbrack;Cuentagotas; El cuentagotas selecciona el canal correspondiente, cuando corresponde
* &lbrack;Cuentagotas; Al entrar en el modo del selector de color se desactivan todos los métodos abreviados
* &lbrack;Cuentagotas; Eliminación de la selección automática del campo hexadecimal
* &lbrack;Cuentagotas; No cerrar el panel al utilizar el selector de materiales
* &lbrack;Cuentagotas; Nuevo estado deshabilitado cuando el canal no está disponible para seleccionar
* &lbrack;Exportar&rbrack; Añadir atributo de tangente a la exportación glTF
* Actualizar Substance Engine a v8.4
* Actualizar Auto Unwrap a 0.9.0
* Actualizar a Qt 5.15.8
* Actualizar a Python 3.9
* &lbrack;Sombreador&rbrack; Añadir compatibilidad con el sombreado de Normales dobladas
* &lbrack;MacOS&rbrack; Compatibilidad con SpaceMouse 3DConnection
* &lbrack;Python&rbrack; Documentar la versión de Python utilizada en la API
* &lbrack;Contenido&rbrack; Añade 6 nuevos sonidos 3D con 105 ajustes preestablecidos
* &lbrack;Contenido&rbrack; 20 nuevos mapas de suciedad y 2 patrones de pliegues de tela
* &lbrack;Contenido&rbrack; Actualizar el ajuste preestablecido de exportación &quot;Mapas de malla&quot; para utilizar nuevos bakeres
* &lbrack;Contenido&rbrack; La Pendiente de desenfoque y el filtro de deformación dependen de la resolución del conjunto de texturas
* &lbrack;Contenido&rbrack; Actualizar proyectos de ejemplo para utilizar los 3 nuevos bakeres

**Corregido:**

* &lbrack;glTF&rbrack; No se puede abrir glTF con un carácter especial
* &lbrack;Motor&rbrack; Artefactos con anisotropía y SVT desactivados
* &lbrack;MacOS&rbrack;&lbrack;M1&rbrack; Los materiales inteligentes no se muestran correctamente
* &lbrack;Procesamiento de malla&rbrack; No se pueden importar mallas desde Modeler
* &lbrack;UI&rbrack; Barra de desplazamiento horizontal en la ventana de nuevo proyecto con la gestión de color activada
* &lbrack;Administración de color&rbrack; Falta el valor del espacio de trabajo en el selector de color con algunas configuraciones de OCIO
* &lbrack;Administración de color&rbrack; La previsualización del pincel en la ventana gráfica no tiene gestión de color
* &lbrack;SpaceMouse&rbrack; La tabla dinámica no se actualiza inmediatamente con el cambio de enfoque y, a veces, se sale del modelo
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Los archivos USD exportados tienen una estructura incorrecta
* &lbrack;USD&rbrack; Problema de oclusión ambiental al exportar
* &lbrack;Contenido&rbrack; Actualizar la malla de la miniatura para que coincida con el proyecto de muestra Previsualizar esfera

**Problemas conocidos:**

* La exportación de texturas mediante relleno de difusión produce mapas negros
* La mezcla normal o de Oclusión ambiental no funciona
* &lbrack;MacOS&rbrack; Bloqueo al lanzar a Irak en algunos casos raros
* &lbrack;Vista previa de miniaturas&rbrack; Las miniaturas simplificadas no se actualizan cuando se utiliza un anclaje
* &lbrack;Administración de color&rbrack; HDR. las conversiones de espacio de color con ACE en Linux producen colores con sujeción

## Versión 7

### 7.4.3

*(Lanzado: 11 de abril de 2022*)Resumen: **Corrección de error compatible con SpaceMouse de conexión 3D en la ventana gráfica 2D**

**Agregado:**

* &lbrack;SpaceMouse&rbrack; Compatibilidad con SpaceMouse de conexión 3D en la ventana gráfica 2D

**Corregido:**

* &lbrack;Selector de color&rbrack; No se puede escribir en campos hexadecimales
* &lbrack;Administración de color&rbrack; Los recursos utilizados en el modo de proyección no tienen gestión de color en la superposición
* &lbrack;Administración de color&rbrack; Los errores no se notifican en el registro
* &lbrack;SpaceMouse&rbrack; Quitar mensaje de error genérico si el usuario no tiene un SpaceMouse
* &lbrack;SpaceMouse&rbrack; Al cargar un proyecto, el punto de giro siempre está oculto
* &lbrack;Bakeres&rbrack; El ajuste &quot;Normales medias&quot; no tiene efecto en los proyectos de Mosaico de UV
* &lbrack;Mosaico de UV&rbrack; Las superposiciones de mosaicos uv inactivos desaparecen al volver a cargar la malla con diferentes mosaicos
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; La secuencia de comandos remota no funciona
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; No se pueden consultar varios canales desde la API y se produce un error
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Bloqueo al utilizar el evento ProjectEditionEntered
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Bloqueo al llamar a get_active_stack()

**Problemas conocidos:**

* Conexión 3D con SpaceMouse no compatible en MacOS
* &lbrack;UI&rbrack; Barra de desplazamiento horizontal con gestión de color que aparece en algunos casos en la ventana de nuevo proyecto
* &lbrack;Mac M1&rbrack; Los materiales inteligentes no se muestran correctamente

### 7.4.2

*(Lanzado: 8 de marzo de 2022*)Resumen: **Corrección de error compatible con SpaceMouse de conexión 3D y mejoras en la administración de color (OCIO)**

**Agregado:**

* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; Compatibilidad con la conexión 3D de SpaceMouse en la ventana gráfica 3D para la navegación
* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; Métodos abreviados/teclas básicos para los modelos Pro y Enterprise SpaceMouse en el área de visualización 3D
* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; Icono del centro de rotación dedicado en la ventana gráfica 3D
* &lbrack;Administración de color&rbrack; Utilizar funciones de OCIO configuración para cambiar la configuración predeterminada
* &lbrack;Administración de color&rbrack; Gestión de color de la ventana de propiedades para widgets de color
* &lbrack;Administración de color&rbrack; Gestión de color de la ventana de propiedades para la previsualización de material
* &lbrack;Administración de color&rbrack; Gestión de color de muestras en el selector de color
* &lbrack;Administración de color&rbrack; Añadir un ajuste para definir el espacio de color sRGB estándar
* &lbrack;Administración de color&rbrack; Añadir el espacio de color sRGB estándar desde OCIO configuración en el selector de color Lista de selectores de visualización
* &lbrack;Administración de color&rbrack; Mejoras en el menú de anulación del espacio de color
* &lbrack;Administración de color&rbrack; Permitir anular el espacio de color del mapa de entorno en Configuración de visualización
* &lbrack;Administración de color&rbrack; Dibujar degradados del selector de color según la visualización actual
* &lbrack;Administración de color&rbrack; Ajustar valores HDR. de forma predeterminada en el editor de color
* &lbrack;Administración de color&rbrack; Usar el paso a través (sin espacio de color) para filtros en el modo Heredado
* &lbrack;Administración de color&rbrack; Limitar la visualización de degradados en el editor de color para que coincida con &lbrack;0-1&rbrack; gama
* &lbrack;Administración de color&rbrack; Ocultar el selector de visualización en el selector de color en el modo Heredado
* &lbrack;Administración de color&rbrack; Hacer que el campo hexadecimal del selector de color esté siempre en el espacio de color sRGB
* &lbrack;Administración de color&rbrack; Desactivar menú desplegable de visualización del selector de color para canales de datos
* &lbrack;Optimización&rbrack; La cuadrícula de deformación vuelve a calcular únicamente los mosaicos UV cubiertos
* &lbrack;Exportar&rbrack; Permitir exportar proyectos de Mosaico de UV para Sketchfab, USD y glTF
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir cambiar la función de asignación de tonos

**Corregido:**

* &lbrack;Sketchfab&rbrack; La actualización de un modelo existente termina creando un nuevo modelo
* &lbrack;Sketchfab&rbrack; Bloqueo al buscar un modelo actualizado anteriormente
* Bloqueo al exportar a USD
* Bloqueo al crear una nueva instancia del sombreador en Máscara de geometría o cuando la geometría está oculta
* &lbrack;Importar ventana de recursos&rbrack; Bloqueo al cambiar el tipo de recursos importados
* Los mapas de malla normales se invierten cuando se utilizan en la pila de capas
* &lbrack;Substance&rbrack; El modo de fusión de datos de usuario no se tiene en cuenta
* &lbrack;Administración de color&rbrack; Los mapas de bits con espacio de color en el nombre de archivo se importan como secuencias de Mosaico de UV
* &lbrack;Administración de color&rbrack; Las salidas de gestión de color del gráfico del Substance están en un espacio de color incorrecto
* &lbrack;Administración de color&rbrack; La herramienta Relleno poligonal muestra un color incorrecto
* &lbrack;Administración de color&rbrack; ACE asignador de tonos se aplica a los canales en modo solo
* &lbrack;Administración de color&rbrack; La iluminación de la esfera de previsualización de herramientas no se gestiona por el color
* &lbrack;Administración de color&rbrack;&lbrack;Exportar&rbrack; Los mapas convertidos aplican una conversión incorrecta
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack;&lbrack;Administración de color&rbrack; Los proyectos creados con plantillas y OCIO variables de entorno están en modo Heredado
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; No se puede utilizar la función de evaluación de JavaScript al inicio
* &lbrack;Oferta de Adobe 3D&rbrack; No se puede iniciar Painter al utilizar la configuración regional con idiomas no admitidos de forma predeterminada

**Problemas conocidos:**

* Conexión 3D con SpaceMouse no compatible en MacOS
* &lbrack;UI&rbrack; Barra de desplazamiento horizontal con gestión de color que aparece en algunos casos en la ventana de nuevo proyecto
* &lbrack;Bakeres&rbrack; El ajuste &quot;Normales medias&quot; no tiene efecto en los proyectos de Mosaico de UV
* &lbrack;Mac M1&rbrack; Los materiales inteligentes no se muestran correctamente
* &lbrack;Administración de color&rbrack; Los recursos utilizados en el modo de proyección no tienen gestión de color en la superposición
* &lbrack;Selector de color&rbrack; No se puede escribir en campos hexadecimales

### 7.4.1

*(Lanzado: 14 de diciembre de 2021*)Resumen: **Corrección de errores con mejoras en la administración de color**

**Agregado:**

* &lbrack;Administración de color&rbrack; Usar función de datos en nombres de archivo exportados
* &lbrack;Administración de color&rbrack; Expanda la sección Administración de color de forma predeterminada cuando se selecciona OCIO en las nuevas ventanas de proyecto y configuración del proyecto
* &lbrack;Administración de color&rbrack; Añadir ACE asignador de tonos en modo heredado
* &lbrack;Administración de color&rbrack; Ajustar la configuración predeterminada
* &lbrack;Administración de color&rbrack;&lbrack;Exportar&rbrack; Rellenar $colorEspacio en nombres de archivo para canales de datos
* &lbrack;Exportar&rbrack; Exportar proyecto de Mosaico de UV a Stager
* &lbrack;Interoperabilidad&rbrack; No disponible para las ediciones Steam y Substance
* &lbrack;Interoperabilidad&rbrack; Permitir enviar un proyecto de Mosaico de UV a Stager

**Corregido:**

* &lbrack;MacOS&rbrack;&lbrack;Bloqueo&rbrack; Painter no empieza con Catalina
* &lbrack;Administración de color&rbrack;&lbrack;Bloqueo&rbrack; Bloqueo aleatorio al jugar con la gestión de color/tipo de datos en el canal del usuario
* &lbrack;Administración de color&rbrack; Recursos utilizados como escala de grises en el espacio de color de visualización de máscara nuevo menú
* &lbrack;Administración de color&rbrack; El canal de usuario es más oscuro en la ventana gráfica en el modo heredado + vista solo
* &lbrack;Administración de color&rbrack; El mapa Env siempre es lineal cuando se utiliza en iRay
* &lbrack;Administración de color&rbrack; El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
* &lbrack;Administración de color&rbrack; El selector de color se interrumpe en el interior de un Substance en modo heredado
* &lbrack;Administración de color&rbrack; El cambio entre vistas de canal solo en la ventana gráfica no se muestra con el espacio de color correcto al utilizar el menú desplegable
* &lbrack;Administración de color&rbrack; La exportación aplica una conversión incorrecta en los canales de usuario con gestión de color en el modo heredado
* Los trazos realizados en la máscara de vista solo no se muestran al volver a la vista de material
* &lbrack;Exportar&rbrack; Los mapas convertidos no se exportan como canales con gestión de color
* &lbrack;Conjunto de texturas&rbrack; Falta la información sobre herramientas con el nombre original en los canales de usuario renombrados
* &lbrack;Vapor&rbrack; Faltan archivos al comprobar su integridad con Steam

**Problemas conocidos:**

* &lbrack;Mac M1&rbrack; Los materiales inteligentes no se muestran correctamente

### 7.4.0

*(Lanzado: 24 de noviembre de 2021*)Resumen: **Versión principal. Introducción de la primera versión de la administración de color, desacoplar vista 2D o 3D, nueva opción de desempaquetado UV automático para evitar islas alargadas, llamar a funciones de JavaScript desde la API de Python y nuevo contenido**

**Agregado:**

* &lbrack;Administración de color&rbrack; Compatibilidad con la gestión de color OpenColorIO versión 2
* &lbrack;Administración de color&rbrack; Añadir ajustes de gestión de color a los ajustes del proyecto
* &lbrack;Administración de color&rbrack; Ventana de advertencia sobre los cambios de configuración de la gestión de color al abrir un proyecto
* &lbrack;Administración de color&rbrack; Mostrar un mensaje de error si se ha seleccionado un archivo de configuración de OCIO no válido
* &lbrack;Administración de color&rbrack; Permitir anular la configuración con OCIO variable de entorno
* &lbrack;Administración de color&rbrack; Varias configuraciones de OCIO integradas de forma predeterminada con la aplicación
* &lbrack;Administración de color&rbrack; Extraer nombre de espacio de color del nombre de archivo de mapa de bits importado
* &lbrack;Administración de color&rbrack; Permitir anular el espacio de color con un espacio de color desde la configuración de la ventana Propiedades
* &lbrack;Administración de color&rbrack; Añadir opciones de gestión de color en Configuración del conjunto de texturas
* &lbrack;Administración de color&rbrack;&lbrack;Viewport&rbrack; Permitir la gestión de color de vistas 2D y 3D por separado
* &lbrack;Administración de color&rbrack; Cargar y convertir mapa de entorno en el espacio de color de trabajo
* &lbrack;Administración de color&rbrack; Ajustar el selector de color y el editor con el espacio de color actual
* &lbrack;Administración de color&rbrack; Permitir seleccionar la visualización transformar espacio de color en la ventana gráfica con un nuevo menú desplegable
* &lbrack;Administración de color&rbrack; Aplicar visualización transformar con resultados de procesamiento de Iray
* &lbrack;Administración de color&rbrack; Exportar texturas con diferentes espacios de color
* &lbrack;Administración de color&rbrack;&lbrack;Python&rbrack; Aplicación de ajustes de gestión de color de la variable de entorno (OCIO) a proyectos nuevos
* &lbrack;Viewport&rbrack; Permitir desacoplar la ventana gráfica 2D o 3D
* &lbrack;Auto Unwrap&rbrack; Nueva opción para evitar islas alargadas
* &lbrack;Secuencia de comandos Python&rbrack; Llamar a funciones de JavaScript desde la API de Python
* &lbrack;Nueva ventana de proyecto&rbrack; Hacer que la sección de mapas importados sea contraíble
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Permitir ocultar normales como una opción en la configuración de Deformación
* &lbrack;Contenido&rbrack; 11 nuevos mapas de suciedades
* &lbrack;Contenido&rbrack; 8 nuevos ajustes preestablecidos de herramientas (cremallera, cable de apriete, brillo)
* &lbrack;Contenido&rbrack; 8 materiales nuevos (cicatriz, bolsillo, ...)
* &lbrack;Contenido&rbrack; 1 generador nuevo (inflar encogimiento)

**Problemas conocidos:**

* &lbrack;Mac M1&rbrack; Los materiales inteligentes no se muestran correctamente
* &lbrack;Administración de color&rbrack;&lbrack;Bloqueo&rbrack; Bloqueo aleatorio al jugar con la gestión de color/tipo de datos en el canal del usuario
* &lbrack;Administración de color&rbrack; El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
* &lbrack;Administración de color&rbrack;&lbrack;Iray&rbrack; Si se guarda el procesamiento en EXR o TIFF mientras la gestión de color está activada en la ventana gráfica, el guardado siempre será lineal
* &lbrack;Administración de color&rbrack; Los recursos utilizados como escala de grises en la máscara muestran el menú Espacio de color incorrecto
* &lbrack;Administración de color&rbrack;&lbrack;Iray&rbrack; El mapa Env siempre es lineal cuando se usa en Irak
* &lbrack;Administración de color&rbrack;&lbrack;Exportar&rbrack; Los mapas convertidos no se exportan como canales con gestión de color
* &lbrack;Administración de color&rbrack;&lbrack;Exportar&rbrack; La exportación ignora si el canal del usuario tiene gestión de color o no está en modo heredado

### 7.3.1

*(Lanzado: 24 de noviembre de 2021*)Resumen: **Corrección de error**

**Agregado:**

* &lbrack;Proyección&rbrack; La escala solo debería funcionar en el espacio de objetos

**Corregido:**

* &lbrack;Mac M1&rbrack; La capa de material no funciona
* &lbrack;Mac M1&rbrack;&lbrack;Proyección&rbrack; La deformación no funciona
* Los detalles del micro no se muestran correctamente
* &lbrack;Proyección&rbrack;&lbrack;Bloqueo&rbrack; Cambio al modo de deformación con una capa creada con una versión anterior
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Voltear no funciona cuando la transformación se establece en el espacio de entorno
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; La opción Dividir permanece seleccionada después de realizar la división
* &lbrack;Proyección&rbrack;&lbrack;UV&rbrack; El punto de giro se restablece al voltear la proyección
* &lbrack;Filtro&rbrack; Hacer un bake El entorno de iluminación cambia al volver a cargar o cambiar un parámetro
* &lbrack;Interoperabilidad&rbrack; No disponible para las ediciones Steam y Substance
* &lbrack;Interoperabilidad&rbrack; El botón &quot;Examinar contenidos 3D en el mercado&quot; siempre debe abrir el CCD en la pestaña 3D de Stock y Mercado

**Problemas conocidos:**

* &lbrack;Mac M1&rbrack; Los materiales inteligentes no se muestran correctamente

### 7.3.0

*(Lanzado: 13 de octubre de 2021*)Resumen: **Versión principal. Contiene una nueva proyección de deformación 3D, una nueva proyección cilíndrica, mejoras del selector de color, nuevas funciones en la API de Python y correcciones de errores**

**Agregado:**

* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Exponer deformación 3D como un nuevo modo de proyección
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Permitir el modo de pegatina para Alpha, Texturas y procedimientos con la función de arrastrar y soltar en la ventana gráfica
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Usar proyección de deformación con método abreviado de pegatina (ALT)
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack;&lbrack;Barra de herramientas&brack; Transformar deformación como completa o por vértices
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack;&lbrack;Barra de herramientas&brack; Añadir puntos de rejilla con las opciones de deformación dividida en sentido cruzado, horizontal o vertical
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack;&lbrack;Barra de herramientas&brack; Menú dedicado para acciones de restablecimiento
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack;&lbrack;Barra de herramientas&brack; Opción para ajustar automáticamente las tangentes al mover puntos
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack;&lbrack;Barra de herramientas&brack; Menú dedicado para la edición de cuadrícula (tamaño, restablecimiento, color y tamaño de control)
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Nuevo método abreviado de teclado para cambiar el modo de edición de deformación de vértices completos (MAYÚS+V)
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Clic+Ctrl permite cambiar entre la herramienta Superficie y otras herramientas
* &lbrack;Proyección&rbrack;&lbrack;Cilíndrico&rbrack; Exponer el modo de proyección cilíndrica
* &lbrack;Proyección&rbrack;&lbrack;Barra de herramientas&rbrack; Configuración del manipulador de grupo (tamaño, pasos de cuadrícula, pasos de ángulo)
* &lbrack;Selector de color&rbrack; Nueva interfaz de usuario del selector de color
* &lbrack;Selector de color&rbrack; Uso de valores sRGB en widgets de selector de color
* &lbrack;Selector de color&rbrack; Permitir guardar y eliminar muestras de color
* &lbrack;Selector de color&rbrack; Cuentagotas accesible desde las ranuras de color y normales
* &lbrack;Selector de color&rbrack; Permitir la edición de color dinámico entre 0 y 255 valores
* &lbrack;Selector de color&rbrack; Hacer común el estado de HSV/RGB en toda la aplicación
* &lbrack;Selector de color&rbrack; La ventana del selector de color es semipersistente
* &lbrack;Selector de color&rbrack; Al pulsar Esc se cierra la ventana del selector de color
* Mejora del rendimiento para la interacción de la interfaz de usuario y la pintura
* &lbrack;Motor&rbrack; Actualizar a la nueva versión del motor de Substance (8.3.0)
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir volver a cargar la malla del proyecto actual
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir la actualización de recursos en proyectos
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir establecer y consultar la resolución de Mosaicos de UV
* &lbrack;Interoperabilidad&rbrack; No disponible para las ediciones Steam y Substance
* &lbrack;Interoperabilidad&rbrack; Recibir varios recursos de Bridge

**Corregido:**

* El selector de color no muestra el color correcto
* &lbrack;Haciendo un bake&rbrack; La lista de conjuntos de texturas no está ordenada correctamente
* &lbrack;FBX import&rbrack; No se tienen en cuenta las transformaciones de pivote de grupo 3ds Max
* &lbrack;Substance Engine&rbrack; Bloqueo con la importación de SBSAR dañado
* &lbrack;MacOS&rbrack; La opción de configuración del proyecto en diferentes idiomas no está presente
* El guardado automático puede congelar Painter durante procesos largos

**Problemas conocidos:**

* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; La opción Dividir permanece seleccionada después de realizar la división
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Voltear no funciona cuando la transformación se establece en el espacio de entorno
* &lbrack;Proyección&rbrack;&lbrack;Deformar&rbrack; Líneas de artefacto entre parches en algunos casos raros
* &lbrack;Proyección&rbrack;&lbrack;UV&rbrack; El punto de giro se restablece al voltear la proyección
* &lbrack;Mac M1&rbrack; Los materiales inteligentes no se muestran correctamente
* &lbrack;M1&rbrack;&lbrack;Regresión&rbrack; La capa de material no funciona

### 7.2.3

*(Lanzado: 24 de agosto de 2021*)Resumen: **Versión secundaria, corrección de errores**

**Agregado:**

* &lbrack;Bibliotecas&rbrack; Agregar una forma de excluir archivos no deseados del rastreo

**Corregido:**

* &lbrack;Win&rbrack; Problemas de suspensión y varias pantallas
* &lbrack;MacOS&rbrack;&lbrack;Bloqueo&rbrack; Cambio de sombreador al utilizar efectos
* &lbrack;Viewport&rbrack; El modo de previsualización completa ya no muestra el cursor del pincel sin alfa
* &lbrack;UI&rbrack; El widget de ángulo gira en la dirección equivocada
* &lbrack;Pila de capas&rbrack; Muchas subcarpetas crean bloqueos muy largos
* &lbrack;Iray&rbrack; Diferentes vistas en Iray y OpenGL: Visible si no funciona
* &lbrack;Iray&rbrack; El índice de refracción no se tiene en cuenta y no aparece en las propiedades de mdl
* &lbrack;JavaScript&rbrack; ShowExportDialog() nunca devuelve true
* No se puede leer mtl desde Adobe Stock

### 7.2.2

*(Lanzado: 27 de julio de 2021*)Resumen: **Versión secundaria, corrección de errores**

**Agregado:**

* Actualizar la versión de requisitos de controlador AMD

**Corregido:**

* &lbrack;Mac M1&rbrack; Detección de memoria incorrecta
* &lbrack;Exportar&rbrack; Los trazados muy largos no se muestran correctamente

**Problemas conocidos:**

* &lbrack;Contenido&rbrack; Sombreadores obsoletos de las muestras

### 7.2.1

*(Lanzado: 02 de julio de 2021*)Resumen: **Versión secundaria, revisión**

**Agregado:**

* &lbrack;Interop&rbrack; Añada información sobre herramientas para indicar que el envío de proyectos de Mosaico de UV a Stager aún no se admite
* &lbrack;Complemento&rbrack;&lbrack;UI&rbrack; Actualización del icono de Livelink

**Corregido:**

* &lbrack;Nvidia&rbrack; La versión del controlador que comienza por 30 se considera obsoleta
* &lbrack;Bibliotecas&rbrack; El estado del panel Activos no se guarda a menos que esté abierto un proyecto
* &lbrack;Bibliotecas&rbrack; La nueva búsqueda guardada conserva la palabra clave de la antigua búsqueda guardada
* &lbrack;Bakeres&rbrack;&lbrack;UVTiles&rbrack; Los mapas de ID por meshID también tienen en cuenta los Mosaicos de UV
* &lbrack;Exportar&rbrack; Los archivos gLTF no importan el color del vértice
* &lbrack;Iray&rbrack; Faltan algunas sugerencias
* &lbrack;Interop&rbrack; Enviar a Stager no siempre está desactivado cuando no se detecta Stager
* &lbrack;Actualizador de recursos&rbrack; No se puede actualizar Photoshop Brushmaker
* &lbrack;Contenido&rbrack; El generador de desgaste de borde de fibra de vidrio está roto

### 7.2.0

*(Lanzado: 23 de junio de 2021*)Resumen: **Versión principal: proporciona una actualización del panel de recursos, un nuevo sombreador con acceso a nuevos canales y parámetros, una actualización general de la interfaz de usuario, algunas mejoras de rendimiento muy solicitadas, compatibilidad con más idiomas y mucho más.**

**Agregado:**

* &lbrack;Bibliotecas&rbrack; Nuevo panel Activos para sustituir el estante
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Nuevo diseño del panel Activos
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Cambiar la orientación y la interfaz de usuario predeterminadas del panel Activos
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Introducir una opción de vista de lista en la biblioteca
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Nueva navegación de rutas de navegación en el panel Activos
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Seleccionar &quot;Todas las bibliotecas&quot; al seleccionar una búsqueda guardada
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Seleccionar &quot;Todas las bibliotecas&quot; cuando se anula la selección de todas las carpetas
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Nueva etiqueta para pinceles de partículas
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Se ha reemplazado &quot;estantería&quot; por &quot;Todas las bibliotecas&quot; en la aplicación.
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Permitir ocultar carpetas vacías
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; La biblioteca de usuario predeterminada debe estar visible aunque esté vacía
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Nuevo método de filtrado mediante iconos de tipo de activo
* &lbrack;Bibliotecas&rbrack; Método abreviado &quot;CTRL&quot; para seleccionar varios tipos de recursos
* &lbrack;Bibliotecas&rbrack; Nueva variable de entorno para controlar el presupuesto de memoria de previsualización de recursos
* &lbrack;Bibliotecas&rbrack;&lbrack;Content&rbrack; Nuevos mapas de entorno
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack;&lbrack;UI&rbrack; Procesar desplazamiento en materiales predeterminados
* &lbrack;Bibliotecas&rbrack;&lbrack;Content&rbrack; Definir sombreador de Adobe Standard Material (ASM) como predeterminado para la generación de vistas previas
* &lbrack;Bibliotecas&rbrack;&lbrack;Contenido&rbrack;&lbrack;ASM&rbrack; Nuevas plantillas de proyecto para el nuevo sombreador de ASM
* &lbrack;Bibliotecas&rbrack;&lbrack;Miniatura&rbrack; Utilizar nuevo mapa de entorno de Studio 6
* &lbrack;Bibliotecas&rbrack;&lbrack;Miniatura&rbrack; Leer miniatura en el recurso en lugar de generarla
* &lbrack;Bibliotecas&rbrack;&lbrack;Miniatura&rbrack; Añadir desplazamiento a la generación de miniaturas
* &lbrack;Configuración del conjunto de texturas&rbrack;
* &lbrack;Configuración del conjunto de texturas&rbrack;&lbrack;UI&rbrack; Exponer el nuevo height al método de conversión normal
* &lbrack;Configuración del conjunto de texturas&rbrack;&lbrack;UI&rbrack; Repaso de la organización de la interfaz de usuario de los canales
* &lbrack;Configuración del conjunto de texturas&rbrack; Límite de canales de usuario aumentado a 16 canales
* &lbrack;Configuración del conjunto de texturas&rbrack;&lbrack;UI&rbrack; Indicar qué canales son compatibles con el sombreador seleccionado actualmente
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Nuevo sombreador de Adobe Standard Material
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Se ha agregado la compatibilidad con Anisotropía, capa transparente, dispersión subsuperficial, Specular edge color y brillo
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Cambiar los valores de color de los canales predeterminados
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack;&lbrack;Export&rbrack; Plantilla de exportación actualizada de Adobe Dimension a Adobe Substance 3D Stager
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Se han añadido rótulos y descripciones emergentes para los parámetros de sombreador y MDL
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Hacer visible el color de la Dispersión en vista 2D aunque no se admita SSS
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack;&lbrack;Iray&rbrack; Apoya al sombreador de ASM en Irak con el nuevo MDL
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack;&lbrack;Iray&rbrack; Dispersión subsuperficial actualizada en brillo y revestimiento de especificaciones PBR heredadas
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack;&lbrack;Content&rbrack; Se ha cambiado el tipo de SSS predeterminado para las muestras.
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Documentación añadida para la API de ASM
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Optimizar sombreadores para ignorar los canales no utilizados
* &lbrack;Sombreador&rbrack; Exponer nuevos canales de Conjunto de texturas
* &lbrack;Sombreador&rbrack; Dispersión subsuperficial mejorada
* &lbrack;Sombreador&rbrack; Parámetros de sombreador nuevos ocultos para algunos sombreadores
* &lbrack;Sombreador&rbrack; Visible si para los parámetros de sombreador
* &lbrack;Rendimiento&rbrack;
* &lbrack;Bibliotecas&rbrack; Mejoras en el tiempo de carga y el rendimiento del cálculo de la previsualización de recursos
* &lbrack;Motor&rbrack; Mejoras de rendimiento de pintura
* &lbrack;Auto Unwrap&rbrack;
* &lbrack;Auto Unwrap&rbrack; Mejoras de rendimiento de empaquetado
* &lbrack;Auto Unwrap&rbrack; Ajuste automático compatible con el flujo de trabajo de Mosaico de UV
* &lbrack;Desenvolvimiento automático&rbrack; Nueva opción para colocar las coordenadas UV según la orientación de la malla
* &lbrack;Otro&rbrack;
* &lbrack;Configuración&rbrack; Dirección de zoom predeterminada cambiada
* &lbrack;UI&rbrack; Actualización general de la IU
* &lbrack;UI&rbrack; Repaso del menú Ayuda
* &lbrack;UI&rbrack; Reemplazar icono de inversión
* &lbrack;UI&rbrack;&lbrack;Complemento&rbrack; Icono Reemplazar para el vínculo del complemento dcc
* &lbrack;UI&rbrack;&lbrack;AMD&rbrack; Actualizar la versión mínima requerida y el mensaje emergente
* &lbrack;Pila de capas&rbrack; Crear una nueva capa dentro de la carpeta vacía seleccionada
* Actualizar documentación de Python
* &lbrack;Marca&rbrack;
* &lbrack;Marca&rbrack;&lbrack;UI&rbrack; Nombre de la aplicación actualizado a Adobe Substance 3D Painter
* &lbrack;Marca&rbrack;&lbrack;UI&rbrack; Se ha actualizado la versión independiente a &#39;Edición de Substance&#39;.
* &lbrack;Marca&rbrack;&lbrack;UI&rbrack; Nombre del ejecutable de la aplicación, ruta de instalación, paquete e iconos actualizados
* &lbrack;Marca&rbrack;&lbrack;UI&rbrack; Ruta y biblioteca predeterminadas renombradas
* &lbrack;Marca&rbrack;&lbrack;UI&rbrack; Ventana Acerca de Actualizada
* &lbrack;Marca&rbrack;&lbrack;UI&rbrack; Pantalla de bienvenida actualizada
* &lbrack;Marca&rbrack;&lbrack;UI&rbrack; Se ha eliminado el número de versión basado en años
* &lbrack;Localización&rbrack; Nuevas traducciones al alemán, francés y chino simplificado
* &lbrack;Interoperabilidad&rbrack; No disponible para las ediciones Steam y Substance
* &lbrack;Interoperabilidad&rbrack; Interoperabilidad con el ecosistema de Adobe: Designer, Sampler, Stager y Bridge
* &lbrack;Interoperabilidad&rbrack;&lbrack;UI&rbrack; Recibir y actualizar recursos de Designer
* &lbrack;Interoperabilidad&rbrack;&lbrack;UI&rbrack; Recibir recursos de Sampler
* &lbrack;Interoperabilidad&rbrack;&lbrack;UI&rbrack; Enviar contenido a Stager
* &lbrack;Interoperabilidad&rbrack;&lbrack;UI&rbrack; Mostrar en Adobe Bridge
* &lbrack;Interoperabilidad&rbrack;&lbrack;UI&rbrack; Permitir el acceso rápido a Adobe 3D Assets
* &lbrack;Interoperabilidad&rbrack; Nuevas etiquetas de uso de sbsar
* &lbrack;Interoperabilidad&rbrack; Gestionar tipos de activos recibidos
* &lbrack;Interoperabilidad&rbrack; Los activos recibidos de Adobe Substance 3D Designer o Adobe Substance 3D Sampler se almacenan en la biblioteca seleccionada de forma predeterminada por el usuario
* &lbrack;Interoperabilidad&rbrack;&lbrack;UI&rbrack; Nuevo icono en la barra de herramientas de la izquierda para enviarlo a Stager o Photoshop

**Corregido:**

* &lbrack;Tablet&rbrack; Bajo rendimiento al pintar con presión
* &lbrack;Tablet&rbrack; Problema en tabletas con controles deslizantes
* &lbrack;Bloqueo&rbrack; El nombre no coincide entre la lista Conjunto de texturas y el Exportador
* &lbrack;Bloqueo&rbrack;&lbrack;Bibliotecas&rbrack; Doble clic en una subbiblioteca
* &lbrack;Bibliotecas&rbrack; Problema al rastrear directorios de la biblioteca
* &lbrack;Bibliotecas&rbrack; La línea de comandos de generación de previsualización forzada no funciona del modo esperado
* &lbrack;Bibliotecas&rbrack;&lbrack;Content&rbrack; El filtro Entorno de luz hecho un bake es negro de forma predeterminada
* &lbrack;Linux&rbrack;&lbrack;MacOS&rbrack;&lbrack;Exportar malla&rbrack; No se puede importar glTF creado en Linux/MacOS
* &lbrack;Linux&rbrack; Arrastrar y soltar un archivo en el panel Recursos puede provocar un bloqueo
* &lbrack;Desenvolvimiento automático&rbrack; El Desenvolvimiento automático está disponible incluso si no se ha seleccionado una malla para la recarga
* &lbrack;Partículas&rbrack; Comportamiento incorrecto de las partículas con la gravedad
* &lbrack;Pila de capas&rbrack; El histograma de niveles solo puede utilizar Luminancia con algunos canales
* &lbrack;Máscara de geometría&rbrack; El menú del botón derecho del ratón en una carpeta al editar la máscara de geometría no funciona
* &lbrack;Proyección&rbrack; Costura con proyección esférica y filtrado bilineal
* &lbrack;Mosaicos de UV&rbrack; Exportar máscara a archivo solo exporta el mosaico 0, 0
* &lbrack;Exportar malla&rbrack; FBX exportación de malla está vacía
* &lbrack;Iray&rbrack; El mapa de normales no se tiene en cuenta en los nuevos proyectos al procesar
* &lbrack;Guardar&rbrack; Guardar problemas en unidades compartidas
* &lbrack;Haciendo un bake&rbrack; Al volver a hornear una malla con parámetros modificados, se muestra una advertencia
* &lbrack;Haciendo un bake&rbrack;&lbrack;Regresión&rbrack; Resultado incorrecto cuando el cuadro delimitador global de mallas de poli altas no incluye el origen de la escena
* &lbrack;Python&rbrack; Las bibliotecas de usuario personalizadas no se tienen en cuenta

**Problemas conocidos:**

* &lbrack;Bibliotecas&rbrack; Las búsquedas guardadas no se guardan si no hay ningún proyecto abierto
* &lbrack;NVIDIA&rbrack; Mensaje para el controlador obsoleto incluso si el controlador está actualizado

### 7.1.1 (2021.1.1)

*(Lanzado: 23 de marzo de 2021*)Resumen: **Versión secundaria, corrección de errores con posibilidad de introducir valores hexadecimales en el selector de color**

**Agregado:**

* &lbrack;Registro&rbrack; Advertencia a los usuarios sobre los controladores de GPU AMD incompatibles
* &lbrack;Selector de color&rbrack; Permitir escribir valores hexadecimales

**Corregido:**

* &lbrack;Baker&rbrack; Disminución del rendimiento
* &lbrack;Máscara de geometría&rbrack; Alt clic en el nombre de la malla puede llevar a un bloqueo
* &lbrack;Motor&rbrack; La pintura no actualiza toda la vista cuando es necesario
* &lbrack;Pila de capas&rbrack; La selección se bloquea después de cambiar el sombreador
* &lbrack;MacOS&rbrack;&lbrack;Selector de color&rbrack; El color es ligeramente diferente del que se ha elegido
* &lbrack;Exportar&rbrack; El uso del formato de archivo PSD no genera un archivo por Mosaico de UV
* &lbrack;Scripting&rbrack;&lbrack;Javascript&rbrack; alg.mapexport.getPathsExportDocumentMaps() no devuelve todos los valores
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Los complementos deshabilitados se vuelven a habilitar al volver a abrir Painter

### 7.1.0 (2021.1.0)

*(Lanzado: 28 de enero de 2021*)Resumen: **Versión principal, nueva máscara de geometría que permite seleccionar y pintura partes de la geometría, copiar y pegar efectos en la pila de capas, mejorar el flujo de trabajo de Mosaico de UV, actualizar Iray, Bakeres, Substance Engine y nuevo contenido**

**Agregado:**

* Nueva máscara de geometría y pintura las partes seleccionadas de la geometría
* &lbrack;Máscara de geometría&rbrack; Permitir la pintura de las partes seleccionadas de la geometría por nombres de malla
* &lbrack;Máscara de geometría&rbrack; Selección rectangular en ambas ventanas gráficas
* &lbrack;Máscara de geometría&rbrack; Permitir ocultar/ignorar la geometría excluida en cualquier capa
* &lbrack;Máscara de geometría&rbrack;&lbrack;Propiedades&rbrack; Selección rápida de casillas de verificación al hacer clic y arrastrar
* &lbrack;Geometry Mask&rbrack;&lbrack;Properties&rbrack;&lbrack;UI&rbrack; Incluir/excluir todo con un menú desplegable en la ventana Propiedades
* &lbrack;Máscara de geometría&rbrack;&lbrack;Propiedades&rbrack; Permitir seleccionar rápidamente un elemento de una lista con ALT+CLIC IZQUIERDO
* &lbrack;Máscara de geometría&rbrack;&lbrack;Propiedades&rbrack; Superposición en las ventanas gráficas al pasar el cursor por los nombres/Mosaicos de UV de malla en la ventana Propiedades
* &lbrack;Máscara de geometría&rbrack;&lbrack;Pila de capas&rbrack; Añadir opciones de Copiar/Pegar a la máscara de geometría
* &lbrack;Máscara de geometría&rbrack; Icono Nuevo para el botón Ocultar/ignorar geometría excluida
* &lbrack;Máscara de geometría&rbrack; Nueva información sobre herramientas para Ocultar/ignorar geometría excluida
* &lbrack;Máscara de geometría&rbrack; Pulse el método abreviado del teclado ALT+H para activar o desactivar el botón &quot;ocultar y omitir geometría excluida&quot;
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Pila de capas&rbrack; Nueva miniatura de vista previa de la esfera de capa de relleno para Mosaicos de UV y modo simplificado
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Pila de capas&rbrack; Permitir salir fácilmente de la máscara de Mosaico de UV
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Lista de conjuntos de texturas&rbrack; Permitir dar una descripción por Mosaico de UV
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Configuración del conjunto de texturas&rbrack;&lbrack;UI&rbrack; Dos nuevos títulos de sección en el menú desplegable para cambiar la resolución de Mosaico de UV
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Viewport&rbrack; Salir de la máscara de Mosaico de UV al arrastrar un material a la ventana gráfica
* &lbrack;Pila de capas&rbrack; Añadir opciones de Copiar/Pegar para efectos
* &lbrack;Pila de capas&rbrack; Permitir copiar y pegar efectos de un conjunto de texturas a otro
* &lbrack;Pila de capas&rbrack; Permitir selección múltiple de efectos
* &lbrack;Pila de capas&rbrack; Añadir opciones de copiar/pegar como métodos abreviados para efectos de capa
* &lbrack;Pila de capas&rbrack; Cambiar automáticamente entre máscara y contenido al arrastrar efectos a otra capa
* &lbrack;Pila de capas&rbrack; Crear automáticamente una máscara al pegar una máscara de otra capa
* &lbrack;Pila de capas&rbrack; Añada acciones de mover efectos dentro del menú contextual del botón derecho de los efectos
* &lbrack;Pila de capas&rbrack; Permitir arrastrar y soltar efectos de una capa a otra
* &lbrack;Pila de capas&rbrack; Al arrastrar elementos a una carpeta, se colocan en la parte superior de la carpeta
* Actualizar Iray a la versión 2020.1.0
* &lbrack;Bakeres&rbrack; Actualizar Bakeres a la versión 2.5.4
* &lbrack;Bakeres&rbrack; Mostrar Mosaicos de UV individuales en la ventana de progreso de hacer un bake
* &lbrack;Bakeres&rbrack;&lbrack;UI&rbrack; Permite hacer un bake rápidamente el conjunto de texturas actual con un nuevo botón
* &lbrack;Bakeres&rbrack; Permitir al usuario seleccionar rápidamente uno de los bakeres con ALT+CLIC IZQUIERDO
* Actualizar Substance Engine a la versión 8.0.8
* &lbrack;Substance Engine&rbrack; Compatibilidad con el color predeterminado en los nuevos archivos .sbsar
* &lbrack;Auto Unwrap&rbrack; Mejora del rendimiento
* &lbrack;Exportar&rbrack; Agregue comentarios visuales para indicar qué resolución de Mosaico de UV difiere de la predeterminada del proyecto
* &lbrack;Exportar&rbrack; Añadir un factor de tamaño de escena al archivo json de sombreador exportado
* &lbrack;Idioma&rbrack; Añadir traducción al japonés
* &lbrack;UI&rbrack; Ventana Actualizar Acerca de con control de versiones de dependencias internas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir la administración de recursos de Shelf
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir saber cuándo un proyecto está listo para hacer un bake y exportar
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir saber cuándo un recurso de plataforma ha terminado de rastrear recursos en el disco
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir consultar la lista de mosaicos UV por conjuntos de texturas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir la asignación de previsualizaciones personalizadas a recursos de estante
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir la gestión de estantes personalizados
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Agregue un índice de método en cada submódulo de la documentación
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Nuevo estilo para la documentación
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Mejora de los recursos y documentación de la estantería
* &lbrack;Contenido&rbrack; Tres nuevos ajustes preestablecidos de herramientas para realizar puntos de sutura
* &lbrack;Shelf&rbrack; Eliminar temporalmente &quot;Exportar a Substance share&quot; al realizar la transición a la nueva plataforma de Substance share

**Corregido:**

* Bloqueo al utilizar monitores con diferentes resoluciones
* Bloqueo en Substance Engine con algunos proyectos raros
* La actualización de la ventana gráfica falla con Ocultar/Ignorar geometría excluida al cambiar de capa
* &lbrack;vista 2D&rbrack; La ventana gráfica 2D puede faltar en algunos proyectos
* &lbrack;Haciendo un bake&rbrack; &quot;Coincidir por nombre de malla&quot; ignora partes del objeto
* &lbrack;Pila de capas&rbrack; Hacer clic en un efecto de capa abre una carpeta
* &lbrack;Máscara de geometría&rbrack; El Mosaico de UV se sigue contando en la máscara incluso al volver a importar la malla sin ella
* &lbrack;Máscara de geometría&rbrack; El menú del botón derecho del ratón en la ventana gráfica no proporciona las herramientas correctas
* &lbrack;Motor&rbrack; Grandes retrasos en proyectos concretos
* &lbrack;Secuencias de comandos&rbrack; Alta latencia con solicitudes de POST JSON remoto en Windows
* &lbrack;Linux&rbrack; La cantidad de Vram no se detecta correctamente con GPU integradas específicas
* &lbrack;Auto Unwrap&rbrack; Bloqueos o desajuste prolongado en algunos proyectos

## Versión 6

### 6.2.2 (2020.2.2)

*(Lanzado: 28 de septiembre de 2020*)Resumen: **Versión secundaria, corrección de errores con algunas funciones en la API de Python**

**Agregado:**

* &lbrack;Rendimiento&rbrack; No compute todos los Mosaicos de UV cuando utilice la selección de ID de color
* &lbrack;Bakeres&rbrack;&lbrack;UI&rbrack; Visualización de descripciones de conjuntos de texturas
* &lbrack;Bakeres&rbrack; Permitir guardar hacer un bake configuración
* &lbrack;Bakeres&rbrack; Añadir opciones de contraer todo/expandir todo a la pestaña Selección
* &lbrack;Lista de conjuntos de texturas&rbrack; Ocultar descripción cuando esté vacía
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Lista de conjuntos de texturas&rbrack; Hacer clic en el Mosaico de UV debe expandir/contraer la lista
* &lbrack;Export&rbrack;&lbrack;UI&rbrack; Permitir cambiar el tamaño horizontal del panel Lista de conjuntos de texturas
* &lbrack;Export&rbrack;&lbrack;UI&rbrack; Texto de información sobre herramientas coherente para el flujo de trabajo de Mosaicos de UV y Conjunto de texturas con texturas no seleccionadas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir el uso de ajustes preestablecidos de exportación para exportar texturas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Añadir un registro de cambios en la documentación
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir consultar todos los canales disponibles en una pila determinada
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Mejoras de IU de consola

**Corregido:**

* &lbrack;AMD&rbrack; Detección incorrecta de una versión obsoleta del controlador
* Bloqueo al volver a importar una malla con un diseño de Mosaicos de UV diferente en algunos casos
* Bloqueo al utilizar partículas con UDIM en mallas muy pesadas
* &lbrack;Mosaicos de UV&rbrack; Bloqueo al exportar una malla con información de desplazamiento en algunos casos
* &lbrack;Export&rbrack;&lbrack;Bloqueo&rbrack; Exportar Vista 2D en formato psd puede causar un bloqueo
* Importar imágenes como secuencias al crear un proyecto no funciona
* Motor atascado en un bucle infinito
* &lbrack;Método abreviado&rbrack; La cámara gira siempre en modo de ajuste al cambiar los métodos abreviados de modo de ajuste
* Las mallas siempre se desenvuelven automáticamente cuando se vuelven a importar aunque la opción esté desactivada
* &lbrack;Lista de conjuntos de texturas&rbrack; El campo de texto de descripción a veces no está completamente visible durante la edición
* &lbrack;Lista de conjuntos de texturas&rbrack; El menú desplegable para ocultar/mostrar conjuntos de texturas no está completamente visible
* &lbrack;Lista de conjuntos de texturas&rbrack; Al hacer clic en el icono del ojo no se debe introducir el nombre &quot;Editar conjunto de texturas&quot;
* &lbrack;Configuración del conjunto de texturas&rbrack; Al quitar un canal, también se elimina el canal siguiente
* &lbrack;Exportar&rbrack; Incluir todo y Restablecer todo no tiene en cuenta los Mosaicos de UV
* &lbrack;Bakeres&rbrack; Aparecen bakeres no seleccionados durante el proceso de hacer un bake
* La actualización de la resolución no se tiene en cuenta para los mapas con bake utilizados como entrada
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Viewport&rbrack; Bloqueo de la ventana gráfica 3D al añadir Material inteligente tras carpeta con la máscara de Mosaico de UV seleccionada
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Viewport&rbrack; La malla metálica sigue siendo visible para los mosaicos ocultos con el modo de pintura directa
* &lbrack;Export&rbrack;&lbrack;Sketchfab&rbrack; Problemas con el tipo de suscripción &quot;más&quot;
* &lbrack;Sketchfab&rbrack; La casilla &quot;Este recurso es privado&quot; no se muestra después de cambiar de cuenta
* &lbrack;Export&rbrack;&lbrack;Content&rbrack; Los ajustes preestablecidos de pincel &quot;ondulado&quot; pueden provocar problemas de rendimiento
* &lbrack;Complemento Photoshop&rbrack; Mensaje en el registro: no compatible con el flujo de trabajo de Mosaico de UV
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; PYTHONPATH env var impide que se inicie la aplicación
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Error tipográfico en la documentación de Python

### 6.2.1 (2020.2.1)

*(Lanzado: 29 de julio de 2020*)Resumen: **Versión secundaria, revisión**

**Agregado:**

* Añada la variable de entorno &quot;SUBSTANCE_PAINTER_VRAM_BUDGET&quot; para anular la cantidad de RVam de la GPU
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Rendimiento&rbrack; No calcular todos los mosaicos UV al utilizar la herramienta Relleno poligonal

**Corregido:**

* &lbrack;Iray&rbrack; Guardar renderizado devuelve un error que produce una imagen en negro
* &lbrack;Linux&rbrack; Bloqueo después de la pantalla de bienvenida en CentOS 7.3
* &lbrack;Linux&rbrack; La cantidad de Vram no se detecta correctamente con configuraciones específicas
* &lbrack;Bloqueo&rbrack; Apertura de un proyecto con el nombre de un conjunto de texturas duplicado
* &lbrack;Motor&rbrack; Problema de invalidación de caché al modificar una máscara
* &lbrack;Lista de conjuntos de texturas&rbrack; Efecto de fuente incorrecto cuando el conjunto de texturas está desactivado

**Problemas conocidos:**

* &lbrack;Lista de conjuntos de texturas&rbrack; No se puede ocultar la descripción
* &lbrack;Lista de conjuntos de texturas&rbrack; Problemas de IU
* &lbrack;Iray&rbrack; El procesamiento del PSD no se abre
* &lbrack;Complemento Photoshop&rbrack; No compatible con el flujo de trabajo de Mosaicos de UV

### 6.2.0 (2020.2.0)

*(Lanzado: 23 de julio de 2020*)Resumen: **Versión principal con nuevo flujo de trabajo de Mosaicos de UV, pintura entre Mosaicos de UV y mejora del rendimiento**

**Agregado:**

* Mosaicos de UV (UDIM)
* &lbrack;Mosaicos de UV&rbrack; Pintura en mosaicos UV
* &lbrack;Mosaicos de UV&rbrack; Permitir elegir entre el flujo de trabajo nuevo y el heredado para Mosaicos de UV
* &lbrack;Mosaicos de UV&rbrack; Importación de secuencias de imágenes de UDIM/Mosaicos de UV como recurso
* &lbrack;Mosaicos de UV&rbrack; Añadir lista de Mosaicos de UV por conjunto de texturas en la ventana Lista de conjuntos de texturas
* &lbrack;Mosaicos de UV&rbrack; Permita editar la resolución de varios Mosaicos de UV a la vez en Configuración del conjunto de texturas
* &lbrack;Mosaicos de UV&rbrack;&lbrack;vista 2D&rbrack; Visualización de Mosaicos de UV como una cuadrícula
* &lbrack;Mosaicos de UV&rbrack;&lbrack;vista 2D&rbrack; Nuevo botón de ventanilla para mostrar u ocultar información de Mosaicos de UV
* &lbrack;Mosaicos de UV&rbrack; Cambiar la herramienta de pintura a un solo canal de forma predeterminada para proyectos de Mosaico de UV
* &lbrack;Mosaicos de UV&rbrack; Botón Nuevo en la barra de herramientas contextual para ignorar los Mosaicos de UV enmascarados mientras se pinta
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Pila de capas&rbrack; Nuevos iconos de pila de capas para mejorar el rendimiento
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Pila de capas&rbrack; Mejorar los iconos de Pintura y relleno en la barra de herramientas
* &lbrack;Máscara de Mosaico de UV&rbrack;&lbrack;vista 2D&rbrack; Permitir incluir o excluir varios Mosaicos de UV a la vez (clic izquierdo, CTRL+clic izquierdo)
* &lbrack;Máscara de Mosaico de UV&rbrack; Nueva máscara de Mosaico de UV para incluir, excluir azulejos por capa con un nuevo icono
* &lbrack;Máscara de Mosaico de UV&rbrack;&lbrack;Pila de capas&rbrack; Mostrar el número de Mosaicos de UV en el icono de máscara de Mosaicos de UV cuando no se incluyen todos
* &lbrack;Máscara de Mosaico de UV&rbrack;&lbrack;2D/Vista 3D&rbrack; Añade el efecto de pasar el cursor para visualizar los Mosaicos de UV bajo el cursor
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Bakeres&rbrack; Permitir seleccionar y hacer un bake Mosaicos de UV específicos
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Bakeres&rbrack; Añadir opciones de selección para conjuntos de texturas/Mosaicos de UV
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Bakeres&rbrack; Opción de menú del botón derecho para seleccionar Mosaicos de UV dentro de un conjunto de texturas
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Bakeres&rbrack; Permitir una selección rápida en el conjunto de texturas/Mosaicos de UV arrastrando
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Bakeres&rbrack; Reemplace los botones &quot;Todo&quot; y &quot;Ninguno&quot; en Mapas de malla por opciones de selección más explícitas
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Bakeres&rbrack; Mostrar el número de texturas que se harán un bake
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Exportar&rbrack; Permitir la selección y exportación de Mosaicos de UV específicos
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Exportar&rbrack; Permitir una selección rápida de Mosaicos de UV arrastrando
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Exportar&rbrack; Añadir opciones del menú desplegable para Mosaicos de UV
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Exportar&rbrack; Hacer que algunos ajustes preestablecidos de exportación no estén disponibles si no funcionan con Mosaicos de UV (Adobe Dimension, Sketchfab, glTF, USD)
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Contenido&rbrack; Actualice los ajustes preestablecidos de exportación para utilizar la nueva etiqueta $udim
* &lbrack;Mosaicos de UV&rbrack; Mejora de los informes de errores al importar mallas con Islas de UV superpuestas
* &lbrack;Mosaicos de UV&rbrack; Mosaicos de UV compatibles en Irak
* &lbrack;Mosaicos de UV&rbrack;&lbrack;Scripting&rbrack; Añadir documentación de exportación de Mosaico de UV a la documentación de Python
* Rendimiento
* &lbrack;Rendimiento&rbrack; Botón Nuevo en la barra de herramientas contextual para pausar el cálculo del motor al trabajar (MAYÚS+ESC)
* &lbrack;Rendimiento&rbrack; Apertura de proyectos más rápida al retrasar el cálculo de la caché del conjunto de texturas
* &lbrack;Rendimiento&rbrack; No espere a que se carguen los mapas de malla al abrir el proyecto
* &lbrack;Rendimiento&rbrack;&lbrack;2D/Vista 3D&rbrack; No calcular el canal de máscara en la ventana gráfica cuando no se utiliza
* &lbrack;Rendimiento&rbrack; No bloquee la aplicación al cargar los mapas de malla mostrados en las ventanas gráficas
* &lbrack;Rendimiento&rbrack; Mejorar la velocidad de guardado incremental al guardar un proyecto
* &lbrack;Rendimiento&rbrack;&lbrack;Bakeres&rbrack; Cambiar la configuración de dilatación predeterminada para mejorar el ahorro de tiempo y el tamaño del proyecto
* &lbrack;Rendimiento&rbrack;&lbrack;Bakeres&rbrack; Cambiar a escala de grises en Bakeres específicos para mejorar el ahorro de tiempo y el tamaño del proyecto
* &lbrack;Rendimiento&rbrack;&lbrack;Exportar&rbrack; Mejorar el rendimiento del motor para exportar texturas más rápido
* &lbrack;Rendimiento&rbrack;&lbrack;Exportar&rbrack; Mejorar la capacidad de respuesta al abrir el cuadro de diálogo de exportación con muchos conjuntos de texturas
* &lbrack;Rendimiento&rbrack;&lbrack;Exportar&rbrack; Mejorar el rendimiento al cambiar a la pestaña &quot;Lista de exportaciones&quot;
* &lbrack;Performance&rbrack;&lbrack;Iray&rbrack; Reducir el tiempo de arranque de Iray
* Otro
* &lbrack;Bakeres&rbrack; Añadir opciones de selección para conjuntos de texturas
* Mover la administración de instancias del sombreador a la configuración del conjunto de texturas
* &lbrack;2D/Vista 3D&rbrack; Añada un mensaje en la parte inferior de la ventana gráfica para indicar qué tipo de máscara se ha editado
* &lbrack;Pila de capas&rbrack; Nueva opción en la configuración para cambiar entre las miniaturas antiguas y nuevas
* &lbrack;Pila de capas&rbrack; Añada comentarios visuales para indicar el estado de carga de las miniaturas
* &lbrack;Proj&rbrack; Nuevo modo de proyección &quot;Fill (Match Per UV-Tile)&quot; para cargar secuencias de imágenes
* &lbrack;Proj&rbrack; Cambie el modo de proyección de capas de relleno a &quot;Rellenar (coincidencia por azulejo UV)&quot; en casos específicos
* &lbrack;Contenido&rbrack; Optimizar ajustes preestablecidos de pincel de carboncillo para mejorar el rendimiento
* Actualizar Iray a la versión 2020.0.0
* &lbrack;Exportar&rbrack; Desactivar la ficha Lista de exportaciones cuando no hay nada seleccionado
* Desempaquetado automático
* &lbrack;Auto Unwrap&rbrack; Mejorar la tasa de éxito del proceso de desempaquetado automático
* &lbrack;Auto Unwrap&rbrack; Parametrización mejorada para aumentar la velocidad y la estabilidad

**Corregido:**

* &lbrack;Alembic&rbrack; Las facetas se omiten al importar archivos
* &lbrack;Alembic&rbrack; Tiempo de carga infinito con archivos específicos
* &lbrack;Importar&rbrack; La secuencia de imágenes de UDIM incorrecta se importa cuando solo difiere la extensión del archivo
* &lbrack;Bloqueo&rbrack; Al intentar abrir un proyecto bloqueado por otro proceso, se produce un bloqueo
* &lbrack;Proyección&rbrack; Artefactos en malla duplicada al utilizar proyección triplanar
* &lbrack;Exportar&rbrack; El canal de emisivo no se exporta con USD formato
* &lbrack;Contenido&rbrack; Material inteligente &quot;Carboncillo&quot; contiene trazos de pintura

**Problemas conocidos:**

* &lbrack;Lista de conjuntos de texturas&rbrack; No se puede ocultar la descripción
* &lbrack;Lista de conjuntos de texturas&rbrack; Problemas de IU

### 6.1.3 (2020.1.3)

*(Lanzado: 16 de junio de 2020*)Resumen: **Corrección de error**

**Agregado:**

* &lbrack;Exportar&rbrack; Agregar configuración de desplazamiento en el archivo json de parámetros de Sombreador

**Corregido:**

* &lbrack;Bloqueo&rbrack;&lbrack;Motor&rbrack; Bloqueo al intentar borrar y reemplazar canales existentes
* &lbrack;Bloqueo&rbrack; Cambio del sombreador después de pintar una máscara en capas de material
* &lbrack;Bloqueo&rbrack;&lbrack;Motor&rbrack; Bloqueos con algunos proyectos pesados
* &lbrack;Bakeres&rbrack; La coincidencia por nombre no funciona con OBJ exportadas desde zBrush
* &lbrack;Desplazamiento&rbrack;&lbrack;SVT&rbrack; Las texturas no se muestran al abrir el proyecto cuando el desplazamiento está activado
* &lbrack;Exportar&rbrack; Algunas texturas se exportan en gris uniforme
* &lbrack;Exportar&rbrack; Los conjuntos de texturas desactivados no se deben exportar para los ajustes preestablecidos de exportación de Dimension y Sketchfab
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Bloqueo al utilizar la API JavaScript para acceder a la configuración de exportación en el evento onProjectOpened
* &lbrack;Scripting&rbrack;&lbrack;Javascript&rbrack; no se llama a onExportFinished() después de una exportación

### 6.1.2 (2020.1.2)

*(Lanzado: 28 de mayo de 2020*)Resumen: **Corrección de error con Substance Engine y actualización de Bakeres**

**Agregado:**

* &lbrack;Bakeres&rbrack; Actualizar a la versión más reciente
* &lbrack;Bakeres&rbrack; Nuevo método de muestreo en bakeres de Oclusión ambiental, curvatura y Thickness
* Actualizar a la versión más reciente de Substance Engine
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir la creación de ResourceID para los recursos del proyecto
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir consultar información del canal
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Añadir funciones de ejecución en seco y devolución de llamada para simular la exportación de textura

**Corregido:**

* &lbrack;Bakeres&rbrack; Normales incorrectas en el baker World Space Normals utilizando un Mapa de normales tangente en casos específicos
* &lbrack;Bakeres&rbrack; Error al hacer un bake la Oclusión ambiental con Optix cuando no hay poli alta
* &lbrack;Trazos dinámicos&rbrack; Retraso al cargar un conjunto de texturas específico
* &lbrack;Exportar&rbrack; No se deben exportar los conjuntos de texturas desactivados para USD, glTF
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; No se puede editar la nueva configuración del baker de curvatura
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; alg.texturesets.addChannel() no devuelve un error en algunos casos
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Error tipográfico en la documentación de la API de Javascript para setProjectExportOptions()
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Exporta siempre todos los conjuntos de texturas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; sys.ejecutable devuelve una ruta de acceso a python.exe en lugar de a Substance Painter
* La caché de textura no es compatible en los sistemas operativos Mac y Windows/Linux
* &lbrack;Livelink UE4&rbrack; Solo se utiliza el último material para todos los conjuntos de texturas en una malla combinada

**Problemas conocidos:**

* &lbrack;Export&rbrack;&lbrack;Dimension&rbrack;&lbrack;Skecthfab&rbrack; No se deben exportar los conjuntos de texturas desactivados
* &lbrack;Bloqueo&rbrack; Cambiar el sombreador después de haber pintado una máscara en capas de material

### 6.1.1 (2020.1.1)

*(Lanzado: 5 de mayo de 2020*)Resumen: **Revisión**

**Agregado:**

* &lbrack;Exportar&rbrack; Comentarios visuales de estado anulado en TextureSet

**Corregido:**

* &lbrack;Exportar&rbrack; El tamaño de la ventana del exportador es demasiado grande en un monitor con resolución especial y no se puede cambiar de tamaño
* &lbrack;Exportar&rbrack; Las opciones no se guardan después de la exportación
* &lbrack;Exportar&rbrack; Bloqueo o no se puede exportar con el ajuste preestablecido exportar &quot;desde caché&quot;
* &lbrack;Exportar&rbrack; Cancelar la exportación genera un mapa vacío adicional inesperado
* &lbrack;Exportar&rbrack; Corregir ajustes preestablecidos de exportación virtual
* &lbrack;Python&rbrack; PYTHONPATH env var no se tiene en cuenta
* &lbrack;Python&rbrack;&lbrack;Exportar&rbrack; Si se cancela la exportación mediante Python, se devuelve un error de excepción
* &lbrack;Python&rbrack;&lbrack;Exportar&rbrack; export_project_texturas resultado incorrecto con formato de archivo psd
* &lbrack;Bakeres&rbrack; Bloqueo en Linux con Trazado de rayos de GPU

**Problemas conocidos:**

* &lbrack;JavaScript&rbrack; No se puede editar la nueva configuración del baker de curvatura
* &lbrack;JavaScript&rbrack;&lbrack;Exportar&rbrack; Exporta siempre todos los conjuntos de texturas
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; No se deben exportar los conjuntos de texturas desactivados
* &lbrack;Bloqueo&rbrack; Cambiar el sombreador después de haber pintado una máscara en capas de material

### 6.1.0 (2020.1.0)

*(Lanzado: 22 de abril de 2020*)Resumen: **Versión principal con nueva textura y exportador de malla (con desplazamiento y teselación), desempaquetado UV actualizado con más controles, nuevos bakeres, nueva API python de scripts, mejor experiencia de usuario para la proyección de pegatinas y nuevo contenido**

**Agregado:**

* Nueva textura y exportador de malla
* &lbrack;Exportar&rbrack; Nueva interfaz de exportador
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Permitir la selección de los canales de mapas que se exportan por conjunto de texturas
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Permitir la modificación del tamaño del conjunto de texturas para todos los conjuntos de texturas en una sola acción
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Permitir una plantilla diferente por conjunto de texturas (excepto para USD, glTF, Sketchfab y Dimension)
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Activación y desactivación rápidas de mapas y conjuntos de texturas
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; La resolución de exportación 8192x8192 ya no es experimental
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Permitir la modificación del formato de archivo y la profundidad de bits por mapa
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Permitir restablecer los valores de los parámetros predeterminados
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Permitir que la configuración se guarde sin exportar
* &lbrack;Exportar&rbrack;&lbrack;Plantillas de salida tab&rbrack; Cambie el nombre de la pestaña &quot;Configuración&quot; a la pestaña &quot;Plantillas de salida&quot;
* &lbrack;Exportar&rbrack;&lbrack;Plantillas de salida tab&rbrack; Permitir la definición del formato de archivo y la profundidad de bits por mapa preestablecido
* &lbrack;Exportar&rbrack;&lbrack;Lista de pestañas de exportaciones&rbrack; Nueva pestaña de vista previa para resumir y ver el proceso de exportación
* &lbrack;Importar/Exportar malla&rbrack; Optimización del rendimiento de tiempo de importación/exportación
* &lbrack;Exportar malla&rbrack; Exportar malla en FBX
* &lbrack;Exportar malla&rbrack; Exportar malla con desplazamiento y teselación
* &lbrack;Exportar malla&rbrack;&lbrack;UI&rbrack; Nuevos ajustes para volver a calcular el vértice normal, aplicar triangulación
* &lbrack;Exportar malla&rbrack; Exportar topología de malla original con nuevas UV generadas por el desajuste automático
* Se ha actualizado el desajuste automático de UV con más controles
* &lbrack;Desempaquetado UV&rbrack;&lbrack;UI&rbrack; Añadir configuración para activar el desajuste automático de UV en la ventana de nuevo proyecto
* &lbrack;Desempaquetado UV&rbrack;&lbrack;UI&rbrack; Nuevas opciones para controlar los pasos de desenvolvimiento (costuras, desenvolvimiento, empaquetado)
* &lbrack;Desempaquetado UV&rbrack;&lbrack;UI&rbrack; Permitir la conservación de las costuras de desenrollado/desenrollado/empaquetado existentes
* &lbrack;Desempaquetado UV&rbrack;&lbrack;UI&rbrack; Nuevas opciones para volver a calcular por completo los pasos de desajuste
* &lbrack;Desempaquetado UV&rbrack;&lbrack;UI&rbrack; Nueva opción para controlar el tamaño del margen (ninguno, pequeño, mediano y grande)
* Nuevos Bakeres
* &lbrack;Bakeres&rbrack; Sustituir la curvatura antigua por la nueva curvatura de la malla
* &lbrack;Bakeres&rbrack; Opción Añadir coincidencia por nombre para ignorar la cara posterior en el baker &quot;Oclusión ambiental&quot;
* &lbrack;Bakeres&rbrack; Opción Añadir plano de tierra en el baker &quot;Oclusión ambiental&quot;
* Nueva API de Python de scripts (3.7.6)
* &lbrack;Python&rbrack;&lbrack;UI&rbrack; Nuevo menú de scripts para Python
* &lbrack;Python&rbrack;&lbrack;UI&rbrack; Nueva documentación de Python en el menú Ayuda
* &lbrack;Python&rbrack; Exponga los módulos python de Substance Painter: substance_painter, alg, display, project.setting, project, texturesets, ui
* &lbrack;Python&rbrack; Exponer el nuevo módulo Python &quot;substance_painter&quot;
* &lbrack;Python&rbrack; Exponer nuevo submódulo de Python: alg, display, log, project, resource, texturesets, ui
* &lbrack;Python&rbrack; Listener para cambios de proyecto
* &lbrack;Python&rbrack; Nuevos ejemplos en la documentación de Python
* &lbrack;JavaScript&rbrack;&lbrack;UI&rbrack; Menú de complementos reemplazado por JavaScript
* &lbrack;Viewport&rbrack; Permitir la creación de una proyección de pegatinas &quot;arrastrando/soltando + ALT&quot; de un recurso desde la estantería
* Nuevo contenido
* &lbrack;Contenido&rbrack; 5 nuevos materiales de pegatina de Substance Source
* &lbrack;Contenido&rbrack; Añadir nuevas plantillas de proyecto y exportar ajustes preestablecidos para el procesador de Maxwell
* &lbrack;Contenido&rbrack; Agregar plantilla de proyecto para la exportación de Keyshot 9
* &lbrack;Contenido&rbrack; Actualizar el ajuste preestablecido de exportación de Keyshot 9 para admitir desplazamiento y emisivo
* &lbrack;Content&rbrack;&lbrack;Exportador&rbrack; Actualización de todos los ajustes preestablecidos de exportación para que coincidan con las últimas versiones de motores de juegos y procesadores
* &lbrack;Content&rbrack;&lbrack;Exportador&rbrack; Actualice los archivos de ajustes preestablecidos de exportación para utilizar nuevos ajustes de tramado y formato
* &lbrack;Contenido&rbrack; Nuevas plantillas y sombreadores para admitir material de VRay (VRayMtl)
* &lbrack;Pila de capas&rbrack; Permitir la eliminación de efectos de capa mediante el icono de la papelera o el método abreviado del teclado Eliminar
* Eliminar el Substance Source de plugins (utilizar el iniciador con la funcionalidad &quot;enviar a&quot;)
* &lbrack;Windows&rbrack; No mostrar la advertencia de TDR en las GPU de gama alta

**Corregido:**

* Problemas de traducción en el cuadro de diálogo Nuevo archivo de proyecto
* &lbrack;Bakeres&rbrack; La opción &quot;Guardar archivo de escena preprocesado&quot; ya no funciona
* &lbrack;Proyección Plana&rbrack; La proyección no funciona en mallas con UV repetidos
* &lbrack;Decal&rbrack; Diferencia de comportamiento en el canal normal al utilizar distintos modos de proyección de la capa de relleno
* &lbrack;Difuminado&rbrack;&lbrack;Clonar&rbrack; Pueden aparecer artefactos al pintar con máscaras
* &lbrack;Motor&rbrack; Bloqueo con contenido de capas específico
* &lbrack;Motor&rbrack; Bloqueo aleatorio al pintar en algunos casos
* &lbrack;Punto de ancla&rbrack; La referencia a una máscara vacía siempre devuelve blanco
* &lbrack;Exportar&rbrack; Capa que no se tiene en cuenta en algunas configuraciones de pila concretas
* &lbrack;Exportar malla&rbrack; No se puede exportar con una ruta que contiene caracteres especiales
* &lbrack;Exportar malla&rbrack; No se pueden leer archivos glTF cuando se exportan desde Linux o MacOS
* &lbrack;Importar mesh&rbrack; La reimportación de DAE, PLY o glTF no funciona según lo previsto

**Problemas conocidos:**

* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; No se puede editar la nueva configuración del baker de curvatura
* &lbrack;Bakeres&rbrack; Bloqueo en Linux con Trazado de rayos de GPU
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; No se deben exportar los conjuntos de texturas desactivados
* &lbrack;Bloqueo&rbrack; Cambiar el sombreador después de haber pintado una máscara en capas de material

## Versión 5

### 5.3.3 (2019.3.3)

*(Lanzado: 06 de febrero de 2020*)Resumen: **Corrección de error con actualización a Iray 2019.3**

**Agregado:**

* Actualización a Irak 2019.3
* &lbrack;Registro&rbrack; Indicar bios obsoletos para la CPU Ryzen que conducen al bloqueo durante el hago un bake
* &lbrack;ABR&rbrack; Extraer alfa ABR a la estantería

**Corregido:**

* &lbrack;Baker&rbrack; Hacer un bake error si la malla de alta densidad no tiene UV
* &lbrack;Linux&rbrack; Los métodos abreviados de ratón personalizados no se guardan
* &lbrack;Brush&rbrack; El contorno desaparece con algunas formas alfa
* &lbrack;Tablet&rbrack; Detección incorrecta al mover los reguladores
* &lbrack;Atajos&rbrack; No se puede configurar ningún método abreviado con &quot;Ctrl+Alt+MouseClick&quot;
* &lbrack;Shelf&rbrack; No se puede ver información sobre herramientas de recursos al utilizar una tableta con lápiz
* &lbrack;vista 2D&rbrack;&lbrack;Exportar&rbrack; El ajuste preestablecido de vista 2D no tiene en cuenta la información normal
* Bloqueo al pintar en alineación UV con determinados pinceles
* Pintar bajo un filtro crea artefactos en el trazo en curso
* &lbrack;Viewport&rbrack; Caché de textura incorrecta en la ventana gráfica después de volver a importar una malla
* &lbrack;Bloqueo&rbrack; Error al guardar después de exportar a Photoshop
* &lbrack;Bloqueo&rbrack; Escribir símbolos especiales en el prefijo al importar recursos
* &lbrack;Bloqueo&rbrack; Haga clic en la referencia en Propiedades del punto de ancla
* &lbrack;Puntos de ancla&rbrack; El canal no se actualiza cuando hay un filtro entre el punto de anclaje y la referencia
* El vínculo de la URL de Iray en el menú Ayuda no funciona

**Problemas conocidos:**

* &lbrack;Desempaquetado UV&rbrack; El procesamiento de mallas de alta polietileno puede tardar mucho tiempo
* &lbrack;Desempaquetado UV&rbrack; Los vértices en las mismas coordenadas exactas se combinan
* &lbrack;Desempaquetado UV&rbrack; La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* &lbrack;Desempaquetado UV&rbrack; Proporción de texel no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* &lbrack;Desempaquetado UV&rbrack; Proporción de textura no uniforme entre conjuntos de texturas
* &lbrack;Desempaquetado UV&rbrack; La isla de UV generada puede ser muy alargada y no encajar en el espacio UV en algunos casos
* &lbrack;Desempaquetado UV&rbrack; Es posible que las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no se desenvuelvan con UV

### 5.3.2 (2019.3.2)

*(Lanzado: 21 de enero de 2020*)Resumen: **Corrección de error**

**Corregido:**

* Al abrir un proyecto guardado en el modo de canal solo, no se muestra la malla
* La ventana gráfica no siempre se actualiza al pintar en una capa con la herramienta de clonación

**Problemas conocidos:**

* &lbrack;Bakeres&rbrack; Bloqueo relacionado con el subprocesamiento múltiple en CPU Ryzen
* &lbrack;Desempaquetado UV&rbrack; El procesamiento de mallas de alta polietileno puede tardar mucho tiempo
* &lbrack;Desempaquetado UV&rbrack; Los vértices en las mismas coordenadas exactas se combinan
* &lbrack;Desempaquetado UV&rbrack; La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* &lbrack;Desempaquetado UV&rbrack; Proporción de texel no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* &lbrack;Desempaquetado UV&rbrack; Proporción de textura no uniforme entre conjuntos de texturas
* &lbrack;Desempaquetado UV&rbrack; La isla de UV generada puede ser muy alargada y no encajar en el espacio UV en algunos casos
* &lbrack;Desempaquetado UV&rbrack; Es posible que las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no se desenvuelvan con UV

### 5.3.1 (2019.3.1)

*(Lanzado: 20 de diciembre de 2019*)Resumen: **Revisión**

**Corregido:**

* Bloqueo al trabajar en mallas con Proyecciones de UV específicas
* &lbrack;ABR&rbrack; Bloqueo al cambiar entre ajustes preestablecidos de Photoshop
* &lbrack;Linux&rbrack; No se puede iniciar el Substance Painter en CentOS 7.4 debido a un problema de dependencia de libGLX
* &lbrack;Bakeres&rbrack; Bloqueo al hacer un bake después de utilizar Archivo > Limpiar
* &lbrack;Bakeres&rbrack; Hacer un bake el cuadro de diálogo de progreso inmovilizar después de cancelar
* &lbrack;Bakeres&rbrack; Hacer un bake malla después de exportar texturas no funciona
* &lbrack;Bakeres&rbrack; El uso de resultados &quot;Coincidir por nombre&quot; con mapas de malla negros
* &lbrack;Bakeres&rbrack; La jaula no se tiene en cuenta
* &lbrack;Shelf&rbrack; La importación de archivos de PSD genera imágenes rotas
* &lbrack;Ejemplo&rbrack; El proyecto de muestra &quot;Mat&quot; tiene cámaras rotas y un ajuste preestablecido de exportación incorrecto

**Problemas conocidos:**

* &lbrack;Bakeres&rbrack; Bloqueo relacionado con el subprocesamiento múltiple en CPU Ryzen
* &lbrack;Desempaquetado UV&rbrack; El procesamiento de mallas de alta polietileno puede tardar mucho tiempo
* &lbrack;Desempaquetado UV&rbrack; Los vértices en las mismas coordenadas exactas se combinan
* &lbrack;Desempaquetado UV&rbrack; La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* &lbrack;Desempaquetado UV&rbrack; Proporción de texel no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* &lbrack;Desempaquetado UV&rbrack; Proporción de textura no uniforme entre conjuntos de texturas
* &lbrack;Desempaquetado UV&rbrack; La isla de UV generada puede ser muy alargada y no encajar en el espacio UV en algunos casos
* &lbrack;Desempaquetado UV&rbrack; Es posible que las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no se desenvuelvan con UV

### 5.3.0 (2019.3.0)

*(Lanzado: 17 de diciembre de 2019*)Resumen: **Versión principal con mejora de la experiencia del usuario al pintar a mano, trabajar con tabletas, desempaquetado automático de UV en versión beta (0.3.0) y nuevo contenido diverso para pintar a mano**

**Agregado:**

* Integrar la versión 0.3.0 del desempaquetado automático de UV en Substance Painter
* &lbrack;desempaquetado UV&rbrack; Desempaquetado automático de UV en el Substance Painter cuando no hay UV o UV parciales
* &lbrack;desempaquetado UV&rbrack; Una configuración global para activarla y desactivarla
* &lbrack;desempaquetado UV&rbrack; Versión registrada en el archivo de registro
* &lbrack;desempaquetado UV&rbrack;&lbrack;UI&rbrack; Indicar progreso de desajuste de UV
* &lbrack;UI&rbrack; Nuevos ajustes en la barra de herramientas contextual para seleccionar la vista previa del pincel: Vista previa completa, contorno de pincel y forma de cruz
* &lbrack;Herramienta&rbrack; Nuevo modo de fusión avanzado en la sección alfa: Aclarar (máxima) además de Normal
* &lbrack;Pila de capas&rbrack; Opción de corrección de gamma por capa para alfa o máscara (menú del botón derecho)
* &lbrack;Pila de capas&rbrack;&lbrack;UI&rbrack; Añada el icono &quot;i&quot; cuando se corrija la gamma de una capa alfa
* &lbrack;Tablet&rbrack;&lbrack;Herramienta&rbrack; Exponer presión mínima para tamaño y flujo
* &lbrack;Tablet&rbrack;&lbrack;UI&rbrack; Nuevo ajuste en la barra de herramientas contextual para seleccionar la presión de curva: lineal, fácil de entrar, fácil de salir
* &lbrack;Tablet&rbrack;&lbrack;UX&rbrack; Agregar Ctrl+Alt+clic para desplazarse
* Importar ajustes preestablecidos de pincel de Photoshop (formato ABR)
* &lbrack;ABR&rbrack; Admitir parámetros de forma
* &lbrack;ABR&rbrack; Compatibilidad con parámetros de dinámica de forma
* &lbrack;ABR&rbrack; Parámetros de transferencia de soporte
* &lbrack;ABR&rbrack; Compatibilidad con parámetros de dispersión
* &lbrack;ABR&rbrack;&lbrack;Trazos dinámicos&rbrack; Compatibilidad con redondez y volteo
* &lbrack;ABR&rbrack;&lbrack;Shelf&rbrack; Exponer la estructura de carpetas del pincel en el Editor de filtros
* &lbrack;ABR&rbrack;&lbrack;Shelf&rbrack; Añadir icono de Photoshop en miniaturas
* &lbrack;ABR&rbrack;&lbrack;Shelf&rbrack; Añada una lista de parámetros no compatibles en la miniatura detallada de ABR
* &lbrack;Herramienta&rbrack;&lbrack;Trazos dinámicos&rbrack; Nuevo ajuste de trazo dinámico para controlar cuántas semillas aleatorias se van a generar
* &lbrack;Herramienta&rbrack;&lbrack;UI&rbrack; Añadir nueva configuración de distribución y eje para la variación de dispersión
* &lbrack;Método abreviado&rbrack; Agregue Ctrl+Mayús+B para abrir la ventana de Hacer un bake
* &lbrack;UI&rbrack;&lbrack;Menú&rbrack; Añada la entrada en el menú &quot;Editar&quot; para abrir la ventana de Haga un bake
* &lbrack;UI&rbrack;&lbrack;Settings&rbrack; Mejora de la alineación de la lista de métodos abreviados
* &lbrack;UI&rbrack; Sustitución de los iconos de los controles de presión (tamaño y flujo) por botones de encendido/apagado
* &lbrack;Viewport&rbrack; Permitir enfocar la ventana gráfica 2D y 3D por separado
* Actualización a QT 5.12.5
* &lbrack;UI&rbrack; Indicar el progreso de carga de malla
* &lbrack;Substance&rbrack; Añade compatibilidad con rangos suaves y sin sujeción con reguladores
* &lbrack;Substance&rbrack; Aumentar la precisión de los parámetros del Substance hasta 6 decimales
* &lbrack;Substance&rbrack; Tenga en cuenta el paso definido por un parámetro
* &lbrack;Substance&rbrack; Optimizar la generación de trazos dinámicos con compatibilidad con condiciones en los datos de usuario
* &lbrack;Substance&rbrack; Permite designar una salida de gráfico como una máscara para todos los canales a través de los datos de usuario
* &lbrack;Contenido&rbrack; Actualizar proyecto de muestra &quot;Mat&quot; con topología compatible con desplazamientos, nuevo mapa de ID y nuevas cámaras
* &lbrack;Contenido&rbrack; Integrar 3 filtros nuevos (MatFx): Comic Book, Acuarela, Pintura al óleo (inspirado en la obra de Emrecan Cubukcu)
* &lbrack;Contenido&rbrack; Integrar 102 ajustes preestablecidos de pincel de Photoshop de los paquetes de Kyle T. Webster
* &lbrack;Contenido&rbrack; Integrar 18 nuevos ajustes preestablecidos de pincel: Flecha de rodillo de pintura, texto de advertencia de rodillo de Pintura, carboncillo fino y más
* &lbrack;Contenido&rbrack; Integrar 9 nuevas alfas: Rodillo de Pintura del creador de pinceles, Photoshop del creador de pinceles, patrones de pinceles y mucho más
* &lbrack;Contenido&rbrack; Integrar 2 nuevos ajustes preestablecidos de herramientas: Gouache denso y Gouache descolorido
* &lbrack;Contenido&rbrack; Integrar 1 nuevo generador: Comprobador UV (Islas de UV de realce y costuras)
* &lbrack;Contenido&rbrack; Integrar 2 nuevos ajustes preestablecidos de exportación: Keyshot 9+ y Spark AR Studio
* &lbrack;Contenido&rbrack; Integrar 1 nueva plantilla de proyecto : Spark AR Studio (Facebook)

**Corregido:**

* &lbrack;Tablet&rbrack; Deshacer trazos de puntero (Ctrl+Z) retrasa más que deshacer trazos del ratón
* &lbrack;Tablet&rbrack; Presión de inicio y fin no tenida en cuenta al trazar una línea recta
* &lbrack;Tablet&rbrack; El primer sello se dibuja dos veces al utilizar una línea recta
* &lbrack;Tablet&rbrack; Mejorar la compatibilidad con los métodos abreviados de la tableta Huion
* &lbrack;Tablet&rbrack; Mejorar la compatibilidad con los botones del lápiz de Huion
* &lbrack;Tablet&rbrack; Desplazamiento entre la vista previa del pincel y el sello dibujado
* &lbrack;Tablet&rbrack; Los métodos abreviados para modificar pinceles con lápiz suelen dar lugar a un rendimiento bajo en casos excepcionales
* &lbrack;Tablet&rbrack; Retraso al pintar en una capa específica
* En raras ocasiones, pueden producirse texturas borrosas al cambiar la ventanilla
* &lbrack;UI&rbrack;&lbrack;Substance&rbrack; Las entradas de imagen no siempre se muestran
* Limpiar no elimina los ajustes preestablecidos del estante que se hayan importado en un proyecto
* &lbrack;Herramienta&rbrack;&lbrack;Trazo dinámico&rbrack; Problema de rendimiento al ajustar el recuento cíclico de sello
* Problemas de actualización al pintar en modo de ventanilla 3D/2D en casos excepcionales
* Pintar un trazo muy largo puede provocar un congelamiento
* &lbrack;Herramienta&rbrack; Problema de rendimiento al pintar con trazos dinámicos específicos
* &lbrack;UI&rbrack; La barra de herramientas contextual sigue mostrando las propiedades del pincel al seleccionar una carpeta
* Los valores del eje de simetría no se restablecen
* La importación de texturas EXR con valores de coma flotante es totalmente negra
* Pulsar Alt+clic en un canal para aislar no funciona para el filtro y el generador
* &lbrack;Exportar&rbrack; Bloqueos específicos del proyecto en la exportación
* &lbrack;Substance&rbrack; Valor predeterminado incorrecto en el menú desplegable si el parámetro está oculto por Visible If
* &lbrack;Sombreador&rbrack; Los canales definidos mediante Material Layering no se ordenan del mismo modo en la interfaz de usuario
* &lbrack;Shelf&rbrack; Los metadatos de ajustes preestablecidos no se guardan en el disco

**Problemas conocidos:**

* &lbrack;Desempaquetado UV&rbrack; El procesamiento de mallas de alta polietileno puede tardar mucho tiempo
* &lbrack;Desempaquetado UV&rbrack; Los vértices en las mismas coordenadas exactas se combinan
* &lbrack;Desempaquetado UV&rbrack; La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* &lbrack;Desempaquetado UV&rbrack; Proporción de texel no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* &lbrack;Desempaquetado UV&rbrack; Proporción de textura no uniforme entre conjuntos de texturas
* &lbrack;Desempaquetado UV&rbrack; La isla de UV generada puede ser muy alargada y no encajar en el espacio UV en algunos casos
* &lbrack;Desempaquetado UV&rbrack; Es posible que las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no se desenvuelvan con UV
* El ejemplo de reunión tiene algunos problemas con cámaras importadas

### 5.2.3 (2019.2.3)

*(Lanzado: 23 de octubre de 2019*)Resumen: **Versión de corrección de errores**

**Agregado:**

* &lbrack;Lista de conjuntos de texturas&rbrack; Botón Añadir para activar o desactivar rápidamente el modo de enfoque
* &lbrack;Registro&rbrack; Añadir el número de versión de Windows 10 en el archivo de registro
* Actualizar a la versión más reciente de Substance Engine
* &lbrack;MacOS&rbrack; Se ha certificado el software para seguir los nuevos requisitos de distribución de MacOS Catalina

**Corregido:**

* &lbrack;Complemento&rbrack; El complemento de origen no funciona
* &lbrack;MacOS&rbrack;&lbrack;Sombreador&rbrack; Mac OS 10.14.5 y AMD: la colocación de los materiales en capas no funciona como se pretende

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.2 (2019.2.2)

*(Lanzado: 20 de septiembre de 2019*)Resumen: **Versión de corrección de errores**

**Corregido:**

* La importación de recursos mediante secuencias de comandos puede provocar un bloqueo
* &lbrack;Complemento&rbrack; Descargar material desde el origen puede provocar un bloqueo

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.2.1 (2019.2.1)

*(Lanzado: 17 de septiembre de 2019*)Resumen: **Versión de corrección de errores**

**Corregido:**

* &lbrack;Mac&rbrack;&lbrack;USD&rbrack; Los archivos USDZ exportados de MacOS no se pueden abrir
* &lbrack;Conjunto de texturas&rbrack; No es posible aislar un conjunto de texturas con el modificador ALT
* &lbrack;Shelf&rbrack; Los ajustes preestablecidos, Materiales inteligentes y Máscaras inteligentes siempre se modifican al salir de la aplicación
* &lbrack;Pila de capas&rbrack; No se puede seleccionar el efecto después de eliminar otro efecto
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

* &lbrack;Bakeres&rbrack; Se ha agregado compatibilidad para Trazado de rayos de GPU con DXR y OptiX (Oclusión ambiental, Thickness)
* &lbrack;Bakeres&rbrack; Optimizaciones y aceleraciones para el Trazado de rayos de CPU
* &lbrack;Bakeres&rbrack;&lbrack;Modo Vis&rbrack;&lbrack;UI&rbrack; Nuevo modo de visualización de hace un bake en la ventana gráfica
* &lbrack;Bakeres&rbrack;&lbrack;Preferences&rbrack;&lbrack;UI&rbrack; Nueva opción de hacer un bake para activar y desactivar el Trazado de rayos de GPU
* &lbrack;Bakeres&rbrack;&lbrack;UI&rbrack; Repaso del cuadro de diálogo de la barra de progreso
* &lbrack;Bakeres&rbrack; Mejora de los mensajes de advertencia y error
* &lbrack;Bakeres&rbrack; Permitir una cancelación más receptiva del proceso de hacer un bake
* &lbrack;Bakeres&rbrack; Volver a abrir la ventana hacer un bake después de hacer clic en Cancelar
* &lbrack;Proj&rbrack;&lbrack;UX&rbrack; Mejora de la usabilidad del manipulador de rotación
* &lbrack;Configuración&rbrack; Opción para mejorar el rendimiento mediante la reducción de la resolución de la ventanilla para pantallas HDPI
* &lbrack;Secuencias de comandos&rbrack; Cambiar la resolución del conjunto de texturas
* &lbrack;Secuencias de comandos&rbrack; Obtener conjunto de texturas seleccionado
* &lbrack;Secuencias de comandos&rbrack; Permitir al usuario seleccionar un conjunto de texturas
* &lbrack;Secuencias de comandos&rbrack; Función para saber cuándo se ha cambiado la selección del conjunto de texturas
* &lbrack;Shelf&rbrack; Se han añadido 40 nuevos materiales inteligentes
* &lbrack;Shelf&rbrack; Se han añadido 20 máscaras inteligentes nuevas

**Corregido:**

* &lbrack;Pila de capas&rbrack; Bloqueo de la interfaz de usuario al seleccionar varias capas
* &lbrack;Pila de capas&rbrack; Agrupar muchas capas bloquea la interfaz de usuario más tiempo de lo habitual
* &lbrack;Pila de capas&rbrack; En algunos casos, se pueden seleccionar una capa y un efecto al mismo tiempo
* Los gráficos de Substance utilizados dentro de las herramientas de pintura no se generan con la resolución adecuada
* &lbrack;Baker&rbrack; El botón &quot;Hacer un bake todos los conjuntos de texturas&quot; no se desactiva si no se selecciona ningún baker
* &lbrack;MacOS&rbrack; Desactivar el mensaje de advertencia sobre teselación
* La herramienta Proyección no tiene previsualización cuando se utiliza con una máscara
* Bloqueos y proyectos dañados al intentar ahorrar con espacio en disco insuficiente
* &lbrack;Shelf&rbrack; Bloqueo al importar un recurso a través de la estantería con espacio insuficiente
* &lbrack;Shelf&rbrack; Bloqueo al restaurar el ajuste preestablecido de sesión
* &lbrack;Shelf&rbrack; Importar un ajuste preestablecido con un nombre que termine con un espacio provoca un bloqueo
* &lbrack;Shelf&rbrack; Importar un recurso con un prefijo que termina en un espacio vacío genera un bloqueo

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al hacer un bake con DXR en las GPU Pascal

### 5.1.3 (2019.1.3)

*(Lanzado: 01 de julio de 2019*)Resumen: **Corrección de error con 2 nuevas características**

**Agregado:**

* Permite especificar el presupuesto de VRam con una línea de comandos (p. ej. —vram-budget 4096)
* &lbrack;QML&rbrack; Exponer las propiedades wrapMode y elide de los botones QML y las casillas de verificación

**Corregido:**

* &quot;Seguir ruta&quot; no funciona todo el tiempo
* La asignación de canales no funciona con SBSAR utilizado en ranuras de un solo canal
* &lbrack;Pila de capas&rbrack; Bajo rendimiento al desplazarse con capas ocultas
* &lbrack;TextureSet&rbrack; Bloqueo al hacer clic entre máscaras
* &lbrack;SVT&rbrack; El desplazamiento no se muestra correctamente y parpadea en algunos casos
* &lbrack;Alembic&rbrack; Bloqueo con malla usando normales de punto en lugar de normales de vértice
* &lbrack;Alembic&rbrack;&lbrack;Log&rbrack; Informar de un error en el registro si no se admite el archivo Alembic durante la importación

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

* &lbrack;Substance&rbrack; Visible Si no se tiene en cuenta para las imágenes de entrada
* &lbrack;SVT&rbrack;&lbrack;Motor&rbrack; El cambio de la resolución del conjunto de texturas provoca un bloqueo en algunos casos
* &lbrack;Motor&rbrack; En algunos casos aparecen texturas negras aleatorias
* &lbrack;Pila de capas&rbrack;&lbrack;UI&rbrack; Al alternar una máscara con MAYÚS, se pueden seleccionar varias capas al mismo tiempo
* &lbrack;Pila de capas&rbrack; La opacidad no afecta al efecto de Pintura con el modo de fusión PassThrough
* &lbrack;Pila de capas&rbrack; La entrada de height a filtro normal no se actualiza correctamente con el trazo del pincel del borrador
* &lbrack;LayersStack&rbrack; Bloqueo al deshacer la caída de una máscara inteligente
* Malla metálica parpadeando con sombras y anti-aliasing temporal activado
* &lbrack;Desplazamiento&rbrack; Retraso en AMD con algunas mallas pesadas
* &lbrack;Windows&rbrack; Bloqueo al abrir algunos proyectos mediante el explorador de archivos
* &lbrack;Histograma&rbrack; Bloqueo al eliminar la máscara con el punto de anclaje en algunos casos
* Bloqueo en la generación de vistas previas en algunos casos raros
* &lbrack;Bloqueo&rbrack; No se puede volver a abrir un proyecto con demasiadas herramientas de clonación y difuminado
* No se muestra ninguna malla en el modo de material después de guardarla en algunos casos
* &lbrack;Secuencias de comandos&rbrack; alg.mapexport.documentStructure() devuelve valores incorrectos para carpetas

**Problemas conocidos:**

* Al hacer doble clic en el nombre del conjunto de texturas, se seleccionará antes de entrar en el modo de cambio de nombre

### 5.1.0 (2019.1.0)

*(Lanzado: 23 de abril de 2019*)Resumen: **Trazo dinámico con nuevo contenido, Desplazamiento y teselación en tiempo real e Iray, efecto Máscara de comparación, simetría radial, Plano y Proyección esférica**

**Agregado:**

* &lbrack;Herramienta&rbrack; Trazo dinámico: Variación Substance junto a un trazo de pincel
* &lbrack;Trazo dinámico&rbrack; Exponer nuevo parámetro de índice de sello con opciones
* &lbrack;Trazo dinámico&rbrack; Tenga en cuenta el parámetro $time
* &lbrack;Trazo dinámico&rbrack; Generar nuevo parámetro $randomseed por trazo y por sello
* &lbrack;Trazo dinámico&rbrack; Iniciar un índice de trazo dinámico desde un número aleatorio
* &lbrack;Trazo dinámico&rbrack;&lbrack;Shelf&rbrack; Ayuda para encontrar un recurso de trazo dinámico con un icono nuevo dedicado
* Desplazamiento y teselación en la ventana gráfica en tiempo real
* Desplazamiento y teselado en Iray
* &lbrack;configuración de Sombreador&rbrack;&lbrack;UI&rbrack; Nueva pestaña para controlar el desplazamiento y la teselación
* &lbrack;Pila de capas&rbrack; Nuevo efecto CompararMáscara: generar una máscara comparando dos canales
* &lbrack;Pila de capas&rbrack;&lbrack;UI&rbrack; Nueva entrada en el menú contextual &quot;Añadir máscara con combinación de height&quot; para insertar un efecto Comparar máscara
* &lbrack;Simetría&rbrack; Nuevo modo de simetría: pintura radial
* &lbrack;configuración de Simetría&rbrack; Expanda ambas secciones &quot;Configuración&quot; y &quot;Pantalla&quot;
* &lbrack;configuración de Simetría&rbrack;&lbrack;UI&rbrack; Vista previa para pintura radial
* Exponga dos nuevos modos de proyección: plano y esférico
* &lbrack;Proj&rbrack; Nuevo modo de recorte de forma para todas las proyecciones
* &lbrack;Proj&rbrack; Modo plano con nuevo manipulador: Herramienta Superficie
* &lbrack;Proj&rbrack;&lbrack;Método abreviado&rbrack; Método abreviado MAYÚS+W para la herramienta Superficie
* &lbrack;Proj&rbrack; Enmascaramiento de proyección plana con selección de profundidad y sacrificio de la cara posterior
* &lbrack;Manipulador&rbrack; Mejora del manipulador de rotación en los tres ejes para triplanar
* &lbrack;Herramienta&rbrack;&lbrack;UX&rbrack; Al pulsar Alt y hacer clic en un canal, se selecciona ese canal (lo activa o desactiva todos los demás)
* &lbrack;Motor&rbrack; Actualizar a la versión más reciente de Substance Engine
* &lbrack;Conjunto de texturas&rbrack; Selección múltiple y cambio de resolución
* &lbrack;Conjunto de texturas&rbrack; Activación y desactivación rápidas de los conjuntos de texturas
* &lbrack;Conjunto de texturas&rbrack; Combinar solo y todas las opciones en un nuevo menú
* &lbrack;Conjunto de texturas&rbrack;&lbrack;Pila de capas&rbrack; Nuevo icono para la activación y desactivación
* &lbrack;Pila de capas&rbrack;&lbrack;UX&rbrack; Inserta efectos por encima de los que ya están seleccionados
* &lbrack;Pila de capas&rbrack;&lbrack;UI&rbrack; Estilo de selección de vista de pila de capas de retrabajo
* &lbrack;Pila de capas&rbrack; El modo de fusión para capas con instancias ahora está en modo Pass Through de forma predeterminada
* &lbrack;Exportar&rbrack; Opción para activar y desactivar el tramado
* &lbrack;Complemento&rbrack; Modificador de precisión de soporte para reguladores (MAYÚS)
* &lbrack;Complemento&rbrack;&lbrack;UI&rbrack; Nuevo icono para autoguardar
* &lbrack;Secuencias de comandos&rbrack; Mostrar el contenido de una carpeta
* &lbrack;Secuencias de comandos&rbrack; Permitir la eliminación de archivos
* &lbrack;Secuencias de comandos&rbrack; Leer toda la información de la pila, incluidos los recursos utilizados
* &lbrack;Content&rbrack;&lbrack;Dynamic stroke&brack; Nuevas herramientas y ajustes preestablecidos de pincel
* &lbrack;Content&rbrack;&lbrack;Dynamic stroke&brack; Dos nuevos degradados procedimientos: Tono de degradado y Generador de degradado
* &lbrack;Contenido&rbrack; 11 nuevos filtros: Pintura de pelado MatFx, gotas de agua MatFx y más
* &lbrack;Contenido&rbrack; 7 nuevos generadores: Stitcher automático, UV Random Color, UV Texel Density y más
* &lbrack;Contenido&rbrack; 93 alfas nuevas: nuevos textos, flechas y otras formas
* &lbrack;Contenido&rbrack; 2 nuevos procedimientos: Tono de degradado, Generador de degradados y mucho más
* &lbrack;Contenido&rbrack; 21 nuevos ajustes preestablecidos de herramienta y pincel para Trazos dinámicos : Guijarros, Huellas, Spray y más
* &lbrack;Contenido&rbrack; 2 Nuevos HDR: Canopus Ground y Autumn Forest
* &lbrack;Contenido&rbrack; Actualizar el contenido con la selección aleatoria de semillas en el estante
* &lbrack;Contenido&rbrack; Nuevo icono con parámetro de semilla aleatoria expuesto en la estantería

**Corregido:**

* &lbrack;Pila de capas&rbrack; La pila de capas sigue arrastrando para siempre
* &lbrack;Mac&rbrack; &quot;Mostrar en Finder&quot; puede provocar la congelación
* &lbrack;Secuencias de comandos&rbrack; La configuración guardada mediante la interfaz de usuario personalizada se pierde si se mueve el archivo de sombreador
* &lbrack;Secuencias de comandos&rbrack; El número de versión de la API es incorrecto y no está actualizado
* &lbrack;Efecto&rbrack; El contenido del histograma no se muestra correctamente
* &lbrack;Efecto&rbrack; El efecto del histograma no se actualiza en algunos casos
* &lbrack;Shelf&rbrack; Los puntos no están correctamente alineados en el material &quot;Pirámide de tela de plástico&quot;

**Problemas conocidos:**

* Al hacer doble clic en el nombre del conjunto de texturas, se seleccionará antes de entrar en el modo de cambio de nombre
* &lbrack;Pila de capas&rbrack;&lbrack;UI&rbrack; Al alternar una máscara con MAYÚS, se pueden seleccionar varias capas al mismo tiempo

## Versión 4

### 4.3.3 (2018.3.3)

*(Lanzado: 7 de marzo de 2019*)Resumen: **corrección de errores**

**Agregado:**

* &lbrack;Contenido&rbrack; Integrar nueva plantilla de proyecto: &quot;PBR - Rugosidad metálica Alpha-blend&quot;
* El orden de búsqueda de la biblioteca dinámica de Linux ha cambiado para priorizar las bibliotecas en el directorio de instalación antes de lo que está instalado en el sistema

**Corregido:**

* La malla desaparece a veces de la ventana gráfica 3D (presione F para restablecer la cámara)
* Actualizar el cargador de Substance Painter de Sketchfab con los nuevos tipos de licencia de Sketchfab
* &lbrack;Import&rbrack;&lbrack;glTF&rbrack; Control incorrecto de la modulación de la textura de entrada como se define en los archivos glTF
* &lbrack;Import&rbrack;&lbrack;glTF&rbrack; El plano de tierra se muestra incorrectamente con la importación glTF en algunos casos
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; La opacidad no funciona en Arkit
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; BLOQUEOS de exportación de USDz en algunos casos
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Exportar a USD sin guardar los posibles clientes en el bloqueo
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Modo de mosaico incorrecto para texturas, modo de subdivisión para mallas y tipos de salida para sombreadores
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Exportaciones dispersas de solo algunos conjuntos de texturas con toda la geometría
* &lbrack;Instancia&rbrack; Bloqueo al intentar eliminar una capa de instancia rota
* &lbrack;Regresión&rbrack;&lbrack;Exportar&rbrack; Algunos mapas no se exportan en la profundidad de bits elegida
* &lbrack;Linux&rbrack; Problema con library libtbb.so.2

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.3.2 (2018.3.2)

*(Lanzado: 24 de enero de 2019*)Resumen: **Revisión con nuevas características (exportación USDZ y filtrado de Texturas en el puerto de visualización)**

**Agregado:**

* &lbrack;Exportar&rbrack; Permitir exportación a USDZ
* &lbrack;Viewport&rbrack; Permita controlar la calidad de la textura en los Ajustes de visualización
* &lbrack;Viewport&rbrack; Se ha añadido el ajuste de sesgo mip en Ajustes de visualización
* &lbrack;Viewport&rbrack; Se ha añadido un filtrado anisotrópico en Configuración de visualización
* &lbrack;plugins&rbrack; Actualizar los complementos oficiales para usar el estilo de Substance Painter 2018
* &lbrack;Licencia&rbrack; Instalar la licencia de forma predeterminada en una carpeta de usuario

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
* &lbrack;Secuencias de comandos&rbrack; La creación de la ruta de archivo no se fuerza al guardar un proyecto
* &lbrack;Secuencias de comandos&rbrack; La devolución de llamada &quot;onProjectAboutToSave()&quot; ya no funciona
* Vínculos de foro rotos en la ventana de informe de errores

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.3.1 (2018.3.1)

*(Lanzado: 06 de diciembre de 2018*)Resumen: **Revisión**

**Agregado:**

* &lbrack;Simetría&rbrack;&lbrack;Viewport&rbrack; La simetría pintada en la Vista 2D ha vuelto y ahora presenta una vista previa del pincel clónico corregida

**Corregido:**

* &lbrack;Exportar&rbrack; La exportación de vista 2D genera una textura negra en algunos casos
* &lbrack;Iray&rbrack; La información normal se vuelve incorrecta en Iray después de crear instancias de una capa de material
* Los conjuntos de texturas no cuadrados pueden provocar en algunos casos bloqueos
* &lbrack;Deshacer&rbrack; Varias teclas Ctrl+Z pueden llevar aleatoriamente en algunos casos al bloqueo
* &lbrack;QML&rbrack; AlgScrollView puede crear una advertencia en el registro en algunos casos (bucles de enlace)

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows
* El suavizado y las sombras cuando están activos juntos pueden dar resultados inesperados

### 4.3.0 (2018.3.0)

*(Lanzado: 20 de noviembre de 2018*)Resumen: **Actualizaciones de la ventana gráfica, exportación adecuada de Vista 2D, nuevos ayudantes de interfaz de usuario, una herramienta de simetría mejorada, nuevo contenido y un gran aumento en el rendimiento**

**Agregado:**

* &lbrack;Suavizado&rbrack;&lbrack;Ventana&rbrack; Nuevo filtrado de suavizado temporal para la ventana gráfica 3D (mediante Configuración de visualización)
* &lbrack;Exportar&rbrack; Exportar el contenido de la ventana gráfica 2D como una sola textura
* &lbrack;Export&rbrack;&lbrack;Tramado&rbrack; Mostrar tramado en la exportación
* &lbrack;Pila de capas&rbrack; Colores en capas y carpetas
* &lbrack;Pila de capas&rbrack; Activación y desactivación rápidas de varias capas y efectos
* &lbrack;Pila de capas&rbrack; Navegación más sencilla para los modos de fusión con las teclas de flecha arriba y desplazamiento del ratón
* &lbrack;Proj&rbrack;&lbrack;UI&rbrack; Manipulador de rotación adicional en los tres ejes para triplanar
* &lbrack;Proj&rbrack;&lbrack;Accesos directos&rbrack; - y + para cambiar el tamaño del manipulador de Proyección de UV
* &lbrack;Sombreador&rbrack; Controlar los parámetros de las capas recubiertas con canales en el sombreador recubierto de PBR
* &lbrack;Substance&rbrack; Exponer nuevas entradas de textura basadas en malla para filtros y generadores
* &lbrack;Simetría&rbrack;&lbrack;Viewport&rbrack;&lbrack;UI&rbrack; Control del desplazamiento de simetría con manipuladores
* &lbrack;Simetría&rbrack;&lbrack;Barra de herramientas contextual&rbrack;&lbrack;UI&rbrack; Nuevo panel simetría con opciones
* &lbrack;Simetría&rbrack; Nuevo modo de intersección de línea de simetría
* &lbrack;Simetría&rbrack; Nuevo cursor de clonación de simetría
* &lbrack;Simetría&rbrack;&lbrack;Atajos&rbrack; Q para ocultar y -, + para cambiar el tamaño y cambiar para ajustar
* &lbrack;Registro&rbrack; Mejore los mensajes de error cuando no se pueden exportar texturas
* &lbrack;Secuencias de comandos&rbrack; Permitir cambiar o actualizar los recursos en Configuración de visualización
* &lbrack;Secuencias de comandos&rbrack; Permitir la creación o eliminación de canales en conjuntos de texturas
* &lbrack;Content&rbrack;&lbrack;Shaders&brack; Añada compatibilidad con la anisotropía con un sombreador específico (pbr-metal-rough-anisotropía-angle)
* &lbrack;Contenido&rbrack; Actualización de la esfera de previsualización con la anisotropía y el ángulo modificado
* &lbrack;Contenido&rbrack; Línea de obturación matFx actualizada
* &lbrack;Contenido&rbrack; Nueva digitalización de caras sin problemas Texturing.XYZ
* &lbrack;Contenido&rbrack; Nuevos procedimientos anisotrópicos
* &lbrack;Contenido&rbrack; Nuevo filtro: entorno de iluminación generado
* &lbrack;Contenido&rbrack; Nuevo mapa de entorno: studio automotive neutral
* &lbrack;Contenido&rbrack; Nueva plantilla de proyecto: PBR - Ángulo de anisotropía de rugosidad metálica (con canales de anisotropía)
* &lbrack;Contenido&rbrack; Nueva plantilla de proyecto: PBR - rugosidad metálica recubierta
* &lbrack;SVT&rbrack;&lbrack;Motor&rbrack; Texturas virtuales dispersas (SVT)
* &lbrack;SVT&rbrack;&lbrack;Preferences&rbrack;&lbrack;UI&rbrack; Opción de aceleración de compatibilidad de hardware SVT
* &lbrack;SVT&rbrack;&lbrack;Log&rbrack; Información adicional para la función de texturas virtuales dispersas (por ejemplo, disco de tamaño)
* &lbrack;SVT&rbrack;&lbrack;UI&rbrack; Ventana de mensaje al inicio si el tamaño del disco es demasiado bajo para la caché
* &lbrack;SVT&rbrack;&lbrack;Preferences&rbrack;&lbrack;UI&rbrack; Ubicación de caché global del Substance Painter
* &lbrack;SVT&rbrack; Nueva variable de entorno para especificar la ruta de acceso de la caché del Substance Painter
* &lbrack;SVT&rbrack; Nueva variable de entorno para activar la aceleración de compatibilidad de hardware SVT
* &lbrack;SVT&rbrack; Detectar compatibilidad dispersa por hardware
* &lbrack;SVT&rbrack;&lbrack;Hardware Sparse&rbrack; Aumentar la versión mínima del controlador para la GPU Nvidia
* &lbrack;SVT&rbrack;&lbrack;Sombreador&rbrack;&lbrack;Viewport&rbrack;&lbrack;UI&rbrack; Avisar al usuario si hay artefactos con texturas virtuales dispersas al abrir el proyecto

**Corregido:**

* &lbrack;Selector de color&rbrack; Cursor de pintura que aparece al intentar seleccionar un color
* El bloqueo al seleccionar o anular la selección de capas en un orden específico puede provocar bloqueos
* Bloqueo al pegar como instancia una capa con una máscara
* &lbrack;Canal de usuario&rbrack;&lbrack;Regresión&rbrack; Bloqueo al cambiar el nombre del canal de usuario
* &lbrack;Canal de usuario&rbrack; Vista previa de pincel gris
* &lbrack;Alembic&rbrack; Solo un conjunto de texturas de varios materiales tras la importación
* &lbrack;Motor&rbrack; La textura exportada difiere de la ventana gráfica para los sellos de pincel
* &lbrack;Motor&rbrack; La inversión con un efecto de nivel no afecta por completo a una textura
* El selector de material está aplicando un trazo de pincel al seleccionar
* Cambiar la resolución a 128x128px conduce a un bloqueo
* Los vínculos de mapa de malla no se actualizan correctamente al rehornear o crear instancias de capas
* &lbrack;Substance&rbrack; UserData ColorSpace no funciona en la malla Hecha un bake Normal solicitada como entrada
* No coincide la asociación MDL al utilizar varias instancias de sombreado
* &lbrack;Simetría&rbrack;&lbrack;Rellenar capa&rbrack; Plano de simetría y su manipulador activos en Capa de relleno
* &lbrack;Viewport&rbrack; El punto de tabla dinámica para la traducción no siempre se actualiza después de hacer clic
* &lbrack;UI&rbrack; Corrección de iconos y eliminación de marcadores de posición para monitores HDPI

**Problemas conocidos:**

* Bloqueo de cálculos en algunos casos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows
* El suavizado y las sombras cuando están activos juntos pueden dar resultados inesperados

### 4.2.3 (2018.2.3)

*(Lanzado: 25 de septiembre de 2018)*

**Corregido:**

* &lbrack;vista 2D&rbrack; El vista 2D se rompe con algunas mallas al crear un nuevo proyecto
* &lbrack;Bloqueo&rbrack; El cambio de la Proyección de UV a la proyección tri-plana conduce a un bloqueo
* &lbrack;RayCollider&rbrack; Varios bloqueos debido a &quot;RayCollider&quot;
* &lbrack;Herramienta&rbrack; Al cambiar las capas, se pierden las propiedades de pincel modificadas
* La configuración del pincel se restablece al cambiar al borrador

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.2.2 (2018.2.2)

*(Lanzado: 11 de septiembre de 2018*)Resumen: **Revisión con actualización de contenido, nuevas funcionalidades de secuencias de comandos y poder deshabilitar la actualización automática**

**Agregado:**

* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; Añadir un ajuste preestablecido de Estante de piel
* &lbrack;Content&rbrack;&lbrack;shelf&brack; Conversión de 19 normales de piel en materiales para dispersión subsuperficial
* &lbrack;Secuencias de comandos&rbrack; Crear una plantilla de proyecto desde un proyecto abierto
* &lbrack;Secuencias de comandos&rbrack; Obtener o establecer la configuración de exportación de un proyecto abierto
* &lbrack;Actualizaciones&rbrack; Puede desactivar la ventana emergente de actualización automática de la variable de entorno y configuración
* &lbrack;Actualizaciones&rbrack; No mostrar hasta la próxima versión en el mantenimiento anticuado emergente

**Corregido:**

* &lbrack;Cámara&rbrack; Zoom incorrecto al cambiar de ortográfico a Perspectiva
* &lbrack;Mostrar&rbrack; Algunos mapas se muestran en modo lineal en lugar de sRGB
* &lbrack;Viewports&rbrack; El enfoque de malla no se comporta correctamente
* &lbrack;vista 2D&rbrack; Proyecto con cámara rota ha desaparecido UVs Cáscaras
* &lbrack;SSS&rbrack;&lbrack;Información sobre herramientas&rbrack; aparece información sobre herramientas de dispersión subsuperficial en el registro
* Algunos proyectos no se pueden abrir en 2018.2 y el mensaje de error no puede guardar un paquete de substance nulo
* &lbrack;Máscara&rbrack; El color de la herramienta pintura se puede bloquear en algunos casos al trabajar en una máscara
* &lbrack;Material&rbrack; Los mapas no aparecen en situaciones específicas
* &lbrack;Proj&rbrack;&lbrack;Herramientas&rbrack; Manipulador activo con un generador
* &lbrack;Substance&rbrack; Faltan grupos de parámetros de Substance
* &lbrack;Secuencias de comandos&rbrack; Nombre de software incorrecto en la documentación
* &lbrack;UDIM&rbrack; No hay información en el registro acerca de los proyectiles UV en múltiples mosaicos UVs

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

* &lbrack;SSS&rbrack;&lbrack;Viewport&rbrack;&lbrack;Iray&rbrack; Dispersión subsuperficial genérica
* &lbrack;SSS&rbrack; Sincronizar MDL y parámetros de dispersión subsuperficial
* &lbrack;SSS&rbrack; Se ha añadido un nuevo canal de escala de grises llamado Dispersión
* &lbrack;SSS&rbrack;&lbrack;Configuración de Sombreador&rbrack; Parámetro de tipo de dispersión para la dispersión subsuperficial (cutánea o translúcida)
* &lbrack;SSS&rbrack;&lbrack;Configuración de Sombreador&rbrack; Parámetro de escala de dispersión para dispersión subsuperficial
* &lbrack;SSS&rbrack;&lbrack;Configuración de Sombreador&rbrack; Parámetro de color de dispersión para dispersión subsuperficial
* &lbrack;SSS&rbrack;&lbrack;Configuración de visualización&rbrack; Dispersión Recuento de muestras para dispersión subsuperficial
* &lbrack;Sombreador&rbrack;&lbrack;Iray&rbrack; Integrar MDL de dispersión subsuperficial para Iray
* &lbrack;Sombreador&rbrack; Actualización de sombreador mediante el actualizador de recursos
* &lbrack;Sombreador&rbrack; Actualizar la documentación y la API del registro de cambios
* &lbrack;Propiedades de herramienta&rbrack;&lbrack;Proj&rbrack; Nuevos parámetros para la proyección triplanar
* &lbrack;Viewport&rbrack;&lbrack;Proj&rbrack; Controlar las propiedades de la capa de relleno en la vista 3D directamente con los manipuladores (proyección triplanar)
* &lbrack;Atajos&rbrack;&lbrack;Proj&rbrack; Nuevos métodos abreviados Q, W, E, R y T para manipuladores de proyección triplanar
* &lbrack;Viewport&rbrack;&lbrack;Proj&rbrack; Controlar las propiedades de la capa de relleno en Vista 2D directamente con los manipuladores (Proyección de UV)
* &lbrack;Atajos&rbrack;&lbrack;Proj&rbrack; Nuevo método abreviado Q para manipuladores de Proyección de UV
* &lbrack;Barra de herramientas contextual&rbrack;&lbrack;Proj&rbrack; Manipuladores de proyección triplanar de control
* &lbrack;Barra de herramientas contextual&rbrack;&lbrack;Proj&rbrack; Manipuladores de Proyección de UV de control
* &lbrack;Propiedades de herramienta&rbrack; Desactivación del mosaico de textura con la herramienta Proyección y Galería de símbolos
* &lbrack;Stencil&rbrack; Usar imágenes no cuadradas con la herramienta o galería de símbolos Proyección
* &lbrack;Stencil&rbrack; Permitir el control del modo de mosaico en la ventana Propiedades
* &lbrack;Stencil&rbrack; El zoom no está centrado en una galería de símbolos que no sea de mosaico
* &lbrack;Cámaras&rbrack; Importar cámaras de Maya, Max, Blender, Modo, DAE
* &lbrack;Cámaras&rbrack;&lbrack;Viewport&rbrack; Selección y control de cámaras importadas en la ventana gráfica
* &lbrack;Cámaras&rbrack;&lbrack;Iray&rbrack; Selección y control de cámaras importadas en Irán
* &lbrack;Cámaras&rbrack;&lbrack;UI&rbrack;&lbrack;Nuevo proyecto&rbrack;&lbrack;Configuración del proyecto&rbrack; Importar cámaras está marcado de forma predeterminada
* &lbrack;Cámaras&rbrack;&lbrack;Accesos directos&rbrack; Añadir métodos abreviados para cambiar de cámara
* &lbrack;Cámaras&rbrack;&lbrack;Viewport&rbrack; Añadir marco en la ventana gráfica
* &lbrack;Cámaras&rbrack;&lbrack;Ajustes de ventana&rbrack; Control de la opacidad del marco
* &lbrack;Cámaras&rbrack;&lbrack;Configuración de la cámara&rbrack; Distancia focal máxima a 500 mm
* &lbrack;Cámaras&rbrack;&lbrack;Configuración de la cámara&rbrack; Proporción de exposición
* &lbrack;Cámaras&rbrack;&lbrack;Configuración de la cámara&rbrack; Añadir una opción de bloqueo
* &lbrack;Cámaras&rbrack;&lbrack;Configuración de la cámara&rbrack; Añadir una opción de restauración
* &lbrack;Cámaras&rbrack;&lbrack;Configuración de la cámara&rbrack; Añadir atributo de distancia de enfoque
* &lbrack;glTF&rbrack; Importación de un archivo glTF
* &lbrack;glTF&rbrack; Importar mapa de oclusión ambiental
* &lbrack;Alembic&rbrack; Importar marco Alembic 1 con geometría estática
* &lbrack;Shelf&rbrack; Arrastre y suelte materiales directamente en la malla mediante mapas de ID con un modificador (CTRL/Comando)
* &lbrack;Pila de capas&rbrack; Creación automática de máscaras de ID con arrastrar y soltar materiales en la malla con mapas de ID
* &lbrack;Pila de capas&rbrack; Desplazamiento automático de capas con arrastrar y soltar por la pila de capas
* &lbrack;UI&rbrack;&lbrack;Propiedades de herramienta&rbrack; Exponer el ajuste preestablecido de Substance
* &lbrack;UI&rbrack;&lbrack;Menú Ayuda&rbrack; Mejora del menú Ayuda
* &lbrack;UI&rbrack;&lbrack;Nuevo proyecto&rbrack;&lbrack;Configuración del proyecto&rbrack; Reorganización de la ventana
* &lbrack;UI&rbrack;&lbrack;Nuevo proyecto&rbrack;&lbrack;Configuración del proyecto&rbrack; Reemplazar término de malla por archivo
* &lbrack;UI&rbrack;&lbrack;Substance&rbrack; Visualización de atributos del Substance en la IU
* &lbrack;Atajos&rbrack; Conmutadores F4 entre la vista 2D y 3D
* &lbrack;Atajos&rbrack; Nuevos métodos abreviados para alternar la galería de símbolos N y la máscara rápida U
* &lbrack;integración de Substance&rbrack; Tenga en cuenta las instrucciones &#39;visible if&#39; en los parámetros del Substance
* &lbrack;Viewport&rbrack; Las sombras no se ven forzadas a calcularse después del movimiento de la cámara
* &lbrack;Contenido&rbrack; Actualizar MeetMat con cámaras importadas
* &lbrack;Contenido&rbrack; Añadir una muestra con la dispersión subsuperficial activada - JadeToad
* &lbrack;Contenido&rbrack; Añade una nueva plantilla de proyecto PBR con la dispersión subsuperficial activada
* &lbrack;Contenido&rbrack; Ajustes preestablecidos de exportación actualizados para añadir un nuevo canal de dispersión
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; Se ha añadido compatibilidad de dispersión subsuperficial para: pbr-metal-rough, pbr-metal-rough-alpha-test, recubierto de pbr, pbr-spec-gloss
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; Se ha añadido canal de dispersión a 5 materiales inteligentes (mármoles y pieles)
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; 1 nuevo material de jade
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; 1 cera nueva Material

**Corregido:**

* &lbrack;CMD&rbrack; Diferentes resultados usando la misma línea de comandos con diferentes versiones
* &lbrack;TDR&rbrack; Si TdrLevel está configurado no tiene ningún error en su registro
* &lbrack;Baker&rbrack; El mapa de oclusión ambiental está volteado
* &lbrack;ID Map&rbrack; Bloqueo al seleccionar fuera del rango 0-1
* &lbrack;Iray&rbrack; Bloqueo al cambiar conjuntos de texturas y volver al modo de Pintura
* &lbrack;Viewport&rbrack; Sincronización de áreas de colocación entre puntos de visión para arrastrar y soltar
* &lbrack;Motor&rbrack; Artefacto de Moiré al aplicar mosaico a capas de relleno o pintar pinceles pequeños
* &lbrack;Licencia&rbrack; Comprobación de versión de software errónea del servicio de licencias
* &lbrack;Licencia&rbrack; Rediseña la forma en que gestionamos la autenticación
* &lbrack;API&rbrack; Llame al evento de la API de scripts onNewProjectCreated incluso al crear con una plantilla
* &lbrack;Sombreador&rbrack; El sombreador compilado no se carga de la memoria caché cuando el archivo de sombreador no se compila
* &lbrack;Shelf&rbrack; Al exportar el archivo HDR. de la estantería, se generará un archivo con valores de sujeción
* &lbrack;Exportar&rbrack; EXR exportar abrazaderas RGB valores de color entre 0 y 1
* &lbrack;Contenido&rbrack; Ruido procedimiento El fragmento de ruido de Perlin 3D se pixeló

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* Problema de la tableta Huion con métodos abreviados en el sistema operativo Windows

### 4.1.3 (2018.1.3)

*(Lanzado: 28 de junio de 2018)*

**Agregado:**

* &lbrack;Preferencias&rbrack; Propuesta de guardar el proyecto cuando se reinicie Painter

**Corregido:**

* &lbrack;Complemento&rbrack; El Substance Source de búsqueda no funciona
* &lbrack;Materiales inteligentes&rbrack; La importación de Materiales inteligentes provoca un bloqueo en algunos casos
* &lbrack;Materiales inteligentes&rbrack; La eliminación de Materiales inteligentes provoca un bloqueo en algunos casos
* &lbrack;Guardar&rbrack; Guardar conduce a un bloqueo en algunos casos raros
* &lbrack;Shelf&rbrack; Invertir no funciona en las Celdas 2 y 3
* &lbrack;Shelf&rbrack; Error tipográfico en algunos Alpha
* &lbrack;Shelf&rbrack; Algunos materiales de Substance no se renderizan correctamente

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.2 (2018.1.2)

*(Lanzado: 12 de junio de 2018*)Resumen: **Mejora en la velocidad de Hace un bake, Sistema de guardado mejorado, Reguladores actualizados, Plugin API actualizado, Traducción al chino, Relleno mejorado ahora Opcional**

**Agregado:**

* &lbrack;Bakeres&rbrack; Mejora del rendimiento con la nueva versión de baker
* Cuadro de diálogo Forzar visualización con GPU no compatible
* &lbrack;Guardar&rbrack; Exponer la nueva funcionalidad de proyecto compacto (modo de guardado completo/compacto)
* &lbrack;Guardar&rbrack; Informar al usuario en caso de error al guardar
* &lbrack;Clean&rbrack; Siguiente guardado en modo completo/compacto
* &lbrack;Reguladores&rbrack; Mejora de la precisión de las barras y los reguladores de color/escala de grises
* &lbrack;Reguladores&rbrack; Adición de controles de flecha arriba/abajo
* &lbrack;Reguladores&rbrack; Misma zona de detección para los reguladores de barras de color y escala de grises
* &lbrack;Complemento&rbrack; Guardado automático siempre en modo incremental
* &lbrack;Complemento&rbrack; Opción para cambiar los complementos al nuevo estilo de interfaz
* &lbrack;Idioma&rbrack; Añadir traducción al chino
* &lbrack;Relleno&rbrack; Opción para cambiar entre el relleno UV y el relleno vecino del espacio 3D por conjunto de texturas en Configuración del conjunto de texturas
* &lbrack;Script&rbrack; Exponer modo de guardado: completo/compacto o incremental
* &lbrack;Script&rbrack; Actualizar documentación de scripts/QML
* &lbrack;Registro&rbrack; Indicar el modo de guardado en el registro (completo/compacto o incremental)

**Corregido:**

* &lbrack;Herramienta&rbrack; La ranura de canal se transforma en una ranura de material en rellenos de un solo canal
* Bloqueo al cargar una malla (FBX) con algunas caras no asignadas por un material
* Bloqueo en Irán con NVIDIA GRID 5.2 en máquina virtual
* Bloqueo al deshacer la eliminación de un ajuste preestablecido de material
* Bloqueo al cargar algunos proyectos
* &lbrack;Línea de comandos&rbrack; Nueva línea de comandos para mallas de UDIM divididas por audio
* &lbrack;Barra de herramientas&rbrack; Reducción de la barra de herramientas
* &lbrack;Instanciando&rbrack; No se pueden crear instancias de mapas de bits en varios conjuntos de texturas
* &lbrack;Viewport&rbrack; La actualización no se completa al pintar en malla con UV en mosaico
* &lbrack;Iray&rbrack; El mapa de normales se aplica dos veces a los dieléctricos
* &lbrack;Shelf&rbrack; Errores tipográficos en algunos parámetros del Substance (alfa, procedimientos y matfx)
* &lbrack;Shelf&rbrack; Error tipográfico del mapa de bits &quot;Solo personal autorizado&quot;
* &lbrack;Script&rbrack; La función alg.shaders.materials() ya no funciona

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.1 (2018.1.1)

*(Lanzado: 3 de abril de 2018)*

**Corregido:**

* &lbrack;Tablet&rbrack; Problema al cambiar las opciones de interacción predeterminadas
* &lbrack;Bakeres&rbrack; Bloqueo con la biblioteca Assimp
* &lbrack;Bakeres&rbrack; Regresión en el rendimiento con el mapa A.O
* &lbrack;Iray&rbrack; La Distorsión de lente no se aplica al canal alfa
* &lbrack;Controladores&rbrack; Actualización de los requisitos mínimos de controladores
* &lbrack;3Dview&rbrack; Las normales no se generan correctamente en mallas de UDIM sin información de normales
* &lbrack;Intel&rbrack; Bloqueo normativo con Substance Painter 2018.1.0
* &lbrack;Intel&rbrack;&lbrack;Viewport&rbrack; Problema con el relleno (defectos negros)

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA

### 4.1.0 (2018.1.0)

*(Lanzado: 15 de marzo de 2018)*

**Agregado:**

* Nuevo estilo general (iconos, color, comportamiento)
* Nuevo diseño predeterminado
* &lbrack;Tablet&rbrack; Mejora de la experiencia del usuario al pintar
* &lbrack;Menú principal&rbrack; Ordenar primero los elementos nativos de las vistas y barras de herramientas
* &lbrack;Menú principal&rbrack; Mover acciones de máscara rápida en la sección de ventanilla
* &lbrack;Menú principal&rbrack; Sección Mover las acciones del botón derecho al área de visualización
* &lbrack;Menú principal&rbrack; Cambiar el nombre del menú &quot;Ver&quot; por &quot;Ventana&quot;
* &lbrack;Menú rápido&rbrack; Nuevas propiedades de la herramienta haciendo clic con el botón derecho en la ventana gráfica
* &lbrack;Widget de acoplamiento&rbrack; Nueva barra de herramientas acoplada para una reducción/recuperación rápida
* &lbrack;Configuración de visualización&rbrack; Combinación de la ventana de configuración de cámara y visor
* &lbrack;Pila de capas&rbrack; Menú contextual del botón derecho
* &lbrack;Pila de capas&rbrack; Arrastra y suelta para mover cualquier efecto dentro de la misma capa
* &lbrack;Barra de herramientas&rbrack; Reorganización de la barra de herramientas y nueva barra de herramientas contextual
* &lbrack;Herramientas barra de herramientas&rbrack; Dividir la herramienta Clonar en dos herramientas independientes
* &lbrack;Herramientas propiedades&rbrack; Valor de escala de grises de fondo más claro en la previsualización
* &lbrack;Herramientas propiedades&rbrack; Organización en fichas (rellenar y herramientas)
* &lbrack;Herramienta&rbrack; El resultado de pintura coincide con la galería de símbolos
* &lbrack;Viewport&rbrack; Cursor nuevo para la capa de relleno
* &lbrack;Viewport&rbrack; Navegación y pintura más fluidas (velocidad de marco más alta)
* &lbrack;Viewport&rbrack; Cuadro combinado Selección de material/canal/mapa en la ventana gráfica
* &lbrack;Viewport&rbrack; Reducir el parpadeo mientras se gira (activar sombra)
* &lbrack;Shelf&rbrack; Mostrar materiales de forma predeterminada al abrir Painter
* &lbrack;Shelf&rbrack; Mejora del tiempo de carga de texturas y materiales Substance (de 2 a 6 veces más rápido)
* &lbrack;Shelf&rbrack; Reorganizar carpetas de materiales para que se ajusten a la estructura del Substance Source
* &lbrack;Shelf&rbrack; Arrastre y suelte materiales directamente en la malla en la ventana gráfica
* &lbrack;Shelf&rbrack; Nuevos ruidos en 3D (Perlin, Perlin Fractal, Simplex y Worley)
* &lbrack;Shelf&rbrack; Nuevo generador de máscaras de 3D linear gradient con posición de malla
* &lbrack;Shelf&rbrack; Ruidos básicos actualizados para admitir la expansión no cuadrada
* &lbrack;Shelf&rbrack; Se ha añadido una nueva plantilla y un ajuste preestablecido de exportación para Lens Studio (aplicación Snap)
* &lbrack;Shelf&rbrack; Materiales inteligentes y Máscaras inteligentes actualizados para utilizar la versión más reciente del Editor de máscaras (microdetalles)
* &lbrack;Shelf&rbrack; Nuevo proyecto de muestra &quot;TilingMaterial&quot; para crear materiales de mosaico sin costuras
* &lbrack;Shelf&rbrack; Nuevos ajustes preestablecidos de pincel (caligrafía, mojado, rayado, etc.)
* &lbrack;Reguladores&rbrack; Nuevo estilo y comportamiento de los reguladores y las barras de escala de grises/color
* &lbrack;Bakeres&rbrack; Permitir el uso del cuadro delimitador de escena completo para calcular el mapa de posición
* &lbrack;Sombreador&rbrack; Quitar el parámetro de fuerza de height de los parámetros de sombreador predeterminados
* &lbrack;Motor&rbrack; Motor del Substance actualizado
* &lbrack;Motor&rbrack; Discontinuidades iguales o inferiores en los fragmentos UV
* &lbrack;Complementos&rbrack; Importar materiales descargados de Substance Source con mayor rapidez
* &lbrack;Complementos&rbrack; Actualizar todos los complementos para que coincidan con el nuevo estilo general
* &lbrack;Preferencias&rbrack; Previsualización de los cambios de color de fondo automáticamente
* &lbrack;Clean&rbrack; Menor riesgo de corrupción de proyectos
* &lbrack;Abrir&rbrack; Mejora del tiempo del proyecto de apertura
* &lbrack;Nuevo proyecto&rbrack; Nuevo proyecto: mejora del tiempo de actualización de malla
* &lbrack;Guardar&rbrack; Ahorro de tiempo del proyecto
* &lbrack;Registro&rbrack; Tipo de licencia registrado en el registro
* &lbrack;TextureSet&rbrack; Cambie el nombre del botón &quot;Hacer un bake Texturas&quot; por &quot;Hacer un bake mapas de malla&quot;
* Cambie el nombre de &quot;Mapas adicionales&quot; por &quot;Mapas de malla&quot;

**Corregido:**

* &lbrack;Viewport&rbrack; Mal rendimiento con mallas que contienen muchos subobjetos
* &lbrack;Herramientas propiedades&rbrack; Canal desactivado al arrastrar y soltar una imagen en la ranura de material
* &lbrack;Herramientas propiedades&rbrack; La vista previa del pincel se rompe con las herramientas de difuminado y clonación
* &lbrack;Conjunto de texturas&rbrack; El orden de los canales es incorrecto al utilizar plantillas
* &lbrack;Shelf&rbrack; Falta icono para el generador de Conversión de escala de grises
* &lbrack;Shelf&rbrack; El número de círculo de Sign alfa está roto (falta la fuente)
* Detección incorrecta de GPU integradas al iniciarse
* &lbrack;Bloqueo&rbrack; Arrastrar y colocar un recurso importado cuyo nombre tenga el carácter #
* &lbrack;Motor&rbrack; Problema de detección de Vram en la GPU integrada
* &lbrack;Motor&rbrack; Se han corregido numerosos bloqueos en Substance Engine Linker
* &lbrack;Motor&rbrack; Artefactos cuadrados al cambiar la resolución
* &lbrack;Efectos de posprocesamiento&rbrack; El cambio de tamaño de la interfaz es lento cuando los efectos de posprocesamiento están activados
* &lbrack;Bakeres&rbrack; La unidad de escena no se respeta correctamente para los valores de distancia de rayos
* &lbrack;Bakeres&rbrack; La distancia AO desde Mesh Occluder se fija a 1 independientemente del valor de entrada
* &lbrack;Bakeres&rbrack; La coincidencia por nombre ignora algunas mallas con nombres específicos
* &lbrack;Bakeres&rbrack; El color de la configuración de Polygroup y Submesh ID siempre devuelve una imagen en negro
* &lbrack;Bakeres&rbrack; La Hace un bake de ID falla con mallas de FBX binarias de Blender
* &lbrack;Sombreador&rbrack; Ruido en el vista 2D con dota-2 y non-pbr-spec-gloss
* &lbrack;Linux&rbrack; Sólo se utiliza un subproceso de CPU al hacer un bake
* &lbrack;MacOS&rbrack; Bloqueo con el cursor del pincel moviéndose sobre la ventana gráfica

**Problemas conocidos:**

* Bloqueo de cálculos en GPU AMD VEGA
* El proceso posterior de distorsión no se tiene en cuenta al exportar en IRay (alfa)

## Versión 3

### 3.4.2 (2017.4.2)

*(Lanzado: 24 de enero de 2018)*

**Agregado:**

* &lbrack;Exportar&rbrack; Obtener el estado de una exportación con el progreso del paso
* &lbrack;Exportar&rbrack; Permitir cancelar una exportación
* &lbrack;Exportar&rbrack; Exportar texturas a Sketchfab sin perder calidad de mapa de normales
* &lbrack;Exportar&rbrack; Exportar en formato binario glTF (glb)
* &lbrack;Exportar&rbrack; Permitir cambiar el tamaño de las columnas en la ficha de configuración de la ventana de exportación
* &lbrack;Sombreador&rbrack; Agregar un registro de cambios para la API del sombreador
* &lbrack;Secuencias de comandos&rbrack; Agregar funciones de devolución de llamada Antes y Después al exportar texturas
* &lbrack;Iray&rbrack; Actualización a SDK 2017.1 (compatibilidad con las GPU Volta)

**Corregido:**

* Bloqueo al salir de la aplicación antes de mostrar la ventana principal
* &lbrack;MAC&rbrack; Bloqueo al cargar mapas en escala de grises con IRA
* &lbrack;MAC&rbrack; VRAM detección no es correcta con el nuevo sistema operativo High Sierra
* &lbrack;Complemento&rbrack; La descarga de recursos de Substance Source ya no funciona
* &lbrack;Secuencias de comandos&rbrack; Detección de versión mínima de complemento incorrecta
* &lbrack;Exportar&rbrack; Error al guardar el ajuste preestablecido de exportación después de exportar texturas
* &lbrack;Instanciando&rbrack; Problema en generadores instanciados en un TextureSet sin asignaciones adicionales
* &lbrack;Viewport&rbrack; El tramado no funciona con una resolución superior a 4k
* &lbrack;Viewport&rbrack; La visualización de material de vista 2D está cubierta de ruido
* &lbrack;Shelf&rbrack; Mejorar el tiempo de carga de los ajustes preestablecidos de estantería
* &lbrack;Motor&rbrack; Fusión incorrecta al pintar en la selección de color

### 3.4.1 (2017.4.1)

*(Lanzado: 15 de diciembre de 2017)*

**Agregado:**

* &lbrack;Secuencias de comandos&rbrack; Exportar malla mediante la API de scripts
* &lbrack;Importar&rbrack; Desactivar la importación de formatos de archivo de malla no compatibles (permitir solo obj, fbx, dae, ply)
* &lbrack;Registro&rbrack; Indique con mayor precisión el problema de TDR en el archivo de registro

**Corregido:**

* Bloqueo si la aplicación se cierra antes de que finalice el rastreo de recursos
* Bloqueo al abrir proyectos con la herramienta Dedo/Clonar
* Bloqueo al utilizar rehacer después de deshacer un cambio de Sombreador en Configuración del visor
* &lbrack;Motor&rbrack; La texturización difiere entre Painter 2017.2 y 2017.4
* &lbrack;Viewport&rbrack; Al seleccionar un mapa de ID de una instancia, se muestra un color incorrecto
* &lbrack;Exportar&rbrack; Bloqueo al exportar una textura normal o de oclusión no válida
* &lbrack;Exportar&rbrack; Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6
* &lbrack;Complemento&rbrack; El complemento de Photoshop ignora la selección de canales y siempre exporta todo
* &lbrack;Capas&rbrack; Los anclajes se rompen al copiar o pegar entre conjuntos de texturas
* &lbrack;Capas&rbrack; Algunas referencias de anclaje no se pueden restaurar si están rotas
* &lbrack;Sombreador&rbrack; el parámetro de rugosidad secundaria con revestimiento de pbr está roto
* &lbrack;Vapor&rbrack; La ventana emergente del comprobador de versiones no debería estar visible al iniciarse

**Problemas conocidos:**

* &lbrack;AMD&rbrack; Bloqueos y bloqueos al intentar realizar una pintura en una malla. Se puede solucionar con una actualización del controlador de la GPU.

### 3.4.0 (2017.4.0)

*(Lanzado: 23 de noviembre de 2017)*

**Agregado:**

* &lbrack;Instanciando&rbrack; Permitir la creación de instancias de parámetros en capas
* &lbrack;Instanciando&rbrack; Permitir saltar entre una capa de origen y una instancia
* &lbrack;Instanciando&rbrack; Añadir una acción &quot;Crear instancias en conjuntos de texturas&quot;
* &lbrack;Instanciando&rbrack; Indicar en la pila de capas las instancias de reentrada (ciclos)
* &lbrack;Instanciando&rbrack; Eliminar instancias cuando se elimina un origen
* &lbrack;Instanciando&rbrack; No permitir referencias de anclaje desde fuera de una carpeta con instancias
* &lbrack;UI&rbrack; Mueva la pila Deshacer a su propia ventana llamada &quot;Historial&quot;
* &lbrack;Complemento&rbrack; Integrar el plugin Live-Link de DCC
* &lbrack;Motor&rbrack; Mejorar el rendimiento de la pintura con pintura dispersa
* &lbrack;Exportar&rbrack; Añadir opciones de borrador y reexportación al exportador de Sketchfab
* &lbrack;Shelf&rbrack; Añadir el control &quot;voltear&quot; para las sustancias de fuentes
* &lbrack;Shelf&rbrack; Añade 20 nuevos materiales de procedimientos
* &lbrack;Shelf&rbrack; Añadir 40 nuevos mapas grunges (basados en mapa de bits y procedimientos)
* &lbrack;Viewport&rbrack; Activar colisiones de previsualización de pincel en otros conjuntos de texturas visibles
* Requisitos mínimos de actualización de controladores de GPU AMD

**Corregido:**

* Bloqueo Al calcular Substance con resoluciones demasiado grandes
* Bloqueo al pintar con partículas
* &lbrack;Viewport&rbrack; Reflejo de specular incorrecto en el Vista 2D con mallas específicas
* &lbrack;UI&rbrack; Aparecen algunas acciones no deseadas en la ventana Historial

**Problemas conocidos:**

* &lbrack;Capas&rbrack; Algunas referencias de anclaje no se pueden restaurar si están rotas
* Bloqueo al utilizar rehacer después de deshacer un cambio de Sombreador en Configuración del visor

### 3.3.3 (2017.3.3)

*(Lanzado: 01 de diciembre de 2017)*

**Corregido:**

* &lbrack;Vapor&rbrack; La ventana emergente del comprobador de versiones no debería estar visible al iniciarse
* &lbrack;Exportar&rbrack; Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6

### 3.3.2 (2017.3.2)

*(Lanzado: 20 de noviembre de 2017)*

**Agregado:**

* &lbrack;UI&rbrack; Mejorar el diálogo de la nueva versión y añadir changelog
* &lbrack;UI&rbrack; Indicar si el mantenimiento ha caducado en el cuadro de diálogo Nueva versión
* &lbrack;Licencia&rbrack; Actualizar el sistema de licencias para gestionar las fechas de mantenimiento
* &lbrack;Exportar&rbrack; Cambiar nombre de Adobe Standard Material a Adobe Dimension

**Corregido:**

* &lbrack;Mac&rbrack; Pintar conduce a cuadrados negros y corrupciones de textura
* &lbrack;Motor&rbrack; La caché a veces puede desaparecer en la ventana gráfica
* &lbrack;Motor&rbrack; Aparecen artefactos de bloque cuando se activa la compresión de memoria
* &lbrack;Haciendo un bake&rbrack; Mensajes de error extraños al hacer un bake mallas específicas
* &lbrack;Exportar&rbrack; Los PSD se escriben incorrectamente y Photoshop no los reconoce correctamente
* &lbrack;Capas&rbrack; No debería ser posible copiar y pegar capas en varios proyectos
* &lbrack;Substance&rbrack; El espacio de color UserData para la entrada Normal se invierte en algunos casos
* &lbrack;Shelf&rbrack; Micro-normal en generadores genera curvatura invertida
* &lbrack;Shelf&rbrack; HSL filtro también afecta al canal alfa
* &lbrack;Linux&rbrack; La instalación en Centos falla debido a la falta de dependencias
* El instalador no elimina todos los recursos de la instalación anterior en ciertos casos

### 3.3.1 (2017.3.1)

*(Lanzado: 26 de octubre de 2017)*

**Agregado:**

* &lbrack;Exportar&rbrack; Permitir exportar la malla desde un proyecto
* &lbrack;Shelf&rbrack; Quitar &quot;Sub-Shelf&quot; de los títulos de las pestañas
* Guardar la configuración posterior al proceso en plantillas
* Haz que el mensaje TDR sea más comprensible
* Mejorar la ventana Configuración para informar de errores

**Corregido:**

* Bloqueo al borrar varios subestantes
* Bloqueo al cambiar de un nivel a otro durante un cálculo del motor
* &lbrack;Mac&rbrack; Bloqueo en la GPU Intel durante los cálculos del motor
* &lbrack;Mac&rbrack;&lbrack;Viewport&rbrack; Rendimiento incorrecto cuando el tramado está activado
* &lbrack;Mac&rbrack; MacOS 10.13 se reconoce como &quot;Versión desconocida&quot; en el archivo de registro
* &lbrack;Baker&rbrack; Hacer un bake con una jaula ya no funciona
* &lbrack;Capas&rbrack; El método abreviado Ctrl+C (acción de copia) ya no funciona
* &lbrack;Capas&rbrack; Al pegar capas, la interfaz de usuario no se actualiza con las referencias del anclaje
* &lbrack;Anchor&rbrack; Duplicar o copiar y pegar capa con referencias rompe vínculos
* &lbrack;Exportar&rbrack; La exportación en 8K puede bloquear o bloquear la aplicación en algunos casos
* &lbrack;Exportar&rbrack; Varios problemas en el formato de archivo glTF generado
* &lbrack;Importar&rbrack; Volver a importar una malla con el mismo nombre de archivo ya no funciona
* &lbrack;Complemento&rbrack; La ventana de guardado automático siempre aparece encima de todo
* &lbrack;UI&rbrack; Bucle infinito al pulsar &quot;Escape&quot; en el cuadro de diálogo TDR
* &lbrack;UI&rbrack; Restaurar IU muestra una segunda barra de título en la ventana de la estantería

### 3.3.0 (2017.3.0)

*(Lanzado: 28 de septiembre de 2017)*

**Agregado:**

* &lbrack;Exportar&rbrack; Permitir la exportación de mallas y texturas para el proyecto de Adobe Felix
* &lbrack;Exportar&rbrack; Permitir exportar a formato de archivo glTF
* &lbrack;Motor&rbrack; Optimizar el tamaño de las texturas en VRAM mediante la compresión de bloques
* &lbrack;Viewport&rbrack; Posibilidad de arrastrar y soltar una malla o un proyecto en la ventana gráfica
* &lbrack;UI&rbrack; Mejorar el mensaje de advertencia sobre TDR
* &lbrack;UI&rbrack; El registro debe mostrarse sólo si se solicita
* &lbrack;UI&rbrack; Permitir borrar el contenido de la ventana de registro
* &lbrack;UI&rbrack; Mostrar advertencias y errores en la barra de estado
* &lbrack;UI&rbrack; Mostrar pestañas en la parte superior como en los navegadores web
* &lbrack;UI&rbrack; Mejorar el contexto y los mensajes &quot;no puede pintarse&quot;
* &lbrack;UI&rbrack; Añadir una acción &quot;Guardar como copia&quot; en el menú Archivo
* &lbrack;Capa&rbrack; Establecer el valor predeterminado de mosaico en 1 de forma predeterminada
* &lbrack;Shelf&rbrack; Filtro de degradado mejorado para admitir 10 colores dinámicos
* &lbrack;Shelf&rbrack; Agregar un espacio en la consulta predeterminada de la miniestantería
* &lbrack;Shelf&rbrack; Añadir una acción &quot;Abrir en el explorador&quot; para los recursos locales en el estante
* &lbrack;Shelf&rbrack; Agregar plantilla y sombreador para Adobe Material Standard (Proyecto Felix)
* &lbrack;Shelf&rbrack; Aumentar mosaico máximo a 128 en sombreadores de capas de material
* &lbrack;Shelf&rbrack; Se ha añadido curvatura sobel para microdetalles de Generadores de máscaras
* &lbrack;Complemento&rbrack; Añadir complemento de autoguardado con intervalo de tiempo personalizable
* &lbrack;Secuencias de comandos&rbrack; Añadir una función &quot;Guardar como copia&quot;

**Corregido:**

* &lbrack;UI&rbrack; El diseño se interrumpe al iniciarse por primera vez
* &lbrack;Exportar&rbrack; El PSD generado al exportar tiene errores de formato
* &lbrack;Exportar&rbrack; EXR siempre exporta el mapa de altura de 8 bits
* &lbrack;Exportar&rbrack; Bloqueo al exportar mapas adicionales dañados
* &lbrack;Importar&rbrack; Los bordes duros no se conservan en mallas de polietileno bajas en algunos casos
* &lbrack;Importar&rbrack; Mensajes de error mejorados al importar mallas con problemas
* &lbrack;Bakeres&rbrack; Error al Hacer un bake la asignación de ID con la opción Coincidir por nombre activada
* &lbrack;Viewport&rbrack; El espacio tangente no se sincroniza con los bakeres
* &lbrack;Efecto&rbrack; Al retroceder una capa no se restaura la referencia de un anclaje
* &lbrack;Efecto&rbrack; Problema de actualización al crear un vínculo entre dos máscaras con anclajes
* &lbrack;Efecto&rbrack; Los anclajes de máscaras encima de la máscara no deben aparecer en la lista
* &lbrack;Efecto&rbrack; La opción Extraer el Alpha de Anclajes no funciona
* &lbrack;Motor&rbrack; La máscara se invierte sola después del primer trazo de pincel
* &lbrack;Motor&rbrack; Bloqueo al cambiar el conjunto de texturas en un proyecto específico
* &lbrack;Shelf&rbrack; Bloqueo al eliminar un ajuste preestablecido de un proyecto
* &lbrack;Shelf&rbrack; Error tipográfico en el filtro Tri-Plano avanzado
* &lbrack;Shelf&rbrack; La escala de ruido del AO de MG Mask Builder no funciona correctamente
* &lbrack;Shelf&rbrack; MG Mask Builder tiene parámetros de curvatura invertidos
* &lbrack;Shelf&rbrack; Los alfa importados generan una previsualización de esfera de material en lugar de una plana

### 3.2.0 (2017.2.0)

*(Lanzado: 27 de julio de 2017)*

**Agregado:**

* Puntos de anclaje: sistema de referencia de capas y máscaras
* &lbrack;Capas&rbrack; Capacidad para cambiar el nombre de los efectos de relleno y Pintura
* &lbrack;Complemento&rbrack; Complemento de Substance Source actualizado
* &lbrack;Secuencias de comandos&rbrack; Permitir consultar la resolución del conjunto de texturas
* &lbrack;Secuencias de comandos&rbrack; Permitir para obtener el estado del motor de pintura
* &lbrack;Rendimiento&rbrack; Optimizaciones mejoradas de carga de proyectos y estampado de pinceles

**Corregido:**

* &lbrack;Herramienta&rbrack; Problemas de rendimiento al ajustar parámetros de material
* &lbrack;Motor&rbrack; Trazos de pincel que desaparecen al cambiar la resolución (4K>2K)
* &lbrack;Vista 3D&rbrack; El espacio tangente no se sincroniza con los bakeres
* &lbrack;Shelf&rbrack; La ruta de los documentos de usuario no se crea automáticamente
* &lbrack;Shelf&rbrack; Hacer ajustes preestablecidos compatibles con versiones anteriores después de una actualización
* &lbrack;Sombreador&rbrack; El sombreador que no es PBR ya no funciona
* &lbrack;Bakeres&rbrack; Error al Hacer un bake la asignación de ID con la opción Coincidir por nombre activada
* &lbrack;Ejemplo&rbrack; Los nombres de los conjuntos de texturas del proyecto de muestra Meet Mat son incorrectos
* Guardar un proyecto antes de crear una plantilla devuelve errores de permisos de escritura

### 3.1.0 (2017.1.0)

*(Lanzado: 20 de junio de 2017)*

**Agregado:**

* &lbrack;Complemento&rbrack; Nuevo complemento de Substance Source (permite descargar contenidos en el estante)
* &lbrack;Shelf&rbrack; 4 Fuentes nuevas (japonés + chino simplificado, máquina de escribir, segmento)
* &lbrack;Shelf&rbrack; 230 nuevos Alpha (combinación de patrones, pinceles y digitalizaciones de huellas digitales)
* &lbrack;Shelf&rbrack; 50 Nuevos Procedurals (Patrones de tela de la ropa medieval y contemporánea)
* &lbrack;Shelf&rbrack; 2 Nuevos mapas ambientales (Mondarrain y Villa Nova Street)
* &lbrack;Shelf&rbrack; 9 Nuevos filtros (Edge Wear de detalle MatFx, Ajustar, HBAO, etc.)
* &lbrack;Shelf&rbrack; Mapa de entorno de panorama predeterminado mejorado
* &lbrack;Shelf&rbrack; Nuevos ajustes preestablecidos de exportación de Arnold 5
* &lbrack;Secuencias de comandos&rbrack; Permitir la importación de recursos en el estante

**Problemas conocidos:**

* &lbrack;Exportar&rbrack; La edición de un ajuste preestablecido de exportación es muy lenta

## Versión 2

### 2.6.2

*(Lanzado: 20 de octubre de 2017)*

**Agregado:**

* &lbrack;Conjunto de texturas&rbrack; Permitir la eliminación de conjuntos de texturas deshabilitados
* &lbrack;Shelf&rbrack; Permitir que varios usuarios escriban dentro de la misma carpeta de la estantería
* &lbrack;Secuencias de comandos&rbrack; Poder volver a cargar la carpeta de complementos
* &lbrack;Secuencias de comandos&rbrack; Añada una versión mínima de API necesaria en los metadatos del plugin para garantizar la compatibilidad
* &lbrack;IRay&rbrack; Mejoras del cuadro de diálogo Exportar imagen

**Corregido:**

* &lbrack;Motor&rbrack; Problema de desaparición de trazos al cambiar la resolución (4K>2K)
* &lbrack;Bakeres&rbrack; Error al Hacer un bake la asignación de ID con la opción Coincidir por nombre activada
* &lbrack;Bakeres&rbrack; Los mensajes de error no son lo suficientemente explícitos
* &lbrack;Vista 3D&rbrack; El espacio tangente no se sincroniza con los bakeres
* &lbrack;Herramienta&rbrack; Artefactos negros al utilizar la herramienta de difuminado
* &lbrack;Sombreador&rbrack; El sombreador que no es PBR ya no funciona
* &lbrack;Sombreador&rbrack; &quot;recubierto de pbr&quot; está roto
* &lbrack;Sombreador&rbrack; La rugosidad del sombreador &quot;recubierto de pbr&quot; ya no tiene impacto
* &lbrack;Sombreador&rbrack; El sombreador del brillo de la especificación no coincide con Iray y SD
* &lbrack;Shelf&rbrack; Bloqueo al cargar dos archivos con el mismo nombre pero extensiones diferentes
* &lbrack;Shelf&rbrack; Ya no se pueden editar los ajustes preestablecidos en los estantes
* &lbrack;Shelf&rbrack; No se puede establecer una vista previa personalizada para los recursos importados en el estante
* Los recursos cargados desde la caché pierden sus usos
* Guardar un proyecto antes de crear una plantilla devuelve errores de permisos de escritura
* Guardado de proyecto incorrecto si el nombre de archivo contiene dos puntos
* Importación de archivos con varios puntos (.) en el nombre de archivo causa problemas

### 2.6.1

*(Lanzado: 12 de mayo de 2017)*

**Agregado:**

* &lbrack;TextureSet&rbrack; No permitir reasignar materiales de malla a nada

**Corregido:**

* Bloqueo al cambiar de TextureSet después de reemplazar mapa con bake
* Bloqueo al hacer &quot;Deshacer y Rehacer&quot; después de cambiar el modo de fusión de la capa
* Bloqueo o congelación al utilizar el efecto &quot;selección de color&quot; con mapa de ID grande
* &lbrack;Exportar&rbrack; Los conjuntos de texturas cuyo nombre se ha cambiado no se ordenan alfabéticamente en la ventana de exportación
* &lbrack;TextureSet&rbrack; Restablecer el nombre predeterminado no comprueba la unicidad
* &lbrack;TextureSet&rbrack; El conjunto de texturas renombrado se desactiva después de volver a abrir el proyecto
* &lbrack;Shelf&rbrack; Falta contenido de plantillas predeterminadas
* &lbrack;Shelf&rbrack; Las texturas no cuadradas se muestran como cuadradas
* &lbrack;Sombreador&rbrack; Cuando se desactiva un conjunto de texturas, se destruye el sombreador asociado
* &lbrack;Secuencias de comandos&rbrack; alg.haga un bake.setTextureSetBakingParameters() ya no funciona
* &lbrack;Secuencias de comandos&rbrack; Tutorial de error tipográfico en websocket
* &lbrack;Secuencias de comandos&rbrack; Varios problemas en AlgWidgets
* &lbrack;Registro&rbrack; Detección incorrecta de memoria virtual disponible en algunos casos

### 2.6.0

*(Lanzado: 27 de abril de 2017)*

**Agregado:**

* Agregar nuevo proyecto de muestra &quot;Meet Mat&quot;
* &lbrack;Complemento&rbrack; Nuevo plugin &quot;Resources Updater&quot;
* &lbrack;TextureSet&rbrack; Permitir cambiar el nombre y añadir una descripción a los conjuntos de texturas
* &lbrack;TextureSet&rbrack; Permitir reasignar materiales
* &lbrack;TextureSet&rbrack; Añadir un botón de configuración en la ventana de lista de conjuntos de texturas
* &lbrack;TextureSet&rbrack; Mostrar los conjuntos de texturas &quot;desactivados&quot; en la parte inferior de la lista
* &lbrack;Substance&rbrack; Utilice mapas adicionales con la resolución actual del conjunto de texturas para mejorar el rendimiento
* &lbrack;Secuencias de comandos&rbrack; Permitir actualizar un recurso utilizado en un proyecto (material, generador, etc.)
* &lbrack;Secuencias de comandos&rbrack; Añadir una forma de añadir o quitar un estante
* &lbrack;Secuencias de comandos&rbrack; Permitir consultar información de recursos en proyectos
* &lbrack;Secuencias de comandos&rbrack; Permitir la recuperación de una lista de aplazamientos disponibles
* &lbrack;Secuencias de comandos&rbrack; Tutorial de mejora de miniaturas de AlgWidget
* &lbrack;Exportar&rbrack; Desactivar o habilitar la profundidad de bits en función de la compatibilidad con el formato de archivo
* &lbrack;Registro&rbrack; Añadir nombre de complemento para imprimir en la consola
* &lbrack;Registro&rbrack; Quitar error sobre conjuntos de texturas ocultos
* Actualizar la pantalla de bienvenida con nuevos iconos y texto para los ejemplos

**Corregido:**

* Bloqueo al actualizar una malla en proyectos específicos
* &lbrack;Viewport&rbrack; El color interior del plano de simetría ya no es visible
* &lbrack;Viewport&rbrack; Algunos efectos posteriores al proceso se activan al utilizar la vista en solitario
* &lbrack;Shaders&rbrack; La fusión &quot;over_premult&quot; no funciona correctamente
* &lbrack;Shaders&rbrack; Advertencia sobre la prueba alfa con el sombreador predeterminado
* &lbrack;Shelf&rbrack; Análisis incorrecto de etiquetas de Substance
* &lbrack;Shelf&rbrack; El intemperismo del Óxido MatFX no funciona correctamente
* &lbrack;Shelf&rbrack; HSL filtro está activado en canales incorrectos de forma predeterminada
* &lbrack;Shelf&rbrack; El enfoque está activado en el canal Height/Normal de forma predeterminada
* &lbrack;Exportar&rbrack; Los distintos ajustes preestablecidos de exportación no utilizan un mapa de normales de OpenGL
* &lbrack;Herramienta&rbrack; Problemas de imprecisión al crear artefactos con la herramienta clonar/difuminar

### 2.5.3

*(Lanzado: 15 de marzo de 2017)*

**Corregido:**

* &lbrack;Baker&rbrack; Bloqueo al hacer un bake con mallas específicas

**Problemas conocidos:**

* &lbrack;Mac&rbrack; En algunos casos, las partículas pueden dañar la textura

### 2.5.2

*(Lanzado: 14 de marzo de 2017)*

**Corregido:**

* &lbrack;Herramienta&rbrack; Las tabletas Wacom no funcionan en Linux
* &lbrack;Herramienta&rbrack; Artefactos negros al utilizar la herramienta de difuminado
* &lbrack;Bakeres&rbrack; Error al hacer un bake si se utiliza Coincidir por nombre con una jaula
* &lbrack;Bakeres&rbrack; Oclusión ambiental rota al hacer un bake sólo con Mapa de normales
* &lbrack;Shelf&rbrack; Los filtros genéricos no controlan alfa correctamente (contraste/luminosidad, paso alto, etc.)
* &lbrack;Viewport&rbrack; Problema de rendimiento al cargar un proyecto con sombras activadas
* &lbrack;Viewport&rbrack; Problema de tramado en Vista 3D en MacOS
* &lbrack;Viewport&rbrack; Las previsualizaciones de objetos se muestran incorrectamente cuando el perfil de color está activado
* &lbrack;Iray&rbrack; Bloqueo al volver a cambiar el proyecto a OpenGL si Iray no se inicializa
* &lbrack;IRay&rbrack; El brillo se omite al procesar el sombreador SpecGloss/mdl
* &lbrack;Sombreador&rbrack; El sombreador de especificaciones/brillo no coincide con Iray y SD
* &lbrack;Sombreador&rbrack; Conversión de sRGB diferente de la conversión de LUT lineal a sRGB
* &lbrack;Sombreador&rbrack; Procesamiento incorrecto al cargar el proyecto con sombreadores obsoletos
* &lbrack;Sombreador&rbrack; los sombreadores &quot;recubiertos de pbr&quot; ya no funcionan
* &lbrack;Exportar&rbrack; Algunos canales aún se exportan aunque no estén presentes en el conjunto de texturas
* &lbrack;Capas&rbrack; El modo de fusión &quot;mapa de normales de detalles inversos&quot; no funciona en canales en escala de grises
* &lbrack;UI&rbrack; Problema en la &quot;ventana de selección de color&quot; con el monitor HDPI y el zoom de visualización al 150 %

**Problemas conocidos:**

* &lbrack;Mac&rbrack; En algunos casos, las partículas pueden dañar la textura

### 2.5.1

*(Lanzado: 27 de febrero de 2017)*

**Corregido:**

* &lbrack;Mac&rbrack; Entrada de la tableta Wacom rota en 3D y Vista 2D
* &lbrack;Bakeres&rbrack; La coincidencia por nombre ya no funciona
* &lbrack;Bakeres&rbrack; El ajuste &quot;Normales medias&quot; ya no funciona
* &lbrack;Iray&rbrack; Representación incorrecta con falta de mapa de normales hecho un bake
* &lbrack;Iray&rbrack; Los perfiles de color se comportan de forma diferente en comparación con el procesador OpenGL
* &lbrack;Iray&rbrack; Al exportar el procesamiento como mapa de bits no se incluye la corrección del perfil de color
* &lbrack;Substance&rbrack; Los Filtros de material ya no funcionan
* &lbrack;Herramienta&rbrack; La opacidad del trazo no se almacena en los ajustes preestablecidos del pincel
* &lbrack;Herramienta&rbrack; La alineación UV del pincel del Clonar ya no funciona
* &lbrack;Exportar&rbrack; El canal de desplazamiento debe estar centrado en 0,5 al exportar en entero
* &lbrack;Plantilla&rbrack; La ruta de acceso absoluta se almacena en Plantillas
* &lbrack;TextureSet&rbrack; La textura del canal persiste después de quitar el canal

**Problemas conocidos:**

* &lbrack;Linux&rbrack; Las entradas de tabletas Wacom no funcionan en 3D ni en Vista 2D
* &lbrack;Mac&rbrack; En algunos casos, las partículas pueden dañar la textura
* &lbrack;Exportar&rbrack; En casos muy raros, pueden aparecer rectángulos negros en las GPU AMD

### 2.5.0

*(Lanzado: 21 de febrero de 2017)*

**Agregado:**

* Compatibilidad añadida para las GPU AMD Radeon Pro y AMD FirePro
* &lbrack;Herramienta&rbrack; Añadir compatibilidad con la opacidad del trazo
* &lbrack;Herramienta&rbrack; Agregue un modificador que permita continuar con el último trazo de pincel
* &lbrack;Iray&rbrack; Actualización compatible con las GPU Pascal
* &lbrack;Viewport&rbrack; Añadir compatibilidad con perfiles de color (LUT)
* &lbrack;Substance&rbrack; Integrar nuevo marco (motor SD6)
* &lbrack;UI&rbrack; Aumentar la lista de tamaño de &quot;archivo reciente&quot; en el menú Archivo
* &lbrack;Importar&rbrack; Usar categoría de sustancias para rellenar el prefijo en el cuadro de diálogo de importación
* &lbrack;Bakeres&rbrack; Permitir hacer un bake texturas 8K
* &lbrack;Bakeres&rbrack; Permitir hacer un bake resoluciones que no sean cuadradas
* &lbrack;Bakeres&rbrack; Mejorar el consumo de memoria al hacer un bake mallas pesadas de alto contenido de polietileno
* &lbrack;Shelf&rbrack; Bloquear estantes (y proyectos) para prohibir la edición simultánea y evitar daños
* &lbrack;Shelf&rbrack; Leer categorías y palabras clave de sustancias para utilizarlas en el filtrado
* &lbrack;Shelf&rbrack; Permitir excluir recursos del resultado de una consulta de búsqueda
* &lbrack;Shelf&rbrack; Cálculo del tiempo de miniaturas mejorado
* &lbrack;Shelf&rbrack; Permitir insertar ajustes preestablecidos en proyectos
* &lbrack;Shelf&rbrack; Permitir contraer o expandir rápidamente la vista de árbol con MAYÚS
* &lbrack;Shelf&rbrack; Permitir guardar miniaturas cuando los recursos son de solo lectura (caché local)
* &lbrack;Shelf&rbrack; Nuevo contenido : nuevos filtros (transformar, espejo, tri-plana, etc.)
* &lbrack;Shelf&rbrack; Nuevo contenido : nuevos perfiles de LUT (clásicos y artísticos, como Film Noir, Vintage, etc.)
* &lbrack;Shelf&rbrack; Nuevo contenido : 10 nuevos Substance de fuentes para generar rápidamente textos personalizados
* &lbrack;Shelf&rbrack; Nuevas plantillas : Unity 5 y Unreal Engine 4
* &lbrack;Shelf&rbrack; Filtro de HSL mejorado para facilitar la labor de los artistas
* &lbrack;Sombreador&rbrack; Añadir compatibilidad para el canal de specular level en sombreadores PBR
* &lbrack;Sombreador&rbrack; Añadir soporte para tramado en sombreador de prueba de Alpha
* &lbrack;Sombreador&rbrack; Añadir compatibilidad para la asignación de oclusión de paralaje en sombreadores PBR
* &lbrack;Sombreador&rbrack; Permitir definir la interfaz de usuario personalizada para los parámetros de sombreador
* &lbrack;MatLayering&rbrack; Creación de un nuevo canal de máscara para el flujo de trabajo de capas de material
* &lbrack;Secuencias de comandos&rbrack; Permitir escribir metadatos en un proyecto de SP
* &lbrack;Secuencias de comandos&rbrack; Permitir la exportación con un ajuste preestablecido de exportación específico
* &lbrack;Secuencias de comandos&rbrack; Permitir recuperar parámetros de sombreador como JSON
* &lbrack;Secuencias de comandos&rbrack; Agregar compatibilidad para conexiones WebSocket
* &lbrack;Secuencias de comandos&rbrack; Añadir la posibilidad de cargar instancias del sombreador
* &lbrack;Secuencias de comandos&rbrack; Añadir la posibilidad de crear un nuevo proyecto
* &lbrack;Secuencias de comandos&rbrack; Permitir recuperar la dirección URL de la malla importada en un proyecto
* &lbrack;Secuencias de comandos&rbrack; Permitir hagas un bake no cuadrados
* &lbrack;Secuencias de comandos&rbrack; Informar de errores al configurar datos mediante la API de scripts
* &lbrack;Substance&rbrack; Agregar etiqueta de datos de usuario para especificar el formato de mapa de normales

**Corregido:**

* Bloqueo al elegir color con substancias
* Bloqueo al cargar una imagen que no es RGBA32f como mapa de entorno
* Bloqueo relacionado con la pintura en GPU AMD
* &lbrack;Malla&rbrack; OBJ importación no reconoce materiales sin el archivo mtl
* &lbrack;Malla&rbrack; La generación del nombre del conjunto de texturas de UDIM puede ser incorrecta en algunas mallas
* &lbrack;UI&rbrack; El botón Deshacer/Rehacer de la configuración del visor roba el foco y detiene el desplazamiento del ratón
* &lbrack;UI&rbrack; Algunas etiquetas se recortan incorrectamente en High-DPI
* &lbrack;Capa&rbrack; El efecto Reemplazar modo de pintura tiene un comportamiento incorrecto en Máscara
* &lbrack;Capa&rbrack; El modo de fusión de Restar se comporta de forma incorrecta con alfa
* &lbrack;Herramienta&rbrack; El tamaño del pincel se vuelve enorme en vista 2D al pintar sobre bordes UV
* &lbrack;Herramienta&rbrack; La línea recta ajustada tiene un comportamiento errático con High-DPI
* &lbrack;Herramienta&rbrack; La resolución de la galería de símbolos a veces es incorrecta
* &lbrack;Bakeres&rbrack; Los valores de &quot;Distancia máxima del oclusor&quot; se fijan si &quot;relativo al cuadro delimitador&quot; está &quot;Desactivado&quot;
* &lbrack;Sombreador&rbrack; Las definiciones de canal de pilas y parámetros automáticos no coinciden
* &lbrack;Vista 3D&rbrack; Visualización incoherente del canal normal según la configuración del proyecto
* &lbrack;Viewport&rbrack; Algunos mapas de normales tienen valores cerrados que aparecen como artefactos
* &lbrack;Viewport&rbrack; Los efectos posteriores siempre están desactivados de forma predeterminada
* &lbrack;Exportar&rbrack; El ajuste de mezcla normal es incorrecto si falta el canal normal
* &lbrack;Exportar&rbrack; Generación de texturas incorrecta en algunos casos en GPU AMD
* &lbrack;Exportar&rbrack; Los parámetros de sombreador no se exportan correctamente si están ubicados dentro de un grupo
* &lbrack;Exportar&rbrack; La edición de un ajuste preestablecido de exportación en una estantería personalizada genera un error de registro
* &lbrack;Shelf&rbrack; El filtrado de vista de árbol no coincide exactamente con el nombre de la carpeta
* &lbrack;Shelf&rbrack; Cambiar el nombre de un ajuste preestablecido de estantería es difícil de leer
* &lbrack;Shelf&rbrack; El recurso de sombreador importado en la estantería no se conserva después de reiniciar
* &lbrack;Shelf&rbrack; Contenido : Falta el ajuste preestablecido de la herramienta Soldadura
* &lbrack;Shelf&rbrack; Contenido : El Tile Generator no funciona correctamente
* &lbrack;Shelf&rbrack; Contenido : Se ha corregido una máscara incorrecta en el material inteligente sucio del neumático de goma
* &lbrack;Shelf&rbrack; Contenido : Se ha corregido un nombre de grupo incorrecto en el material de la bolsa de cuero
* &lbrack;Iray&rbrack; La mitad de las mallas están desaparecidas en Irán
* &lbrack;Linux&rbrack; Bloqueo al arrastrar un recurso por encima del Vista 3D
* &lbrack;Mac&rbrack; Las preferencias se restablecen en cada inicio en Sierra

**Problemas conocidos:**

* &lbrack;Exportar&rbrack; En casos muy raros, pueden aparecer rectángulos negros en las GPU AMD
* &lbrack;Iray&rbrack; Los perfiles de color pueden comportarse de formas extrañas en ocasiones

### 2.4.1

*(Lanzado: 28 de octubre de 2016)*

**Corregido:**

* Bloqueo al crear un proyecto con una plantilla
* Bloqueo al cerrar el cuadro de diálogo de exportación durante una exportación
* &lbrack;Mac&rbrack; Errores al guardar el proyecto (error al guardar el ajuste preestablecido de exportación)
* &lbrack;Shelf&rbrack; Al crear un nuevo ajuste preestablecido, este se mostrará dos veces
* &lbrack;Shelf&rbrack; Los ajustes preestablecidos no se pueden cargar en modo de solo lectura sin derechos de administrador

### 2.4.0

*(Lanzado: 27 de octubre de 2016)*

**Agregado:**

* &lbrack;Shelf&rbrack; Nueva interfaz para examinar recursos (vista de árbol, filtros, etc.)
* &lbrack;Shelf&rbrack; Permitir guardar una búsqueda como un ajuste preestablecido
* &lbrack;Shelf&rbrack; Permitir la creación de una nueva ventana a partir de un ajuste preestablecido
* &lbrack;Shelf&rbrack; Nueva interfaz para importar recursos
* &lbrack;Shelf&rbrack; No copiar la estantería algorítmica predeterminada en la carpeta Documentos
* &lbrack;Shelf&rbrack; Nuevos ajustes preestablecidos de partículas : Circuito eléctrico, Líneas eléctricas, Rococó, Venas pequeñas
* &lbrack;Shelf&rbrack; Se han mejorado los ajustes preestablecidos de partículas antiguas para que sean más fáciles de usar (como &quot;Lluvia&quot;).
* &lbrack;Shelf&rbrack; Agregar nueva información en el menú contextual de recursos
* &lbrack;Viewport&rbrack; Mejorar el rendimiento al cargar mapas de entorno
* &lbrack;Viewport&rbrack; Agregar compatibilidad con mapas de entorno que no sean potencia de dos

**Corregido:**

* Bloqueo al quitar una máscara
* Bloqueo al pintar después de guardar un ajuste preestablecido
* Bloqueo con el desenfoque de entorno en algunas GPU
* Bloqueo al asignar un recurso incorrecto con el estante mini
* &lbrack;Shelf&rbrack; Limpiar y guardar eliminar etiquetas y metadatos para los recursos del proyecto
* &lbrack;Shelf&rbrack; al importar un ajuste preestablecido, sus recursos se mostrarán en el estante
* &lbrack;Exportar&rbrack; El mapa de normales generado a partir del canal de height tiene una intensidad baja
* &lbrack;Exportar&rbrack; La malla normal no siempre está presente en el mapa de normales final
* &lbrack;Exportar&rbrack; La dilación con la transparencia puede resultar a veces sin transparencia
* &lbrack;Secuencias de comandos&rbrack; &quot;alg.plugin_root_directory&quot; puede devolver una ruta de red truncada
* &lbrack;TextureSet&rbrack; El botón Bloquear se activa al volver a abrir proyectos no cuadrados

### 2.3.1

*(Lanzado: 07 de octubre de 2016)*

**Agregado:**

* &lbrack;Complemento&rbrack;&lbrack;Photoshop&rbrack; Permitir especificar qué material/pila/canales se van a exportar
* &lbrack;Secuencias de comandos&rbrack; Los nombres de función tienen algunas incoherencias

**Corregido:**

* &lbrack;Exportar&rbrack; Alpha se puede descartar en los ajustes preestablecidos de exportación personalizados
* &lbrack;Exportar&rbrack; El Alpha obtiene una conversión de gamma incorrecta en canales sRGB
* &lbrack;Exportar&rbrack; Los documentos no cuadrados se exportan como cuadrados
* &lbrack;Exportar&rbrack; Imposible exportar mapas adicionales si falta uno
* &lbrack;Iray&rbrack; Algunos parámetros (como la intensidad del emisivo) no tienen ningún efecto
* &lbrack;NVIDIA&rbrack; Bloqueo al inicio con NVIDIA Quadro K2200/GTX 750/760
* &lbrack;AMD&rbrack; Conjunto de colores incorrecto para miniaturas y previsualizaciones
* &lbrack;AMD&rbrack; Bloqueos y error del controlador al abrir archivos nuevos y abiertos
* &lbrack;Registro&rbrack; Falta &quot;software-version&quot; en el archivo de registro

### 2.3.0

*(Lanzado: 15 de septiembre de 2016)*

**Agregado:**

* &lbrack;Complemento&rbrack; Nuevo plugin &quot;Exportar a Photoshop&quot; (exportar pila de capas completa)
* &lbrack;Exportar&rbrack; Permitir especificar la anchura del relleno (en píxeles o infinito)
* &lbrack;Exportar&rbrack; Permitir establecer el tipo de fondo fuera de las UV
* &lbrack;Shelf&rbrack; Sombreador de capas de material nuevo para mezclar 10 materiales
* &lbrack;Shelf&rbrack; Nuevo sombreador de arcilla para ver los detalles con el canal height/normal
* &lbrack;Shelf&rbrack; Nuevo filtro de iluminación hecho un bake con entrada de entorno
* &lbrack;Shelf&rbrack; Se han actualizado algunos generadores de máscaras para añadir transformaciones que no son cuadradas
* &lbrack;Viewport&rbrack; Añadir mapa de normales compuesto (normal+height+hacer un bake) al modo solo
* &lbrack;Secuencias de comandos&rbrack; Permitir la exportación de mapas adicionales
* &lbrack;Secuencias de comandos&rbrack; Permitir consultar mapas adicionales disponibles por conjunto de texturas
* &lbrack;Secuencias de comandos&rbrack; Permitir recuperar formato de canal
* &lbrack;Secuencias de comandos&rbrack; Añadir ejemplos en la documentación que hace un bake
* &lbrack;Secuencias de comandos&rbrack; Permitir consultar la visibilidad de una capa
* &lbrack;Secuencias de comandos&rbrack; Permitir consultar el modo de fusión y la opacidad de la capa
* &lbrack;Secuencias de comandos&rbrack; Permitir la exportación de mapas convertidos (mapas de normales finales, archivos AO mixtos, etc.)
* &lbrack;Substance&rbrack; Leer y conectar usos personalizados
* &lbrack;Atajos&rbrack; Agregar tecla modificadora (MAYÚS) para retroceder en el modo solo cíclico
* &lbrack;Exportar&rbrack; Se ha actualizado el ajuste preestablecido de exportación predeterminado para desactivar alfa
* &lbrack;UI&rbrack; Las miniaturas ahora solo se calculan si el motor está disponible
* &lbrack;UI&rbrack; Mostrar una mención cuando las miniaturas se estén calculando

**Corregido:**

* Bloqueo con algunos proyectos antiguos al abrirlos
* Bloqueo con caché de canales de textura dañada
* Bloqueo al mezclar más de 4 materiales con el flujo de trabajo de capas de material
* &lbrack;UI&rbrack; Los métodos abreviados de herramientas no funcionan si la barra de herramientas está oculta
* &lbrack;UI&rbrack; La barra de herramientas de Iray se etiqueta como &quot;Sin título&quot; en el menú Ver
* &lbrack;UI&rbrack; Las barras de herramientas del complemento se denominan &quot;Sin inclinar&quot; en el menú Ver
* &lbrack;Baker&rbrack; Al pulsar Intro mientras se edita un ajuste de hacer un bake, se inicia el proceso de hacer un bake
* &lbrack;Baker&rbrack; Rangos incorrectos para algunos parámetros
* &lbrack;Importar&rbrack; Imposible importar OBJ mallas debido a números muy grandes
* &lbrack;Importar&rbrack; Algunos archivos OBJ se importan con demasiados subobjetos
* &lbrack;Exportar&rbrack; el fondo del canal se rellena con negro en lugar del color predeterminado en la exportación
* &lbrack;Herramienta&rbrack; Las partículas no funcionan correctamente si FOV es demasiado bajo
* &lbrack;Herramienta&rbrack; El color de previsualización del pincel es incorrecto con las máscaras en subpilas
* &lbrack;Viewport&rbrack; Cuando el pincel entra en áreas vacías de la Vista 2D se vuelve gigantesco
* &lbrack;Viewport&rbrack; Vista previa del pincel en blanco al pintar texturas normales
* &lbrack;Secuencias de comandos&rbrack; Documentación incorrecta : &quot;ao&quot; en lugar de &quot;ambientocclusion&quot;
* &lbrack;Secuencias de comandos&rbrack; El proceso iniciado con subprocess() se mata al cerrar Painter
* &lbrack;Shelf&rbrack; El filtro de iluminación hecho un bake utiliza una entrada de AO incorrecta
* &lbrack;MacOS&rbrack; Se ha eliminado el proyecto Fire Hydrant (incompatible)
* El proyecto predeterminado se abre al cargar un archivo \*.spt (en lugar de \*.spp)

**Problemas conocidos:**

* &lbrack;Complemento&rbrack; Debido a Photoshop, el height y el canal normal no se pueden traducir tal cual

### 2.2.0

*(Lanzado: 22 de julio de 2016)*

**Agregado:**

* &lbrack;Shelf&rbrack; Mejorar el sistema de búsqueda y las consultas
* &lbrack;Shelf&rbrack; Añadir campo de búsqueda para miniestantes
* &lbrack;Sombreador&rbrack; Permitir definir la precisión de paso de los reguladores
* &lbrack;Sombreador&rbrack; Añadir un botón Deshacer/Rehacer para parámetros de sombreador
* &lbrack;Sombreador&rbrack; La recarga de un sombreador no debe restablecer sus parámetros
* &lbrack;MatLayering&rbrack; Añadir compatibilidad con Controles dinámicos de capas de materiales y subpilas
* &lbrack;MatLayering&rbrack; Permitir la importación de archivos json para configurar los ajustes de sombreador
* &lbrack;MatLayering&rbrack; Desbloquear límite de muestras de textura (cambiar a texturas sin enlace)
* &lbrack;Secuencias de comandos&rbrack; Permitir definir la configuración de bakeres e iniciar su cálculo
* &lbrack;Substance&rbrack; Usar &quot;uso&quot; para conexiones de entrada/salida además de identificadores
* &lbrack;Herramienta&rbrack; Permitir seleccionar el canal de previsualización en la ventana gráfica para la herramienta Proyección

**Corregido:**

* Bloqueo durante el lanzamiento si las sustancias se encuentran en una carpeta incorrecta
* El informe de bloqueo a veces no funciona debido a un archivo de registro incorrecto
* &lbrack;Iray&rbrack; Los efectos de posprocesamiento no se actualizan cuando Iray está en pausa
* &lbrack;Iray&rbrack; El método abreviado de enfoque automático ya no funciona
* &lbrack;Iray&rbrack; El comportamiento del regulador de apertura cambia en función del tamaño del recurso
* &lbrack;Capas&rbrack; El primer canal de materiales no está activado de forma predeterminada si todos están desactivados
* &lbrack;Sombreador&rbrack; No se imprimen errores si un &quot;param auto&quot; es incorrecto

**Problemas conocidos:**

* &lbrack;Mac&rbrack; El límite de muestras de textura está bloqueado en 16 (problema de controlador de GPU)

### 2.1.1

*(Lanzado: 01 de julio de 2016)*

**Agregado:**

* &lbrack;Licencia&rbrack; Poder cambiar la ubicación del archivo de licencia
* &lbrack;Viewport&rbrack; Añada un método abreviado &quot;B&quot; para desplazarse entre mapas adicionales
* &lbrack;Importar&rbrack; Permitir la importación FBX 2016/2017 correctamente
* &lbrack;Herramienta&rbrack; Quitar fichas al utilizar la máscara rápida
* &lbrack;Iray&rbrack; Añadir información de dimensiones de escena
* &lbrack;Iray&rbrack; Permitir aumentar el número máximo de muestras y el tiempo de procesamiento
* &lbrack;UI&rbrack; Actualizar el resultado inmediatamente al utilizar el botón +/- en los reguladores
* &lbrack;UI&rbrack; Permitir una mayor precisión para los reguladores de escala de grises
* &lbrack;Exportar&rbrack; No exportar un canal alfa para texturas que sean solo RGB
* &lbrack;Exportar&rbrack; Actualizar ajuste preestablecido de exportación de Dota 2
* &lbrack;Shelf&rbrack; Nuevo patrón de &quot;azulejos hexagonales&quot;
* &lbrack;Shelf&rbrack; Nueva herramienta &quot;Soldadura&quot;
* &lbrack;Shelf&rbrack; Filtros de acabado actualizados para proporcionar controles de dirección

**Corregido:**

* &lbrack;Exportar&rbrack; Imposible exportar archivos de PSD en 8 bits
* &lbrack;Exportar&rbrack; La exportación en 8K no está disponible en algunas configuraciones de hardware
* &lbrack;Exportar&rbrack; La ventana de Sketchfab se recorta
* &lbrack;Exportar&rbrack; Mapa de rugosidad incorrecto en el ajuste preestablecido de exportación de especificación/brillo
* &lbrack;UI&rbrack; Escribir en los reguladores de escala de grises ya no funciona
* &lbrack;UI&rbrack; Imposible colocar filtros en entradas de sustancias (como Generadores)
* &lbrack;UI&rbrack; Algunos reguladores tienen comportamientos extraños
* &lbrack;UI&rbrack; El paso DeltaTime +/- para partículas es demasiado grande
* &lbrack;Iray&rbrack; Algunos proyectos bloquean la aplicación al cambiar a Irak
* &lbrack;Iray&rbrack; Bloqueo al detectar hardware
* &lbrack;Herramienta&rbrack; El color de previsualización del pincel es incorrecto en el modo Máscara
* &lbrack;Herramienta&rbrack; El selector de material se puede utilizar con herramientas incompatibles
* &lbrack;Herramienta&rbrack; La previsualización de proyección no cambia a Difuso con el flujo de trabajo de especificación/brillo
* &lbrack;Shelf&rbrack; Al cambiar el sombreador predeterminado, se rompen las previsualizaciones de máscaras inteligentes y alfombras inteligentes
* &lbrack;Shelf&rbrack; Algunos materiales inteligentes tienen nombres incorrectos
* &lbrack;Shelf&rbrack; Las formas alfa adicionales están dañadas y no se cargarán
* &lbrack;Viewport&rbrack; Cambio al modo &quot;Mapa adicional&quot; para mostrar primero &quot;otro&quot;
* &lbrack;Viewport&rbrack; La ventana gráfica vuelve a cambiar a &quot;otro&quot; cuando no existe un mapa adicional
* &lbrack;Bloqueo&rbrack;&lbrack;Linux&rbrack; El informe de bloqueo no funciona en Ubuntu (Steam)
* &lbrack;Bloqueo&rbrack;&lbrack;Linux&rbrack; Los vínculos de URL web no funcionan en Ubuntu (Steam)
* &lbrack;Bloqueo&rbrack;&lbrack;Windows&rbrack; Quitar &quot;Crashwatcher&quot; cuando Substance Painter ya no corra
* &lbrack;Bloqueo&rbrack;&lbrack;Mac&rbrack; El sistema de informes de bloqueos no funciona correctamente
* &lbrack;Bloqueo&rbrack; La importación de una malla al importar una malla ya genera un bloqueo
* El conjunto de texturas que recoge el método abreviado se restablece en nada después de reiniciar

### 2.1.0

*(Lanzado: 02 de junio de 2016)*

**Agregado:**

* &lbrack;UDIM&rbrack; Importación de mosaicos UDIM de una malla como conjuntos de texturas
* &lbrack;Linux&rbrack; Se ha agregado la compatibilidad con CentOS 6.6 y Ubuntu 12.4
* &lbrack;Exportar&rbrack; Añadir resolución 8K (experimental)
* &lbrack;Exportar&rbrack; Permitir la selección de la profundidad de bits durante la exportación
* &lbrack;Baker&rbrack; Permitir hacer un bake varios conjuntos de texturas a la vez
* Compatibilidad con monitores de alta resolución (escala de PPP alta)
* &lbrack;Secuencias de comandos&rbrack; Establecer resolución y relleno personalizados por textura en la exportación
* &lbrack;Viewport&rbrack; Permitir cambiar entre el conjunto de texturas haciendo clic en la malla (mediante Ctrl+Alt+Clic)
* &lbrack;Viewport&rbrack; Ir a donde se encuentra el cursor del ratón al hacer zoom con la rueda del ratón
* &lbrack;UI&rbrack; Actualizar el color de fondo predeterminado y la visualización del mapa de entorno
* &lbrack;UI&rbrack; Añadir información sobre herramientas con nombres originales para los canales de usuario
* &lbrack;UI&rbrack; Cambiar el color de fondo de los canales a los que no se puede cambiar el nombre
* &lbrack;Herramienta&rbrack; Quitar fichas al utilizar la máscara rápida
* &lbrack;Sombreador&rbrack; Permitir definir grupos para parámetros de sombreador y materiales/máscaras
* &lbrack;Motor&rbrack; Optimización del estampado de tamaño pequeño
* &lbrack;Stencil&rbrack; Añada &quot;W&quot; como método abreviado para cambiar temporalmente la máscara
* &lbrack;Shelf&rbrack; Agregue un botón de cruz para borrar el campo de búsqueda
* &lbrack;Shelf&rbrack; Cargar el Alpha con un solo clic
* &lbrack;Shelf&rbrack; Nuevo ajuste preestablecido de exportación : UDIM Vray, Arnold UDIM, Especificación/Brillo de Metal/Rugoso
* &lbrack;Shelf&rbrack; Nuevas alfas : formas geométricas, vetas y signos
* Agregar nombre y versión en las propiedades del ejecutable de Substance Painter

**Corregido:**

* &lbrack;Substance&rbrack; Imposible utilizar el canal normal y el mapa adicional al mismo tiempo
* &lbrack;Iray&rbrack; La refracción de MDL y el ajuste de absorción no funcionan
* &lbrack;Iray&rbrack; La escala de escena original no se conserva
* &lbrack;Shelf&rbrack; Plantilla de specular/Brillo que usa un sombreador incorrecto
* &lbrack;Exportar&rbrack; El ajuste preestablecido de exportación predeterminado no exporta algunos mapas (como AO)
* &lbrack;Viewport&rbrack; El punto de tabla dinámica no se actualiza al hacer clic fuera de las coordenadas UV en la vista 2D
* &lbrack;UI&rbrack; Los valores del regulador se redondean
* &lbrack;UI&rbrack; A veces, al editar los valores de los reguladores, hay un espacio libre muy pequeño
* &lbrack;Nuevo proyecto&rbrack; La lista desplegable de plantillas no se ha actualizado correctamente (de 1.x a 2.x)
* &lbrack;Secuencias de comandos&rbrack; Se ha corregido el comportamiento de &quot;pasar cursor&quot; en los botones personalizados
* &lbrack;Mac&rbrack; La acción de deshacer en un proyecto vacío bloquea la cámara

**Problemas conocidos:**

* El informe de bloqueo no está disponible en Ubuntu
* Es posible que algunos botones de URL no funcionen. Consulta nuestras preguntas frecuentes para obtener una solución alternativa

### 2.0.5

*(Lanzado: 29 de abril de 2016)*

**Agregado:**

* &lbrack;Shelf&rbrack; Se ha agregado o actualizado una plantilla que no es de pbr, sombreador y ajuste preestablecido de exportación
* &lbrack;Shelf&rbrack; Se ha actualizado el ajuste preestablecido de exportación UE4 para incluir Oclusión ambiental

**Corregido:**

* Bloqueo al abrir y guardar algunos proyectos con recursos dañados
* &lbrack;Viewport&rbrack; La malla metálica parece rota en la Vista 2D
* &lbrack;Shelf&rbrack; Rendimiento mejorado de algunos mapas de entorno de estudio
* &lbrack;Shelf&rbrack; Se duplican algunos mapas de entorno de estudio
* &lbrack;Shelf&rbrack; Falta &quot;Material de iluminación Hecho un bake&quot;
* &lbrack;Shelf&rbrack; Falta el generador de conversión de escala de grises

### 2.0.4

*(Lanzado: 26 de abril de 2016)*

**Agregado:**

* Mejora de los choques de malla y optimiza la representación de mallas metálicas
* Mejorar el rendimiento y la gestión de la memoria con grandes proyectos
* Mejorar la precisión y el paso del regulador
* &lbrack;UI&rbrack; Actualizar el motor sólo al validar un regulador (no al introducir un valor)
* &lbrack;UI&rbrack; Mover Iray cambiar a un botón dedicado en la barra de herramientas principal (y cambiar su método abreviado)
* &lbrack;Herramienta&rbrack; Añadir configuración para el comportamiento de ubicación de origen de la herramienta de clonación
* &lbrack;Sombreador&rbrack; Permitir la lectura de colores de vértices de malla en sombreadores personalizados
* &lbrack;Secuencias de comandos&rbrack; Permite recuperar la lista de conjuntos de texturas, canales y capas
* &lbrack;Secuencias de comandos&rbrack; Añadir funciones auxiliares (url a ruta, obtener ruta de exportación desde proyecto)
* &lbrack;Mac&rbrack; Detectar la versión &quot;El Capitan&quot; de Mac Os en el archivo de registro

**Corregido:**

* Bloqueo después de la segunda exportación a Substance share
* Bloqueo al copiar una capa entre conjuntos de texturas con datos de Máscara rápida.
* Algunos proyectos tienen un actualizador muy largo que consume mucha memoria
* &lbrack;Herramienta&rbrack; Bloqueo al seleccionar un ajuste preestablecido de partículas con la herramienta clonar/difuminar
* &lbrack;Baker&rbrack; La carga de FBX archivos tarda demasiado tiempo en cargar mallas pesadas
* &lbrack;Viewport&rbrack; Mapa de entorno estirado en algunos equipos
* &lbrack;Viewport&rbrack; Conversión de gamma incorrecta del alfa del pincel
* &lbrack;Exportar&rbrack; El Alpha se almacena como transparencia en lugar de un canal independiente con archivos Tiff.
* &lbrack;Exportar&rbrack; El canal normal siempre se exporta como OpenGL
* &lbrack;Iray&rbrack; Faltan nombres de reguladores para la configuración de Iray
* &lbrack;Iray&rbrack; El procesamiento se realiza con una resolución incorrecta en Retina/alta PPP
* &lbrack;Iray&rbrack; Bloqueo al cambiar el tamaño de la interfaz en modo Iray
* &lbrack;Iray&rbrack; Gran ralentización del rendimiento al renderizar en algunas resoluciones bajas
* &lbrack;Iray&rbrack; La pausa no funciona (Iray sigue calculando en segundo plano)
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

* &lbrack;Iray&rbrack; Actualizar la plantilla y el sombreador Spec/Gloss para que sean compatibles con Iray
* &lbrack;Exportar&rbrack; Exportar capturas de pantalla a ArtStation
* &lbrack;Secuencias de comandos&rbrack; Ejecución de soporte desde el directorio de plugins
* &lbrack;Secuencias de comandos&rbrack; Permitir &quot;Guardar como&quot;
* &lbrack;UI&rbrack; Permitir hacer doble clic en un regulador para editar su valor
* Mover muestra de Vela al Substance share
* Nuevo proyecto de muestra : Previsualización de esfera
* Advertencia a los usuarios sobre el conflicto de extensión de shell

**Corregido:**

* El instalador anula la instalación de Substance Painter 1.x
* &lbrack;UI&rbrack; El diseño de la lista de canales se rompe con los filtros
* &lbrack;UI&rbrack; No se muestran los parámetros de sombreador
* &lbrack;UI&rbrack; Al cambiar el tamaño de la ventana de capa se recorta incorrectamente el contenido
* &lbrack;Herramienta&rbrack; El canal de opacidad no siempre se usa correctamente
* &lbrack;Herramienta&rbrack; El difuminado/Clonar no funciona con la Simetría
* &lbrack;Herramienta&rbrack; La opacidad de la vista previa del pincel es incorrecta en algunos canales
* &lbrack;Iray&rbrack; Bloqueo al usar Iray cuando todavía no se ha creado
* &lbrack;Iray&rbrack; No se pueden cargar datos de configuración de iris del proyecto
* &lbrack;Iray&rbrack; Iray no se ocupa de la modificación de la configuración después de haber sido pausado
* &lbrack;Shelf&rbrack; Importar un material al estante no funciona
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
* &lbrack;Herramienta&rbrack; Nueva herramienta de difuminado para fusionar y difundir colores
* &lbrack;Herramienta&rbrack; Nueva herramienta de Clonar para copiar parte de las texturas
* &lbrack;Herramienta&rbrack; Permitir la selección de canales para la herramienta de difuminado, Clonar y Borrador
* &lbrack;Capa&rbrack; Añadir nombre de Substance para el nombre del efecto Rellenar
* &lbrack;Capa&rbrack; Permitir exportar la máscara al portapapeles
* &lbrack;Viewport&rbrack; Cambiar entre el modo de Perspectiva y el ortográfico
* &lbrack;Viewport&rbrack; Permitir el control del campo de visión en el modo de Perspectiva
* &lbrack;Viewport&rbrack; Permitir definir la Profundidad de la distancia del campo con CTRL+clic central
* &lbrack;Viewport&rbrack; Permita arrastrar y soltar mapas de entorno en el Vista 3D.
* &lbrack;Viewport&rbrack; Se han mejorado los comentarios cuando el motor realiza cálculos potentes.
* &lbrack;Exportar&rbrack; Permitir la exportación de parámetros de sombreador en un archivo json
* &lbrack;UI&rbrack; Interfaz de actualización con nuevos iconos, colores y diseño
* &lbrack;UI&rbrack; Añadir nombres de recursos a los miniestantes
* &lbrack;UI&rbrack; Contraer &quot;asignación de canales&quot; de forma predeterminada
* &lbrack;Sombreador&rbrack; Selección de un color personalizado para los parámetros de textura de sombreador
* &lbrack;Shelf&rbrack; Preguntar dónde importar archivos al arrastrar y soltar recursos
* &lbrack;Shelf&rbrack; Nueva esfera de previsualización para Materiales inteligentes y generadores
* &lbrack;Shelf&rbrack; Añadir sombreador de Brillo de Specular
* &lbrack;Shelf&rbrack; Nuevas formas de superficie dura
* &lbrack;Shelf&rbrack; Nuevas formas y texturas de Alpha
* &lbrack;Shelf&rbrack; Nuevas texturas de piel
* &lbrack;Shelf&rbrack; Nuevos materiales basados en Scan y materiales inteligentes
* &lbrack;Shelf&rbrack; Nuevos materiales inteligentes y compatibilidad con especificaciones/brillo de los antiguos
* &lbrack;Shelf&rbrack; Nuevos filtros de acabado para la simulación de superficies metálicas
* &lbrack;Shelf&rbrack; Nuevo generador de máscaras potente &quot;Mask Editor&quot;
* &lbrack;Shelf&rbrack; Materiales antiguos retrabajados y limpiados
* Nuevo proyecto de muestra &quot;Vela&quot;

**Corregido:**

* &lbrack;Configuración&rbrack; El proyecto anula la rotación de la cámara y la velocidad de zoom
* &lbrack;Viewport&rbrack; Un problema de precisión en la textura normal predeterminada genera reflejos incorrectos
* &lbrack;Viewport&rbrack; Viñeta está activada de forma predeterminada
* &lbrack;Viewport&rbrack; Aparecen artefactos en los bordes del mapa de entorno (GPU de NVIDIA)
* &lbrack;Viewport&rbrack; La miniatura en modo de proyección/galería de símbolos es muy larga de cargar
* &lbrack;Baker&rbrack; Almacenar texturas hechas un bake en un entero de 16 bits en lugar de 32 bits
* &lbrack;Capa&rbrack; Las sustancias obsoletas se muestran incorrectamente en la pila
* El color predeterminado y la profundidad de bits de algunos canales son incorrectos (p. ej.: Specular, Brillo)
* Se ha corregido el comportamiento del borrador para deshabilitar la fusión en modo de paso a través

**Problemas conocidos:**

* La simetría no funciona con la herramienta de difuminado y Clonar
* Falta la exportación de ArtStation

## Versión 1

### 1.7.3

*(Lanzado: 1 de marzo de 2016)*

**Agregado:**

* &lbrack;Exportar&rbrack; Añadir una opción para desactivar el relleno
* &lbrack;Shelf&rbrack; Admitir jerarquía de subestanterías dentro de una carpeta de estanterías

**Corregido:**

* Bloqueo al guardar sobre un archivo de solo lectura anterior
* Bloqueo al abrir un segundo proyecto
* Bloqueo al cargar algunas miniaturas (estanterías, capas o información sobre herramientas)
* La desactivación de &quot;Conservar posiciones de trazos en la malla&quot; no funciona
* &lbrack;Exportar&rbrack; La ampliación de los mapas de bits se realiza con el filtrado más cercano
* &lbrack;Shelf&rbrack; El descubrimiento de recursos es muy lento
* &lbrack;Shelf&rbrack; Los filtros de desenfoque no son compatibles con 16 bits
* &lbrack;Herramienta&rbrack; La simetría no funciona si carga un ajuste preestablecido antiguo de la herramienta
* El cuadro de diálogo Color del canal de Specular no convierte el espacio de color

### 1.7.2

*(Lanzado: 13 de enero de 2016)*

**Agregado:**

* &lbrack;Capas&rbrack; Permitir especificar el segmentado predeterminado para las capas de relleno

**Corregido:**

* &lbrack;Exportar&rbrack; La exportación de Sketchfab ya no funciona
* &lbrack;Capa&rbrack; El filtrado bilineal se aplica incluso en Rellenar sin ninguna transformación
* &lbrack;Herramienta&rbrack; Rendimiento deficiente al utilizar Substance con entradas de imagen en modo de proyección
* &lbrack;Herramienta&rbrack; El selector de material está roto

### 1.7.1

*(Lanzado: 18 de diciembre de 2015)*

**Corregido:**

* Bloqueo al cambiar el conjunto de texturas
* Reproducciones lentas al pintar

### 1.7.0

*(Lanzado: 17 de diciembre de 2015)*

**Agregado:**

* &lbrack;Performance&rbrack; Calcular el contenido de las capas y sus miniaturas al mismo tiempo
* &lbrack;Exportar&rbrack; Guardar la ruta de exportación como relativa cuando esté al lado del proyecto
* &lbrack;Capas&rbrack; Se ha añadido un nuevo modo de fusión : restar y agregar/sub
* &lbrack;Capas&rbrack; Nuevo filtrado HQ bilineal para capas de relleno
* &lbrack;Sombreador&rbrack; Establezca un sombreador predeterminado para la generación de miniaturas en las preferencias.
* &lbrack;Sombreador&rbrack; Permitir especificar un sombreador por conjunto de texturas
* &lbrack;Sombreador&rbrack; Permitir tomar muestras de texturas de la estantería
* &lbrack;Herramienta&rbrack; Nuevo comportamiento de pincel de &quot;ceñir&quot; para pintar
* &lbrack;Herramienta&rbrack; Filtrado mejorado y suavizado reducido al pintar
* &lbrack;Herramienta&rbrack; Calidad de pintura de subpíxeles mejorada
* &lbrack;Herramienta&rbrack; Se ha eliminado la visualización &quot;básica&quot; de la configuración del pincel y se ha mejorado el icono de apertura/cierre del marco
* &lbrack;Menú&rbrack; Añadir iconos de efectos en el menú contextual
* Creación de plantillas desde Proyectos
* &lbrack;Shelf&rbrack; Nuevas plantillas : PBR, Dota 2
* &lbrack;Shelf&rbrack; Nuevo ajuste preestablecido de exportación : Dota 2
* &lbrack;Shelf&rbrack; Nuevos sombreadores : Dota 2, pintura de coches PBR, revestimiento PBR, terciopelo PBR
* &lbrack;Shelf&rbrack; Nuevo material : Óxido de acero y desgaste, iluminación estilizada
* &lbrack;Shelf&rbrack; Nuevos filtros : Difuminado direccional, iluminación estilizada
* &lbrack;Shelf&rbrack; Nuevo pincel : disco duro por defecto suave y duro por defecto con un nuevo alfa para un mejor control de la dureza
* &lbrack;Shelf&rbrack; Nuevos generadores : Distancia y luz 3D
* &lbrack;Shelf&rbrack; Pinceles actualizados con proyección de ceñido y sacrificio de caras posteriores (activado de forma predeterminada)
* &lbrack;Shelf&rbrack; Se ha actualizado Ruido blanco con la versión de procesador de píxeles para agilizar el cálculo

**Corregido:**

* &lbrack;Pantalla de bienvenida&rbrack; Tutorials vínculo enviar a vídeos antiguos
* &lbrack;Canales&rbrack; Si se indica &quot;no&quot; para rellenar la creación de capas con AO, se sigue creando la capa
* &lbrack;Canales&rbrack; Los nombres de canales UserX no se propagan en la interfaz
* &lbrack;Viewport&rbrack; La entrada de máscara está vacía en la lista de canales solo
* &lbrack;Compartir&rbrack; Exportar un alfa para compartir desde SP crea un archivo .image ilegible
* &lbrack;Licencia&rbrack; Solucionar problemas de activación para nombres de usuario con caracteres que no sean ASCII
* &lbrack;Sombreador&rbrack; El cuadro de diálogo de parámetros de color desaparece al seleccionar un color
* &lbrack;Shelf&rbrack; Las miniaturas no se descargan de la memoria cuando no se utilizan
* &lbrack;Shelf&rbrack; Filtro de degradado fijo
* &lbrack;Herramienta&rbrack; La simetría no funciona con la galería de símbolos o la proyección
* &lbrack;Herramienta&rbrack; Nombre incorrecto al crear un nuevo ajuste preestablecido de pincel
* La opción Conservar trazo permanece desactivada incluso al volver a importar una malla
* Restablecimiento del controlador (TDR) al calcular partículas con un tamaño grande.

### 1.6.1

*(Lanzado: 09 de noviembre de 2015)*

**Corregido:**

* Bloqueo al abrir el proyecto si Vista 2D está visible
* Bloqueo al crear un nuevo ajuste preestablecido de exportación si el estante actual no existe
* &lbrack;Herramienta&rbrack; El icono del selector de material puede permanecer visible
* &lbrack;Herramienta&rbrack; El selector de material oculta el cursor del ratón al pintar al mismo tiempo
* &lbrack;Shelf&rbrack; Los metadatos se escriben en el disco después de cada salida

### 1.6.0

*(Lanzado: 29 de octubre de 2015)*

**Agregado:**

* Compatibilidad oficial con Windows 10
* &lbrack;Substance&rbrack; Contraer grupos de parámetros de sustancia de forma predeterminada
* &lbrack;Substance&rbrack; Añadir nueva estructura (mejorar el rendimiento del Procesador de píxeles)
* &lbrack;Viewport&rbrack; Permita desactivar la visualización del plano de simetría en el modo de simetría.
* &lbrack;Viewport&rbrack; Mejorar el procesamiento y el rendimiento de las sombras
* &lbrack;Viewport&rbrack; Pausar cálculo de sombras al pintar
* &lbrack;Viewport&rbrack; Mejorar el rendimiento de representación de malla metálica
* &lbrack;Motor&rbrack; Mejorar la administración de la memoria Vram para reducir su huella
* &lbrack;Motor&rbrack; Mejore la actualización de la textura en las GPU AMD para obtener un mejor rendimiento
* &lbrack;Motor&rbrack; Deshabilite la configuración de optimización enlazada en GPU NVIDIA para obtener un mejor rendimiento
* &lbrack;Efecto&rbrack; Añada una etiqueta para solicitar la entrada de imagen &quot;acolchada&quot;
* &lbrack;Capa&rbrack; Aumentar la precisión del Desplazamiento de UV/escala en el relleno
* &lbrack;Capa&rbrack; Hacer que el regulador de escala sea exponencial en el relleno
* &lbrack;Capa&rbrack; Permita arrastrar y soltar materiales directamente en la pila de capas.
* &lbrack;Capa&rbrack; Permitir arrastrar y soltar filtros directamente en la pila de capas
* &lbrack;Capa&rbrack; Ajustar el color del pincel de máscara al color de máscara recién creado
* &lbrack;Sombreador&rbrack; Exponer varias texcocords
* &lbrack;Sombreador&rbrack; Función de asignación de gamma y tono para permitir funciones personalizadas
* &lbrack;Bakeres&rbrack; Cambiar la configuración predeterminada del baker de posición para el uso TriPlanar
* &lbrack;Herramienta&rbrack; Cambie el nombre &quot;Geometry Decal&quot; por &quot;Polygon Fill&quot;.
* &lbrack;Shelf&rbrack; Actualice los generadores para que sean compatibles con TriPlanar : MG Desgaste del borde del metal, MG Constructor de la máscara, MG Fibra de vidrio, MG Dirt
* &lbrack;Shelf&rbrack; Actualizar materiales con nuevas configuraciones y eliminar materiales no utilizados
* &lbrack;Shelf&rbrack; 22 materiales inteligentes nuevos (plástico, hierro, tela, acero y más)
* &lbrack;Shelf&rbrack; Actualiza los filtros Enfocar, Desenfocar y Deformar con entrada de imagen acolchada para evitar costuras
* &lbrack;Shelf&rbrack; Mejora de la configuración de deformación para facilitar su uso
* &lbrack;Shelf&rbrack; 2 Nuevos ruidos procedimientos : Ruido de Perlin 3D y ruido de Worley 3D

**Corregido:**

* &lbrack;Motor&rbrack; La detección de la cantidad de Vram para la GPU dedicada es incorrecta en Mac
* &lbrack;Motor&rbrack; Las texturas se convierten en una versión más oscura en la ventana gráfica
* &lbrack;Motor&rbrack; Rendimiento deficiente al pintar debajo de varias capas
* &lbrack;Motor&rbrack; Las capas calculadas al abrir el proyecto difieren de la versión almacenada en caché
* &lbrack;Substance&rbrack; Resultados incorrectos en 4K en Mac
* &lbrack;Substance&rbrack; Los parámetros están en el orden incorrecto
* &lbrack;Sombreador&rbrack; Los sombreadores de tono y pixelado son totalmente negros
* &lbrack;Sombreador&rbrack; Los parámetros desaparecen después de cambiar el mapa de entorno
* &lbrack;Shelf&rbrack; Bloqueo al colocar archivos png en la carpeta generator
* &lbrack;Shelf&rbrack; Las miniaturas se generan con una rugosidad baja
* &lbrack;Herramienta&rbrack; Bloqueo al utilizar un mapa de bits en el pincel alfa en windows
* &lbrack;Exportar&rbrack; El ajuste preestablecido de exportación de mapa adicional ahora exporta un mapa del RGB para Posición

### 1.5.7

*(Lanzado: 24 de septiembre de 2015)*

**Corregido:**

* El informe de bloqueos ya no funciona

### 1.5.6

*(Lanzado: 21 de septiembre de 2015)*

**Agregado:**

* &lbrack;Shelf&rbrack; Mejora la calidad de representación de miniaturas (utiliza texturas 1K)

**Corregido:**

* &lbrack;Compartir&rbrack; Imposible firmar con otra cuenta
* &lbrack;Shelf&rbrack; Las miniaturas pesan demasiado en el disco
* &lbrack;Shelf&rbrack; Los materiales inteligentes son muy lentos de cargar
* &lbrack;Windows&rbrack; Solucionar problemas de instalación del servicio de licencias
* &lbrack;Canales&rbrack; El mapa de transmisivo se crea como G8 de forma predeterminada

### 1.5.5

*(Lanzado: 15 de septiembre de 2015)*

**Agregado:**

* &lbrack;Shelf&rbrack; Exportar contenidos a Substance share
* &lbrack;Shelf&rbrack; Adición de una nueva previsualización de esfera para materiales
* &lbrack;Shelf&rbrack; Utilice el mapa de env &quot;Patio acristalado&quot; para generar miniaturas
* &lbrack;Shelf&rbrack; Aumentar resolución de tamaño de miniatura a 512x512 píxeles
* &lbrack;Vista 3D&rbrack; Exponer valor de rotación de entorno
* &lbrack;Windows&rbrack; Firmar la aplicación

**Corregido:**

* &lbrack;Bakeres&rbrack; Resultados incorrectos al hacer un bake mapas al mismo tiempo
* &lbrack;Vista 3D&rbrack; El mapa de env se muestra cuando no hay ningún proyecto abierto
* &lbrack;Capas&rbrack; Los generadores de máscaras no funcionan en el contenido de capas
* &lbrack;Capas&rbrack; Puede realizar la pintura en capas ocultas
* &lbrack;Shelf&rbrack; El dirt_5 y el Dirt_6 son idénticos
* &lbrack;Shelf&rbrack; Algunos generadores de máscaras están pixelados o son de baja calidad
* &lbrack;Herramienta&rbrack; Rotación de gizmo incorrecta en determinados ángulos.
* &lbrack;Herramienta&rbrack; Si hay demasiados canales, los botones de canal se recortan
* &lbrack;Herramienta&rbrack; El método abreviado de inversión de máscara para Máscara rápida no funciona
* &lbrack;Exportar&rbrack; Bocetos: el botón de cancelación no se ha tenido en cuenta correctamente
* &lbrack;Licencia&rbrack; Error de activación cuando no se puede copiar la licencia
* El limitador de velocidad de fotogramas ya no funciona en la IU

### 1.5.0

*(Lanzado: 20 de agosto de 2015)*

**Agregado:**

* &lbrack;Sombreador&rbrack; Agregar número de línea en Sombreador compilando mensajes de error
* &lbrack;Shelf&rbrack; Mejorar la calidad de las vistas previas en miniaturas
* &lbrack;Shelf&rbrack; Generación automatizada de miniaturas para Materiales inteligentes
* &lbrack;Herramienta&rbrack; Método abreviado para controlar el ajuste de la dureza en la sustancia
* &lbrack;Herramienta&rbrack; Usar el widget de escala de grises para la pegatina geométrica al pasar sobre una máscara
* &lbrack;Herramienta&rbrack; Método abreviado para invertir el color de la pintura mientras se pinta en un mapa en escala de grises
* &lbrack;Viewport&rbrack; Permitir mostrar la malla metálica y cambiar su color
* &lbrack;Viewport&rbrack; Desenfocar el fondo del entorno
* &lbrack;Controles&rbrack; Añadir rotación a los métodos abreviados de pincel del ratón
* &lbrack;Exportar&rbrack; Exportar a Sketchfab
* &lbrack;Exportar&rbrack; Creación de ajustes preestablecidos de exportación para procesadores
* &lbrack;Exportar&rbrack; Añadir reflejo del mapa convertido, F0 y 1/IOR
* &lbrack;UI&rbrack; Pantalla Añadir bienvenida
* &lbrack;UI&rbrack; Actualizar diseño predeterminado
* &lbrack;UI&rbrack; Añadir información sobre herramientas que falta y cambiar el nombre de alguna entrada del menú
* &lbrack;Capas&rbrack; Exportar la máscara seleccionada actualmente como mapa de bits
* &lbrack;Capas&rbrack; Añade la acción &quot;invertir máscara&quot; en el menú del botón derecho

**Corregido:**

* &lbrack;Proyecto&rbrack; Si los pivotes de las mallas son diferentes en el FBX, las mallas se explotan al importar
* &lbrack;Substance&rbrack; Los Substance utilizados en las herramientas de proyección están bloqueados en 256\*256
* &lbrack;Capas&rbrack; Bloqueo al utilizar la opción borrar máscara
* &lbrack;Exportar&rbrack; Conversión de gamma incorrecta en texturas muy oscuras
* &lbrack;Exportar&rbrack; El mapa de posición solo se puede utilizar en los ajustes preestablecidos de exportación como mapa de escala de grises
* &lbrack;Herramienta&rbrack; El color de inicio de la calcomanía geométrica es negro cuando se utiliza en una máscara
* &lbrack;Herramienta&rbrack; El método abreviado de rotación no funciona si no hay dureza en el alfa

### 1.4.2

*(Lanzado: 15 de julio de 2015)*

**Corregido:**

* &lbrack;Herramienta&rbrack; Bloqueo al utilizar la pegatina geométrica con máscara rápida
* La actualización de un proyecto de la versión 1.4.0 a la 1.4.1 consume toda la memoria del equipo
* Importación incorrecta del formato de proyecto antiguo
* Los estantes personalizados analizan toda la jerarquía y duplican activos en todas partes

### 1.4.1

*(Lanzado: 23 de junio de 2015)*

**Agregado:**

* &lbrack;Viewport&rbrack; Permitir acoplar paneles uno al lado del otro
* &lbrack;Efecto&rbrack; Adición de un fondo y una regla para el efecto de nivel
* &lbrack;Efecto&rbrack; Añada un efecto de Pintura que permita trabajar sobre otro efecto

**Corregido:**

* &lbrack;Shelf&rbrack; La generación de miniaturas se interrumpe si no hay ningún proyecto abierto
* &lbrack;Shelf&rbrack; La previsualización de ajustes preestablecidos de material no se genera
* &lbrack;Shelf&rbrack; Las previsualizaciones de material se generan en una malla con normales invertidas
* &lbrack;Shelf&rbrack; Las miniaturas siempre se vuelven a calcular debido a una función hash incorrecta
* &lbrack;Shelf&rbrack; Hacer clic en un material de Substance no conecta mapas adicionales
* &lbrack;Herramienta&rbrack; Valor incorrecto muestreado con el selector de material
* &lbrack;Herramienta&rbrack; Color del cursor de ventanilla de selección del selector de color
* &lbrack;vista 2D&rbrack; Velocidad de fotogramas/rendimiento muy baja
* &lbrack;Exportar&rbrack; Bloqueo al abrir la ventana de exportación con ajustes preestablecidos de exportación demasiado recientes.
* &lbrack;Exportar&rbrack; El canal de height al Mapa de normales se convierte en el espacio incorrecto
* &lbrack;Mac&rbrack; El color base de los efectos de Substance se muestra como lineal
* &lbrack;Mac&rbrack; El widget de líneas rectas se dibuja incorrectamente en Retina
* Las líneas rectas pueden permanecer activadas incluso con el método abreviado liberado.
* Las líneas rectas del guizmo desaparecen después de rotar el mapa de entorno
* Las salidas de oclusión ambiental de sustancias no se conectan automáticamente al canal AO
* Solucionar el problema de copia de licencia en Windows con un carácter especial en el nombre de usuario

### 1.4.0

*(Lanzado: 10 de junio de 2015)*

**Agregado:**

* &lbrack;Exportar&rbrack; Añadir mapas adicionales en la lista de los mapas de entrada disponibles
* &lbrack;Shelf&rbrack; Usar materiales sbsar como ajustes preestablecidos de materiales
* &lbrack;Shelf&rbrack; Permitir el uso de rutas de biblioteca personalizadas
* &lbrack;Shelf&rbrack; Cambiar el tamaño mínimo
* &lbrack;Shelf&rbrack; Nuevo contenido : 20 materiales inteligentes nuevos
* &lbrack;Shelf&rbrack; Nuevo contenido : nueva sustancia procedimienta (tejido, malla)
* &lbrack;Shelf&rbrack; Filtro de desenfoque actualizado
* Dibujo de líneas rectas mediante una tecla modificadora
* Adición de un canal de Oclusión ambiental y modificación del comportamiento AO/Normal en la pila de capas
* Leer el color predeterminado de la entrada de imagen definida en los datos de usuario del Substance
* Permitir la exportación del registro desde el menú de ayuda

**Corregido:**

* &lbrack;Baker&rbrack;&lbrack;Mac&rbrack; Bloqueo con baker Normal desde malla
* &lbrack;Baker&rbrack; Bloqueo si no hay UV en el archivo de la jaula
* &lbrack;Baker&rbrack; La coincidencia por nombres no funciona con OBJ exportados desde zBrush
* &lbrack;Baker&rbrack; Hacer un bake con una jaula sobrescribe hacer un bake si se utilizan varios conjuntos de texturas y UV superpuestos
* &lbrack;Baker&rbrack; Los archivos OBJ específicos dan como resultado texturas negras
* &lbrack;Shelf&rbrack; No se pueden leer los recursos si se establece como de sólo lectura
* &lbrack;Shelf&rbrack; Los archivos de recursos se escriben en Painter si se han utilizado en el proyecto.
* &lbrack;Shelf&rbrack; La recarga de sustancias también actualiza la capa
* &lbrack;Exportar&rbrack; Tiff exporta imágenes de 32 bits que Photoshop o los motores de juegos no pueden leer correctamente
* &lbrack;Exportar&rbrack; El ajuste preestablecido de canales predeterminados siempre exporta como RGB
* &lbrack;Material&rbrack; Asignación de BaseColor con substancias en anulación de canal de Difuso
* &lbrack;Vista 3D&rbrack; Iluminación de Difuso incorrecta con mapas de entorno específicos
* &lbrack;Herramienta&rbrack; No se puede rotar un pincel a un ángulo específico
* La ventana gráfica se enfoca al pasar el cursor por encima mientras se escribe en un campo de texto
* Bloqueo con ajustes preestablecidos demasiado recientes para la versión actual del estante
* Bloqueo después de reemplazar la malla
* Bloqueo al volver a cargar una sustancia con un número diferente de entradas
* FBX mallas de la importación de Cinema4D con nombres de material incorrectos

### 1.3.5

*(Lanzado: 29 de mayo de 2015)*

**Agregado:**

* &lbrack;Licencia&rbrack; Problema de activación cuando ya hay un archivo de licencia
* &lbrack;Mac&rbrack; Bloqueo al cargar archivos FBX específicos
* &lbrack;Mac&rbrack;&lbrack;Vista 3D&rbrack; Reflejo incorrecto para la GPU integrada
* &lbrack;Vista 3D&rbrack; La fuente de la máscara rápida está rota
* &lbrack;Vista 3D&rbrack; El selector de material hace que la ventana gráfica sea totalmente negra
* Bloqueo después de abrir proyectos creados en 1.3.3
* La previsualización de material está vacía al utilizar sombreadores con alfa
* La pintura deja de funcionar en mallas específicas
* Las prestaciones disminuyen mucho con mallas OBJ específicas
* Los canales de usuario no se asignan al utilizar efectos
* Las carpetas temporales no se limpian al inicio

**Corregido:**

* Mejoras de tiempo de cálculo en el proyecto extremadamente largo de carga
* Cambie la ventana &quot;Solución de problemas de GPU&quot; para que sea más comprensible
* &lbrack;Capas&rbrack; Guarde el estado del bloqueo de proporción para las capas de relleno y active esta opción de forma predeterminada
* &lbrack;Bakeres&rbrack; La coincidencia por nombre ahora usa el sufijo como separador

### 1.3.4

*(Lanzado: 27 de abril de 2015)*

**Agregado:**

* &lbrack;Mac&rbrack; Bloqueo con Mac OS X Yosemite (10.10)
* &lbrack;Mac&rbrack; Imposible salir del modo de pantalla completa
* &lbrack;Bakeres&rbrack; La opción de hacer un bake coincidencia por nombre no funciona
* &lbrack;Bakeres&rbrack; El espacio de tangente de tinta utilizado en SP no funciona con UE4
* &lbrack;Bakeres&rbrack; El baker de ID. no puede hacer un bake colores de ID. de material
* &lbrack;vista 2D&rbrack; La malla metálica no aparece al utilizar la herramienta Calcomanía geométrica
* &lbrack;Herramienta&rbrack; El canal alfa del pincel se muestra como verificador en lugar de como transparencia con los materiales
* &lbrack;Herramienta&rbrack; Bloqueo con pegatina geométrica
* &lbrack;Capas&rbrack; La ranura de material se contrae de forma predeterminada en la capa Relleno
* &lbrack;Exportar&rbrack; Bloqueo al exportar a un tamaño mayor que la resolución del conjunto de texturas
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
* &lbrack;Shelf&rbrack; Añadir nuevos mapas de entorno : Corsica beach, studio 05, Tornoco studio y más
* &lbrack;Shelf&rbrack; Actualizar MG Mask Builder con nuevos parámetros
* &lbrack;Shelf&rbrack; Actualización y calibración de mapas de entorno antiguos

**Corregido:**

* Bloqueo al abrir la ventana de exportación
* No es posible arrastrar y soltar en el widget de interfaz de usuario cuando no está acoplado
* &quot;Buscar actualizaciones&quot; no funciona
* &lbrack;Capas&rbrack; No seleccionar la máscara al pulsar ALT + clic en ella
* &lbrack;Herramienta&rbrack; Tri-plana no funciona con el canal Normal
* &lbrack;Vista 3D&rbrack; La iluminación del mapa de env es incorrecta
* &lbrack;Vista 3D&rbrack; El cálculo de la exposición es diferente de Designer
* &lbrack;Vista 3D&rbrack; Las sombras no deben ser visibles en superficies 100 % metálicas
* &lbrack;Vista 3D&rbrack; La malla con UV reflejados tiene tangentes/binomales volteados
* &lbrack;Vista 3D&rbrack; Las sombras producen resultados incorrectos en determinadas mallas
* &lbrack;Bakeres&rbrack; Eliminar la carpeta &quot;.alg_meta&quot; creada por los archivos de asignación
* &lbrack;Bakeres&rbrack; Bloqueo al hacer un bake si Painter vuelve a calcular un TextureSet al mismo tiempo
* &lbrack;Mac&rbrack; Error de IU de White Box al iniciar la aplicación

### 1.3.2

*(Lanzado: 6 de marzo de 2015)*

**Corregido:**

* &lbrack;Vista 3D&rbrack; No es posible volver a cargar un mapa env guardado con el proyecto

### 1.3.1

*(Lanzado: 5 de marzo de 2015)*

**Agregado:**

* &lbrack;Bakeres&rbrack; Agregar una versión en caché de mallas de alta densidad de poli para acelerar el cálculo
* &lbrack;Bakeres&rbrack; Añada un icono de advertencia si no se ha cargado ninguna malla de alta densidad
* &lbrack;Bakeres&rbrack; Si no se carga ninguna malla de alta densidad, utilice en su lugar la malla del proyecto

**Corregido:**

* &lbrack;Bakeres&rbrack; Al pulsar &quot;Intro&quot; al editar el valor de un regulador, cierre la ventana
* &lbrack;Bakeres&rbrack; La activación/desactivación de un baker también activará el botón
* &lbrack;Bakeres&rbrack; Imposible de hacer un bake si utiliza el botón &quot;all/none&quot;
* &lbrack;Bakeres&rbrack; La ordenación de los botones del baker no está en el orden correcto
* &lbrack;Bakeres&rbrack; Las casillas se omiten y todos los bakeres siempre se procesan
* &lbrack;Bakeres&rbrack; Progreso de la barra de progreso fijo

### 1.3.0

*(Lanzado: 4 de marzo de 2015)*

**Agregado:**

* &lbrack;Bakeres&rbrack;&lbrack;Vista 3D&rbrack; Usar cálculo de espacio de tangente Mikkt si no se encuentran tangentes/binormales
* &lbrack;Bakeres&rbrack; Se han añadido nuevos bakeres : Normal, ID, Oclusión, Curvatura, Thickness, Posición
* &lbrack;Efectos&rbrack; La pila de efectos ahora se invierte y se muestra de arriba abajo (como capas)
* &lbrack;Efectos&rbrack; Añadir nuevos iconos en la pila de efectos
* &lbrack;Efectos&rbrack; Añadir modo de fusión entre acciones de relleno en la pila de efectos
* &lbrack;Efectos&rbrack; Cambiar nombre de efectos (efecto de sustancia = filtro, etc.)
* Añadir un archivo &quot;lock&quot; durante el proceso de guardado
* &lbrack;Efectos&rbrack; Agregar acción de relleno en la pila de efectos
* Se ha añadido un nuevo recurso : Materiales inteligentes
* &lbrack;Capas&rbrack; Permitir reordenar efectos de capa
* &lbrack;Herramienta&rbrack; Agregar proyección Tri-Plana
* &lbrack;Vista 3D&rbrack; Añadir compatibilidad con sombras
* &lbrack;Vista 3D&rbrack; Posibilidad de definir los estados de OpenGL necesarios en sombreadores personalizados
* &lbrack;Vista 3D&rbrack; Compatibilidad con alfa mediante nuevos sombreadores
* &lbrack;Vista 3D&rbrack; Ahora se crean versiones de los sombreadores y se guardan completamente en un proyecto
* &lbrack;Vista 3D&rbrack; Avisar al usuario si el sombreador ya no se compila

**Corregido:**

* &lbrack;Capas&rbrack; corregir colocación en una carpeta contraída
* &lbrack;Shelf&rbrack; Corrección del filtrado de contenido en miniestantes
* &lbrack;Shelf&rbrack; Cambiar el nombre de categorías y reorganizar pestañas

### 1.2.1

*(Lanzado: 12 de febrero de 2015)*

**Agregado:**

* Los archivos \*.spp ahora se pueden abrir haciendo doble clic en el explorador
* &lbrack;Exportar&rbrack; Nueva etiqueta &quot;$project&quot; para los ajustes preestablecidos de exportación
* &lbrack;Exportar&rbrack; Añadir lista de mapas (con nomenclatura) debajo de cada conjunto de texturas
* &lbrack;Exportar&rbrack; Añada un botón Todo/Ninguno para seleccionar los conjuntos de texturas
* &lbrack;Exportar&rbrack; Los mapas vacíos se descartan durante la exportación

**Corregido:**

* &lbrack;Exportar&rbrack; Los ajustes preestablecidos de Unity5 tienen mapas invertidos
* &lbrack;Exportar&rbrack; Si se añade una barra diagonal en un nombre de ajuste preestablecido, se creará una carpeta dañada
* &lbrack;Exportar&rbrack; El canal de height exportado en formatos de 32 bits no está sujeto correctamente
* &lbrack;Exportar&rbrack; La lista de conjuntos de texturas no se ordena como en el proyecto
* &lbrack;Herramienta&rbrack; El sacrificio de la cara posterior ya no funciona
* Guardar no funciona con caracteres especiales en el trazado

### 1.2.0

*(Lanzado: 28 de enero de 2015)*

**Agregado:**

* Nuevo canal Normal que permite la pintura de datos de mapa de normales y combinar los resultados
* &lbrack;Exportar&rbrack; Nueva ventana de exportación con la capacidad de crear empaquetados personalizados y definir nombres personalizados
* El formato del archivo de proyecto ahora es un único archivo en lugar de carpetas
* &lbrack;Exportar&rbrack; Admite diferentes formatos normales (DirectX, OpenGL)
* &lbrack;Exportar&rbrack; Crear un archivo de bloqueo temporal durante la exportación
* &lbrack;Capas&rbrack; Mayús + clic izquierdo del ratón se puede utilizar para cambiar una máscara
* &lbrack;Parámetros&rbrack; Exponer el espacio de color en la parte inferior de una entrada de imagen
* &lbrack;Shelf&rbrack; Efecto &quot;MG Mask Builder&quot; ahora tiene nuevos ajustes
* &lbrack;Vista 3D&rbrack; El mapa de oclusión ambiental ahora oculta el aporte difuso, no el specular

**Corregido:**

* El material de proyección o la previsualización de la galería de símbolos no se muestran correctamente en la ventana gráfica
* &lbrack;Vista 3D&rbrack; La información sobre herramientas de método abreviado no se muestra al utilizar métodos abreviados &quot;S&quot; (esténcil)
* &lbrack;Shelf&rbrack; El efecto &quot;MatFx Skin Scale&quot; tiene ahora mejores prestaciones en baja resolución
* &lbrack;Exportar&rbrack; Las texturas de la exportación solo se aumentan al especificar un tamaño de documento más grande

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

* &lbrack;Capa&rbrack; Seleccionar la capa superior al abrir un proyecto o cambiar un conjunto de texturas
* Se ha mejorado la velocidad de &quot;Guardar&quot; y &quot;Guardar como&quot; con el nuevo algoritmo de compresión
* Mostrar un error al abrir un proyecto demasiado reciente para Painter

**Corregido:**

* &lbrack;Herramienta&rbrack; La calcomanía geométrica produce corrupciones de memoria
* &lbrack;Brush&rbrack; No es posible introducir manualmente valores flotantes por debajo de 1 para el tamaño de pincel
* &lbrack;Capa&rbrack; Crear un efecto de selección de color no lo añade a la pila de capas
* &lbrack;Capa&rbrack; Al mover el ratón sobre las capas, Painter se mueve en la barra de tareas
* &lbrack;Capa&rbrack; Añadir un mapa de bits como máscara puede provocar un bloqueo
* La interfaz gráfica de usuario para el modo solo con el canal de Height es incorrecta
* &quot;Guardar proyecto&quot; puede dar error y dañar un proyecto
* Bloqueo al abrir un proyecto después de cargar otro con un sombreador obsoleto

### 1.1.0

*(Lanzado: 16 de diciembre de 2014)*

**Agregado:**

* &lbrack;Efecto&rbrack; Nuevo creador de máscaras de ID de material
* Nueva línea punteada blanca/negra para el gizmo del pincel
* Nuevo parámetro de seguimiento de ángulo
* Nuevo parámetro de sacrificio de la cara posterior
* Nuevo parámetro de Ratón perezoso
* &lbrack;Capas&rbrack; Compatibilidad con varias selecciones y administración
* &lbrack;Capas&rbrack; Copiar y pegar de un conjunto de texturas entre sí
* &lbrack;Exportar&rbrack; Formato de PSD de Adobe Photoshop
* &lbrack;Shelf&rbrack; Nueva herramienta : piel, puntadas metálicas y cremallera
* &lbrack;Shelf&rbrack; Nuevo pincel : molde, lápiz, línea afilada y puntada
* &lbrack;Shelf&rbrack; Nuevo alfa : Ruido gaussiano, línea afilada, molde, pluma, salpicadura, puntada, cremallera
* Se han mejorado las prestaciones de pintura actualizando solo partes de las texturas necesarias

**Corregido:**

* &lbrack;Shelf&rbrack; Imposible cargar una sustancia con un gráfico que tiene etiquetas idénticas
* &lbrack;Capas&rbrack; El modo de fusión Pass Through no funciona con máscaras
* &lbrack;Stencil&rbrack; La escala se rompe en el Vista 2D
* Problemas y bloqueo en el sistema operativo Mac Yosemite

### 1.0.2

*(Lanzado: 09 de noviembre de 2014)*

**Agregado:**

* Rendimiento mejorado en la previsualización de materiales con sustancias
* Se han mejorado las prestaciones con la vista previa del trazo de pincel al actualizar el documento
* Rendimiento mejorado en la ventana gráfica con una velocidad de actualización más baja para el área no operativa
* &lbrack;Efectos de posprocesamiento&rbrack; Interfaz de usuario mejorada para administrar la configuración
* &lbrack;Efectos de posprocesamiento&rbrack; Restablecer los valores predeterminados
* Operaciones de capas y efectos de Substance en el menú contextual
* Apoyo a los insumos/productos premultiplicados en sustancias

**Corregido:**

* &lbrack;Vista 3D&rbrack; Los parámetros de sombreador personalizados están separados por un espacio grande
* &lbrack;Exportar&rbrack; Falta la conversión sRGB para el ajuste preestablecido Unity4
* Posible Bloqueo al cargar mallas fbx
* Bloqueo a veces al cargar mallas obj simples
* La barra de cálculo permanece bloqueada al 100% al cargarse
* Volver a cargar una sustancia la coloca en todas las categorías
* Interruptor DirectX/OpenGL roto

### 1.0.1

*(Lanzado: 27 de octubre de 2014)*

**Agregado:**

* &lbrack;Herramienta&rbrack; Uso de parámetros de material mejorado
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
* &lbrack;Exportar&rbrack; Añadir un pase de dilatación antes del postproceso de difusión
* Argumentos de la línea de comandos en SP para operaciones simples
* Nuevos materiales y efectos
* Previsualización de herramientas (área separada de previsualización de materiales en tiempo real y prueba de trazos)
* No crear un documento predeterminado al iniciar Painter
* &lbrack;Herramienta&rbrack; Añadir la posibilidad de editar manualmente un valor de escala de grises
* Varias mejoras para los patrones (Ajustar, Restablecer)
* Las partículas son ahora subherramientas de las herramientas Pincel, Borrador y Proyección
* &lbrack;Vista 3D&rbrack; Usar AO hecho un bake en el procesamiento de la ventana gráfica
* División de los controles de galerías de símbolos entre la vista 2D y 3D
* Ajuste de tamaño de pulgar pequeño en la biblioteca
* Los campos de búsqueda son específicos de cada ventana
* Ajuste de IU

**Corregido:**

* &lbrack;Substance&brack; El conmutador no funciona
* &lbrack;Diálogo de color&rbrack; Degradado de tono no actualizado
* No es posible actualizar una malla si el nombre del archivo es idéntico
* La herramienta no está visible en las vistas cuando es demasiado pequeña
* La herramienta de pegatina de la pantalla Retina no funciona correctamente
* &lbrack;Substance&rbrack; Int1 se muestran como float1
* &lbrack;Substance&rbrack; no se reconoce la entrada/salida basecolor
* &lbrack;Substance&rbrack; los filtros no se pueden volver a cargar
* &lbrack;Herramienta&rbrack; el widget de escala de grises siempre está contraído

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
* &lbrack; y &brack; Métodos abreviados de teclado para Tamaño de pincel
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
