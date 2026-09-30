---
title: Iluminación hecha un bake Estilizada
description: Aprenda a utilizar el filtro Iluminación Hecha un bake estilizada de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 1%
---

# Iluminación hecha un bake Estilizada

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono de iluminación Hecha un bake y estilizada](./Resources/icon_baked_lighting_stylized.png "Iluminación Hecha un bake y estilizada")

<b>En:</b> Efectos/estilizado, luz, color

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Estilizado de iluminación Hecha un bake hace un bake información de iluminación y material en el canal de color.

Se utiliza en una capa de pintura configurada en modo de paso y se aplica a todos los canales. Resulta útil para flujos de trabajo estilizados en los que no se requiere una iluminación simulada precisa o cuando los recursos son limitados, como en proyectos móviles o activos que se basan únicamente en un mapa de color.

</td>
</tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| <b>Oclusión ambiental:</b> Escala de grises | Utilice el mapa de Oclusión ambiental hecho un bake. |
| <b>Curvatura:</b> Escala de grises | Utilice el mapa de curvatura hecho un bake. |
| <b>Normal:</b> Color | Utilice el Mapa de normales hecho un bake. |
| <b>Normales del espacio mundial:</b> Color | Utilice el mapa hecho un bake de las normas espaciales mundiales. |

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Entrada:</b> | Seleccione el flujo de trabajo de material de entrada. |
| <b>Salida:</b> | Seleccione el modo de salida. |
| <b>Reflejo dieléctrico:</b> | Ajusta la reflectancia dieléctrica. |
| <b>Difuso AO:</b> | Ajuste la oclusión ambiental a la luz difusa. |
| <b>Cavidad de Difuso:</b> | Ajuste la contribución de la cavidad a la iluminación difusa. |
| <b>Specular AO:</b> | Ajuste la oclusión ambiental de la iluminación del specular. |
| <b>Cavidad del Specular:</b> | Ajuste la contribución de la cavidad a la iluminación del specular. |
| <b>Smoothness de cavidades:</b> | Ajuste el smoothness del efecto de la cavidad. |
| <b>Intensidad de bordes:</b> | Ajuste la intensidad del efecto de borde. |
| <b>Smoothness de bordes:</b> | Ajuste el smoothness del efecto de borde. |
| <b>Tipo de detalles normales:</b> | Seleccione los detalles normales que se utilizarán. |
| <b>Height a intensidad normal:</b> | Ajuste la intensidad de la conversión de height a normal. |
| <b>Intensidad del sol:</b> | Ajusta la intensidad de la luz solar. |
| <b>Ángulo horizontal del sol:</b> | Ajuste el ángulo horizontal de la luz solar. |
| <b>Ángulo vertical del sol:</b> | Ajuste el ángulo vertical de la luz solar. |
| <b>Color Sun:</b> | Ajusta el color de la luz solar. |
| <b>Intensidad del cielo:</b> | Ajusta la intensidad de la luz del cielo. |
| <b>Color del cielo:</b> | Ajusta el color de la luz del cielo. |
| <b>Color de horizonte:</b> | Ajusta el color de la luz del horizonte. |
| <b>Color de tierra:</b> | Ajusta el color de la luz de tierra. |
| <b>Ángulo horizontal:</b> | Ajuste el ángulo horizontal de la luz adicional. |
| <b>Ángulo vertical:</b> | Ajuste el ángulo vertical de la luz adicional. |
| <b>Intensidad:</b> | Ajusta la intensidad de la luz adicional. |
| <b>Color:</b> | Ajusta el color de la luz adicional. |
| <b>Ángulo horizontal:</b> | Ajuste el ángulo horizontal de la segunda luz adicional. |
| <b>Ángulo vertical:</b> | Ajuste el ángulo vertical de la segunda luz adicional. |
| <b>Intensidad:</b> | Ajusta la intensidad de la segunda luz adicional. |
| <b>Color:</b> | Ajusta el color de la segunda luz adicional. |

### Material

<table>
<tr>
<td><b>Reflejo dieléctrico:</b></td>
<td>Establezca la cantidad de reflectancia dieléctrica.</td>
</tr>
<tr>
<td><b>Difuso AO:</b></td>
<td>Controlar la cantidad de oclusión ambiental que afecta a los detalles difusos.</td>
</tr>
<tr>
<td><b>Cavidad de Difuso:</b></td>
<td>Controle la cantidad de áreas de cavidad que influyen en los detalles difusos.</td>
</tr>
<tr>
<td><b>Specular AO:</b></td>
<td>Controle la cantidad de oclusión ambiental que afecta a los detalles del specular.</td>
</tr>
<tr>
<td><b>Cavidad del specular:</b></td>
<td>Ajuste la cantidad de áreas de cavidad que influyen en los detalles del specular.</td>
</tr>
<tr>
<td><b>Smoothness de la cavidad:</b></td>
<td>Ajuste la suavidad de las zonas de las cavidades.</td>
</tr>
<tr>
<td><b>Intensidad de bordes:</b></td>
<td>Establezca la intensidad de los detalles de los bordes.</td>
</tr>
<tr>
<td><b>Smoothness de bordes:</b></td>
<td>Ajuste el smoothness de las áreas de los bordes.</td>
</tr>
<tr>
<td><b>Tipo de detalles normal:</b></td>
<td>Seleccione los detalles que se utilizarán para las normales: Solo malla o Malla + Height + Normal.</td>
</tr>
<tr>
<td><b>Height a Intensidad Normal:</b></td>
<td>Ajuste la intensidad de los detalles normales generados.</td>
</tr>
</table>

### Sol y cielo

<table>
<tr>
<td><b>Intensidad del sol:</b></td>
<td>Controla la fuerza del sol.</td>
</tr>
<tr>
<td><b>Ángulo horizontal del sol:</b></td>
<td>Ajusta el ángulo horizontal del sol.</td>
</tr>
<tr>
<td><b>Ángulo vertical del sol:</b></td>
<td>Ajusta el ángulo vertical del sol.</td>
</tr>
<tr>
<td><b>Color del sol:</b></td>
<td>Controla el color del sol.</td>
</tr>
<tr>
<td><b>Intensidad del cielo:</b></td>
<td>Ajusta la fuerza del cielo.</td>
</tr>
<tr>
<td><b>Color del cielo:</b></td>
<td>Define el color del cielo.</td>
</tr>
<tr>
<td><b>Color del horizonte:</b></td>
<td>Ajusta el color del horizonte.</td>
</tr>
<tr>
<td><b>Color de tierra:</b></td>
<td>Define el color del suelo.</td>
</tr>
</table>

### Luz 1

<table>
<tr>
<td><b>Ángulo horizontal:</b></td>
<td>Ajuste el ángulo horizontal de la luz adicional.</td>
</tr>
<tr>
<td><b>Ángulo vertical:</b></td>
<td>Ajuste el ángulo vertical de la luz adicional.</td>
</tr>
<tr>
<td><b>Intensidad:</b></td>
<td>Ajuste la intensidad de la luz adicional.</td>
</tr>
<tr>
<td><b>Color:</b></td>
<td>Defina el color de la luz adicional.</td>
</tr>
</table>

### Luz 2

<table>
<tr>
<td><b>Ángulo horizontal:</b></td>
<td>Ajuste el ángulo horizontal de la segunda luz adicional.</td>
</tr>
<tr>
<td><b>Ángulo vertical:</b></td>
<td>Ajuste el ángulo vertical de la segunda luz adicional.</td>
</tr>
<tr>
<td><b>Intensidad:</b></td>
<td>Ajuste la intensidad de la segunda luz adicional.</td>
</tr>
<tr>
<td><b>Color:</b></td>
<td>Defina el color de la segunda luz adicional.</td>
</tr>
</table>
