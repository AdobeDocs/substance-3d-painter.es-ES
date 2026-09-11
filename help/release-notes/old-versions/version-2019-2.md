---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/release-notes/old-versions/version-2019-2.html"
breadcrumb-title: ''
description: Consulte las notas de la versión 2019.2 de Substance 3D Painter para obtener más información sobre las nuevas funciones, mejoras y correcciones de errores.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2019.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versión 2019.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1538'
ht-degree: 1%

---


# Versión 2019.2

**Substance Painter 2019.2** incorpora nuevas y potentes funciones a sus Bakeres y ofrece un nuevo conjunto de Materiales inteligentes y Máscaras inteligentes en la estantería.

Fecha de publicación : *25 de julio de 2019*

## Funciones principales

### Mejoras del flujo de trabajo para Bakeres

![](../../assets/header-image-vizu.jpg)

El flujo de trabajo de hacer un bake se ha mejorado con esta versión con algunas funciones nuevas. Estas mejoras agilizarán y facilitarán el trabajo diario con Substance Painter.

* **Visualización del proceso de cocción**\
  De forma predeterminada, con esta nueva versión, cualquier proceso de hace un bake será visible en la ventana gráfica. Permite previsualizar el resultado de los panaderos en tiempo real e incluso cancelarlo si es necesario sin esperar hasta el final del proceso para ofrecer iteraciones más rápidas. Este comportamiento se puede deshabilitar entrando en la configuración principal y desmarcando la configuración &quot;**Habilitar proceso de horneado de vista previa en vivo**&quot; en la sección &quot;**Opciones de horneado**&quot;.

  ![](../../assets/baking-options-v2.png)

  ![](../../assets/bake-process.gif){width="500px"}
* **Se ha mejorado el cuadro de diálogo hacer un bake**\
  El cuadro de diálogo de horneado se ha rediseñado y ahora muestra un estado mejor del proceso de horneado actual. Ahora hay un contador para indicar cuántas texturas se calcularán, así como una lista explícita por panadero y conjunto de texturas de lo que se está calculando. En caso de error, se muestra una cruz roja junto al nombre del baker. Al final del proceso, un nuevo botón permite abrir rápidamente la ventana de registro para obtener más información sobre el problema.\
  ![](../../assets/baking-dialog.png)
* **Cancelando hace un bake en curso** El proceso de hace un bake ya no bloquea la aplicación. Substance Painter ahora es más flexible, lo que significa que es posible cancelar un hago un bake que está en curso sin esperar a que finalice. Sin embargo, la cancelación no es inmediata y puede requerir unos segundos para que surta efecto. Esto se debe a que internamente el proceso de hacer un bake funciona en texturas en fragmentos y no se puede detener mientras se está calculando un fragmento. Al cancelar el proceso de hacer un bake, la ventana de Hacer un bake se vuelve a abrir automáticamente.\
  ![](../../assets/baking-cancel-optim.gif)

### Mejoras de rendimiento para Bakeres

![](../../assets/header-image-baker.jpg)

Con la mejora del flujo de trabajo, también aprovechamos la oportunidad para actualizar nuestros Bakeres y mejorar su rendimiento. También hemos añadido el soporte de DXR y Optix para permitir que el Trazado de rayos de GPU que permite hacer un bake mucho más rápido que antes. Tenga en cuenta, sin embargo, que el Trazado de rayos de GPU solo afecta al baker de Oclusión ambiental y Thickness.

* **Se ha mejorado el Trazado de rayos de la CPU**\
  El cálculo del trazado de rayos en la CPU es ahora de 2 a 3 veces más rápido que antes. Por lo tanto, aunque la GPU no sea compatible con Trazado de rayos de GPU, el rendimiento mejorará en general.
* **Soporte de Trazado de rayos de GPU con DXR y Optix**\
  Con el hardware compatible, los bakeres ahora pueden calcular directamente en la GPU, lo que reduce drásticamente el tiempo de cálculo, especialmente cuando el suavizado está activado y se definen muchos rayos. DXR es la opción predeterminada cuando está disponible; de lo contrario, se utilizará Optix. Es posible deshabilitar el Trazado de rayos de GPU yendo a la [configuración principal](../../interface/settings/settings.md) y buscando &quot;**opciones de Haga un bake**&quot;:

  ![](../../assets/baking-options-v2.png)

>[!NOTE]
>
> Para habilitar la función Trazado de rayos de GPU, asegúrese de actualizar a los siguientes controladores : **Controladores NVIDIA 430.86**.\
> DXR está disponible en las GPU RTX y [GeForce GTX 10xx GPU](https://www.nvidia.com/en-us/geforce/news/geforce-gtx-dxr-ray-tracing-available-now/). DXR también requiere que Windows 10 esté actualizado para ser accesible (versión 1809), consulte esta página para obtener más información.

>[!WARNING]
>
> Cuando se utiliza Trazado de rayos de GPU, el baker puede fallar si la malla de alto contenido de poli no cabe en VRam. Cuando ocurra, se recomienda ir a la [configuración principal](../../interface/settings/settings.md) y deshabilitar &quot;**Trazado de rayos de GPU**&quot; en la sección &quot;**Opciones de Haga un bake**&quot;. Después de eso, simplemente puede volver a iniciar el proceso de hacer un bake.

### Nuevas funciones y mejoras diversas

![](../../assets/header-image-misc.jpg)

En esta versión también hemos añadido y reelaborado algunas cosas para mejorar la calidad de vida dentro de Substance Painter.

* **manipulador de rotación mejorado**\
  El manipulador de rotación era un poco lento en el pasado haciendo rotaciones a veces tediosas de realizar. La velocidad de rotación ahora está vinculada a la cámara y al tamaño de la escena.
* **Rendimiento mejorado en pantallas High DPI con reducción de escala de la ventana gráfica**\
  En la [configuración principal](../../interface/settings/settings.md), ahora hay un nuevo parámetro llamado &quot;Escala de ventana gráfica&quot; con el valor &quot;**Ninguno**&quot; y &quot;**Automático**&quot; (predeterminado). Cuando el Substance Painter detecta que una pantalla utiliza una escala HDPI (como pantallas Retina en MacOS), divide automáticamente la resolución del puerto de visualización entre 2. Este comportamiento evita que la ventana gráfica sea demasiado grande y mejora el rendimiento general sin ninguna pérdida de calidad apreciable.

  ![](../../assets/settings-viewport-downscale.png)
* **Nuevo complemento de consola para scripts**\
  Hemos creado un nuevo plug-in para ejecutar fácilmente comandos desde nuestra API de scripts. Está disponible en Github : <https://github.com/AllegorithmicSAS/painter-plugin-console>. La consola también admite la finalización automática.

  ![](../../assets/console-plugin.png)

### Nuevo contenido

![](../../assets/header-image-content.jpg)

Se ha añadido un nuevo conjunto de Materiales inteligentes y Máscaras inteligentes al estante predeterminado para cubrir diversos usos. Esta es la lista completa de activos que se han añadido :

* **40 Materiales inteligentes nuevos**

  * Tela
    * Lienzo de tela plegado
    * Tejido compuesto reforzado usado
    * Tela Denim Lavado
    * Tartán de franela
    * Tela de lino arrugado
    * Tela de lino desgastado
    * Tela puntos sintéticos
    * Tela sintética Deporte usado
  * Cuero
    * Grano de pantorrilla de cuero
    * Cuero plisado
    * Cuero natural de color
    * Cuero áspero oscuro
  * Mármol: granito
    * Mármol Verde Alpi
  * Metal
    * Dorado dañado
    * Hierro forjado viejo
    * Acero pintado descascarillado sucio
    * Acero pintado áspero dañado
    * Acero pintado raspado sucio
    * Acero pintado raspado verde
    * Acero pintado desgastado
    * Acero arruinado
  * Orgánico
    * Criatura Piel Alien Blue
    * Criatura Piel verde liso
    * Dientes de criaturas
    * Lengua de Criatura
  * Plástico: goma
    * Plástico Polvoriento
    * Plástico brillante esposado
    * Plástico brillante manchado
    * Plástico granulado suave
    * Plástico áspero Rascado
    * Plástico termoformado
    * Plástico grueso agrietado
    * Herramienta de plástico desgastada
    * Plástico usado suave
  * Piedra
    * Corindón de zafiro
  * Translúcido
    * Espejo sucio de película de vidrio
  * Madera
    * Carboncillo
    * Acajou de madera
    * Casco de madera nórdico
    * Casco de barco de madera viejo
* **20 nuevas máscaras inteligentes**

  * Arrugas
  * Cavidades de dirt
  * Masa del dirt
  * Fuga de dirt seca
  * Dirt de bordes suaves
  * Salpicaduras de dirt
  * Manchas de dirt
  * Dust Plástico
  * Dust de bordes suaves
  * Superficie de dust
  * Bordes anchos de dust
  * Grietas de Edge Dirty
  * Grietas de piedra de borde
  * Bordes fuertes rayados
  * Subproceso de tejido
  * Pintura dañada
  * Pintura sutil rasguño
  * Cavidades de arena
  * Dust de arena
  * Goteos de agua

## Notas de la versión

### 2019.2.3

*(Publicado El 23 De Octubre De 2019)*\
Resumen : **Corrección de error**

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

### 2019.2.2

*(Publicado El 20 De Septiembre De 2019)*\
Resumen : **Corrección de error**

**Corregido:**

* La importación de recursos mediante secuencias de comandos puede provocar un bloqueo
* [Plugin] Descargar material de la fuente puede llevar a un bloqueo

### 2019.2.1

*(Publicado El 17 De Septiembre De 2019)*\
Resumen : **Corrección de error**

**Corregido:**

* [Mac]&#x200B;[USD] Los archivos USDZ exportados de MacOS no se pueden abrir
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

### 2019.2

*(Publicado El 25 De Julio De 2019)*\
Resumen : **Versión principal con actualizaciones de los bakeres en términos de rendimiento y un nuevo modo de previsualización + nuevo contenido**

**Agregado:**

* [Bakeres] Se ha agregado compatibilidad para Trazado de rayos de GPU con DXR y OptiX (Oclusión ambiental, Thickness)
* [Baker] Optimizaciones y aceleraciones para el Trazado de rayos de la CPU
* [Bakeres]&#x200B;[Modo Vis]&#x200B;[IU] Nuevo modo de visualización de hace un bake en la ventana gráfica
* [Bakeres]&#x200B;[Preferencias]&#x200B;[IU] Nueva opción de hacer un bake para activar y desactivar el Trazado de rayos de GPU
* [Bakeres]&#x200B;[IU] Repaso del cuadro de diálogo de la barra de progreso
* [Bakeres] Mejora de los mensajes de advertencia y error
* [Bakeres] Permitir una cancelación más receptiva del proceso de hacer un bake
* [Baker] Vuelva a abrir la ventana hacer un bake después de hacer clic en Cancelar
* [Proj]&#x200B;[UX] Mejora de la usabilidad del manipulador de rotación
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
* [Baker] El botón &quot;Hornear todos los conjuntos de texturas&quot; no se desactiva si no se ha seleccionado ningún panadero
* [MacOS] Desactivar el mensaje de advertencia sobre la teselación
* La herramienta Proyección no tiene previsualización cuando se utiliza con una máscara
* Se bloquea y se dañan los proyectos al intentar guardar sin suficiente espacio en disco
* [Shelf] Bloqueo al importar un recurso en el disco a través de la estantería con espacio insuficiente
* [Shelf] Bloqueo al restaurar el ajuste preestablecido de sesión
* [Estante] Importar un ajuste preestablecido con un nombre que termina en un espacio provoca un bloqueo
* [Shelf] Importar un recurso con un prefijo que termina en un espacio vacío provoca un bloqueo

**Problemas conocidos:**

* No se pueden importar archivos Alembic con subdivisiones
* Los bloqueos raros al importar algunos archivos Alembic
* La interfaz de usuario no responde temporalmente al realizar el procesamiento con DXR en las GPU Pascal
