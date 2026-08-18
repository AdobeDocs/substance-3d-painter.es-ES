---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-2.html"
breadcrumb-title: ''
description: Consulte las notas de la versión 2.2 de Substance 3D Painter para obtener más información sobre las nuevas funciones, mejoras y correcciones de errores.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versión 2.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---


# Versión 2.2

**Substance Painter 2.2** agrega un nuevo flujo de trabajo que es el Control dinámico de capas de materiales.

Fecha de publicación : *21 de julio de 2016*

## Funciones principales

### Nuevo flujo de trabajo de Control dinámico de capas de materiales

![](../../assets/dynamic-material-blending-materials-preview.jpg)

Con esta nueva versión, agregamos un nuevo **flujo de trabajo** denominado **Material Layering**. Los flujos de trabajo de texturas tradicionales se basan en la creación de texturas con **alta resolución** para **conservar los detalles**, pero esto no es **conveniente** para el caso de uso. Un enfoque más interesante es **crear material de labranza pequeño** y **repetirlo dentro de un sombreador**. Permite conservar una cierta calidad y la capacidad de **acercar de verdad** el objeto mediante este sombreador **sin perder detalles**. El único problema es que para obtener una vista previa del resultado final era obligatorio ir al motor/procesador del juego que muestra el sombreador final. Eso ya no es cierto, ya que en esta nueva versión ahora es posible usar un sombreador similar dentro de Substance Painter, que te permite **visualizar el resultado final y pintar al mismo tiempo**.

Se ha agregado un **nuevo proyecto de muestra** denominado &quot;**FireHydrant**&quot; para mostrar el nuevo flujo de trabajo.

![](../../assets/layer-stacks.png)

Este nuevo flujo de trabajo abre dos formas de trabajar:

* Los materiales se definen en el sombreado, solo puede pintar máscaras para fusionarlos
* Los materiales y las máscaras se pueden pintar juntos

En cualquier caso, es posible definir una nueva pila de capas cada vez, lo que proporciona más libertad al crear las máscaras y los materiales. La gestión de capas es mucho más fácil de esta manera y cada pila puede tener su propio conjunto de canales específicos que se pueden fusionar en el sombreado final.\
También tenemos un sombreador especial para Unity 5 y Unreal Engine 4 disponible en Share :

* [Unity 5](https://share.allegorithmic.com/libraries/2126)
* [Unreal Engine 4](https://share.allegorithmic.com/libraries/2125)

Para obtener más información, consulte la página dedicada de la documentación : [Control dinámico de capas de materiales](../../features/dynamic-material-layering.md)

### Nuevo campo de búsqueda de miniestante

![](../../assets/mini-shelf-search.gif)

Hemos mejorado el **mini estante** que aparece en varios lugares de la aplicación con un campo de búsqueda dedicado. Esta mejora hace que la búsqueda de recursos sea mucho más cómoda y agradable de usar. La búsqueda personalizada se conserva durante la sesión actual de la aplicación. Por ejemplo, si usa muchos ruidos de suciedad, el uso de esta palabra clave generará

## Tutorial

Nuestro último tutorial en vídeo abarca las nuevas funciones :

## Notas de la versión

### 2.2.0

(Publicado el 21 de julio de 2016)

**Agregado :**

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

**Solucionado :**

* Bloqueo durante el lanzamiento si las sustancias se encuentran en una carpeta incorrecta
* El informe de bloqueo a veces no funciona debido a un archivo de registro incorrecto
* [Iray] Los efectos posteriores no se actualizan cuando Iray está en pausa
* [Iray] El método abreviado de enfoque automático ya no funciona
* [Iray] El comportamiento del regulador de apertura cambia en función del tamaño del activo
* [Capas] El primer canal de materiales no está activado de forma predeterminada si todos están desactivados
* [Shader] No se imprimen errores si un &quot;param auto&quot; es incorrecto

**Problema conocido:**

* [Mac] El límite de muestras de textura está bloqueado en 16 (problema del controlador de la GPU)
