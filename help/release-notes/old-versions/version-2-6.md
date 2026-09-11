---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-6.html"
breadcrumb-title: ''
description: Consulte las notas de la versión 2.6 de Substance 3D Painter para obtener más información sobre las nuevas funciones, mejoras y correcciones de errores.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.6
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versión 2.6
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---


# Versión 2.6

Con **Substance Painter 2.6**, nuestro objetivo era proporcionar una forma de administrar los conjuntos de texturas directamente dentro de Substance Painter, sin la necesidad de hacer un nuevo proyecto o volver a importar tu malla con nombres de materiales actualizados. También queríamos ofrecer una forma de actualizar los recursos utilizados en los proyectos, algo que vimos que solicitaba mucho en el pasado.

Fecha de publicación : *27 de abril de 2017*

## Funciones principales

### Nuevo proyecto de muestra &quot;Meet Mat&quot;

![](../../assets/meetmat-render.jpg)

Este nuevo proyecto de muestra ofrece un nuevo personaje brillante y adorable llamado &quot;**Mat**&quot;. Contiene tres conjuntos de texturas listos para ser pintados.\
Participa en el concurso **Meet Mat** con él para ganar algunos premios geniales: <https://www.allegorithmic.com/contest/meet-mat-2017-substance-3d-painting-contest>

### Nueva API de scripts con capacidad para actualizar recursos en proyectos

![](../../assets/resources-updater-ui.jpg)

La API de scripts de Substance Painter se ha mejorado para agregar nuevas funciones que permiten **reemplazar recursos** en el proyecto con otras versiones. Para demostrar esta nueva característica, se ha agregado un nuevo **plugin** creado con la API de scripts y permite examinar todos los recursos contenidos en un proyecto determinado. Los recursos marcados como rojos se detectan como &quot;obsoletos&quot; y se pueden reemplazar automáticamente. Esta función no se limita a los recursos &quot;obsoletos&quot;, sino que cualquier activo se puede sustituir por otro. Esto ofrece muchas posibilidades nuevas y muestra aún más cómo Substance Painter es una **herramienta de pintura no destructiva**.

El **complemento** está disponible en GitHub, no dudes en ayudar si ves posibles mejoras : <https://github.com/AllegorithmicSAS/painter-plugin-resources-updater>

![](../../assets/resource-update-demo.gif)

### Nueva capacidad para renombrar y reasignar conjuntos de texturas

![](../../assets/texture-set-rename-description.png)

Ahora es posible cambiar el nombre de un conjunto de texturas directamente dentro de Substance Painter. El cambio de nombre de un conjunto de texturas afectará al nombre de las texturas que se exporten en el disco (en función del ajuste preestablecido de exportación utilizado).\
Para cambiar el nombre de un conjunto de texturas, solo tiene que hacer doble clic en su nombre para modificarlo o hacer clic con el botón derecho del ratón para abrir el menú contextual. También es posible añadir descripciones personalizadas para proporcionar más información sobre lo que hacen los conjuntos de texturas. Esto puede resultar muy útil al trabajar en un [proyecto de UDIM](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html). Use el botón &quot;**settings**&quot; para configurar la forma en que se muestran las descripciones en la lista.

![](../../assets/reasign-texture-set.png)

Los conjuntos de texturas ahora se pueden reasignar a diferentes materiales de malla. Esto significa que es posible **recuperar** conjuntos de texturas deshabilitados anteriormente (porque faltaban en la malla) o incluso **intercambiarlos**. Simplemente haga clic en el nuevo botón &quot;**settings**&quot; en la ventana Lista de conjuntos de texturas y haga clic en la entrada &quot;**Reasignar conjuntos de texturas**&quot;. Abrirá una nueva ventana dedicada a administrar los conjuntos de texturas y cómo se vinculan a los materiales de malla. **Arrastra y suelta** el nombre del conjunto de texturas donde quieras para realizar la administración.

## Tutorial

Las nuevas funciones principales se describen en nuestro último tutorial de vídeo :

## Notas de la versión

### 2.6.2

(Publicado el 20 de octubre de 2017)

**Agregado :**

* [Conjunto de texturas] Permitir la eliminación de conjuntos de texturas deshabilitados
* [Estante] Permite que varios usuarios escriban dentro de la misma carpeta de estante
* [Scripting] Poder recargar la carpeta de plugins
* [Scripting] Añada una versión mínima de API necesaria en los metadatos del plugin para garantizar la compatibilidad
* [IRay] Mejoras en el cuadro de diálogo Exportar imagen

**Solucionado :**

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

(Publicado el 12 de mayo de 2017)

**Agregado :**

* [TextureSet] No permitir la reasignación de materiales de malla a nada

**Solucionado :**

* Bloqueo al cambiar TextureSet después de reemplazar mapa con bake
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

(Publicado el 27 de abril de 2017)

**Agregado** :

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

**Corregido**:

* Bloqueo al actualizar una malla en proyectos específicos
* [Ventana gráfica] El color interior del plano de simetría ya no es visible
* [Ventana gráfica] Algunos efectos posteriores al proceso se activan al utilizar la vista en solitario
* [Shaders] La fusión &quot;over\_premult&quot; no funciona correctamente
* [Shaders] Advertencia sobre la prueba alfa con el sombreador predeterminado
* [Shelf] Análisis incorrecto de etiquetas de Substance
* [Shelf] El intemperismo del Óxido MatFX no funciona correctamente
* [Shelf] El filtro de HSL está activado de forma predeterminada en canales incorrectos
* [Estante] El enfoque está activado de forma predeterminada en el canal Height/Normal
* [Exportar] Los ajustes preestablecidos de exportación no utilizan un mapa normal de OpenGL
* [Herramienta] Problemas de imprecisión al crear artefactos con la herramienta clonar/difuminar
