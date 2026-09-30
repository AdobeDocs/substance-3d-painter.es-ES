---
title: Ajustar
description: Aprenda a utilizar el filtro Ajustar de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 2%
---

# Ajustar

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ajustar icono](./Resources/icon_clamp.png "Ajustar")

<b>En:</b> Efectos/ajustes

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Ajustar fija los valores a los límites definidos.

Se utiliza directamente en una capa de relleno para limitar aspectos específicos de un material, o bien en una máscara para restringir los valores a un rango determinado.

</td>
</tr>
</table>

>[!NOTE]
>
> Cuando se utiliza en una capa de relleno o como paso a través para obtener información de color, la abrazadera afecta a cada canal de color de forma individual. Por lo tanto, si un píxel determinado tiene un color de (R 0, G 0,5, B 1,0) y se fija a 0,5, el color resultante de ese píxel será (R 0, G 0,5, B 0,5). Esto se debe a que el canal Azul tenía un valor lo suficientemente alto como para ser sujetado, pero los otros canales no lo tenían. Esto significa que el filtro Ajustar puede cambiar el tono del contenido en color.
>
>Si no desea modificar el tono, otros filtros como Niveles pueden ser una mejor opción.

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Mín.:</b> | Ajuste el valor mínimo. |
| <b>Máx.:</b> | Ajuste el valor máximo. |
