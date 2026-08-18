---
title: Tri-Planar avanzado
description: Aprenda a utilizar el generador Tri-Planar Advanced de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 2%

---


# Tri-Planar avanzado

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_tri_planar_advanced.png" alt=""/><br><strong>En:</strong> máscara, generador</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador Tri-Planar Advanced es una versión independiente del modo de fusión triplanar con controles manuales para la proyección completa, incluido el control sobre todos los valores de rotación y desplazamiento para cada eje independiente. En comparación con la proyección de relleno nativa, el generador Tri-Planar Advanced utiliza normales de espacio de mundo para fusionar los tres ejes de proyección, mientras que la implementación nativa solo se basa en geometría de baja polimerización. Esto se traduce en un mayor control y resultados más precisos.<br><br>El generador Tri-Planar Advanced genera una textura monocromática (blanco y negro). Por lo tanto, resulta útil para generar una fusión triplanar de una máscara personalizada o un punto de ancla que se vaya a utilizar como máscara.Se requieren mapas normales de posición de horneado y espacio de entorno como entradas de imagen. <br><br><a href="../../../baking/baking.md">Obtenga más información sobre el horneado aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| **Espacio normal del mundo** Color | Utilice el mapa de normas espaciales mundiales horneadas. |
| Color de **Posición** | Utilice el mapa de posición horneado. |
| **máscara** en escala de grises | Utilice una textura personalizada o un punto de ancla. |

## Parámetros

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Proyección</strong></td>
    <td>Seleccione si desea proyectar todos los ejes o sólo un único eje.</td>
  </tr>
  <tr>
    <td><strong>Modo de fusión</strong></td>
    <td>Seleccione el Modo de fusión para fusionar los ejes.<br><ul><li><strong>Lineal</strong>: En el modo de fusión lineal, la línea de transición de fusión es recta.</li><li><strong>Avanzado</strong>: En el modo de fusión Avanzado, los ejes se fusionan en función del valor máximo entre los 3 ejes y el ángulo normal en la ubicación dada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de fusión</strong></td>
    <td>Ajuste cuánto se desenfoca la línea de transición de fusión.</td>
  </tr>
  <tr>
    <td><strong>Mosaico de textura</strong></td>
    <td>Ajuste el mosaico de la textura de la máscara.</td>
  </tr>
</table>

### Eje X

| Nombre del parámetro | Descripción |
| --- | --- |
| **Rotación X** | Gire la proyección de textura del eje X. |
| **Desplazamiento X X** | Mueva la proyección de textura del eje X hacia la izquierda o hacia la derecha. |
| **Desplazamiento X Y** | Mueva la proyección de textura del eje X hacia arriba o hacia abajo. |

### Eje Y

| Nombre del parámetro | Descripción |
| --- | --- |
| **Rotación X** | Gire la proyección de textura del eje Y. |
| **Desplazamiento Y X** | Mueva la proyección de textura del eje Y hacia la izquierda o la derecha. |
| **Desplazamiento Y** | Mueva la proyección de textura del eje Y hacia arriba o hacia abajo. |

### Eje Z

| Nombre del parámetro | Descripción |
| --- | --- |
| **Rotación X** | Gire la proyección de textura del eje Z. |
| **Desplazamiento Z X** | Mueva la proyección de textura del eje Z hacia la izquierda o hacia la derecha. |
| **Desplazamiento Z Y** | Mueva la proyección de textura del eje Z hacia arriba o hacia abajo. |
