---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/painting/advanced-channel-painting/height-map-painting.html"
breadcrumb-title: ''
description: Aprenda a pintar mapas de heightes directamente en Substance 3D Painter para crear efectos de elevación de desplazamientos y superficies.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Height Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pintura de mapa de height
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---


# Pintura de mapa de height

## Idea general

Trabajar en un mapa de alturas en lugar de hacerlo directamente en una zona normal ofrece varias ventajas, como una mejor calidad, un mejor control, flexibilidad y una mayor coherencia entre los activos.

El proceso es el siguiente:

* Un mapa normal, cocido de una malla de polietileno alta, se carga en la malla de polietileno baja.
* Pintará detalles adicionales en el canal del mapa de altura.
* El Height que pinta se compone a través de todas las capas y se convierte en un mapa normal en tiempo real, y finalmente se mezcla con el normal de la malla de polietileno alta.

Todo lo que tienes que preocuparte es pintar ese height, todo lo demás se hace automáticamente.

### Formato HDR de height

El canal de Height usa un formato de color **HDR**, que permite pintar valores positivos y negativos sin llegar nunca a un límite de brillo, a diferencia de los mapas de height tradicionales, que se saturarán entre 0 y 255.

* Cuando se pinta con un mapa de bits o una sustancia en un height, ese origen se reasigna de su rango original [0,255] a un rango [-1,1].

Un gris medio se reasignará a 0. Por lo tanto, los valores por debajo de 127 **restarán** del mapa de altura, mientras que los valores por encima de 127 **agregarán** al mismo cuando se utilice el modo de fusión predeterminado establecido para los mapas de height, **Sobreexposición lineal (agregar)**.

* Cuando pinte con color liso, podrá seleccionar directamente valores entre -1 y 1.

### Visualización de height

Al visualizar el mapa de Height en modo Solo, la previsualización predeterminada solo mostrará valores positivos, con una fuerte saturación de negro para los valores negativos.

La configuración **+/- color** permite visualizar todo el rango con un color diferente para los valores positivos y negativos.

La configuración **Scale** permite modificar el intervalo visible de ese mapa HDR en caso de que haya agregado o restado más del intervalo [-1,1] predeterminado.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/height1.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/height2.png)

</td>
</tr>
</table>
