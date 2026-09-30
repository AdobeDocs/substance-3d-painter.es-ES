---
title: Cuantificar
description: Aprenda a utilizar el filtro Cuantizar de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 1%
---

# Cuantificar

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Cuantificar icono](./Resources/icon_quantize.png "Cuantificar")

<b>En:</b> Efectos/cuantificar, color

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Cuantizar reduce una imagen a un conjunto limitado de colores.

Se utiliza en una capa de textura para crear regiones de color más planas, posterizadas o estilizadas.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Cantidad de color:</b> | Ajuste el número máximo de colores utilizados en la imagen cuantificada. Este valor también controla la paleta extraída, aunque el recuento real puede ser menor en función del método de cuantificación. Compruebe el resultado de Cantidad de color de la paleta para el número final de colores extraídos. |
| <b>Suavizado de contorno:</b> | Ajuste el radio de suavizado aplicado a la imagen de entrada para simplificar el resultado cuantificado en formas más sólidas y cohesivas. Los valores más altos aumentan notablemente el tiempo de cálculo. |
| <b>Tramado:</b> | Ajuste la cantidad de tramado utilizada para recrear degradados y fusiones de color sin dejar de utilizar únicamente los colores que quedan después de la cuantificación. Utilice un valor de Suavizado de contorno de 0 para el efecto de tramado esperado. |
| <b>Patrón de tramado:</b> | Seleccione el patrón de tramado utilizado para recrear degradados y fusiones de color en la imagen original. |
| <b>Espacio de color de distancia:</b> | Seleccione el espacio de color utilizado para comparar y distribuir colores durante la cuantificación. Utilice Lab (Color) para imágenes de color perceptual y RGB (Datos) para datos sin procesar como mapas de normales. |
| <b>Aplicar al Alpha:</b> | Alternar la cuantificación del canal alfa de la capa. |
| <b>Umbral de Alpha:</b> | Ajuste el umbral alfa. |

