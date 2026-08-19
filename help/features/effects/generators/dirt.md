---
title: Tierra
description: Aprenda a utilizar el generador de Dirtes de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 1%

---


# Tierra

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_dirt.webp" alt=""/><br><strong>En:</strong> máscara, generador</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de Dirt agrega una acumulación realista de dirt y suciedad en grietas, bordes y superficies planas en función de la curvatura y la oclusión del ambiente. Si lo desea, también puede usar los mapas Micro Height y Micro Normal para agregar más detalles.<br><br>El generador de Dirt emite una textura monocromática (blanco y negro). Como resultado, resulta útil para generar máscaras y añadir detalles de dirt o suciedad a tu modelo.Se requieren mapas normales de posición, curvatura, oclusión ambiente y espacio mundial de <br><br>al horno como entradas de imagen. <a href="../../../baking/baking.md">Obtenga más información sobre el horneado aquí</a>.</td>
  </tr>
</table>

>[!NOTE]
>
> El generador de Dirtes es una poderosa herramienta para agregar rápidamente dirt a su malla. Para obtener los mejores resultados, se recomienda utilizar máscaras adicionales para controlar cómo se aplica el dirt, siempre teniendo en cuenta el entorno y el historial del recurso.

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| Escala de grises **Curvatura** | Utilice el mapa de curvatura horneado. |
| **Oclusión ambiental** en escala de grises | Utilice el mapa de Oclusión ambiente al horno. |
| **Espacio normal del mundo** Color | Utilice el mapa de normas espaciales mundiales horneadas. |
| Color de **Posición** | Utilice el mapa de posición horneado. |
| **suciedad personalizada** Escala de grises | Utilice una textura personalizada o un punto de ancla. |
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
    <td><strong>Invertir</strong></td>
    <td>Invierte la máscara de dirt.</td>
  </tr>
  <tr>
    <td><strong>Nivel de dirt</strong></td>
    <td>Ajuste la intensidad del efecto dirt.</td>
  </tr>
  <tr>
    <td><strong>Contraste de dirt</strong></td>
    <td>Ajusta el contraste del efecto dirt.</td>
  </tr>
  <tr>
    <td><strong>Usar triplanar</strong></td>
    <td>Cuando la opción Triplanar está activada, la textura se proyecta desde tres direcciones (ejes X, Y, Z) en lugar de depender únicamente de UV. <br><ul><li>Sin la opción triplanar activada, la textura sigue el diseño UV.</li><li>Con triplanar activado, la textura se proyecta desde múltiples ángulos y se mezcla.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de fusión triplanar</strong></td>
    <td>Ajuste la suavidad con la que se fusiona una textura cuando se proyecta mediante la asignación triplanar. Ajusta la suavidad de la fusión entre las proyecciones desde cada dirección.</td>
  </tr>
  <tr>
    <td><strong>Importe de suciedades</strong></td>
    <td>Ajuste la intensidad de los detalles de la suciedad.</td>
  </tr>
  <tr>
    <td><strong>Escala de suciedad</strong></td>
    <td>Ajuste el tamaño de los detalles de la suciedad.</td>
  </tr>
  <tr>
    <td><strong>Usar Suciedad personalizada</strong></td>
    <td>Activar o desactivar el uso de un mapa de suciedad personalizado.</td>
  </tr>
  <tr>
    <td><strong>Enmascaramiento de bordes</strong></td>
    <td>Ajuste la máscara de los bordes en función del mapa de curvatura.</td>
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
    <td>Ajuste la intensidad de la curvatura en los modos Estándar y Curvatura sobel.</td>
  </tr>
  <tr>
    <td><strong>Intensidad de detalles del height</strong></td>
    <td>Ajuste la cantidad de detalles del Height Micro.</td>
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
