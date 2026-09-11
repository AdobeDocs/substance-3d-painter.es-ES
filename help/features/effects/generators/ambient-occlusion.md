---
title: Oclusión ambiental (OA)
description: Aprenda a utilizar el generador de Oclusiones ambientales de Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 4%

---


# Oclusión ambiental

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_ambient_occlusion.webp" alt=""/><br><strong>En:</strong> máscara, generador, escala de grises, fusión</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de Oclusiones ambientales crea una máscara basada en el mapa de Oclusiones ambientales hecho un bake con la opción de fusionar una textura o microdetalles en la máscara.<br><br>Si usas el generador de Oclusiones ambientales para crear una máscara de Oclusión ambiental, es posible que tengas que invertir la salida de la capa. De forma predeterminada, el generador genera áreas ocluidas como áreas oscuras y áreas no ocluidas como luz. Si se utiliza como máscara, la capa enmascarada solo es visible en áreas no ocluidas. Si invierte el resultado, la capa con máscara solo aparecerá en las áreas ocluidas.Se requieren <br><br>mapas normales de posición, oclusión ambiental y espacio mundial Hechos un bake como entradas de imagen. <a href="../../../baking/baking.md">Obtenga más información sobre cómo hacer un bake aquí</a>.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| Color de textura | Utilice una textura personalizada o un punto de ancla. |
| Micro Normal Color | Utilice una textura normal personalizada o un punto de ancla. |
| Color de Height micro | Utilice una textura personalizada o un punto de ancla. |
| Escala de grises de oclusión ambiental | Utilice el mapa de Oclusión ambiental hecho un bake. |
| Color normal del espacio mundial | Utilice el mapa hecho un bake de las normas espaciales mundiales. |
| Color de degradado de posición | Utilice el mapa de posición hecha un bake. |

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| **Inversión global** | Invierte el resultado final después de combinar todos los efectos. |
| **Desenfoque global** | Suaviza la máscara final uniformemente después de combinar todos los efectos. |
| **Equilibrio global** | Cambia el equilibrio de la máscara final después de que todos los efectos se combinen entre blanco o negro, como un ajuste de brillo. |
| **Contraste global** | Ajuste el contraste de la máscara final después de combinar todos los efectos. |
| **Usar Textura** | Activar o desactivar el uso de un mapa de textura personalizado. |
| **Usar detalles micro** | Activa o desactiva el uso de los detalles de la microfotografía personalizada. |

### Oclusión ambiental

| Nombre del parámetro | Descripción |
| --- | --- |
| **Invertir** | Invierte solo los detalles de Oclusión ambiental y micro. |
| **Desenfocar** | Suaviza solo los detalles de Oclusión ambiental y micro. |
| **Saldo** | Ajusta el equilibrio de solo los detalles de Oclusión ambiental y micro, desplazando el punto medio hacia el blanco o el negro como un control de brillo. |
| **Contraste** | Ajusta el contraste/difuminado de solo la Oclusión ambiental y los detalles micro. |

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
    <td>Cuando la opción Triplanar está activada, la textura se proyecta desde tres direcciones (ejes X, Y, Z) en lugar de depender únicamente de UV.<br><ul><li>Sin triplanar, la textura sigue el diseño UV.</li><li>Con triplanar, la textura se proyecta desde múltiples ángulos y se mezcla.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanar</strong></td>
    <td>Controle la suavidad con la que se fusiona una textura cuando se proyecta mediante la asignación triplanar. Este ajuste ajusta la suavidad de la fusión entre las proyecciones desde cada dirección.</td>
  </tr>
</table>

### Detalles de Micro

| Nombre del parámetro | Descripción |
| --- | --- |
| **Micro Height** | Activar o desactivar el uso de un mapa de altura micro personalizado. |
| **Micro Normal** | Activar o desactivar el uso de un Mapa de normales Micro personalizado. |
| **Radio AO** | Ajuste el radio (rango) de la Oclusión ambiente con detalles micro. |
| **Profundidad AO** | Ajuste la profundidad (intensidad) de la Oclusión ambiental con detalles micro. |
