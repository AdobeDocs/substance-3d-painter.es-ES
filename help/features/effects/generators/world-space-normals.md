---
description: Aprenda a utilizar el generador World Space Normals de Substance 3D Painter.
title: Normales de espacio de mundo
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---


# Normales de espacio de mundo

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_world_space_normals.png" alt=""/><br><strong>En:</strong> máscara, generador, escala de grises, fusión</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador World Space Normal usa el mapa normal de espacio de mundo horneado para colorear el modelo o aplicar efectos en función de la dirección en la que se encuentra cada superficie en el espacio 3D. Por ejemplo, de arriba abajo.<br><br>El generador de World Space Normals produce una textura monocromática (en blanco y negro). Como resultado, resulta útil para generar máscaras aplicar diversos efectos como dirt, dust, nieve o óxido en función de las direcciones de la cara.Se requieren mapas normales de posición de horneado y espacio de entorno como entradas de imagen. <br><br><a href="../../../baking/baking.md">Obtenga más información sobre el horneado aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| Color de **textura** | Utilice una textura personalizada o un punto de ancla. |
| **Normales del espacio mundial** Color | Utilice el mapa de normas espaciales mundiales horneadas. |
| **Degradado de posición** Color | Utilice el mapa de posición horneado. |

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| **Inversión global** | Invierte el resultado final después de combinar todos los efectos. |
| **Desenfoque global** | Suaviza la máscara final uniformemente después de combinar todos los efectos. |
| **Equilibrio global** | Cambia el equilibrio de la máscara final después de que todos los efectos se combinen entre blanco o negro, como un ajuste de brillo. |
| **Contraste global** | Ajuste el contraste de la máscara final después de combinar todos los efectos. |
| **Usar textura** | Activar o desactivar el uso de un mapa de textura personalizado. |

### Normal de espacio de mundo

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte solo las normales del espacio mundial. |
| **Desenfocar** | Suaviza el espacio mundial solo normales. |
| **Saldo** | Ajusta el equilibrio de las normales del espacio mundial únicamente, desplazando el punto medio hacia el blanco o el negro como un control de brillo. |
| **Contraste** | Ajusta el contraste/difuminación de las normales del espacio mundial solamente. |
| **Brillo** | Ajusta la luminosidad de las normales del espacio mundial. |
| **De derecha a izquierda** | Ajuste cómo se aplica el efecto de izquierda a derecha en la malla. |
| **De arriba abajo** | Ajuste cómo se aplica el efecto de arriba abajo en la malla. |
| **De frente a atrás** | Ajuste cómo se aplica el efecto de delante hacia atrás en la malla. |

#### Espacio del mundo normal/de derecha a izquierda

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte la dirección del degradado de derecha a izquierda. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para la capa actual. |

#### Espacio Mundial Normal/De Arriba Abajo

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierta la dirección del degradado de arriba a abajo. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para la capa actual. |

#### Espacio Mundial Normal/Delantero a Atrás

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierta la dirección del degradado de delante a detrás. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para la capa actual. |

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
    <td>Invierte solo la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Conversión de escala de grises</strong></td>
    <td>Establezca el método utilizado para convertir de color completo a escala de grises. El generador de <a href="grayscale-conversion.md">conversión de escala de grises tiene más información sobre cómo funciona cada método</a>.</td>
  </tr>
  <tr>
    <td><strong>Modo de fusión</strong></td>
    <td>Ajuste la operación de fusión que se va a utilizar. Consulte la página dedicada sobre los modos de fusión.</td>
  </tr>
  <tr>
    <td><strong>Escala</strong></td>
    <td>Ajuste el tamaño de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Ajuste el contraste y el difuminado de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Brillo</strong></td>
    <td>Ajuste la luminosidad de la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Cuando la opción Triplanar está activada, la textura se proyecta desde tres direcciones (ejes X, Y, Z) en lugar de depender únicamente de UV.<br><ul><li>Sin triplanar, la textura sigue el diseño UV.</li><li>Con triplanar, la textura se proyecta desde múltiples ángulos y se mezcla.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanar</strong></td>
    <td>Ajuste la suavidad con la que se fusiona una textura cuando se proyecta mediante la asignación triplanar. Esto ajusta la suavidad de la fusión entre las proyecciones desde cada dirección.</td>
  </tr>
</table>
