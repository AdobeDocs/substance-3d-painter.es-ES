---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/presets/creating-particles-presets/creating-a-new-particle-script.html"
breadcrumb-title: ''
description: Aprenda a crear un nuevo script de objeto en Substance 3D Painter para definir efectos y comportamientos de pincel de objeto personalizados.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Creating A New Particle Script
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Creación De Un Nuevo Script De Partículas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---


# Creación De Un Nuevo Script De Partículas

Descargue el paquete PopcornFX preconfigurado: [Plantillas\_EmitterReceiver.pkkg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/67403778/68419585/1/1411557944000/templates-emitterreceiver.pkkg)

Este paquete es un &quot;kit de inicio&quot; que contiene un emisor y un receptor que editaremos e importaremos en Substance 3D Painter.

## Configuración de Popcorn fx

Inicie el Editor de PopcornFX, cree un nuevo proyecto y, a continuación, ábralo.

En su proyecto, haga clic con el botón derecho en un área vacía y seleccione &quot;Importar paquete de palomitas&quot;. A continuación, seleccione &quot;Templates\_EmitterReceiver.pkkg&quot;.

Ahora, usted debe tener:

* Un sistema de partículas &quot;\_Emitter&quot; que es una plantilla base de un emisor.
* Un sistema de partículas &quot;\_Receptor&quot; que es una plantilla base de un Receptor.
* Malla de esfera utilizada como fondo predeterminado de la escena

&quot;\_Emitter&quot; y &quot;\_Receiver&quot; ya están &quot;Painter ready&quot;. Ya se han configurado con los evolucionadores necesarios, campos, fondos, etc...

## Importar la malla

PopcornFX solo admite **FBX**. Asegúrese de exportar la malla en este formato. Durante el paso de exportación, compruebe el tamaño de su malla para tratar de encajar con las unidades correctas en el &quot;mundo real&quot;.

Copie y pegue en la carpeta &quot;mallas&quot; de su proyecto (en PopcornFX, puede hacer clic con el botón derecho en la carpeta &quot;mallas&quot; y seleccionar &quot;Abrir ubicación del archivo&quot;).

Vuelve al editor, abre la malla (haz doble clic en ella) y haz clic en &quot;**Build**&quot;. Cierre la ventana y guarde el cambio.

## Edición de emisor y receptor

Duplicaremos los sistemas de partículas existentes y los adaptaremos para tener en cuenta correctamente la nueva malla.

Haga clic con el botón derecho en el sistema de partículas &quot;\_Emitter&quot; (en la carpeta &quot;Partículas&quot;) y seleccione &quot;Clonar&quot; (o &quot;Duplicar&quot;) para crear su propio emisor.

Ábralo y, en la ventana &quot;Vista de árbol de objetos&quot; (abajo a la izquierda), selecciona &quot;**Capa\_Modelo** &quot;, que debe estar ubicada en : &quot;Propiedades del editor => Telón de fondo => Capas 3D&quot;.

Luego, en la ventana &quot;Propiedades del nodo&quot; reemplace &quot;dummymesh.fbx&quot; por su modelo. Guarde la modificación (Archivo => Guardar) y cierre la ventana del emisor.

Ahora, **clone &quot;\_Receiver** **&quot;** (en la carpeta &quot;Particles&quot;), para crear su propio Receptor a partir de este.

Ábralo y, en cuanto al emisor, reemplace la malla ficticia por su modelo en &quot;Layer\_Model&quot;. **Modificamos la malla** **mostrada en la pantalla**, pero también necesitamos modificar **la malla** **usada por las partículas** .

Para ello, en la ventana &quot;Vista de árbol de partículas&quot;, haga clic en &quot;**Forma** &quot;, que debe estar ubicada en : &quot;Efecto de partícula => Generador => Capa\_1 => Muestras => Malla&quot;.

Luego, reemplace el &quot;MeshResource&quot; por su modelo.

Una vez hecho esto, hay una última cosa que hacer: necesitamos &quot;vincular&quot; el emisor y el receptor con el que acabamos de crear.

En la vista de árbol de su Receptor, seleccione &quot;Propiedades del Editor&quot;, luego seleccione su emisor en &quot;OverSpawnEffect&quot;. Guarde el receptor.

Abra su emisor (el que duplicamos anteriormente) y en la ventana &quot;Vista del árbol de partículas&quot;, haga clic en &quot;Eventos&quot; que deben estar ubicados en : &quot;Efecto de partícula => Generador&quot;. Luego reemplace el receptor por su receptor haciendo clic en &quot;Externo&quot;.\
¡Ya está hecho! Ahora, si selecciona la vista 3D (de su emisor o receptor), puede crear partículas pulsando el botón &quot;espacio&quot;.

## Opcional: modificación del comportamiento del receptor

Abra el receptor y, en la ventana &quot;Vista de árbol de partículas&quot;, seleccione &quot; CParticleEvolver\_Script &quot; (el que está dedicado a usted :)) que debe estar ubicado en : &quot;Efecto de partícula => Capa\_1 => Estado\_0&quot;.

En la ventana &quot;Editor de nodos especializado&quot;, en la función, agregue &quot;Life = 0.5;&quot; para cambiar la vida útil de las partículas. A continuación, utilice el método abreviado &quot;Ctrl+s&quot; para guardar el script. Debería poder notar la diferencia en la vista 3D.

Para obtener más información sobre cómo funciona, visite el siguiente vínculo:

<http://wiki.popcornfx.com/index.php/Main_Page>

## Importar emisor/receptor en Substance 3D Painter

En Substance 3D Painter, haz &quot;Archivo&quot; > &quot;Importar partículas&quot; o Ctrl-Alt-R y luego elige tu Emisor y tu Receptor (ambos en formato .pkfx) en tu Pack.

Substance 3D Painter detectará automáticamente los requisitos (campos de partículas, eventos OnCollide) para decidir si su pkfx es un emisor, un receptor o no es compatible.

Ahora, debería ver su Emisor/Receptores en la Estantería (en las pestañas &quot;Emisores&quot; y &quot;Receptores&quot;).

Para utilizarlas, primero debe hacer clic en el botón &quot;Alternar partículas&quot;.

A continuación, en la ventana &quot;Herramienta&quot;, en &quot;Física&quot; tendrá la posibilidad de seleccionar su emisor (para reemplazar &quot;default\_emitter&quot;) y su receptor (para reemplazar default\_recipient).

Ahora puede hacer clic con el botón derecho en la ventana &quot;Herramienta&quot; y guardar la herramienta.
