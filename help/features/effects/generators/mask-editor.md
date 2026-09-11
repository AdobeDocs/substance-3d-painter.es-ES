---
title: Editor de máscaras
description: Aprenda a utilizar el generador del Editor de máscaras de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 3%

---


# Editor de máscaras

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_mask_editor_dark.png" alt=""/><strong>En:</strong> máscara, generador</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador del Editor de máscaras es un generador de máscaras multiusos que te permite combinar Texturas, Oclusión ambiental, Curvatura, Espacio normal del mundo, Degradado, Thickness y Micro detalles en una sola máscara.<br>El generador Mask Builder es muy flexible, pero debido a su complejidad, puede afectar el rendimiento más que la mayoría de los generadores.<br><br>El generador del Editor de máscaras genera una textura monocromática (en blanco y negro). Por lo tanto, resulta útil para generar máscaras basadas en los distintos mapas con bake. Se requieren mapas normales de posición, thickness, curvatura, oclusión de ambiente y espacio de entorno como entradas de imagen. <br><br><a href="../../../baking/baking.md">Obtenga más información sobre cómo hacer un bake aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| Color de **Textura** | Utilice una textura personalizada o un punto de ancla. |
| Color de **Textura (secundaria)** | Utilice una textura personalizada o un punto de ancla. |
| **Normales del espacio mundial** Color | Utilice el mapa hecho un bake de las normas espaciales mundiales. |
| **Degradado de posición** Color | Utilice el mapa de posición hecha un bake. |
| **Thickness** en escala de grises | Utilice el mapa de espesor hecho un bake. |
| Escala de grises **Curvatura** | Utilice el mapa de curvatura hecho un bake. |
| **Oclusión ambiental** en escala de grises | Utilice el mapa de Oclusión ambiental hecho un bake. |
| **Micro Normal** Color | Utilice una textura normal personalizada o un punto de ancla. |
| **Micro Height** Color | Utilice una textura personalizada o un punto de ancla. |

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| **Inversión global** | Invierte el resultado final después de combinar todas las capas. |
| **Desenfoque global** | Desenfoca la máscara final uniformemente después de combinar todas las capas. |
| **Equilibrio global** | Ajusta el equilibrio de la máscara final después de que todas las capas se combinen entre blanco o negro, como un ajuste de brillo. |
| **Contraste global** | Ajuste el contraste de la máscara final después de combinar todas las capas. |
| **Opacidad de Textura** | Ajuste la visibilidad de la textura personalizada. |
| Opacidad de **Textura 2** | Ajuste la visibilidad de la segunda textura personalizada. |
| **Opacidad de Oclusión ambiental** | Ajuste la visibilidad de los detalles de la oclusión ambiental. |
| **Opacidad de curvatura** | Ajuste la visibilidad de los detalles de curvatura. |
| **Opacidad normal del espacio mundial** | Ajuste la visibilidad de los detalles normales del espacio mundial. |
| **Opacidad de degradado de posición** | Ajuste la visibilidad de los detalles de la posición. |
| **Opacidad del Thickness** | Ajuste la visibilidad de los detalles del thickness. |

### Textura

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Invertir</strong></td>
    <td>Invierte la textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Conversión de escala de grises</strong></td>
    <td>Establezca el método utilizado para convertir de color completo a escala de grises. El generador de Conversiones de escala de grises <a href="grayscale-conversion.md">tiene más información sobre cómo funciona cada método</a>.</td>
  </tr>
  <tr>
    <td><strong>Modo de fusión</strong></td>
    <td>Seleccione el <a href="../../../interface/layer-stack/blending-modes.md">modo de fusión</a> que desea usar para la capa actual.</td>
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
  <tr>
    <td><strong>Mosaico no cuadrado</strong></td>
    <td>Active o desactive Mosaico no cuadrado.</td>
  </tr>
</table>

### TEXTURA 2

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Invertir</strong></td>
    <td>Invierte la textura secundaria personalizada.</td>
  </tr>
  <tr>
    <td><strong>Conversión de escala de grises</strong></td>
    <td>Establezca el método utilizado para convertir de color completo a escala de grises. El generador de Conversiones de escala de grises <a href="grayscale-conversion.md">tiene más información sobre cómo funciona cada método</a>.</td>
  </tr>
  <tr>
    <td><strong>Modo de fusión</strong></td>
    <td>Seleccione el <a href="../../../interface/layer-stack/blending-modes.md">modo de fusión</a> que desea usar para la capa actual.</td>
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
  <tr>
    <td><strong>Mosaico no cuadrado</strong></td>
    <td>Active o desactive Mosaico no cuadrado.</td>
  </tr>
</table>

### Oclusión ambiental

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte las capas Oclusión ambiental y Detalles del microprocesador. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para la capa actual. |
| **Desenfocar** | Ajusta la suavidad de Oclusión ambiental y microdetalles. |
| **Saldo** | Ajusta el equilibrio de la Oclusión ambiental y los detalles micro, desplazando el punto medio hacia el blanco o el negro como un control de brillo. |
| **Contraste** | Ajusta el contraste/difuminado de la Oclusión ambiental y los microdetalles. |

### Curvatura

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Invertir</strong></td>
    <td>Invierte la curvatura.</td>
  </tr>
  <tr>
    <td><strong>Modo de fusión</strong></td>
    <td>Seleccione el <a href="../../../interface/layer-stack/blending-modes.md">modo de fusión</a> que desea usar para la capa actual.</td>
  </tr>
  <tr>
    <td><strong>Modo</strong></td>
    <td>Defina el modo Curvatura. <br><ul><li><strong>Bordes</strong>: Enmascara los bordes (áreas convexas)</li><li><strong>Cavidades</strong>: Enmascara las cavidades (áreas cóncavas)</li><li><strong>Doble</strong>: Máscaras de áreas cóncavas y convexas.</li><li><strong>Sin procesar</strong>: Máscara de curvatura normal.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Nítido</strong></td>
    <td>Ajuste la visibilidad de los detalles de curvatura nítidos.</td>
  </tr>
  <tr>
    <td><strong>Bien</strong></td>
    <td>Ajuste la visibilidad de los detalles de curvatura fina.</td>
  </tr>
  <tr>
    <td><strong>Suave</strong></td>
    <td>Ajuste la visibilidad de los detalles de la curvatura suave.</td>
  </tr>
  <tr>
    <td><strong>Medio</strong></td>
    <td>Ajuste la visibilidad de los detalles de la curvatura media.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajuste la visibilidad de los detalles de curvatura grandes.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajuste la visibilidad de los detalles de curvatura grandes.</td>
  </tr>
  <tr>
    <td><strong>Enorme</strong></td>
    <td>Ajuste la visibilidad de los detalles de curvatura enormes.</td>
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

### Normal de espacio de mundo

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte las normales del espacio mundial. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para la capa actual. |
| **Desenfocar** | Ajusta la suavidad normal del espacio del mundo. |
| **Saldo** | Ajusta el equilibrio de las normales del espacio mundial, desplazando el punto medio hacia el blanco o el negro como un control de brillo. |
| **Contraste** | Ajusta el contraste/difuminación de las normales del espacio mundial. |
| **Brillo** | Ajusta la luminosidad de las normales del espacio mundial. |
| **De derecha a izquierda** | Ajuste cómo se aplica el efecto de izquierda a derecha en la malla. |
| **De arriba abajo** | Ajuste cómo se aplica el efecto de arriba abajo en la malla. |
| **De frente a atrás** | Ajuste cómo se aplica el efecto de delante hacia atrás en la malla. |

### Espacio del mundo normal/de derecha a izquierda

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierta la dirección de derecha a izquierda. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para la capa actual. |

### Espacio Mundial Normal/De Arriba Abajo

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierta la dirección de arriba a abajo. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para la capa actual. |

### Espacio Mundial Normal/Delantero a Atrás

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierta la dirección de la parte delantera a la trasera. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para la capa actual. |

### Degradado de posición

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte la capa de degradado de posición. |
| **Saldo** | Ajusta el equilibrio de la capa de degradado de posición, desplazando el punto medio hacia el blanco o el negro como un control de brillo. |
| **Contraste** | Ajuste el contraste o la difuminación de la capa de degradado de posición. |
| **Brillo** | Ajuste la luminosidad de la capa de degradado de posición. |
| **Modo de fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para la capa actual. |
| **De derecha a izquierda** | Ajuste cómo se aplica el efecto de izquierda a derecha en la malla. |
| **De arriba abajo** | Ajuste cómo se aplica el efecto de arriba abajo en la malla. |
| **De frente a atrás** | Ajuste cómo se aplica el efecto de delante hacia atrás en la malla. |

>[!TIP]
>
> El degradado Posición se compone de hasta tres degradados, de derecha a izquierda, de arriba abajo y de adelante hacia atrás. Cada uno de los subdegradados tiene su propio modo de fusión que se puede utilizar para crear diferentes efectos o enmascarar diferentes áreas del modelo. Los modos de fusión de estos degradados solo interactúan entre sí para crear una capa de degradado de posición final, no interactúan directamente con otras capas del generador fuera del degradado de posición.

### Degradado de posición - De derecha a izquierda

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte la dirección del degradado de derecha a izquierda. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para el degradado de derecha a izquierda. |

### Degradado de posición - De arriba abajo

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierta la dirección del degradado de arriba a abajo. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para el degradado superior e inferior. |

### Degradado de posición: de delante hacia atrás

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierta la dirección del degradado de delante a detrás. |
| **Modo De Fusión** | Seleccione el [modo de fusión](../../../interface/layer-stack/blending-modes.md) que desea usar para el degradado de delante a atrás. |

### Grosor

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte el thickness. |
| **Desenfocar** | Ajuste la suavidad de los detalles en la capa de thickness. |
| **Contraste** | Ajuste el contraste o la difuminación de la capa de thickness. |
| **Brillo** | Ajuste la luminosidad de la capa de thickness. |

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
    <td>Defina el tipo de curvatura. <br><ul><li><strong>Estándar</strong>: Generalmente produce un resultado bastante nítido, pero puede carecer de detalles más amplios.</li><li><strong>Sobel</strong>: Produce resultados similares en comparación con el estándar, pero ligeramente más borrosos porque evalúa el mapa de normales utilizando un filtro Sobel.</li><li><strong>Suave</strong>: Produce diferentes niveles de desenfoque (como mipmaps) para acumular información. Esto suele proporcionar curvas más suaves, pero los detalles pueden perderse.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Intensidad de curvatura</strong></td>
    <td>Ajuste la intensidad de la curvatura en el modo de curvatura <strong>Estándar</strong> y <strong>Sobel </strong>Curvatura.</td>
  </tr>
  <tr>
    <td><strong>Intensidad de detalles del height</strong></td>
    <td>Ajuste la intensidad de los detalles del Micro Height.</td>
  </tr>
  <tr>
    <td><strong>Radio AO</strong></td>
    <td>Ajuste el radio (rango) de la Oclusión ambiental con detalles micro.</td>
  </tr>
  <tr>
    <td><strong>PROFUNDIDAD AO</strong></td>
    <td>Ajuste la profundidad (intensidad) de la Oclusión ambiental con detalles micro.</td>
  </tr>
</table>
