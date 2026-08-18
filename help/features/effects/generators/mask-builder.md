---
title: Creador de máscaras
description: Aprenda a utilizar el generador del Creador de máscaras de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 2%

---


# Creador de máscaras

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_mask_builder_dark.png" alt=""/><strong>En:</strong> máscara, generador</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador del Creador de máscaras es una versión heredada del generador del Editor de máscaras. Es un generador de máscaras multiusos que le permite combinar Suciedad, AO, Curvatura, Degradado, Espacio Mundial Normal, Scratches, Dispersión y Micro Detalles en una sola máscara.<br><br>El generador Mask Builder es muy flexible, pero debido a su complejidad, puede afectar el rendimiento más que la mayoría de los generadores.<br><br>El generador del Generador de máscaras genera una textura monocromática (en blanco y negro). Por lo tanto, resulta útil para generar máscaras basadas en los distintos mapas con bake. Se requieren mapas normales de posición, curvatura, oclusión ambiente y espacio mundial de <br><br>al horno como entradas de imagen. <a href="../../../baking/baking.md">Obtenga más información sobre el horneado aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| **Espacio mundial normal** Color | Utilice el mapa de normas espaciales mundiales horneadas. |
| **suciedad personalizada 1** Escala de grises | Utilice una textura personalizada o un punto de ancla. |
| **suciedad personalizada 2** Escala de grises | Utilice una textura personalizada o un punto de ancla. |
| **Entrada de Dispersión** Escala de grises | Utilice una textura personalizada o un punto de ancla. |
| Color de **Posición** | Utilice el mapa de posición horneado. |
| Escala de grises **Curvatura** | Utilice el mapa de curvatura horneado. |
| **Oclusión ambiental** en escala de grises | Utilice el mapa de Oclusión ambiente al horno. |
| **Micro Normal** Color | Utilice una textura normal personalizada o un punto de ancla. |
| **Micro Height** Color | Utilice una textura personalizada o un punto de ancla. |

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
    <td><strong>Nivel</strong></td>
    <td>Ajuste el nivel del punto medio de la máscara final después de que todos los efectos se combinen entre blanco o negro, como un ajuste de brillo.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Ajuste el contraste o la difuminación de la máscara final.</td>
  </tr>
  <tr>
    <td><strong>Invertir</strong></td>
    <td>Invierte el resultado final de la máscara combinada.</td>
  </tr>
  <tr>
    <td><strong>Usar triplanar</strong></td>
    <td>Cuando <strong>Usar triplanar </strong> está habilitado, la textura se proyecta desde tres direcciones (ejes X, Y, Z) en lugar de depender solo de UV. <br><ul><li>Sin la opción triplanar activada, la textura sigue el diseño UV.</li><li>Con triplanar activado, la textura se proyecta desde múltiples ángulos y se mezcla.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de fusión triplanar</strong></td>
    <td>Ajuste la suavidad con la que se fusiona una textura cuando se proyecta mediante la asignación triplanar. Ajusta la suavidad de la fusión entre las proyecciones desde cada dirección.</td>
  </tr>
  <tr>
    <td><strong>Suciedad</strong></td>
    <td>Ajuste el impacto de la configuración de Suciedad en el resultado final de la máscara.</td>
  </tr>
  <tr>
    <td><strong>AO</strong></td>
    <td>Ajuste en qué medida los ajustes de AO (Oclusión ambiental) afectan al resultado final de la máscara.</td>
  </tr>
  <tr>
    <td><strong>Curvatura</strong></td>
    <td>Ajuste en qué medida los ajustes de Curvatura afectan al resultado final de la máscara.</td>
  </tr>
  <tr>
    <td><strong>Degradado superior/inferior</strong></td>
    <td>Ajuste el impacto del degradado superior/inferior en el resultado final de la máscara.</td>
  </tr>
  <tr>
    <td><strong>Normal de espacio de mundo</strong></td>
    <td>Ajuste en qué medida los ajustes de Normal de espacio de entorno afectan al resultado final de la máscara.</td>
  </tr>
  <tr>
    <td><strong>Rayones</strong></td>
    <td>Ajuste en qué medida la configuración de Scratches afectará al resultado final de la máscara. Para que los Scratches sean visibles, la Suciedad, el AO o la curvatura deben estar por encima de 0.</td>
  </tr>
  <tr>
    <td><strong>Dispersión</strong></td>
    <td>Ajusta cuánto afecta la Dispersión a la máscara.</td>
  </tr>
</table>

### Suciedad

| Nombre del parámetro | Descripción |
| --- | --- |
| **Escala** | Ajuste el tamaño de la textura de la suciedad. |
| **Usar Suciedad personalizada** | Activar o desactivar el uso de un mapa de Suciedad personalizado. Es sólo la visibilidad de la Suciedad personalizada 1. Para controlar la visibilidad de la Suciedad personalizada 2, ajuste el regulador Suciedad personalizada secundaria . |
| **Suciedad secundaria personalizada** | Ajuste la visibilidad de la textura Suciedad personalizada 2. |
| **Invertir** | Invierte los mapas de suciedades. |

### Oclusión ambiental

| Nombre del parámetro | Descripción |
| --- | --- |
| **Intervalo** | Ajuste el rango de la máscara AO. |
| **Contraste** | Ajuste el contraste/difuminación de la máscara AO. |
| **Ruido** | Añada ruido al resultado AO, reduciendo de forma efectiva el brillo de la máscara. |
| **Invertir** | Invierte la máscara AO. |

### Curvatura

| Nombre del parámetro | Descripción |
| --- | --- |
| **Rango convexo** | Ajuste el ángulo convexo mínimo que debe resaltar la máscara. |
| **Contraste convexo** | Ajusta el contraste de la máscara convexa. |
| **Inversión convexa** | Invierte la máscara convexa. |
| **Rango cóncavo** | Ajuste el ángulo cóncavo mínimo que resaltará la máscara. |
| **Contraste cóncavo** | Ajusta el contraste de la máscara cóncava. |
| **Invertir cóncavo** | Invierte la máscara cóncava. |
| **Smoothness** | Ajuste la fusión entre las áreas claras y oscuras de la máscara de curvatura. |
| **Aumento de nivel** | Utilice esta opción para ampliar el rango del área enmascarada. Actúa como un multiplicador para los parámetros **Rango convexo** y **Rango cóncavo**. |
| **Ruido** | Añada ruido al resultado Curvatura , lo que reduce de forma efectiva el brillo de la máscara. |

### Degradado

La posición del degradado se basa en el mapa de posición, que se puede hornear con la escala de normalización Escena completa o Por material. Si el material solo aparece en un área pequeña de la escena, pero el mapa de posición se realiza con una escala de Normalización de escena completa, puede resultar difícil ajustar el Rango de degradado para obtener el resultado deseado.

| Nombre del parámetro | Descripción |
| --- | --- |
| **Intervalo** | Ajuste el rango de degradado. |
| **Contraste** | Ajusta el contraste del degradado. |
| **Invertir** | Invierte el degradado. |

### Normal de espacio de mundo

Es posible que los valores **Front**, **back**, **left** y **right** no se correspondan con el lado frontal, posterior, izquierdo y derecho de la malla. De forma predeterminada, **Front** corresponde al eje X positivo, y Right corresponde al eje Z positivo.

| Nombre del parámetro | Descripción |
| --- | --- |
| **Intensidad superior** | Ajuste el rango (intensidad) del degradado descendente superior. |
| **Intensidad inferior** | Ajuste el rango (intensidad) del degradado ascendente de la parte inferior. |
| **Intensidad frontal** | Ajuste el rango (intensidad) del degradado posterior delantero. |
| **Intensidad De Respaldo** | Ajuste el rango (intensidad) del degradado frontal posterior. |
| **Intensidad derecha** | Ajuste el rango (intensidad) del degradado izquierdo derecho. |
| **Intensidad izquierda** | Ajuste el rango (intensidad) del degradado izquierdo derecho. |

### Rayones

| Nombre del parámetro | Descripción |
| --- | --- |
| **Importe** | Ajuste la densidad de los arañazos. |
| **Escala** | Ajuste el tamaño de los arañazos. |

### Dispersión

| Nombre del parámetro | Descripción |
| --- | --- |
| **Escala** | Ajusta el tamaño del efecto de dispersión. Una escala más alta produce más sellos más pequeños, mientras que una escala más baja aumenta el tamaño de los sellos individuales con menos visibles. |
| **Densidad** | Ajuste el número de sellos dispersos. |
| **Tamaño** | Ajuste el tamaño de los sellos dispersos. |
| **Variación de tamaño** | Ajuste la cantidad de aleatoriedad que hay en el tamaño de cada instancia del sello disperso. Una variación de tamaño mayor reduce aleatoriamente los tamaños de sello, por lo que aumentar la variación de tamaño puede significar que también necesita aumentar el valor de tamaño para mantener el mismo tamaño medio. |
| **Variación de opacidad** | Ajuste la cantidad de aleatoriedad que hay en la opacidad de cada instancia del sello disperso. |

### Detalles de Micro

<table>
  <tr>
    <th>Nombre del parámetro</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td><strong>Micro Height</strong></td>
    <td>Activar o desactivar el uso de un mapa de Height Micro personalizado.</td>
  </tr>
  <tr>
    <td><strong>Micro Normal</strong></td>
    <td>Activar o desactivar el uso de un mapa Micro Normal personalizado.</td>
  </tr>
  <tr>
    <td><strong>Tipo de curvatura</strong></td>
    <td>Defina el tipo de curvatura. <br><ul><li><strong>Estándar</strong>: Generalmente produce un resultado bastante nítido, pero puede carecer de detalles más amplios.</li><li><strong>Sobel</strong>: Produce resultados similares en comparación con el estándar, pero ligeramente más borrosos porque evalúa el mapa normal utilizando un filtro Sobel.</li><li><strong>Suave</strong>: Produce diferentes niveles de desenfoque (como mipmaps) para acumular información. Esto suele proporcionar curvas más suaves, pero los detalles pueden perderse.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Intensidad de curvatura</strong></td>
    <td>Ajuste la intensidad de la curvatura en el modo de curvatura <strong>Estándar </strong> y <strong>Sobel </strong>.</td>
  </tr>
  <tr>
    <td><strong>Intensidad de detalles del height</strong></td>
    <td>Ajuste la intensidad de los detalles del Height Micro.</td>
  </tr>
  <tr>
    <td><strong>Radio AO</strong></td>
    <td>Ajuste el radio (rango) de la Oclusión ambiente con detalles micro.</td>
  </tr>
  <tr>
    <td><strong>PROFUNDIDAD AO</strong></td>
    <td>Ajuste la profundidad (intensidad) de la Oclusión ambiente con detalles micro.</td>
  </tr>
</table>
