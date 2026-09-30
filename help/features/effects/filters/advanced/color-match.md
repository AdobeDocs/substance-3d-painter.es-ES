---
title: Coincidencia de color
description: Aprenda a utilizar el filtro de coincidencia de color en Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%
---

# Coincidencia de color

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_color_match.png" alt="Icono de coincidencia de color" title="Coincidencia de color"/><br><strong>En:</strong> Efectos/ajustes</td>
    <td style="border: 0;" valign="top">Descripción<br>El filtro Coincidencia de color hace coincidir un rango de color de origen definido con un rango de color de destino, con compatibilidad con ranuras de entrada para definir valores de origen y de destino. La coincidencia de color le permite mantener los detalles mientras cambia el color de una superficie, con control sobre cómo se controlan el tono, el croma y la luminancia.<br>La coincidencia de color se usa en una capa de relleno para realizar ajustes de color precisos.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| **Color de origen:** | Ranura de entrada para el color de origen. Utilice un mapa de color personalizado o un punto de ancla. |
| **Color de destino:** | Ranura de entrada para el color de destino. Utilice un mapa de color personalizado o un punto de ancla. |

## Parámetros

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Modo de color de origen:</strong></td>
    <td>Seleccione el origen del color de origen.<br><ul><li><strong>Promedio</strong>: Utilice el color del material existente como color de origen. Tenga en cuenta que esto requiere que el modo de fusión de capas esté establecido en <strong>Acceso directo</strong>.</li><li><strong>Parámetro</strong>: Defina el color de origen mediante un parámetro.</li><li><strong>Entrada</strong>: Defina el color de origen con una entrada de imagen.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Color de origen:</strong></td>
    <td>Ajuste el color de origen cuando <strong>Modo de color de origen</strong> esté establecido en <strong>Parámetro</strong>.</td>
  </tr>
  <tr>
    <td><strong>Modo de color de destino:</strong></td>
    <td>Seleccione el origen del color de destino.<br><ul><li><strong>Parámetro</strong>: Defina el color de destino mediante un parámetro.</li><li><strong>Entrada</strong>: Defina el color de destino con una entrada de imagen.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Color de destino:</strong></td>
    <td>Ajuste el color de destino cuando <strong>Modo de color de destino</strong> esté establecido en <strong>Parámetro</strong>.</td>
  </tr>
  <tr>
    <td><strong>Variación de color personalizada:</strong></td>
    <td>Cambia los controles personalizados de variación de tono, croma y luminancia.</td>
  </tr>
  <tr>
    <td><strong>Tono:</strong></td>
    <td>Ajuste la variación de tono aplicada al resultado.</td>
  </tr>
  <tr>
    <td><strong>Croma:</strong></td>
    <td>Ajuste la variación de croma aplicada al resultado.</td>
  </tr>
  <tr>
    <td><strong>Luminancia:</strong></td>
    <td>Ajuste la variación de luminancia aplicada al resultado.</td>
  </tr>
</table>