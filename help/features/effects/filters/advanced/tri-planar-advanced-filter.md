---
title: Tri-Plano avanzado
description: Aprenda a utilizar el filtro Tri-Plano avanzado de Substance 3D Painter.
source-git-commit: 5078774d081555f586a50965b91d85f7c340ef13
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 1%
---

# Tri-Plano avanzado

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono Avanzado Triple Plano](./Resources/icon_tri_planar_advanced_filter.png "Icono Avanzado Triple Plano")

<b>En:</b> Efectos/proyección

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Tri-Plana Advanced es la versión filtrante del generador Tri-Plana Advanced, con controles manuales para la proyección completa. Le permite controlar los valores de rotación y desplazamiento de cada eje. A diferencia del generador, este filtro funciona directamente en el contenido de la capa, mientras que el generador requiere una entrada de máscara personalizada para la fusión.

Se utiliza en una capa de textura o dentro de una máscara para añadir una fusión tri-plana.

</td>
</tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| <b>Espacio Mundial Normal:</b> | Utilice el mapa hecho un bake de World Space Normal. |
| <b>Posición:</b> | Utilice el mapa de posición hecha un bake. |

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Proyección:</b> | Seleccione los ejes sobre los que se va a proyectar el proyecto. |
| <b>Modo de fusión:</b> | Seleccione cómo se fusionan las proyecciones de ejes. |
| <b>Contraste de fusión:</b> | Ajuste el contraste de la fusión de la proyección. |
| <b>Mosaico de Textura:</b> | Ajuste el mosaico de la textura proyectada. |
| <b>Rotación X:</b> | Ajuste la rotación de la proyección del eje X. |
| <b>Desplazamiento X:</b> | Ajuste el desplazamiento de la proyección del eje X. |
| <b>Rotación Y:</b> | Ajuste la rotación de la proyección del eje Y. |
| <b>Desplazamiento Y:</b> | Ajuste el desplazamiento de la proyección del eje Y. |
| <b>Rotación Z:</b> | Ajuste la rotación de la proyección del eje Z. |
| <b>Desplazamiento Z:</b> | Ajuste el desplazamiento de la proyección del eje Z. |

### Eje X

| Nombre del parámetro | Descripción |
| --- | --- |
| **Rotación X:** | Ajuste la rotación de la proyección de textura del eje X. |
| **Desplazamiento X X:** | Ajuste el desplazamiento de proyección del eje X a lo largo del eje X. |
| **Desplazamiento X Y:** | Ajuste el desplazamiento de proyección del eje X a lo largo del eje Y. |

>[!NOTE]
>
> Los parámetros de desvío contienen dos ejes en su título. El primero define el eje de proyección y el segundo define el eje de desvío. Así que **Desplazamiento X Y** examina específicamente la proyección en el eje X y desplaza esa proyección a lo largo del eje Y local de las proyecciones.
>
>Otra forma de pensar en ello es que **Desplazamiento X X** desplaza la proyección X **horizontalmente**, y **Desplazamiento X Y** desplaza la proyección X **verticalmente**.

### Eje Y

| Nombre del parámetro | Descripción |
| --- | --- |
| **Rotación X:** | Ajuste la rotación de la proyección de textura del eje Y. |
| **Desplazamiento Y X:** | Ajuste el desplazamiento de proyección del eje Y a lo largo del eje X. |
| **Desplazamiento Y:** | Ajuste el desplazamiento de proyección del eje Y a lo largo del eje Y. |

>[!NOTE]
>
> Los parámetros de desvío contienen dos ejes en su título. El primero define el eje de proyección y el segundo define el eje de desvío. Por lo tanto, **Desplazamiento Y X** examina específicamente la proyección en el eje Y y desplaza dicha proyección a lo largo del eje X local de las proyecciones.
>
>Otra forma de pensar en ello es que **Desplazamiento Y X** desplaza la proyección Y **horizontalmente**, y **Desplazamiento Y** desplaza la proyección Y **verticalmente**.

### Eje Z

| Nombre del parámetro | Descripción |
| --- | --- |
| **Rotación X:** | Ajuste la rotación de la proyección de textura del eje Z. |
| **Desplazamiento Z X:** | Ajuste el desplazamiento de proyección del eje Z a lo largo del eje X. |
| **Desplazamiento Z Y:** | Ajuste el desplazamiento de proyección del eje Z a lo largo del eje Y. |

>[!NOTE]
>
> Los parámetros de desvío contienen dos ejes en su título. El primero define el eje de proyección y el segundo define el eje de desvío. Por lo tanto, el **Desplazamiento Z Y** examina específicamente la proyección en el eje Z y desplaza dicha proyección a lo largo del eje Y local de las proyecciones.
>
>Otra forma de pensar en ello es que **Desplazamiento Z X** desplaza la proyección Z **horizontalmente**, y **Desplazamiento Z Y** desplaza la proyección Z **verticalmente**.
