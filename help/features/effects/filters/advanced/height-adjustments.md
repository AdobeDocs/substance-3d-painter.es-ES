---
title: Ajuste de height
description: Aprenda a utilizar el filtro Ajustar Height de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 1%
---

# Ajuste de height

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono de ajuste de Height](./Resources/icon_height_adjust.png "Ajuste de Height")

<b>Entrada:</b> Efectos/ajustes, escalar, desplazar, invertir

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El Height Ajustar filtro invierte, desplaza o multiplica el canal de height por el valor elegido.

Se utiliza en una capa de textura o dentro de una máscara (salida en blanco y negro) para ajustar la información de height de forma no destructiva.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Invertir:</b> | Alternar la inversión del resultado. |
| <b>Desplazamiento:</b> | Ajuste el valor de height sumando o restando la cantidad especificada. |
| <b>Multiplicar:</b> | Multiplique los valores de height por este valor. Como multiplicador, esto hace que las áreas más altas y las más bajas sean más bajas. |

>[!NOTE]
>
> Los parámetros **Multiply** y **Offset** se apilan, aplicándose primero Offset. Si el desplazamiento produce un valor de height de cero en un punto determinado, la multiplicación se multiplicará por cero, lo que significa que no provocará ningún cambio en ese punto. Para multiplicar y, a continuación, desplazar los valores multiplicados, puede agregar un segundo filtro Ajustar Height.
