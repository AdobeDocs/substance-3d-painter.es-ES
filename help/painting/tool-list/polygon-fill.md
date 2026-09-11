---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/painting/tool-list/polygon-fill.html"
breadcrumb-title: ''
description: Utilice la herramienta Relleno de polígono de Substance 3D Painter para rellenar los polígonos seleccionados con pintura para pintar texturas de forma eficaz.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Polygon fill
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Relleno poligonal
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 1%

---


# Relleno poligonal

La herramienta **Relleno de polígono** (![](../../assets/image2018-6-12-18-15-12.png)) le permite dibujar máscaras rápidamente convirtiendo los polígonos seleccionados en una máscara de píxeles. Puede parecer una herramienta de selección 3D de otras aplicaciones de 3D CC, pero en realidad es una herramienta de relleno de pintura que genera datos de píxeles. Eso significa seleccionar y anular la selección de las obras mediante su uso para la pintura de blanco o negro.

La herramienta Relleno poligonal funciona en [Capas de pintura](../../interface/layer-stack/layer-stack.md), pero está limitada a solo color base y no está diseñada para este fin. [Utilícelo solo para máscaras](../../interface/layer-stack/masking-and-effects.md).

Dispone de 4 modos de selección:

* ![](../../assets/image2020-9-30-11-31-53.png) **Relleno de triángulo**: llena los tri de malla individuales.
* ![](../../assets/image2020-9-30-11-32-12.png) **Relleno de polígono**: rellena polígonos completos. No realiza ninguna acción diferente de Relleno triangular si la malla ya se trianguló al exportar.
* **![](../../assets/image2020-9-30-11-32-42.png)Relleno de malla**: llena todas las submallas conectadas. Al igual que el modo &quot;subobjeto&quot; en las aplicaciones 3D, rellenará todos los polígonos conectados al que se ha hecho clic.
* **![](../../assets/image2020-9-30-11-32-54.png)Relleno de fragmentos UV**: llena todo el fragmento UV o &quot;isla&quot;. Funciona como relleno de malla, pero observando polígonos conectados en el espacio UV. El relleno se detiene en los bordes UV.

![](../../assets/polygon-fill.gif)

Estos 4 modos se pueden combinar y cambiar, lo que significa que un uso inteligente le permite marcar y desmarcar rápidamente secciones en una máscara usando el modo de fragmentos de malla y UV.

Los métodos abreviados de teclado (predeterminados) asociados a la herramienta Relleno poligonal son:

* *Clave numérica 4*: selecciona la herramienta Relleno poligonal.
* *X*: Invierte el color actual al pintar máscaras. Cambiará rápidamente negro por blanco. En el modo de pintura de materiales, esta tecla de acceso rápido no tiene efecto.
