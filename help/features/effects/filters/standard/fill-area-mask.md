---
title: Máscara de área de relleno
description: Aprenda a utilizar el filtro Máscara de área de relleno de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 2%
---

# Máscara de área de relleno

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono de máscara de área de relleno](./Resources/icon_fill_area_mask.png "Máscara de área de relleno")

<b>En:</b> Efectos/relleno, forma, contorno, escala de grises

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Máscara de área de relleno convierte contornos en formas rellenas. Cualquier área con un borde continuo se rellena.

Se utiliza en una capa de máscara (salida en blanco y negro) después de añadir una capa de pintura para rellenar los trazos pintados cerrados.

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
| <b>Umbral de detección de bordes UV:</b> | Ajuste el umbral utilizado para ignorar las áreas UV que, de otro modo, el proceso de detección de áreas podría rellenar. |
