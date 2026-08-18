---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/sparse-virtual-textures.html"
breadcrumb-title: ''
description: Aprende a usar texturas virtuales dispersas en Substance 3D Painter para trabajar con texturas de ultra alta resolución de manera eficiente.
helpx_creative_field: ""
helpx_description: Painter > Features > Sparse Virtual Textures
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Texturas virtuales dispersas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---


# Texturas virtuales dispersas

![](../assets/svt-header.jpg)

A partir de la versión **2018.3**, Substance 3D Painter usa **Texturas virtuales dispersas** ( **SVT** ) en su ventana gráfica en tiempo real para administrar una gran cantidad de texturas. Esta tecnología permite transmitir texturas que solo son necesarias desde un punto de vista determinado para mantener un espacio específico en la memoria de la GPU. Mejora el rendimiento en proyectos con una gran cantidad de conjuntos de texturas (o UDIM).

## Plataformas compatibles

![](../assets/sparse-settings.png)

Las texturas dispersas se basan en una configuración de hardware específica para obtener un rendimiento completo. Si la configuración actual no la admite correctamente, Substance 3D Painter **devolverá** a una implementación de software (que será menos precisa y de menor rendimiento).

Es posible forzar que Substance 3D Painter utilice la función de reserva de software en lugar de la aceleración de hardware en [Configuración](../interface/settings/settings.md) .

Esta es la configuración que admite las texturas virtuales dispersas aceleradas por hardware :

| Platform | Compatible (acelerado por hardware) | No compatible (software alternativo) |
| --- | --- | --- |
| **Windows** | <ul data-preserve-html="true"><li data-preserve-html="true">NVIDIA GeForce (controladores 411.63 o posterior)</li><li data-preserve-html="true">NVIDIA Quadro (controladores 411.63 o superior)</li><li data-preserve-html="true">AMD FirePro y Radeon Pro (controladores 18.9.3 o posteriores) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon (controladores 18.9.3 o superior)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true"> NVIDIA Quadro M2000 </li><li data-preserve-html="true">  NVIDIA Geforce GTX 970 </li><li data-preserve-html="true"> GPU Intel </li></ul> |
| **SO Mac** | <ul data-preserve-html="true"><li data-preserve-html="true"> Función de hardware no compatible con el sistema operativo </li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Cualquier modelo de GPU</li></ul> |
| **Linux** | <ul data-preserve-html="true"><li data-preserve-html="true">NVIDIA GeForce (controladores 410.73 o superior)</li><li data-preserve-html="true">NVIDIA Quadro (controladores 410.73 o superior)</li><li data-preserve-html="true">AMD FirePro y Radeon Pro (controladores 18.9.3 o posteriores) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon (controladores 18.9.3 o superior)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">GPU Intel</li></ul> |


* **\*** : La aceleración de hardware está deshabilitada de forma predeterminada y se puede habilitar manualmente en [Configuración](../interface/settings/settings.md) .

## ¿Por qué Substance 3D Painter utiliza texturas virtuales dispersas?

Substance 3D Painter utiliza su motor principal para calcular las texturas que se muestran en las ventanas gráficas. Esto significa que el motor y la ventanilla tienen que compartir la memoria de la GPU (VRam) para calcular y mostrar estas texturas. Cuantos más **conjuntos de texturas** (o mosaicos UV) contenga un proyecto, más memoria se necesitará para la ventana gráfica. Si la ventana gráfica ocupa demasiada memoria en la GPU, el motor principal no tiene suficiente espacio para calcular texturas y tendrá que expulsar texturas a la memoria del sistema (Ram). Esto dará como resultado un rendimiento deficiente y cálculos lentos.

El objetivo del SVT es calcular cuánto puede utilizar la ventanilla en la memoria de la GPU, lo que deja el máximo margen posible para que el motor principal realice los cálculos. La ventaja del sistema es que también desbloquea la capacidad de cargar proyectos mucho más grandes en Substance 3D Painter sin dejar de funcionar de la forma habitual.

## ¿Cómo funciona Texturas dispersas?

Las texturas virtuales dispersas son un tipo de texturas que no están completas. Esto significa que la aplicación solo carga partes de texturas en la memoria. Sólo se carga lo necesario y el resto se coloca en la memoria del sistema o en el disco (caché). Cuando es necesario de nuevo, las texturas se recuperan de la caché y se colocan de nuevo en la ventana gráfica. Para realizar transferencias lo suficientemente rápidas, el sistema se basa en **mipmaps** y salta rápidamente entre diferentes resoluciones de textura. Por esta razón, al entrar rápidamente en la ventana gráfica, es posible que aparezcan texturas desenfocadas en un primer momento, que luego aumentan de calidad al cabo de unos segundos.

Para obtener más información técnica, consulte :  [Texturas virtuales dispersas](https://silverspaceship.com/src/svt/) .

## Ubicación de caché

![](../assets/settings-temp.png)

Cuando no hay suficiente memoria del sistema (Ram) disponible para almacenar la caché de SVT, Substance 3D Painter cambiará al disco duro del equipo en lugar de almacenar la caché.\
La ubicación de esta caché se establece de forma predeterminada en la carpeta Archivos temporales del sistema operativo. Esta ubicación se puede cambiar entrando en la configuración principal de la aplicación, consulte [Preferencias generales](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/general-71008262.html) .

## Compatibilidad con sombreadores

Para aprovechar al máximo el SVT, los sombreadores tienen que solicitar y leer texturas del sistema Sparse. Por lo tanto, las funciones anteriores basadas en las coordenadas de textura **vec2** y los **muestreadores** han quedado obsoletas. Ahora se proporcionan funciones auxiliares en lugar de utilizar las texturas dispersas.

Para actualizar los sombreadores :

* Para **sombreador de Substance 3D Painter predeterminado** : Siga el procedimiento paso a paso de la página [Actualizando un sombreado](../interface/shader-settings/updating-a-shader.md).
* Para **sombreador personalizado** : echa un vistazo a los mensajes de error del registro, así como a la página [API del sombreador](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).

>[!WARNING]
>
> Los proyectos más antiguos pueden mostrar destellos blancos si sus sombreados no están actualizados. Consulte esta página para obtener más información : [Parpadeo de malla a blanco al mover la cámara](../technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.md).
