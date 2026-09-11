---
title: Costura automática
description: Aprenda a utilizar el generador de grapado automático de Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 1%

---


# Costura automática

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_auto_stitcher.png" alt=""/><br><strong>En:</strong> punto, puntos</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de elementos de unión automática crea automáticamente un efecto de unión a lo largo de las rutas generadas por el procedimiento. Estos trazados se pueden generar en función de las costuras UV, la curvatura o un mapa de entrada personalizado.<br><br>El generador Auto Stitcher emite una textura monocromática (en blanco y negro). Como resultado, resulta útil para generar máscaras y aplicar efectos de costura.<br><br>Para usar el modo Máscara de curvatura, se requiere un mapa de curvatura horneado. <a href="../../../baking/baking.md">Obtenga más información sobre cómo hacer un bake aquí</a>.</td>
  </tr>
</table>

## Entradas

<table>
  <tr>
    <th>Nombre de entrada</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td>Escala de grises <strong>Curvatura</strong></td>
    <td>Seleccione cómo generar los trazados de unión:<br><ul><li><strong>Máscara UV</strong> genera las rutas a lo largo de las uniones UV.</li><li><strong>La curvatura </strong> genera trazados cerca de los bordes duros.</li><li><strong>La entrada personalizada</strong> le permite controlar dónde se generan las rutas de acceso mediante un mapa.<br>Cuando se usa <strong>entrada personalizada</strong>, las rutas se generan en áreas de alto contraste.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Entrada personalizada</strong> en escala de grises</td>
    <td>Utilice una textura personalizada o un punto de ancla.</td>
  </tr>
</table>

## Parámetros

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Modo Máscara</strong></td>
    <td>Seleccione el modo Máscara .<br><ul><li>Máscara UV: Máscaras basadas en Islas de UV.</li><li>Curvatura: Máscaras basadas en el mapa de curvatura.</li><li>Entrada personalizada: Máscaras basadas en una textura de entrada personalizada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Smoothness de trazado</strong></td>
    <td>Suaviza el trazado en el que se aplican los puntos.</td>
  </tr>
  <tr>
    <td><strong>Posición del trazado</strong></td>
    <td>Desplazar la posición del trazado.</td>
  </tr>
  <tr>
    <td><strong>Tamaño de puntada</strong></td>
    <td>Ajuste la escala de los puntos.</td>
  </tr>
  <tr>
    <td><strong>Ancho de unión</strong></td>
    <td>Ajuste la anchura de los puntos.</td>
  </tr>
  <tr>
    <td><strong>Longitud de puntada</strong></td>
    <td>Ajustar la longitud de los puntos.</td>
  </tr>
  <tr>
    <td><strong>Redondez de puntada</strong></td>
    <td>Ajustar la redondez de los puntos.</td>
  </tr>
  <tr>
    <td><strong>Variación</strong></td>
    <td>Ajuste la variación en la dirección del flujo de puntos.</td>
  </tr>
</table>

## Ejemplos

<table>
  <tr>
    <td><img src="../../../assets/generators/examples/auto-stitcher/custom-input2.png" alt=""/></td>
    <td>En este ejemplo se muestra cómo la entrada personalizada crea trazados de unión. <br><ul><li>El color base en blanco y negro muestra las texturas de ruido que utilizamos como entrada personalizada para el generador de autostitcher.</li><li>El generador de autostitcher está enmascarando la capa roja, dejando visibles los trazados unidos en rojo.</li><li>Observe que los trazados unidos en rojo se ajustan a regiones negras o blancas suficientemente grandes de la textura de ruido de entrada personalizada. La costura roja nunca se cruza de blanco a negro o de negro a blanco.</li></ul><br>La imagen siguiente muestra la configuración de capa simple utilizada para crear este ejemplo.<br><br><img src="../../../assets/generators/examples/auto-stitcher/custom-input-layer-stack.png" alt=""/></td>
  </tr>
</table>
