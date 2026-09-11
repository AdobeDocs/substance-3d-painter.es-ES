---
title: Curvatura
description: Aprenda a utilizar el generador de curvatura de Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 4%

---


# Curvatura

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_curvature.webp" alt=""/><br><strong>En:</strong> máscara, generador, escala de grises, fusión</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de curvatura crea una máscara basada en el mapa de curvatura hecho un bake con la opción de fusionar una textura o microdetalles en la máscara.<br><br>El generador de curvatura emite una textura monocromática (blanco y negro). Como resultado, es útil para generar máscaras en lugar de aplicarlas directamente a una capa.<br><br>Se requiere un mapa de posición hecho un bake como entrada. <a href="../../../baking/baking.md">Obtenga más información sobre cómo hacer un bake aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| Color de **Textura** | Utilice una textura personalizada o un punto de ancla. |
| **Micro Normal** Color | Utilice una textura normal personalizada o un punto de ancla. |
| **Micro Height** Color | Utilice una textura personalizada o un punto de ancla. |
| Escala de grises **Curvatura** | Utilice el mapa de curvatura hecho un bake. |
| **Normales del espacio mundial** Color | Utilice el mapa hecho un bake de las normas espaciales mundiales. |
| **Degradado de posición** Color | Utilice el mapa de posición hecha un bake. |

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| **Inversión global** | Invierte el resultado final después de combinar todos los efectos. |
| **Desenfoque global** | Suaviza la máscara final uniformemente después de combinar todos los efectos. |
| **Equilibrio global** | Desplaza el equilibrio de la máscara final después de que todos los efectos se combinen entre blanco o negro, como un ajuste de brillo. |
| **Contraste global** | Ajusta el contraste de la máscara final después de combinar todos los efectos. |
| **Usar Textura** | Activar o desactivar el uso de un mapa de textura personalizado. |
| **Usar detalles micro** | Activa o desactiva el uso del mapa de detalles de la micro personalizada. |

### Curvatura

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Invertir</strong></td>
    <td>Invierte el mapa de curvatura generado.</td>
  </tr>
  <tr>
    <td><strong>Modo</strong></td>
    <td>Defina el modo Curvatura. <br><ul><li><strong>Bordes</strong>: Enmascara los bordes (áreas convexas)</li><li><strong>Cavidades</strong>: Enmascara las cavidades (áreas cóncavas)</li><li><strong>Doble</strong>: Máscaras de áreas cóncavas y convexas.</li><li><strong>Sin procesar</strong>: Máscara de curvatura normal.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Nítido</strong></td>
    <td>Ajuste la intensidad de los detalles de curvatura nítidos.</td>
  </tr>
  <tr>
    <td><strong>Bien</strong></td>
    <td>Ajuste la intensidad de los detalles de curvatura fina.</td>
  </tr>
  <tr>
    <td><strong>Suave</strong></td>
    <td>Ajuste la intensidad de los detalles de la curvatura suave.</td>
  </tr>
  <tr>
    <td><strong>Medio</strong></td>
    <td>Ajuste la intensidad de los detalles de la curvatura media.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajuste la intensidad de los detalles de curvatura grandes.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajuste la intensidad de los detalles de curvatura grandes.</td>
  </tr>
  <tr>
    <td><strong>Enorme</strong></td>
    <td>Ajuste la intensidad de los detalles de curvatura enormes.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Ajuste el contraste/atenuación de la curvatura.</td>
  </tr>
  <tr>
    <td><strong>Brillo</strong></td>
    <td>Ajuste la luminosidad de la curvatura.</td>
  </tr>
</table>

### Textura

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Opacidad de textura</strong></td>
    <td>Controlar la visibilidad de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Invertir</strong></td>
    <td>Invierte solo la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Conversión de escala de grises</strong></td>
    <td>Seleccione el método utilizado para convertir la entrada de color en blanco y negro. </td>
  </tr>
  <tr>
    <td><strong>Modo de fusión</strong></td>
    <td>Defina el modo de fusión para la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Escala</strong></td>
    <td>Ajuste el tamaño de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Establezca el contraste o la difuminación de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Brillo</strong></td>
    <td>Ajuste la luminosidad de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Cuando la opción Triplanar está activada, la textura se proyecta desde tres direcciones (ejes X, Y, Z) en lugar de depender únicamente de UV. <br><ul><li>Sin la opción triplanar activada, la textura sigue el diseño UV.</li><li>Con triplanar activado, la textura se proyecta desde múltiples ángulos y se mezcla.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanar</strong></td>
    <td>Ajuste la suavidad con la que se fusiona una textura cuando se proyecta mediante la asignación triplanar. Esto ajusta la suavidad de la fusión entre las proyecciones desde cada dirección.</td>
  </tr>
</table>

### Detalles de Micro

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Micro Height</strong></td>
    <td>Activar o desactivar el uso de un mapa de altura micro personalizado.</td>
  </tr>
  <tr>
    <td><strong>Micro Normal</strong></td>
    <td>Activar o desactivar el uso de un Mapa de normales Micro personalizado.</td>
  </tr>
  <tr>
    <td><strong>Tipo de curvatura</strong></td>
    <td>Defina el tipo de curvatura. <br><ul><li><strong>Estándar</strong>: Generalmente produce un resultado bastante nítido, pero puede carecer de detalles más amplios.</li><li><strong>Sobel</strong>: Produce resultados similares en comparación con el estándar, pero ligeramente más borrosos porque evalúa el mapa normal utilizando un filtro Sobel.</li><li><strong>Suave</strong>: Produce diferentes niveles de desenfoque (como mipmaps) para acumular información. Esto suele proporcionar curvas más suaves, pero los detalles pueden perderse.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Intensidad de curvatura</strong></td>
    <td>Ajuste la intensidad de la curvatura en los modos de curvatura <strong>Estándar </strong> y <strong>Sobel </strong>.</td>
  </tr>
  <tr>
    <td><strong>Intensidad de detalles del height</strong></td>
    <td>Ajuste la intensidad de los detalles del Height Micro.</td>
  </tr>
</table>
