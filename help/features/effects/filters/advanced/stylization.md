---

title: Estilización
description: Aprenda a utilizar el filtro Estilización de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 1%
---

# Estilización

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono de estilización](./Resources/icon_stylization.png "Estilización")

<b>En:</b> Efectos/estilizado, estilización, realista, a mano, pintado, pincel

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Estilización da a un material un aspecto estilizado y pintado a mano.

Se utiliza en una capa de textura para añadir trazos de pincel pictórico, variación de smoothness, reasignación de color y efectos de luz hecha un bake.

</td>
</tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| <b>Base de Oclusión ambiental:</b> Color |  |
| <b>Curvatura:</b> Color |  |
| <b>Base normal:</b> color |  |

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Estilización:</b> | Ajuste la intensidad global del filtro. |
| <b>Trazos de pincel:</b> | Ajuste la intensidad general del efecto de trazo de pincel. |
| <b>Smoothness:</b> | Ajuste la intensidad global del efecto smoothness. |
| <b>Colorear:</b> | Ajustar la intensidad global del efecto colorear. |
| <b>Degradado:</b> | Ajuste la intensidad global del efecto de degradado. |
| <b>Iluminación Hecha un bake:</b> | Ajusta la intensidad general del efecto de iluminación hecho un bake. |
| <b>Bordes y cavidades:</b> | Ajuste la intensidad global del efecto de bordes y cavidades. |

### Trazos de pincel

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Cantidad de trazos:</b> | Ajuste la cantidad de trazos de pincel que utiliza el filtro. |
| <b>Modo de trazos:</b> | Seleccione el tipo de trazos de pincel utilizados por el filtro. |
| <b>Selección de trazos:</b> | Seleccione las formas de trazo de pincel que desee proyectar cuando utilice varios trazos. |
| <b>Selección de trazos:</b> | Seleccione la forma de trazo de pincel que desee proyectar cuando utilice un solo trazo. |
| <b>Escala de trazos:</b> | Ajuste la escala de los trazos de pincel. |
| <b>Tamaño no uniforme:</b> | Cambiar la escala no uniforme de los trazos de pincel proyectados. |
| <b>Tamaño de trazos:</b> | Ajuste la proporción de los trazos de pincel proyectados. |
| <b>Escala aleatoria de trazos:</b> | Ajuste la cantidad de variación de escala aleatoria aplicada a los trazos de pincel. |
| <b>Los Trazos Siguen La Superficie:</b> | Alterna la alineación de los trazos de pincel con la orientación de la malla. |
| <b>Rotación de trazos:</b> | Ajuste el ángulo de rotación del trazo del pincel. |
| <b>Rotación aleatoria de trazos:</b> | Ajuste la cantidad de rotación aleatoria aplicada a los trazos de pincel. |
| <b>Dureza de proyección:</b> | Ajuste la dureza de la proyección de la marca. |
| <b>Umbral normal:</b> | Ajuste el umbral normal utilizado para la proyección de trazos. |

### Efectos de trazos de pincel

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Color personalizado:</b> | Active o desactive el uso de un color personalizado en los trazos de pincel. |
| <b>Variación de color:</b> | Ajuste el grado de fusión de los trazos de pincel con el color base. |
| <b>Opacidad de color:</b> | Ajuste la opacidad del color personalizado aplicado a los trazos de pincel. |
| <b>Color:</b> | Ajuste el color personalizado aplicado a los trazos de pincel. |
| <b>Aleatorio de color:</b> | Ajuste la cantidad de variación de color aleatoria aplicada a los trazos de pincel. |
| <b>Rugosidad personalizada:</b> | Active o desactive el uso de un valor de rugosidad personalizado en los trazos de pincel. |
| <b>Variación de rugosidad:</b> | Ajuste la variación de rugosidad en los trazos de pincel. |
| <b>Rugosidad:</b> | Ajuste el valor de rugosidad de los trazos de pincel. |
| <b>Personalizado metálico:</b> | Active o desactive el uso de un valor metálico personalizado en los trazos de pincel. |
| <b>Variación metálica:</b> | Ajuste la variación metálica de los trazos de pincel. |
| <b>Metálico:</b> | Ajuste el valor metálico de los trazos de pincel. |
| <b>Personalizado normal:</b> | Active o desactive las opciones de asignación normal adicionales para los trazos de pincel. |
| <b>Variación normal:</b> | Ajuste la intensidad de los trazos de pincel en el canal normal. |
| <b>Aleatorio normal:</b> | Ajuste la cantidad de variación normal aleatoria aplicada a los trazos de pincel. |
| <b>Modo de fusión (normal):</b> | Seleccione el modo de fusión normal utilizado para los trazos de pincel. |

### Suavidad

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Smoothness de color:</b> | Ajuste el efecto de suavizado de Kuwahara aplicado al Color base. |
| <b>Smoothness de rugosidad:</b> | Ajuste el efecto de suavizado de Kuwahara aplicado a Rugosidad. |
| <b>Smoothness metálico:</b> | Ajuste el efecto de suavizado de Kuwahara aplicado a Metallic. |
| <b>Smoothness de Height:</b> | Ajuste el efecto de suavizado de Kuwahara aplicado al Height. |
| <b>Smoothness normal:</b> | Ajuste el efecto de suavizado de Kuwahara aplicado a Normal. |
| <b>Smoothness de Oclusión ambiental:</b> | Ajuste el efecto de suavizado de Kuwahara aplicado a la Oclusión ambiental. |

### Colorear

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Opacidad de color:</b> | Ajuste la opacidad de la anulación de color aplicada al Color base. |
| <b>Color:</b> | Seleccione el color utilizado para anular el Color base. |
| <b>Variación de Suciedad:</b> | Seleccione la forma de motivo utilizada para la variación de color. |
| <b>Opacidad de Suciedad:</b> | Ajuste la cantidad de variación de color basada en motivos en Color base. |
| <b>Color de Suciedad:</b> | Ajuste el matiz de la variación de color basada en motivos en Color base. |
| <b>Cantidad de laboreo:</b> | Ajuste el número de motivos asignados a la variación de color. |
| <b>Escala de motivo:</b> | Ajuste la escala de los motivos asignados a la variación de color. |

### Degradado

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Modo de degradado:</b> | Seleccione si el degradado utiliza uno o dos colores. |
| <b>Color:</b> | Ajuste el primer color de degradado. |
| <b>Opacidad de color:</b> | Ajuste la opacidad del primer color de degradado. |
| <b>Modo De Fusión De Color:</b> | Seleccione el modo de fusión del primer color de degradado. |
| <b>Color 2:</b> | Ajuste el segundo color de degradado. |
| Opacidad <b>Color 2:</b> | Ajuste la opacidad del segundo color de degradado. |
| <b>Modo de fusión de color 2:</b> | Seleccione el modo de fusión del segundo color de degradado. |
| <b>Rotación horizontal:</b> | Ajuste la rotación horizontal del degradado. |
| <b>Rotación vertical:</b> | Ajuste la rotación vertical del degradado. |
| <b>Inversión de degradado:</b> | Alternar la inversión de la máscara de degradado. |
| <b>Desplazamiento de degradado:</b> | Ajuste el desplazamiento de la máscara de degradado. |
| <b>Contraste de degradado:</b> | Ajuste el contraste de la máscara de degradado. |

### Iluminación hecha un bake

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Trazos De Pincel En Iluminación:</b> | Ajuste la variación de trazo de pincel que aparece en la iluminación hecha un bake. |
| <b>Intensidad de Difuso:</b> | Ajusta la intensidad de la luz difusa. |
| <b>Color de Difuso:</b> | Ajusta el color de la luz difusa. |
| <b>Radio de Difuso:</b> | Ajuste el radio de la luz difusa. |
| <b>Contraste de Difuso:</b> | Ajusta el contraste de la luz difusa. |
| <b>Intensidad de Specular:</b> | Ajusta la intensidad de la luz del specular. |
| <b>Color de Specular:</b> | Ajusta el color de la luz del specular. |
| <b>Radio del Specular:</b> | Ajuste el radio de la luz del specular. |
| <b>Contraste de Specular:</b> | Ajusta el contraste de la luz del specular. |
| <b>Rotación horizontal:</b> | Ajuste la rotación horizontal de la fuente de luz. |
| <b>Rotación vertical:</b> | Ajuste la rotación vertical de la fuente de luz. |
| <b>Enfoque de color:</b> | Ajuste el enfoque aplicado al Color base. |
| <b>Enfoque de superficie:</b> | Ajuste el efecto de detalle de superficie basado en malla en el Color base. |

### Bordes Y Cavidades

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Modo:</b> | Seleccione si desea asignar cavidades, aristas o ambos en el Color base. |
| <b>Contraste de bordes y cavidades:</b> | Ajuste el contraste de los bordes y cavidades de la máscara. |
| Opacidad de <b>cavidades:</b> | Ajusta la intensidad de las cavidades mezcladas en Color base. |
| <b>Dispersión de cavidades:</b> | Ajusta la extensión de las cavidades mezcladas en Color base. |
| <b>Trazos De Pincel En Cavidades:</b> | Ajuste en qué medida los trazos de pincel enmascaran la fusión de las cavidades. |
| <b>Color de cavidades personalizadas:</b> | Alterne el uso de un color personalizado en las cavidades. |
| <b>Color de cavidades:</b> | Ajuste el color personalizado mezclado en las cavidades. |
| Opacidad de <b>bordes:</b> | Ajusta la intensidad de los bordes fusionados en Color base. |
| <b>Extensión de bordes:</b> | Ajuste la extensión de los bordes mezclados en Color base. |
| <b>Trazos De Pincel En Bordes:</b> | Ajuste en qué medida los trazos de pincel enmascaran la fusión de los bordes. |
| <b>Color de bordes personalizados:</b> | Alterne el uso de un color personalizado en los bordes. |
| <b>Color de bordes:</b> | Ajuste el color personalizado fusionado en los bordes. |

#### Ayudantes

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Ayudantes de visualización:</b> | Seleccione la máscara auxiliar o la información de depuración que se va a mostrar en Color base. |

