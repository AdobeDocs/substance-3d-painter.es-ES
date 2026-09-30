---
title: Deformar
description: Aprenda a utilizar el filtro Deformación de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 2%
---

# Deformar

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icono de deformación](./Resources/icon_warp.png "Deformar")

<b>En:</b> Efectos/escala de grises

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descripción

El filtro Deformar se utiliza para diversos efectos de deformación. El filtro Deformar proporciona acceso a la deformación normal, una deformación direccional que se deforma en una dirección específica y una deformación multidireccional para obtener más variación.

La deformación se utiliza en una capa de textura o dentro de una máscara (salida en blanco y negro) para deformar materiales, formas, máscaras, contornos, etc.

</td>
</tr>
</table>

## Entradas

| Nombre de entrada | Descripción |
| --- | --- |
| <b>Ruido personalizado</b> | Utilice una textura personalizada como mapa de entrada de ruido. |

<a name="parameters"></a>

## Parámetros

| Nombre del parámetro | Descripción |
| --- | --- |
| <b>Raíz:</b> | Asigne un valor aleatorio para crear una variación diferente sin cambiar la configuración general. |
| <b>Modo de deformación:</b> | Seleccione el modo de deformación. |
| <b>Intensidad:</b> | Ajusta la intensidad de deformación. |
| <b>Divisor de intensidad:</b> | Seleccione cómo se divide la intensidad de deformación. |
| <b>Ángulo:</b> | Ajuste el ángulo de deformación. |
| <b>Modo de fusión:</b> | Seleccione el modo de fusión utilizado por la deformación. |
| <b>Instrucciones:</b> | Seleccione el número de direcciones de deformación. |

### Parámetros de origen

<table>
<tr>
<td><b>Modo de origen:</b></td>
<td>Determina el modo de origen.<br><br> - Ruido predeterminado: Utiliza el ruido predeterminado para el efecto de deformación.<br> - Entrada anterior: Utiliza la entrada anterior para el efecto de deformación. Cuando se aplica un patrón de ruido específico a una capa de relleno, el uso de un efecto de deformación en el modo "Entrada anterior" hará que el efecto utilice el mismo patrón de ruido que la capa de relleno.<br> - Ruido personalizado: Utiliza la entrada de ruido personalizada para el efecto de deformación.</td>
</tr>
<tr>
<td><b>Desenfoque de origen:</b></td>
<td>Desenfoca el ruido de origen.</td>
</tr>
<tr>
<td><b>Saldo de origen:</b></td>
<td>Ajusta el equilibrio del ruido de origen, desplazando el punto medio hacia el blanco o el negro como un control de brillo.</td>
</tr>
<tr>
<td><b>Contraste de origen:</b></td>
<td>Ajusta el contraste del ruido de origen.</td>
</tr>
<tr>
<td><b>Mosaico de origen:</b></td>
<td>Controla el mosaico del ruido de origen.</td>
</tr>
</table>
