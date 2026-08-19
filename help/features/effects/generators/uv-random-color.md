---
title: Color aleatorio UV
description: Aprenda a utilizar el generador de colores aleatorios UV de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 2%

---


# Color aleatorio UV

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_uv_random_color.png" alt=""/><br><strong>En:</strong> utilidad, máscara</td>
    <td style="border: 0;" valign="top"><strong>Descripción</strong><br>El generador de colores aleatorios UV asigna colores únicos y sólidos a cada Isla de UV. Esto suele ser útil como herramienta de diagnóstico con mallas complejas.<br><br>El color aleatorio UV se puede usar para crear una máscara (salida en blanco y negro) o directamente como capa de relleno para aplicar variación de color a la malla en función de las Islas de UV, por ejemplo, para aleatorizar cada tablón de un piso de madera.</td>
  </tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| **Degradado personalizado** | Utilice un mapa de degradado para definir la gama de colores. |

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
    <td><strong>Modo de origen de color</strong></td>
    <td>Determina el modo de origen de color utilizado. <br><ul><li><strong>Aleatorio</strong>: En el modo Aleatorio, los colores se definen y asignan aleatoriamente.</li><li><strong>Degradado personalizado</strong>: En el modo Degradado personalizado, tiene una entrada adicional para agregar un mapa de degradado personalizado en el que se eligen los colores.</li></ul></td>
  </tr>
</table>
