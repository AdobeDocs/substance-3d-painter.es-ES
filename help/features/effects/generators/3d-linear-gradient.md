---
title: 3D linear gradient
description: Aprenda a utilizar el generador de 3D linear gradient de Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---


# 3D linear gradient

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Degradado <img src="../../../assets/generators/icon_3d_linear_gradient.webp" alt=""/><br><strong>In:</strong>, escala de grises</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de 3D linear gradient usa el mapa de posición para crear un degradado entre dos puntos de la malla. <br><br>3D linear gradient emite una textura monocromática (blanco y negro). Como resultado, es útil para generar máscaras colocar un degradado lineal en un área específica.<br><br>Se requiere un mapa de posición hecho un bake como entrada de imagen. <a href="../../../baking/baking.md">Obtenga más información sobre cómo hacer un bake aquí</a>.<br><br>El mapa Posición asigna un color a cada punto de la malla que corresponde a su posición entre 0 y 1 a lo largo de los ejes X, Y y Z. Esto significa que cada punto de la malla tiene un color único. Puede definir puntos de inicio y fin para el degradado lineal seleccionando el color del mapa de posición en las ubicaciones de inicio y fin.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| **Posición** | Utilice el mapa de posición hecha un bake. |

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte el degradado lineal. |
| **Saldo** | Cambie la posición del punto medio del degradado lineal. |
| **Contraste** | Ajuste el contraste del degradado lineal. |
| **Inicio de posición 3D** | Establezca el punto inicial del degradado en función de los colores del mapa de posición. Para definir fácilmente el punto de inicio, visualice el mapa de posición en la pantalla de la ventana gráfica y utilice el selector de color para seleccionar el punto de inicio. |
| **Fin de posición 3D** | Establezca el punto final del degradado en función de los colores del mapa de posición. Para definir fácilmente el punto final, muestre el mapa de posición en la pantalla en la ventana gráfica y utilice el selector de color para seleccionar el punto final. |
