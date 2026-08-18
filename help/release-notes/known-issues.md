---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html'
breadcrumb-title: ''
description: Revise los problemas conocidos de Substance 3D Painter para estar informado de las limitaciones actuales y las soluciones alternativas en la última versión.
helpx_creative_field: ''
helpx_description: Substance 3D Painter
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Problemas conocidos
user-guide-description: ''
user-guide-title: ''
source-git-commit: c95676d7a6269addb3a0b42ab671a649a93caa10
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---


# Problemas conocidos

En esta página se enumeran todos los problemas conocidos activos presentes en la versión 12.1.0 de Substance 3D Painter:

* Error de `[Engine]` al usar materiales inteligentes si el conjunto de texturas no tiene el mosaico 1001
* `[Engine]` Pintar con la herramienta Clonar en colores de cambio de canal normales incorrectamente
* La máscara de geometría `[Engine]` muestra artefactos en los bordes UV con capas con instancias
* El relleno UV `[Engine]` del modo &quot;Vecino del espacio 3D&quot; no funciona bien en triángulos finos
* El resultado del punto de anclaje `[Engine]` no se procesa entre una máscara y un canal de color

* `[Baking]` AO incorrecto en cubos simples
* `[Baking]` La interpretación del sufijo de coincidencia por nombre es incorrecta
* `[Baking]` Las costuras Uv no aparecen después de la reimportación de mes
* `[Baking]` artefactos similares a una cuadrícula con algunos valores

* `[Substance]` Varios errores ortográficos en los recursos
* `[Substance]` El espacio en blanco rompe la condición de visibilidad
* `[Substance]` Los ajustes preestablecidos de algunos materiales tardan demasiado en cargarse
* `[Substance]` No se puede importar el recurso con usos mixtos

* `[Color Management]` Enlaces incompatibles con generador no utilizados en máscara
* `[Color Management]` Los resultados del filtro no se tienen en cuenta correctamente
* Las conversiones de espacio de color HDR de `[Color Management]` con ACE en Linux producen colores con sujeción

* Los recursos de `[Shelf]` obtienen un uso incorrecto si se colocan en una carpeta con un nombre específico
* `[Shelf]` `[Substance]` Datos de usuario no tomados en cuenta para la generación de miniaturas de estantería.

* `[Shader]` No se reconoce el parámetro &quot;camera_vp_matrix_inverse&quot;
* El canal user0 de `[Shader]` no siempre se puede leer como sRGB con sombreador específico

* Error de `[Scripting]` `[Javascript]` &quot;Deshabilitado&quot; al especificar el parámetro de tramado en las funciones de exportación
* `[Scripting]` `[Python]` Varios errores tipográficos en el módulo substance_painter.project

* `[Single Channel View]` El proyecto guardado en la vista de color base se ve más oscuro después de actualizar la versión de Painter
* `[Single Channel View]` El proyecto guardado en la vista de color base se ve más oscuro después de actualizar la versión de Painter

* `[gltf]` No se pueden abrir archivos exportados a través del exportador de Babylon
* Error de `[Displacement]` al pintar
* `[Polygon Fill Tool]` Selección incorrecta con simetría
* A veces, `[2D view]` trazos no aparecen al pintar
* `[Console]` No es posible escribir símbolos asociados a métodos abreviados
* El mensaje de error de `[LOG]` es incorrecto al producirse un error de exportación
* La galería de símbolos de `[3D View]` no funciona en objetos duplicados
* `[Resource updater]` Los diferentes recursos del estante con el mismo nombre se leen como un recurso
* `[Sample]` Cámara rota en muestra de vista previa
* `[Instancing]` `[Projection]` Al seleccionar una instancia en un proyecto plano, se selecciona otro proyecto plano en otro conjunto de texturas
* `[Slider]` Las entradas numéricas no están seleccionadas cuando el cursor sale de la ventana
* `[Anchor point]` Referencias rotas al copiar y pegar contenido de máscara
* `[Mesh export]` No tener en cuenta los nuevos nombres de conjuntos de texturas
* `[Anchor Points]` Color incorrecto cuando se usa en el generador
* El panadero del mapa de identificación de `[Bakers]` no tiene en cuenta el material físico de 3ds Max 2021
* `[UV Tiles]` No hay mensaje de error en espacios UV superpuestos con una malla específica
* `[GLTF]` `[Crash]` Al crear un proyecto con un archivo gltf comprimido, se produce un bloqueo
* Los mapas de posición de `[UV Tile sequence]` no se importan correctamente
* La máscara de combinación de Heightes `[UVTiles]` no se actualiza con la máscara de mosaico UV
* `[Import]` No se puede importar el archivo obj con valores &quot;nan&quot;
* `[Export]` GLTF se exporta con un tamaño incorrecto
* El nombre de `[Texture Set]` puede estar vacío
* `[Layer stack]` Copiar en máscara cambia al modo de material
* Error de `[UI]` en la configuración del fabricante de pinceles
* `[Texture Set Settings]` Nombre de instancia de sombreador incorrecto después de cambiar el nombre
* `[Blending]` El modo de fusión de color y saturación también cambia el brillo
* `[Librairies]` Ancho de las búsquedas guardadas y filtrar por ventanas de ruta no se guarda al cambiar
* `[Geometry mask]` Problema al reimportar malla y capas con instancias
* No se encuentra el espacio de color `[Color management]` cuando falta el azulejo 1001
* El Desplazamiento `[Export mesh]` no se exporta con la configuración de mosaicos UV específicos
* `[RedHat]` Problemas con el selector de color
* `[Regression]` `[UI]` El menú contextual es demasiado pequeño en la pantalla HD
* La actualización automática omite los mapas de malla importados de `[Resources]`
* La vista previa del espacio de mezcla de color de `[User Channels]` es incorrecta
* La selección de geometría `[Mask]` sigue activa después de cambiar al modo de cocción
* Los iconos de `[Sonoma]` no aparecen en los menús
* El Height `[Path]` que mezcla muchas rutas puede causar artefactos
* `[USD]` Asignación de usda incorrecta en algunos casos
* `[Polygon Fill]` Al cambiar el espacio de color del color base no se actualiza el selector de color
* La herramienta `[Paint Skew]` seleccionada en el sesgo de pintura permanece seleccionada después de cambiar al modo de pintura
* El selector `[Color Picker]` permanece abierto después de cambiar la herramienta
* `[UV Padding]` artefactos al aumentar la textura de 4k a 8k en la exportación
* La configuración de la distancia de la jaula de `[Baking Common Settings]` no actualiza la visualización de la malla metálica de la jaula y del sombreador
* `[Send to Photoshop]` No se puede exportar la máscara de la capa
* `[Skew Baking]` La corrección de sesgo se rompe al pintar y deshacer
* La herramienta de proyección bloquea la interacción Ventana gráfica `[Projection Tool]`
* Los recursos no cuadrados se amplían cuando se utilizan en las ranuras del canal del pincel
* Error al descodificar la sustancia
* Los UV no perfectamente superpuestos pueden crear artefactos
* Malla normal no válida con algunos fbx
* La vista no se actualiza al cambiar el canal afectado por un nivel
* Los proyectos con un conjunto de texturas se vuelven a abrir en el modo solo Color base
* La interfaz de usuario del botón de canal en las propiedades de Material/pintura se puede romper
* El orden de los canales en las propiedades se puede romper
* Los trazos realizados en L16F y RBG16F pueden mostrar defectos
* El comportamiento del botón Restaurar no interactúa con la tecla de bloqueo en los ajustes de la cámara
* La exportación de Photoshop ignora la selección de máscara geométrica
* La Pendiente de desenfoque y el filtro de deformación dependen de la resolución del conjunto de texturas
* Las asignaciones sin nombres se crean fuera de la carpeta de exportación
* La galería de símbolos no se actualiza al cambiar el ajuste preestablecido del pincel
* Problema de transparencia en archivos de PSD
* Los parámetros del pincel que se modifican desde la barra de herramientas contextual no aparecen en el historial
* No se puede cambiar el nombre de los ajustes preestablecidos de exportación ni eliminarlos si ya los ha eliminado y creado de nuevo en esta sesión
* La asignación de canales no funciona para la previsualización de la herramienta de proyección en algunos casos.
* Abrir y guardar algunos proyectos puede tardar más de lo habitual.

## Estabilidad

* `[Crash]` Al hacer clic en la lista Conjunto de texturas después de una creación de proyecto errónea, se produce un bloqueo
* `[Crash]` Error crítico al bloquearse cuando el mismo proyecto está abierto dos veces
* `[Crash]` Seleccionar &quot;Exportar malla&quot; cuando la malla no se pudo cargar
* `[Crash]` Al hacer clic en &quot;Comenzar a pintar&quot; después de intentar abrir un proyecto antiguo
* `[Crash]` La creación de textos muy largos en la cinta de opciones puede bloquearse
* `[Crash]` Volver al modo de pintura después de que el dispositivo se perdiera al hornear
* `[Crash]` Salir de Painter después de cancelar la exportación de mapas
* `[Crash]` Exportando malla con algunos símbolos especiales en el nombre de la cámara
* `[Crash]` Si se elimina un canal mientras se está en el modo de vista de máscara, se produce un bloqueo
* `[Crash]` Algunos Substance pueden provocar un bloqueo al procesarse
* `[Crash]` Volver a importar la malla en modo de repostería
* `[Crash]` La recarga de varias mallas puede provocar un bloqueo
