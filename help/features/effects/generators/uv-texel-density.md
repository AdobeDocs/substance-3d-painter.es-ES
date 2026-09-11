---
title: Densidad de texel UV
description: Aprenda a utilizar el generador de densidad de texto UV de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# Densidad de texel UV

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_uv_texel_density.png" alt=""/><br><strong>En:</strong> uv, tamaño, utilidad</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de densidad de texel UV visualiza la densidad de texel de una malla aplicando un degradado de color de bajo a alto.<br>El generador de densidad de texto UV genera una textura a todo color y es mejor usarlo en una capa de relleno para identificar escalas UV incoherentes y garantizar detalles de textura uniformes en un modelo.</td>
  </tr>
</table>

>[!NOTE]
>
> La densidad del texto se refiere al número de texeles (píxeles de textura) de una superficie determinada del modelo. Una densidad de texel alta significa que puedes incluir muchos detalles en una zona pequeña del modelo, donde una densidad de texel baja podría limitar la cantidad de detalles pero mejorar el rendimiento. En general, independientemente de la resolución de los materiales, se recomienda mantener una densidad de texel coherente en toda la malla, ya que las grandes diferencias en la densidad de texel suelen notarse en los espectadores y pueden hacer que un activo parezca de menor calidad o menos realista.

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| **Color bajo** | Establezca el color utilizado para las áreas con una densidad de texel **baja**. |
| **Medio de color** | Establezca el color utilizado para las áreas con densidad de texel **medium**. |
| **Color alto** | Establece el color usado para áreas con una densidad de texel **alta**. |
