---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/release-notes/old-versions/version-2017-3.html"
breadcrumb-title: ''
description: Consulte las notas de la versión 2017.3 de Substance 3D Painter para obtener más información sobre las nuevas funciones, mejoras y correcciones de errores.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2017.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versión 2017.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 0%

---


# Versión 2017.3

**Substance Painter 2017.3** se centra en el nuevo ajuste preestablecido de exportación avanzado con la compatibilidad del **Proyecto de Adobe Felix** y el formato abierto **glTF**. Esta nueva versión también se centra en la experiencia del usuario, ya que mejora la interfaz y añade un plugin de guardado automático.

Fecha de publicación : *28 de septiembre de 2017*

## Funciones principales

### Ajuste preestablecido de exportación de Adobe Standard Material

![](../../assets/adobe-dimension-meetmat.jpg)

Uno de los nuevos exportadoras que incluimos en esta versión es el soporte del Adobe Standard Material, que se utilizará con Adobe Dimension (anteriormente, Adobe Project Felix). Le permitimos exportar la malla de escenas y sus texturas para importarlas en el proyecto Felix con un solo clic. Para acceder a él, solo tiene que elegir &quot;**Adobe Standard Material**&quot; en la ventana de texturas de exportación. Para obtener más información, consulte: [http://www.adobe.com/es/products/dimension.html](https://www.adobe.com/es/products/dimension.html)

También puedes consultar nuestra entrada de blog sobre ello : <https://www.allegorithmic.com/blog/new-dimension-substance-ecosystem>

### ajuste preestablecido de exportación glTF 2.0

![](../../assets/gltf-export.jpg)

También hemos agregado compatibilidad con el formato de archivo **glTF**, con la exportación de la **malla de escena** y las **texturas PBR** (metálicas/rugosas). Para acceder a él, solo tiene que elegir &quot;**glTF PBR Metal Roughness**&quot; en la ventana texturas de exportación. **glTF** es un formato de archivo de código abierto dirigido por el grupo Khronos. Puedes ver tu archivo glTF desde **Windows 10** o simplemente usar un visor de WebGL como [**Babylon**](http://sandbox.babylonjs.com/).

Para obtener más información, consulte: <https://github.com/KhronosGroup/glTF>

### Complemento de autoguardado

![](../../assets/autosave-details.png)

En esta versión también incluimos un nuevo complemento que tiene la posibilidad de **crear copias de seguridad** del proyecto abierto actualmente. Crea un archivo de copia de seguridad en el lateral del proyecto abierto actualmente.\
Por ello, también hemos añadido una entrada &quot;**Guardar como copia**&quot; en el menú Archivo. El **autosave** se puede detener deshabilitando el plugin, se puede acceder a su **configuración** a través del panel de configuración **.** Cuando se alcanza el retraso del tiempo de advertencia, aparece una **barra de progreso** debajo del botón en la barra de herramientas principal, lo que permite posponerlo durante unos minutos si es necesario (útil si desea finalizar algo antes de la copia de seguridad).

Si se crea una copia de seguridad pero el proyecto no se ha guardado (también conocido como Untilted), la copia de seguridad se almacenará dentro de la carpeta **Documents/Allegorithmic/Substance Painter/autosave**. De lo contrario, la copia de seguridad estará junto al proyecto en sí (a menos que el panel de configuración reemplace la ruta de acceso).

### Filtro de degradado mejorado

![](../../assets/gradient-rust.jpg)

El **filtro de degradado** se ha renovado por completo. Actuando de una manera mucho más similar al nodo **gradient map** disponible en **Substance Designer**. Ahora admite hasta **10 colores diferentes**, con la posibilidad de especificar **dónde se ubica el color dentro de** el degradado **&#x200B;**, lo que abre muchas puertas nuevas. Esto permite crear más **patrones de color avanzados**, pero también **reasignar mapas de altura**&#x200B;y crear **nuevas formas**.

El regulador principal (cantidad de color) define el número de colores totales utilizados para crear el degradado. El botón situado justo debajo define el modo de fusión de color (sRGB o Lineal). Esto es importante si desea tener una fusión adecuada entre colores. Por ejemplo, mezclar un rojo puro y un verde puro debería dar un amarillo bonito en medio. Este no será el caso si el botón está desactivado (se dará un marrón oscuro en su lugar). Al reasignar el height o cualquier otro canal de escala de grises, este botón debe desactivarse para evitar la conversión de gamma.

El botón de arriba permite reemplazar el resultado del filtro con el degradado en sí, para visualizar el degradado en el Vista 2D.

![](../../assets/gradient-height-demo.jpg)

### Mejoras de interfaz y comportamiento

![](../../assets/tabs-top.png)

En esta versión, las **pestañas** de los diferentes muelles de la aplicación se encuentran ahora **en la parte superior en lugar de en la parte inferior** de sus respectivas ventanas. Esta elección se hizo para ayudar a la legibilidad de la interfaz, pero también para ser más coherente con otra aplicación. A continuación de este cambio, aparece la **pequeña cruz** junto al título de la pestaña para **cerrarla fácilmente**. También es posible **hacer clic con el botón derecho** en la pestaña para abrir un **menú contextual** (que permite cerrar o desacoplar la ventana). Un método abreviado para desacoplar la ventana es simplemente arrastrar y soltar la pestaña fuera del área de la ventana.

Ahora también es posible **abrir proyectos** simplemente arrastrándolos y soltándolos **en la ventana gráfica** desde el explorador de archivos. Esto también funciona con archivos **mesh** : arrastrar y soltar un archivo de malla en una **ventana gráfica vacía** abrirá la **ventana de nuevo proyecto**, pero si lo haces en un **proyecto ya abierto**, se abrirá el **cuadro de diálogo de configuración del proyecto**, lo que permitirá **actualizar una malla** rápidamente.

**Nota**: si tienes problemas al arrastrar y soltar, asegúrate de[comprobar nuestras preguntas frecuentes sobre el tema](../../technical-support/technical-issues/miscellaneous-issues/impossible-to-drag-and-drop-files-into-the-shelf.md).

### Mejoras de rendimiento

Esta versión de Substance Painter también incluye una nueva y sólida mejora del rendimiento en lo que respecta a la forma en la que gestionamos la memoria de la GPU (VRam). Los colores uniformes (como las capas de relleno) ahora se comprimen en texturas más pequeñas, lo que acelera su transferencia entre la memoria principal y la memoria de la GPU, pero también reduce su espacio de memoria y su tiempo de cálculo. Esto debería ser especialmente visible al abrir proyectos enormes y al alcanzar los límites de la memoria de la GPU.

## Notas de la versión

### 2017.3.3

(Publicado el 1 de diciembre de 2017)

**Solucionado :**

* [Steam] La ventana emergente del comprobador de versiones no debería estar visible al iniciarse
* [Exportar] Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6

### 2017.3.2

(Publicado el 20 de noviembre de 2017)

**Agregado :**

* [UI] Mejora el diálogo de la nueva versión y añade el registro de cambios
* [IU] Indique si el mantenimiento ha caducado en el cuadro de diálogo Nueva versión
* [Licencia] Actualizar el sistema de licencias para gestionar las fechas de mantenimiento
* [Exportar] Cambiar el nombre de Adobe Standard Material a Adobe Dimension

**Solucionado :**

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

### 2017.3.1

(Publicado el 26 de octubre de 2017)

**Agregado :**

* [Exportar] Permita exportar la malla desde un proyecto
* [Estante] Quitar &quot;Sub-Shelf&quot; de los títulos de las pestañas
* Guardar la configuración posterior al proceso en plantillas
* Haz que el mensaje TDR sea más comprensible
* Mejorar la ventana Configuración para informar de errores

**Solucionado :**

* Bloqueo al borrar varios subestantes
* Bloqueo al cambiar de un nivel a otro durante un cálculo del motor
* bloqueo [Mac] en la GPU Intel durante los cálculos del motor
* [Mac] [Ventana gráfica] Se producen errores de rendimiento cuando el tramado está activado
* [Mac] MacOS 10.13 se reconoce como &quot;Versión desconocida&quot; en el archivo de registro.
* [Baker] Hacer un bake con una jaula ya no funciona
* [Layers] Ctrl+C método abreviado (copia) no funciona más
* [Capas] Al pegar capas, no se actualiza la interfaz de usuario con las referencias del anclaje
* [Anclaje] Duplicar o Copiar/Pegar capa con referencias rompe vínculos
* [Export] En algunos casos, la exportación en 8K puede provocar bloqueos o interbloqueos en las aplicaciones
* [Exportar] Varios problemas en el formato de archivo glTF generado
* [Importar] Volver a importar una malla con el mismo nombre de archivo ya no funciona
* [Plugin] La ventana de guardado automático siempre aparece encima de todo
* [UI] Bucle infinito al pulsar &quot;Escape&quot; en el cuadro de diálogo TDR
* [UI] Restaurar IU muestra una segunda barra de título en la ventana de la estantería

### 2017.3

(Publicado el 28 de septiembre de 2017)

**Agregado :**

* [Exportar] Permitir la exportación de mallas y texturas para el proyecto de Adobe Felix
* [Export] Permitir la exportación al formato de archivo glTF
* [Motor] Optimice el tamaño de las texturas en VRAM mediante la compresión de bloques
* [Ventana gráfica] Puede arrastrar y soltar una malla o un proyecto en la ventana gráfica
* [UI] Mejora el mensaje de advertencia sobre TDR
* [UI] El registro solo se debe mostrar si se solicita
* [UI] Permitir borrar el contenido de la ventana de registro
* [UI] Mostrar advertencias y errores en la barra de estado
* [UI] Mostrar pestañas en la parte superior como en los navegadores web
* [UI] Mejorar el contexto y los mensajes &quot;no puede pintarse&quot;
* [IU] Añada una acción &quot;guardar como copia&quot; en el menú Archivo
* [Capa] Establecer el ajuste de mosaico predeterminado en 1 de forma predeterminada
* [Shelf] Filtro de degradado mejorado para admitir 10 colores dinámicos
* [Estante] Agregue un espacio en la consulta predeterminada de la miniestantería
* [Estante] Agregue una acción Abrir en el explorador para los recursos locales del estante
* [Estante] Añadir plantilla y sombreador para Adobe Material Estándar (Proyecto Félix)
* [Estante] Aumentar el mosaico máximo a 128 en sombreadores de capas de material
* [Estante] Se ha añadido curvatura sobel para microdetalles de Generadores de máscaras
* [Plugin] Añadir complemento de guardado automático con intervalo de tiempo personalizable
* [Scripting] Añadir una función &quot;Guardar como copia&quot;

**Solucionado :**

* [UI] El diseño se interrumpe al iniciarse por primera vez
* El PSD [Export] generado en la exportación tiene errores de formato
* [Exportar] EXR siempre exporta el mapa de altura de 8 bits
* [Exportar] Bloqueo al exportar mapas adicionales dañados
* [Importar] En algunos casos, los bordes duros no se conservan en mallas de polietileno bajas
* [Importar] Mensajes de error mejorados al importar mallas con problemas
* [Bakers] Error de procesamiento de asignación de ID con la opción Coincidir por nombre activada
* [Viewport] El espacio tangente no se sincroniza con los panaderos
* [Efecto] Al retroceder una capa no se restaura la referencia de un anclaje
* [Efecto] Problema de actualización al crear un vínculo entre dos máscaras con anclajes
* [Efecto] No se deben enumerar los anclajes de máscaras encima de la máscara
* [Efecto] La opción Extraer Alpha de Anclajes no funciona
* [Motor] La máscara se invierte a sí misma tras el primer trazo del pincel
* [Motor] Bloqueo al cambiar el conjunto de texturas en un proyecto específico
* [Shelf] Bloqueo al eliminar un ajuste preestablecido de un proyecto
* [Shelf] Error en el filtro avanzado Tri-Planar
* [Estante] La escala de ruido de MG Mask Builder AO no funciona correctamente
* [Estante] MG Mask Builder tiene parámetros de curvatura invertidos
* [Estante] Los alfa importados generan una previsualización de esfera de material en lugar de una plana
