---
title: Posición
description: Aprenda a utilizar el generador Posición de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 3%

---


# Posición

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_position.webp" alt=""/><br><strong>En:</strong> malla, uv, distancia</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador Posición utiliza los mapas normales de posición y espacio de mundo hechos un bake para crear una máscara de degradado basada en la posición del material en el espacio 3D (como de arriba a abajo o de lado a lado).<br><br>El generador Posición genera una textura monocromática (en blanco y negro). Por lo tanto, resulta útil para generar máscaras de degradado basadas en la posición en el espacio de entorno.Se requieren mapas normales de posición Hecha un bake y espacio mundial como entradas de imagen. <br><br><a href="../../../baking/baking.md">Obtenga más información sobre cómo hacer un bake aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| Color de **Textura** | Utilice una textura personalizada o un punto de ancla. |
| **Degradado de posición** Color | Utilice el mapa de posición hecha un bake. |
| **Normales del espacio mundial** Color | Utilice el mapa hecho un bake de las normas espaciales mundiales. |

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| **Inversión global** | Invierte el resultado final después de combinar todos los efectos. |
| **Desenfoque global** | Desenfoca la máscara final uniformemente después de combinar todos los degradados. |
| **Equilibrio global** | Ajuste el equilibrio de la máscara final después de que todos los degradados se combinen entre blanco o negro, como un ajuste de brillo. |
| **Contraste global** | Ajuste el contraste de la máscara final después de combinar todos los degradados. |
| **Usar Textura** | Activar o desactivar el uso de un mapa de textura personalizado. |

### Degradado de posición

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte solo el degradado de posición. |
| **Saldo** | Ajusta el equilibrio de solo el degradado de posición, desplazando el punto medio hacia el blanco o el negro como un control de brillo. |
| **Contraste** | Ajuste el contraste o la difuminación solo del degradado de posición. |
| **Brillo** | Ajuste la luminosidad solo del degradado de posición. |
| **De derecha a izquierda** | Ajuste cómo se aplica el efecto de izquierda a derecha en la malla. |
| **De arriba abajo** | Ajuste cómo se aplica el efecto de arriba abajo en la malla. |
| **De frente a atrás** | Ajuste cómo se aplica el efecto de delante hacia atrás en la malla. |

#### Degradado de posición/de derecha a izquierda

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte la dirección del degradado de derecha a izquierda. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para el degradado de derecha a izquierda. |

#### Degradado de posición/De arriba abajo

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierta la dirección del degradado de arriba a abajo. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para el degradado superior e inferior. |

#### Degradado de posición/Delantero hacia atrás

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierta la dirección del degradado de delante a detrás. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para el degradado de delante a atrás. |

### Textura

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Opacidad de textura</strong></td>
    <td>Ajuste la visibilidad de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Invertir</strong></td>
    <td>Invierte el mapa de textura personalizado.</td>
  </tr>
  <tr>
    <td><strong>Conversión de escala de grises</strong></td>
    <td>Establezca el método utilizado para convertir de color completo a escala de grises. El generador de Conversiones de escala de grises <a href="grayscale-conversion.md">tiene más información sobre cómo funciona cada método</a>.</td>
  </tr>
  <tr>
    <td><strong>Modo de fusión</strong></td>
    <td>Seleccione el <a href="../../../interface/layer-stack/blending-modes.md">modo de fusión</a> que desea usar.</td>
  </tr>
  <tr>
    <td><strong>Escala</strong></td>
    <td>Ajuste el tamaño de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Ajuste el contraste/difuminado de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Brillo</strong></td>
    <td>Ajuste la luminosidad de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Cuando <strong>Usar triplanar </strong> está habilitado, la textura se proyecta desde tres direcciones (ejes X, Y, Z) en lugar de depender solo de UV. <br><ul><li>Sin la opción triplanar activada, la textura sigue el diseño UV.</li><li>Con triplanar activado, la textura se proyecta desde múltiples ángulos y se mezcla.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanar</strong></td>
    <td>Ajuste la suavidad con la que se fusiona una textura cuando se proyecta mediante la asignación triplanar. Esto ajusta la suavidad de la fusión entre las proyecciones desde cada dirección.</td>
  </tr>
</table>
