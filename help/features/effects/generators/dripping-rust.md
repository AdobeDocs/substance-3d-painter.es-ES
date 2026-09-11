---
title: Óxido goteo
description: Aprenda a utilizar el generador de Óxidos de goteo de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 2%

---


# Óxido goteo

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_dripping_rust.webp" alt=""/><br><strong>En:</strong> generador, escala de grises, color</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de Óxido de goteo crea rayas de óxido que fluyen hacia abajo, simulando la corrosión causada por la gravedad y la escorrentía de agua.<br><br>El generador de Óxido de goteo genera una textura monocromática (blanco y negro). Como resultado, resulta útil para generar máscaras y crear un efecto de óxido por goteo.Se requiere <br><br>posición, curvatura y oclusión ambiental Hechas un bake como entradas de imagen. <a href="../../../baking/baking.md">Obtenga más información sobre cómo hacer un bake aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| Escala de grises **Curvatura** | Utilice el mapa de curvatura hecho un bake. |
| **Oclusión ambiental** en escala de grises | Utilice el mapa de Oclusión ambiental hecho un bake. |
| Color de **Posición** | Utilice el mapa de posición hecha un bake. |

## Parámetros

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Grano</strong></td>
    <td>Defina el valor de inicialización utilizado para generar la textura de dirt. <br><ul><li>Haga clic en Aleatorio para cambiar a otra semilla aleatoria.</li><li>Haga clic en el lápiz para ver el valor de inicialización actual e introduzca un valor específico si lo desea.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Invertir</strong></td>
    <td>Invierte mapas internos específicos (por ejemplo, Curvatura, AO) antes de que se combinen en la máscara final.</td>
  </tr>
  <tr>
    <td><strong>Difusión de óxido</strong></td>
    <td>Ajuste la expansión del efecto óxido de goteo.</td>
  </tr>
  <tr>
    <td><strong>Contraste de óxido</strong></td>
    <td>Ajusta el contraste del efecto de óxido de goteo.</td>
  </tr>
  <tr>
    <td><strong>Smoothness de difusión</strong></td>
    <td>Ajuste la suavidad de expansión del efecto óxido de goteo.</td>
  </tr>
  <tr>
    <td><strong>Intensidad de goteo</strong></td>
    <td>Ajuste la longitud del efecto óxido de goteo.</td>
  </tr>
  <tr>
    <td><strong>Smoothness de goteo</strong></td>
    <td>Ajuste la suavidad del efecto óxido de goteo.</td>
  </tr>
  <tr>
    <td><strong>Cantidad de muestras de goteos</strong></td>
    <td>Ajuste la calidad del efecto (más muestras para una mejor calidad).</td>
  </tr>
  <tr>
    <td><strong>Eje de posición</strong></td>
    <td>Cambie entre el canal verde Y, el canal rojo X y el canal azul B para cambiar la dirección del efecto del óxido de goteo.</td>
  </tr>
</table>
