---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/release-notes/old-versions/version-2017-4.html"
breadcrumb-title: ''
description: Consulte las notas de la versión 2017.4 de Substance 3D Painter para obtener más información sobre las nuevas funciones, mejoras y correcciones de errores.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2017.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versión 2017.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---


# Versión 2017.4

**Substance Painter 2017.4** agrega una nueva característica de flujo de trabajo con la **creación de instancias de capas**, lo que permite sincronizar fácilmente las capas en diferentes conjuntos de texturas dentro de un proyecto.

Fecha de publicación : *23 de noviembre de 2017*

## Funciones principales

### Creación de instancias de capas

![](../../assets/instancing.jpg)

La **creación de instancias de capas** es un nuevo sistema que permite mantener la capa **sincronizada** y los **parámetros** en **otras capas y conjuntos de texturas**. Al crear una instancia de capa, la capa original se convierte en el **origen** y las instancias **se mantendrán actualizadas** a menos que se rompa el vínculo entre ellas. Las capas instanciadas son una **excelente manera** de **texturizar un activo con solo unos clics**, así como evitar ir cambiando de una capa a otra para actualizarlas. Para aplicar texturas a un activo con facilidad, basta con **crear instancias de una carpeta** en otros conjuntos de texturas y ponerle un material inteligente o cualquier otra capa, se **replicará en todas partes** al instante.

Hay dos formas de crear una instancia:

* Elija &quot;**pegar como instancia**&quot; (o utilice el método abreviado CTRL+MAYÚS+V), después de copiar una capa
* Elija &quot;**crear instancias entre conjuntos de texturas**&quot; (o utilice el método abreviado CTRL+MAYÚS+D) después de seleccionar una capa

>[!NOTE]
>
> Hay algunas limitaciones relacionadas con la creación de instancias de capas :
> 
> * Las acciones de pintura solo estarán presentes en la capa de origen; las capas con instancias no replicarán trazos de pincel.
> * Las referencias de anclaje deben tener el punto de anclaje en el mismo nivel de la instancia; un punto de anclaje no puede estar fuera de una carpeta con instancias; de lo contrario, se romperá.
> * Si se guarda un material inteligente con capas instanciadas, la capa de origen debe estar en la carpeta de material inteligente; de lo contrario, el vínculo de instancia se romperá.
> * Según la configuración de la pila de capas, las capas con instancias pueden crear un ciclo, lo que no se admite y romperá el resultado de la instancia. Elimine o mueva la instancia para corregirla.

Para obtener más detalles y ejemplos, consulte la página dedicada : [Creación de instancias de capas](../../interface/layer-stack/layer-instancing.md)

### Live-link de DCC compatible con Unreal Engine 4

![](../../assets/livelink.jpg)

La versión beta anterior de nuestro **plugin live-link** se ha **integrado** en Substance Painter. Aprovechamos la ocasión para apoyar el Unreal Engine 4 que ahora permite ver el resultado de un proyecto en el motor de forma automática.

Para conectar la aplicación con **Unreal Engine 4** (se requiere la versión **4.18** como mínimo), descarga los complementos del Substance aquí : <https://www.unrealengine.com/marketplace/substance-plugin>

### Nuevo contenido de estante

![](../../assets/materials-1.jpg)

Agregamos **20 nuevos materiales de procedimientos** y también **40 nuevos mapas de suciedades** (algunos de ellos son de procedimientos). Los nuevos materiales se pueden encontrar en la sección &quot;**Materiales**&quot; del **estante**, como los 6 metales nuevos, los 8 plásticos nuevos, algunas telas y 2 superficies de madera nuevas. Los nuevos mapas de suciedades se encuentran directamente en la sección &quot;**Suciedad**&quot; del **estante**.

![](../../assets/grunges-1.jpg)

Muchas gracias a Clément Feuillet y Nicolas Longchamps por permitirnos licenciar su contenido para esta nueva versión.

### Exportación de Sketchfab mejorada

![](../../assets/sketchfab.jpg)

Hemos actualizado nuestra exportación de Sketchfab y hemos añadido la capacidad de publicar su proyecto como borrador e incluso actualizar proyectos ya cargados. Esto debería facilitar las iteraciones de los proyectos.

### Mejoras de rendimiento

Continuamos nuestro trabajo con respecto a las mejoras de las actuaciones. En esta nueva versión hemos rediseñado gran parte de nuestro renderizado OpenGL en las ventanas gráficas, lo que debería dar un buen impulso a la velocidad. También hemos mejorado la forma en que se calculan los trazos de pincel y deberían requerir cálculos de texturas mucho menos grandes en la memoria. En general, dará resultados mucho más rápidos y mejores sensaciones de pintura.

## Tutorial

Las nuevas funciones se detallan en nuestros vídeos más recientes :

## Notas de la versión

### 2017.4.2

(Publicado El 24 De Enero De 2018)

**Agregado:**

* [Exportar] Obtenga el estado de una exportación con el progreso del paso
* [Exportar] Permitir cancelar una exportación
* [Exportar] Exporte texturas a Sketchfab sin perder la calidad normal del mapa
* [Export] Exportación en formato binario glTF (glb)
* [Exportar] Permitir cambiar el tamaño de las columnas en la ficha de configuración de la ventana de exportación
* [Shader] Agregar un registro de cambios para la API del sombreador
* [Scripting] Añadir funciones de devolución de llamada Antes y Después al exportar texturas
* [Israel] Actualización a SDK 2017.1 (compatibilidad con las GPU Volta)

**&#x200B;**&#x200B;Corregido:**&#x200B;**

* Bloqueo al salir de la aplicación antes de que se muestre la ventana principal
* [MAC] Bloqueo al cargar mapas en escala de grises con IRA
* [MAC] La detección de VRAM no es correcta con el nuevo sistema operativo High Sierra
* [Complemento] La descarga de recursos de Substance Source ya no funciona
* [Scripting] Detección de versión mínima de plugin incorrecta
* [Exportar] Error al guardar el ajuste preestablecido de exportación después de exportar texturas
* [Instancing] Problema en generadores instanciados en un TextureSet sin Mapas Adicionales
* [Ventana gráfica] El tramado no funciona con una resolución superior a 4k
* [Ventana gráfica] La visualización de material 2D View está cubierta de ruido
* [Estante] Mejorar el tiempo de carga para los ajustes preestablecidos de estante
* [Motor] Fusión incorrecta al pintar en la selección de color

### 2017.4.1

(Publicado el 15 de diciembre de 2017)

**Agregado:**

* [Scripting] Exportar malla mediante la API de scripting
* [Importar] Desactivar la importación de formatos de archivo de malla no compatibles (permitir solo obj, fbx, dae, ply)
* [Log] Indique con mayor precisión el problema de TDR en el archivo de registro

**Corregido:**

* Bloqueo si la aplicación se cierra antes de que finalice el rastreo de recursos
* Bloqueo al abrir proyectos con la herramienta Difuminar/Clonar
* Bloqueo al utilizar rehacer después de deshacer un cambio de sombreado en la configuración del visor
* [Motor] Las texturas difieren entre Painter 2017.2 y 2017.4
* [Ventana gráfica] Al seleccionar un mapa de ID de una instancia, se muestra un color incorrecto
* [Export] Bloqueo al exportar una textura normal o de oclusión no válida
* [Exportar] Los grupos de archivos de PSD se bloquean al abrirse en Photoshop CS6
* [Plugin] El plugin de Photoshop ignora la selección de canales y siempre exporta todo
* [Capas] Los anclajes se rompen al copiar o pegar entre conjuntos de texturas
* [Capas] Algunas referencias de anclaje no se pueden restaurar si se rompen
* El parámetro de rugosidad secundaria con revestimiento de pbr [Shader] está roto
* [Steam] La ventana emergente del comprobador de versiones no debería estar visible al iniciarse

**Problemas conocidos:**

* [AMD] Se bloquea al intentar pintar en una malla. Se puede solucionar con una actualización del controlador de la GPU.

### 2017.4

(Publicado el 23 de noviembre de 2017)

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
