---
title: Daños en el borde MatFX
description: Aprenda a utilizar el filtro de daños en el borde MatFX de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 1%
---

# Daños en el borde MatFX

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono de daños en bordes de MatFX](./Resources/icon_matfx_edge_damages.png "Daños en bordes de MatFX")

<b>En:</b> Efectos/desenfoque, escala de grises

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Daños en el borde de MatFX crea detalles en los bordes astillados y dañados. Edge Damage se comporta de forma diferente al filtro MatFX Detail Edge Wear, ya que Edge Damage no cambia el color del área dañada. Esto significa que puede ser más útil para simular daños a materiales como plástico o resina, en lugar de Edge Wear, que es mejor utilizar para materiales como el metal pintado.

MatFX Edge Damages se utiliza en capas de textura o pilas de materiales para añadir detalles de bordes desgastados, rayados o dañados.

</td>
</tr>
</table>

>[!NOTE]
>
> Para que el filtro MatFX Edge Damages modifique el canal de height, debe haber datos de height existentes en el canal. En otras palabras, si no hay capas debajo de la capa de height que tengan datos de height, el filtro no tendrá un efecto observable en el canal de filtro.

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Intensidad de desenfoque:</b> | Ajuste la intensidad del efecto de desenfoque. |
| <b>Ajuste de desenfoque:</b> | Alternar el ajuste de desenfoque. Cuando está activado, el efecto toma muestras de los píxeles del lado opuesto de la textura. |
| <b>Nivel:</b> | Ajuste el nivel de daño global. |
| <b>Contraste:</b> | Ajuste el contraste o la atenuación del resultado. |
| <b>Intensidad de Scratches:</b> | Ajusta la intensidad de los arañazos. |
| <b>Rugosidad de daños:</b> | Ajuste la dureza de las áreas dañadas. |
| <b>Profundidad de daños:</b> | Ajuste la profundidad de las áreas dañadas. |
