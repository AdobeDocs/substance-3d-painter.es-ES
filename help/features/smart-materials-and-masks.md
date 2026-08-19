---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/smart-materials-and-masks.html"
breadcrumb-title: ''
description: Aprende a usar materiales y máscaras inteligentes en Substance 3D Painter para crear texturas de procedimiento que se adapten a la geometría.
helpx_creative_field: ""
helpx_description: Painter > Features > Smart Materials and Masks
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Materiales y máscaras inteligentes
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---


# Materiales y máscaras inteligentes

Substance 3D Painter admite el uso de **ajustes preestablecidos de capa** avanzados. Estos ajustes preestablecidos se pueden usar para **compartir rápidamente entre** conjuntos de texturas o proyectos, un **proceso de texturizado similar** mientras se mantienen los resultados diferentes, **adaptados a la topología de malla** .

>[!NOTE]
>
> Tenga en cuenta que, una vez añadido en la pila de capas, no hay forma de recuperar qué material inteligente se utilizó. En caso de que sea necesario actualizar un material inteligente, el proceso deberá realizarse manualmente.\
> Sin embargo, los recursos individuales se pueden actualizar con [Resources Updater](plugins/resources-updater.md) .

## ¿Cómo se usan los materiales/máscaras inteligentes?

Los materiales inteligentes se pueden usar en cualquier parte de la pila de capas, mientras que las máscaras inteligentes solo se pueden usar en la pila de efectos.\
Para obtener más información sobre las diferencias, consulte : [Pila de capas](../interface/layer-stack/layer-stack.md) y [Efectos](effects/effects.md)

### Adición de un material inteligente

Los materiales inteligentes se pueden añadir de dos formas diferentes:

* Arrastrando y soltando materiales inteligentes del estante en la pila de capas :\
  ![](../assets/sm-drop.gif)
* Al hacer clic en el botón Smart Material para abrir una miniestantería :\
  ![](../assets/sm-button.gif)

### Adición de una máscara inteligente

Dado que las máscaras inteligentes son ajustes preestablecidos de efectos, solo se pueden añadir a pilas de efectos (para máscaras específicas).

* Para añadir máscaras inteligentes, solo **arrastra y suelta** una desde la estantería a la capa **target** :\
  ![](../assets/smm-drop.gif)
* Si arrastras y sueltas **varias** máscaras inteligentes, se acumularán :\
  ![](../assets/smm-drop-accum.gif)
* Sin embargo, es posible **reemplazar** toda la pila de efectos presionando **CTRL** durante el arrastrar y soltar :\
  ![](../assets/smm-drop-replace.gif)

### ¿Cómo se crean materiales/máscaras inteligentes?

Para crear materiales inteligentes, se requiere una **carpeta**.\
El contenido de los materiales inteligentes se incluirá en la carpeta. A continuación, solo tienes que hacer clic con el botón derecho en la carpeta y seleccionar &quot;**Crear material inteligente**&quot;. A continuación, el material inteligente se añadirá al estante actual y se le asignará un nombre según la carpeta seleccionada.

![](../assets/create-sm.png)

Para crear una máscara inteligente, simplemente haz clic con el botón derecho sobre una capa y elige &quot;**Crear máscara inteligente**&quot;.

![](../assets/create-smm.png)

## ¿Cómo compartir/recuperar un material/máscara inteligente?

Los ajustes preestablecidos se guardan **en el disco** y se pueden recuperar de su carpeta dedicada.\
Para encontrar la **ubicación del estante**, consulte : [Agregando contenido al disco duro](../content/importing-assets/adding-content-on-the-hard-drive.md) .

Entonces cualquiera puede simplemente **importar** el archivo en su estante de Substance 3D Painter para usar el ajuste preestablecido.
