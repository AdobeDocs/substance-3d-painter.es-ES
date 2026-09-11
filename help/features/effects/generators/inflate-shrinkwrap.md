---
title: Inflar envoltura de contracción
description: Aprenda a utilizar el generador de envoltura de contracción de inflado de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 3%

---


# Inflar envoltura de contracción

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_inflate_shrinkwrap.webp" alt=""/><br><strong>En:</strong> envolver, inflar, generador, semilla aleatoria</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador Inflate Shrinkwrap añade arrugas que imitan el efecto de un material delgado que se estira sobre la superficie de la malla.<br><br>El generador Inflate Shrinkwrap genera una textura monocromática (en blanco y negro). Por lo tanto, resulta útil para generar máscaras que creen el efecto de envolver con contracción. Sin embargo, también se puede colocar directamente sobre una capa de relleno para añadir arrugas al height y a los canales normales.<br><br>Se requiere un mapa de curvatura hecho un bake como entrada de imagen. <a href="../../../baking/baking.md">Obtenga más información sobre cómo hacer un bake aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| Escala de grises **Curvatura** | Utilice el mapa de curvatura hecho un bake. |

## Parámetros

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Ajuste preestablecido</strong></td>
    <td>Cambie entre los ajustes preestablecidos Inflado, Tirado al vacío y Apretado.</td>
  </tr>
  <tr>
    <td><strong>Grano</strong></td>
    <td>Defina el valor de inicialización utilizado para generar la textura de dirt. <br><ul><li>Haga clic en Aleatorio para cambiar a otra semilla aleatoria.</li><li>Haga clic en el lápiz para ver el valor de inicialización actual e introduzca un valor específico si lo desea.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Inflar o envolver</strong></td>
    <td>Cambie entre el modo de inflado y enrollado.</td>
  </tr>
  <tr>
    <td><strong>Intensidad de costura</strong></td>
    <td>Ajuste la pronunciación de los bordes.</td>
  </tr>
  <tr>
    <td><strong>Anchura de borde elevada</strong></td>
    <td>Ajuste cuánto se balancean los bordes inflados.</td>
  </tr>
  <tr>
    <td><strong>Intensidad del borde elevado</strong></td>
    <td>Ajuste la intensidad del efecto Borde elevado.</td>
  </tr>
  <tr>
    <td><strong>Densidad de arrugas</strong></td>
    <td>Ajuste el número de arrugas.</td>
  </tr>
  <tr>
    <td><strong>Tensión de arruga</strong></td>
    <td>Ajuste cómo se juntan las arrugas en los bordes UV.</td>
  </tr>
  <tr>
    <td><strong>Rango de arrugas</strong></td>
    <td>Ajuste hasta dónde llegan las arrugas desde los bordes UV.</td>
  </tr>
  <tr>
    <td><strong>Escala de arrugas</strong></td>
    <td>Ajuste el tamaño de las arrugas.</td>
  </tr>
</table>

### Parámetros técnicos

| Nombre del parámetro | Descripción |
| --- | --- |
| **Intervalo de Height** | Defina el rango de height. |
| **Posición del Height** | Ajuste el height hacia el negro (0) o el blanco (1). |
| **Tamaño de superficie (cm)** | Defina el tamaño físico de la superficie. |
| **Profundidad superficial (cm)** | Establezca la profundidad física de la superficie. |
