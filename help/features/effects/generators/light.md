---
title: Claro
description: Aprenda a utilizar el generador de luz de Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---


# Luz

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_light.webp" alt=""/><br><strong>En:</strong> máscara, generador</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de luz finge una luz direccional que brilla en tu malla, basándose en los mapas de Posición y Normal del Espacio Mundial.<br><br>El generador de luz se puede usar en una capa de relleno o como para crear una máscara. Cuando se utiliza en una capa de relleno, el generador emite canales de color, metal, rugosidad del specular, normales y de height que se pueden utilizar en diversas combinaciones para crear diferentes efectos. Se recomienda recorrer las vistas de los canales en el área de visualización para comprender cómo el generador de luz afecta a cada canal.Se requieren mapas normales de posición de horneado y espacio de entorno como entradas de imagen. <br><br><a href="../../../baking/baking.md">Obtenga más información sobre el horneado aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| **Espacio normal del mundo** Color | Utilice el mapa de normas espaciales mundiales horneadas. |
| Color de **Posición** | Utilice el mapa de posición horneado. |

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte el mapa de color de salida. |
| **Ángulo horizontal** | Define el ángulo horizontal de la luz falsa. |
| **Ángulo vertical** | Define el ángulo vertical de la luz falsa. |
| **Resaltar brillo** | Ajuste el pliego de difuminado del área resaltada. |
| **Nivel de resaltado** | Ajusta el contraste del resaltado. |
| **Atenuación de luz** | Ajusta la difuminación de la luz. |
