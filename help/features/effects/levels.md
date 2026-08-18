---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/effects/levels.html"
breadcrumb-title: ''
description: Aprenda a utilizar el efecto Niveles en Substance 3D Painter para ajustar el brillo, el contraste y la gama tonal de las texturas.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Levels
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Niveles
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Niveles

El nivel es un efecto que se utiliza para ajustar las gamas de colores de una imagen. Permite equilibrar y tonificar colores y/o valores de escala de grises. Puede añadirlo abriendo el menú de efectos :

![](../../assets/level-menu.png)

La interfaz principal muestra un histograma (la montaña de colores en el centro de la interfaz) que es la representación de cómo se distribuyen los píxeles en una imagen en cada nivel de intensidad de color. El histograma muestra los detalles en las sombras (parte izquierda), los medios tonos (parte central) y las iluminaciones (parte derecha). El histograma también ofrece una visión rápida de la gama tonal de los colores, lo que permite determinar qué tan oscura o brillante es la imagen.

![](../../assets/image2015-3-20-11-24-24.png)

Para ajustar la gama de colores de la imagen, hay dos conjuntos de controles disponibles en la parte superior e inferior del histograma:

* Los tres botones superiores controlan las sombras, los tonos medios y las iluminaciones y se pueden utilizar para redistribuir la gama tonal y contrastar la imagen global.
* Los dos botones inferiores controlan el negro y el punto blanco de la imagen (normalmente 0 y 255). Esto puede resultar útil para invertir los colores de una imagen, por ejemplo.

>[!NOTE]
>
> El efecto de niveles solo se puede aplicar a un canal a la vez, como se selecciona en la opción *Canal afectado*. Si desea aplicar un nivel en varios canales, tendrá que crear varios efectos de niveles.

* El cuadro desplegable Colores de la parte superior derecha le permite cambiar los niveles en la imagen rgb completa o solo en uno de los canales rojo, verde y azul.
* La opción Abrazadera de la parte inferior derecha le permite fijar los valores de los niveles entre 0 y 1 (0-255). Esta opción siempre debe marcarse al trabajar con canales que no sean HDR (como **Color base**).

[Para entender mejor los niveles, debería ver nuestro curso sobre la Academia de Substance dedicado al tema.](https://academy.substance3d.com/courses/Mastering-Levels-Histogram)
