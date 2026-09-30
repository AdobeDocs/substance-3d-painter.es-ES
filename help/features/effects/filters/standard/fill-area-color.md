---
title: Color del área de relleno
description: Aprenda a utilizar el filtro Color de área de relleno de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 1%
---

# Color del área de relleno

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono Color de área de relleno](./Resources/icon_fill_area_color.png "Color de área de relleno")

<b>En:</b> Efectos/relleno, forma, contorno, rgba, color

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Color de área de relleno convierte contornos en formas rellenas. Cualquier área con un borde continuo se rellena. La versión de color utiliza alfa para determinar los bordes de área.

Se utiliza en una capa de pintura (canal de color) para rellenar trazos pintados cerrados.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Detección de área:</b> | Seleccione cómo se identifica el área que se va a rellenar. |
| <b>Umbral de detección de área:</b> | Ajuste el umbral de detección de área. |
| <b>Detección de área de depuración:</b> | Alternar la visualización del contorno detectado por el ajuste Detección de área. Esto puede ayudar a identificar las áreas que pueden no estar completamente cerradas. |
| <b>Comportamiento de borde UV:</b> | Seleccione cómo se manejan los bordes UV durante el relleno de área. |
| <b>Umbral de borde UV:</b> | Ajuste el umbral utilizado para ignorar las áreas UV que, de otro modo, el proceso de detección de áreas podría rellenar. |
| <b>Modo de color:</b> | Seleccione qué método se utiliza para rellenar el interior del área. |
| <b>Color de relleno:</b> | Ajustar el color de relleno. |
| <b>Intensidad de desenfoque:</b> | Ajusta la intensidad del desenfoque. |
| <b>Ejemplos de desenfoque:</b> | Ajusta el número de muestras de desenfoque. |
| <b>Iteraciones de difusión:</b> | Ajuste el número de iteraciones de difusión que desea realizar. Los valores más altos mejoran el resultado, pero son más lentos. Los valores útiles se encuentran en el intervalo [8, 48]. |
