---
title: Entorno de iluminación generado
description: Aprenda a utilizar el filtro de Entorno de iluminación generado de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 2%
---

# Entorno de iluminación generado

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![icono de Entorno de iluminación generado](./Resources/icon_baked_lighting_environment.png "Entorno de iluminación generado")

<b>En:</b> Efectos/iluminación, hacer un bake, entorno, PBR

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro de Entorno de iluminación generado hace un bake información de iluminación de materiales y entornos en el canal de color.

Se utiliza en una capa de pintura configurada en modo de paso y se aplica a todos los canales. Resulta útil para flujos de trabajo estilizados en los que no se requiere una iluminación simulada precisa o cuando los recursos son limitados, como en proyectos móviles o activos que se basan únicamente en un mapa de color.

</td>
</tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| <b>Oclusión ambiental:</b> Escala de grises | Utilice el mapa de Oclusión ambiental hecho un bake. |
| <b>Mapa de entorno:</b> Escala de grises | Utilice el mapa de entorno. |
| <b>Normal:</b> Color | Utilice el Mapa de normales hecho un bake. |

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Rotación horizontal:</b> | Ajuste la rotación horizontal de la iluminación del entorno. |
| <b>Rotación vertical:</b> | Ajuste la rotación vertical de la iluminación del entorno. |
| <b>Exposición:</b> | Ajuste la exposición del resultado hecho un bake. |
| <b>Intensidad de Height:</b> | Ajuste la intensidad con la que la información de height afecta al resultado. |
| <b>Intensidad de Oclusión ambiental:</b> | Ajuste la intensidad de la oclusión ambiental en el haga un bake. |
| <b>Intensidad de Oclusión del Specular:</b> | Ajuste la intensidad de la oclusión del specular en el haga un bake. |
