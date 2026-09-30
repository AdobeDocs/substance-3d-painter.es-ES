---
title: Gotas de agua MatFX
description: Aprenda a utilizar el filtro de gotas de agua MatFX de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 3%
---

# Gotas de agua MatFX

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono de gotas de agua MatFX](./Resources/icon_matfx_water_drops.png "Gotas de agua MatFX")

<b>En:</b> Efectos/desenfoque, escala de grises

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro MatFX Water Drops crea efectos de gota de agua y escorrentía en un material.

Se utiliza en capas de textura o pilas de materiales para añadir gotas, rayas direccionales y variaciones de superficie húmeda.

</td>
</tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| <b>Oclusión ambiental:</b> Escala de grises | Utilice el mapa de oclusión ambiental hecho un bake. |
| <b>Normales del espacio mundial:</b> Color | Usa el mapa hecho un bake de normalidad del espacio mundial. |
| <b>Posición:</b> Color | Utilice el mapa de posición hecho un bake. |

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Cantidad de gotas:</b> | Ajusta la cantidad de gotas de agua. |
| <b>Escala X de Drops:</b> | Ajuste la escala X de las gotas. |
| <b>Escala Y de gotas:</b> | Ajuste la escala Y de las gotas. |
| <b>Escala aleatoria de gotas:</b> | Ajuste la cantidad de variación de escala aleatoria en las gotas. |
| <b>Intensidad de dirección de caída:</b> | Ajusta la intensidad direccional de las gotas. |

### Posición

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Influence X:</b> | Ajuste la influencia X de la entrada de posición. |
| <b>Influencia Y:</b> | Ajuste la influencia Y de la entrada de la posición. |
| <b>Influence Z:</b> | Ajuste la influencia Z de la entrada de la posición. |

### Acumulación de agua

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Intensidad:</b> | Ajusta la intensidad de la acumulación de agua. |
| <b>Difusión:</b> | Ajuste la propagación de la acumulación de agua. |
| <b>Intensidad basada en AO:</b> | Ajuste cuánta oclusión ambiental afecta a la acumulación de agua. |

### Espacio de mundo

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Intensidad de enmascaramiento:</b> | Ajusta la intensidad de las máscaras espacio-mundo. |
| <b>Intensidad superior:</b> | Ajuste la intensidad de las gotas en las áreas orientadas hacia arriba. |
| <b>Intensidad inferior:</b> | Ajuste la intensidad de las caídas en las áreas orientadas hacia abajo. |
| <b>Intensidad frontal:</b> | Ajuste la intensidad de las caídas en las áreas frontales. |
| <b>Intensidad de la espalda:</b> | Ajuste la intensidad de las caídas en las áreas orientadas hacia la espalda. |
| <b>Intensidad derecha:</b> | Ajuste la intensidad de las gotas en las áreas orientadas a la derecha. |
| <b>Intensidad izquierda:</b> | Ajuste la intensidad de las gotas en las áreas orientadas a la izquierda. |

### Material

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Intensidad de deformación de Color base de gotas:</b> | Ajuste la intensidad de deformación aplicada al color base bajo las gotas. |
| <b>Multiplicador de mapa vectorial de rotación de gotas:</b> | Ajuste el multiplicador aplicado al mapa vectorial de rotación de colocación. |
| <b>Intensidad del Height de gotas:</b> | Ajusta la intensidad del efecto de height de caída. |
| <b>Rugosidad de gotas:</b> | Ajusta la rugosidad de las gotas. |
| <b>Fusión de rugosidad de gotas:</b> | Ajusta la forma en que la rugosidad de la gota se fusiona con el material. |
| <b>Drops Metallic:</b> | Ajuste el valor metálico de las gotas. |
| <b>Fusión Metálica De Drops:</b> | Ajuste cómo se fusiona el valor de colocación metálica con el material. |
| <b>Intensidad normal:</b> | Ajusta la intensidad del efecto normal. |
