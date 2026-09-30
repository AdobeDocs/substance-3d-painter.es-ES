---
title: Kuwahara anisotrópico
description: Aprende a usar el filtro Kuwahara Anisotrópico de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%
---

# Kuwahara anisotrópico

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono Kuwahara anisotrópico](./Resources/icon_anisotropic_kuwahara.png "Kuwahara anisotrópico")

<b>En:</b> Efectos/escala de grises, kuwahara, anisotrópico, estilizado

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Kuwahara anisotrópico crea efectos de estilización pictórica a la vez que conserva fuertes características direccionales.

Se utiliza en una capa de textura o dentro de una máscara (salida en blanco y negro) para crear un aspecto estilizado de materiales, sonidos y máscaras completos.

</td>
</tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| <b>Mapa de radio:</b> Escala de grises | Utilice una textura personalizada o un punto de ancla. |
| <b>Entrada personalizada:</b> Color | Utilice una textura personalizada o un punto de ancla. |

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Dirección de extracción:</b> | Selecciona cómo el filtro deriva la dirección del desenfoque. |
| <b>Radio:</b> | Ajusta el radio de desenfoque. Los valores más altos producen un efecto de desenfoque más fuerte. El valor máximo es 32. |
| <b>Smoothness:</b> | Ajuste la cantidad de colores que se fusionan en la dirección calculada. En 0, los colores se desplazan principalmente en esa dirección con muy poca fusión. |
| <b>Enfoque:</b> | Ajusta el contraste en las áreas desenfocadas para que parezcan más planas y definidas con mayor claridad. |
| <b>Smoothness del tensor:</b> | Ajuste la cantidad de desenfoque aplicado a las direcciones calculadas a partir de la imagen y almacenadas en el mapa de dirección. Los valores más altos producen un resultado más suave cuando la imagen contiene muchos detalles de alta frecuencia. |
| <b>Anisotropía:</b> | Ajusta en qué medida el mapa de dirección influye en el desenfoque. El mapa de dirección y sus modificadores todavía afectan el resultado incluso cuando este valor es 0, porque el mapa se usa en el núcleo del filtro Kuwahara. |
| <b>Ángulo de anisotropía:</b> | Ajuste la rotación aplicada al mapa de dirección por turnos. Esta rotación se añade al valor desde la entrada Mapa de Ángulo de anisotropía. |

