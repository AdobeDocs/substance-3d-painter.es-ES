---
title: Validación PBR
description: Aprenda a utilizar el filtro Validación PBR de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 2%
---

# Validación PBR

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono de Validación PBR](./Resources/icon_pbr_validate.png "Validación PBR")

<b>En:</b> Efectos/pbr, metálico, rugosidad

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Validación PBR valida los datos de PBR comprobando los valores de oscuridad del albedo y los rangos de reflectancia del metal.

Se utiliza en una capa de relleno para comprobar que los valores de material se mantienen dentro de los intervalos de PBR esperados. Las Validaciones PBR no deben estar habilitadas cuando se exportan materiales.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Modo de validación:</b> | Seleccione si desea validar el albedo, la reflectancia del metal o ambas cosas. |
| <b>Umbral de rango oscuro de Albedo:</b> | Seleccione el umbral mínimo de valor oscuro permitido para la validación de albedos. |
| <b>Rango de reflejo de metal:</b> | Seleccione el rango de reflectancia utilizado para validar valores metálicos. |
| <b>Mapa de superposición:</b> | Alternar la superposición de validación sobre los datos del mapa. |

