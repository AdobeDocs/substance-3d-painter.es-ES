---
breadcrumb-title: ""
description: Aprenda a utilizar la dilatación de textura y el relleno en Substance 3D Painter para evitar artefactos de borde en las texturas exportadas.
title: Dilatación de textura o relleno
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%
---

# Dilatación de textura o relleno

**Relleno** (también llamado a veces **dilatación**) es un proceso que ocurre después de la generación de una textura. Su propósito es dilatar los bordes de las Islas de UV para llenar áreas vacías con píxeles similares.

Generar un relleno de buena calidad es importante para garantizar una buena generación de [mipmaps](../../../getting-started/glossary.md) más tarde mediante motores de juegos o procesadores sin conexión.\
Substance 3D Painter puede generar un relleno infinito: esto significa que se estirará un píxel hasta que alcance otra Isla de UV o los bordes de la textura.

## Generación de relleno infinito

A continuación se muestra un ejemplo de cómo funciona el relleno infinito :

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/padding.gif){width="512px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/padding-zoom.gif)

</td>
</tr>
</table>

## MipMaps

En los gráficos de equipos 3D, **mipmaps** son secuencias de texturas optimizadas y precalculadas, cada una de las cuales representa una misma imagen a una resolución cada vez menor. Su objetivo es aumentar la velocidad de procesamiento y reducir los artefactos de suavizado. Una imagen mipmap de alta resolución se utiliza para objetos cercanos a la cámara. Las imágenes de baja resolución se utilizan ya que el objeto aparece más lejos. Se trata de una forma eficaz de procesar en lugar de leer todos los píxeles de la textura original. Los mipmaps (cada nivel) se incrustan dentro de la propia textura (cuando es compatible con el formato de archivo).

El relleno es muy importante para mipmaps, ya que evita que los colores incorrectos se sangren dentro de los UV de la malla cuando se van a resoluciones de textura más bajas.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-padding.gif){width="400px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-nopadding.gif){width="400px"}

</td>
</tr>
</table>

En el ejemplo anterior, el fondo gris se desvanece en los UV (imagen derecha), mientras que con el relleno se mantiene el color limpio (imagen izquierda).

Dentro de una aplicación 3D, este es el resultado:

![](../../../assets/padding-toggle.gif)

## Controles de relleno

Substance 3D Painter permite cambiar el comportamiento de la generación de relleno (como desactivarlo) en diferentes lugares :

* **Al hacer un bake** : consulte [haciendo un bake documentación](../../../baking/baking.md) para obtener más información.
* **Al generar texturas para un conjunto de texturas** : consulte la documentación de [Configuración de conjuntos de texturas](../../../interface/texture-set/texture-set-settings.md) para obtener más información.
* **Al exportar texturas** : consulte la sección &quot;Configuración de relleno&quot; de la documentación de [configuración de exportación](../../../export/export-window/export-window.md) para obtener más información.
