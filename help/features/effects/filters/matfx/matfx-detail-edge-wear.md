---
title: Edge Wear de detalles MatFX
description: Aprenda a utilizar el filtro Edge Wear de detalles MatFX en Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 1%
---

# Edge Wear de detalles MatFX

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_matfx_detail_edge_wear.png" alt="Icono de Edge Wear de detalles MatFX" title="Edge Wear de detalles MatFX"/><br><strong>En:</strong> Efectos/desgaste, borde, material</td>
    <td style="border: 0;" valign="top">Descripción<br>El filtro Edge Wear de detalles MatFX crea detalles de borde desgastados que se pueden mezclar en un material.<br>Se usa en una capa de textura o en una pila de materiales para agregar desgaste en los bordes, ruptura de suciedades y ajustes de materiales de apoyo mediante máscaras y datos de curvatura.</td>
  </tr>
</table>

>[!NOTE]
>
> Para que el filtro Edge Wear de detalles MatFX tenga un efecto visible, debe haber información normal variada existente en la pila de capas debajo del filtro. Si no hay datos o no hay variedad en el canal normal, el filtro no será capaz de encontrar bordes que se dañen y no tendrá ningún efecto visible.

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| **Intensidad de desenfoque:** | Ajuste la intensidad del efecto de desenfoque. |
| **Ajuste de desenfoque:** | Alternar el ajuste de desenfoque. Cuando está activado, el efecto toma muestras de los píxeles del lado opuesto de la textura. |
| **Modo de entrada:** | Seleccione el modo de entrada utilizado para controlar el efecto de desgaste. |
| **Nivel de desgaste:** | Ajuste el nivel de desgaste general. |
| **Contraste de desgaste:** | Ajusta el contraste de la máscara de desgaste. |
| **Smoothness de bordes:** | Ajuste el smoothness de los bordes desgastados. |
| **Cantidad de Suciedades:** | Ajusta la cantidad de suciedad añadida al desgaste. |
| **Escala de Suciedad:** | Ajusta la escala del patrón de suciedad. |

### Material

**Rugosidad metálica PBR**

|  |  |
| --- | --- |
| **Color base:** | Ajuste la contribución de color base. |
| **Metálico:** | Ajuste el valor metálico. |
| **Rugosidad:** | Ajuste el valor de rugosidad. |

**Brillo de Specular PBR**

|  |  |
| --- | --- |
| **Difuso:** | Ajuste la contribución difusa. |
| **Color de Specular:** | Ajusta el color del specular. |
| **Brillo:** | Ajuste el valor de brillo. |

### Configuración

|  |  |
| --- | --- |
| **Control de máscara del generador:** | Ajuste la influencia de la máscara del generador. |
| **Contraste de máscara de generador:** | Ajuste el contraste de la máscara del generador. |
| **Desenfoque de máscara del generador:** | Ajuste el desenfoque aplicado a la máscara del generador. |
| **Valor en segundo plano del Alpha:** | Ajuste el valor alfa del fondo. |
| **Intensidad de curvatura:** | Ajuste la intensidad de la entrada de curvatura. |
| **Invertir curvatura:** | Alternar la inversión de la entrada de curvatura. |
| **Combinar curvatura:** | Alterne la combinación de los datos de curvatura invertidos y no invertidos. |
| **Intensidad normal:** | Ajusta la intensidad normal. |
| Difusión de **AO:** | Ajuste la extensión del efecto oclusión ambiental. |
