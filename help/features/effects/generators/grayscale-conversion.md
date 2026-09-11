---
title: Conversión de escala de grises
description: Aprenda a utilizar el generador de Conversiones de escala de grises de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 5%

---


# Conversión de escala de grises

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_grayscale_conversion.png" alt=""/><br><strong>En:</strong> generador, escala de grises, color</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de Conversiones de escala de grises convierte una textura o asignación en valores de escala de grises.<br><br>El generador de Conversión de escala de grises emite una textura monocroma (en blanco y negro). Como resultado, resulta útil para generar máscaras a partir de un mapa de entrada a todo color.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| Color de **origen** | Utilice una textura de color personalizada o un punto de ancla. |

## Parámetros

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Tipo de escala de grises</strong></td>
    <td>Establezca el método de conversión de escala de grises: <br><ul><li><strong>Desaturación</strong>: Utiliza el valor situado a medio camino entre el más fuerte y el más débil de los canales de RGB.</li><li><strong>Luminancia</strong>: Utiliza coeficientes RGB ponderados que coinciden con el brillo percibido por el ojo humano (favoreciendo el verde).</li><li><strong>Promedio</strong>: Mezcla los canales rojo, verde y azul en la misma cantidad.</li><li><strong>Máx.</strong>: Utiliza el valor más alto de los canales de RGB.</li><li><strong>Min</strong>: Utiliza el valor más bajo de los canales de RGB.<ul><li>Canal rojo: Utiliza únicamente el canal rojo.</li><li>Canal verde: Utiliza únicamente el canal verde.</li><li>Canal azul: Utiliza únicamente el canal azul.</li></ul></li></ul></td>
  </tr>
  <tr>
    <td><strong>Invertir</strong></td>
    <td>Invierte la máscara.</td>
  </tr>
  <tr>
    <td><strong>Equilibrio</strong></td>
    <td>Ajusta el equilibrio de la imagen de origen convertida, desplazando el punto medio hacia el blanco o el negro como un control de brillo.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Define el contraste o la atenuación de la imagen de origen convertida.</td>
  </tr>
  <tr>
    <td><strong>Mosaico</strong></td>
    <td>Establece el mosaico de la imagen de origen convertida.</td>
  </tr>
  <tr>
    <td><strong>Rotación</strong></td>
    <td>Ajusta el ángulo de la imagen de origen convertida.</td>
  </tr>
  <tr>
    <td><strong>Giro seguro</strong></td>
    <td>Activa o desactiva el modo de rotación segura . Cuando es verdadero, la rotación segura bloquea la rotación en ángulos de 45 grados.</td>
  </tr>
</table>
