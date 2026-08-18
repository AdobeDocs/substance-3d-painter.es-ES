---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/presets/photoshop-brush-presets-abr/photoshop-brush-parameters-compatibility.html"
breadcrumb-title: ''
description: Obtenga más información sobre la compatibilidad de los parámetros de pincel de Photoshop en Substance 3D Painter al importar ajustes preestablecidos de pincel ABR.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Photoshop Brush Presets (ABR) > Photoshop Brush Parameters Compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Compatibilidad de parámetros de pincel de Photoshop
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 1%

---


# Compatibilidad de parámetros de pincel de Photoshop

En esta página se muestran todos los parámetros de pincel de Photoshop y su compatibilidad con el motor de pinceles de Substance 3D Painter.

## Compatibilidad general

Al buscar dentro del archivo ABR, Substance 3D Painter solo recuperará los ajustes preestablecidos específicos de Pincel/herramienta :

| *Tipo de ajuste preestablecido* | *Asistencia técnica* | *Descripción* |
| --- | --- | --- |
| **Pincel (mapa de bits)** | Importado | Los ajustes preestablecidos de pincel se basan en mapas de bits, ya que se importarán sus alfa. |
| **Pincel (de procedimiento)** | Ignorado | Los ajustes preestablecidos de pincel basados en formas de procedimiento (como un círculo) no se importan. |
| **Pincel (Aerógrafo)** | Ignorado | Los ajustes preestablecidos de pincel con ajustes de Aerógrafo no se importan. |
| **Pincel (cerdas)** | Ignorado | Los ajustes preestablecidos de pincel con ajustes de cerdas no se importan. |
| **Pincel (erosionable)** | Ignorado | Los ajustes preestablecidos de pincel con ajustes erosionables no se importan. |
| **Lápiz** | Ignorado | Los ajustes preestablecidos de Lápiz no se importan. |
| **Pincel mezclador** | Ignorado | Los ajustes preestablecidos del pincel mezclador no se importan. |
| **Tampón de clonar** | Ignorado | Los ajustes preestablecidos de Tampón de clonar no se importan. |
| **Difuminado** | Ignorado | Los ajustes preestablecidos de difuminado no se importan. |

## Parámetros

Para obtener más información sobre lo que pueden hacer esos parámetros, consulta la [documentación oficial de Photoshop](https://helpx.adobe.com/photoshop/using/creating-modifying-brushes.html) .

No todos los parámetros de pincel de Photoshop son compatibles. Consulte la leyenda para conocer el estado de cada parámetro que se describe a continuación:

* **Cuadrado (■)**: Para indicar que el parámetro es compatible, consulte la descripción para saber cómo acceder a él.
* **Cruz (✖)** : indica que el parámetro no es compatible.

>[!NOTE]
>
> Aunque los parámetros de control de los ajustes preestablecidos de pincel se pueden controlar mediante diversos métodos, como la inclinación de la pluma, el fundido y la presión de la pluma, actualmente solo se admite la **presión de la pluma**.

| *Grupo* | *Parámetro* | *Asistencia técnica* | *Descripción* |
| --- | --- | --- | --- |
| Forma de punta de pincel | **Tamaño** | ■ | Coincidencia con el parámetro Tamaño de la herramienta de pintura.  **Nota:** Photoshop define el tamaño en píxeles, mientras que el tamaño de Substance 3D Painter se basa en el cuadro delimitador del proyecto. Por lo tanto, no es posible una coincidencia exacta y solo será relativa. |
| **Voltear X** | ■ | Se gestiona mediante el archivo de Substance &quot;Brush Maker Photoshop&quot;. |  |
| **Voltear Y** | ■ | Se gestiona mediante el archivo de Substance &quot;Brush Maker Photoshop&quot;. |  |
| **Ángulo** | ■ | Coincidencia con el parámetro Ángulo de la herramienta de pintura. |  |
| **Redondez** | ■ | Se gestiona mediante el archivo de Substance &quot;Brush Maker Photoshop&quot;. |  |
| **Dureza** | ■ | Se gestiona mediante el archivo de Substance &quot;Brush Maker Photoshop&quot;. |  |
| **Espaciado** | ■ | Coincidencia con el parámetro Espaciado de la herramienta de pintura. |  |
|  |  |  |  |
| Dinámica de forma | Variación de tamaño **1&rbrace;** | ■ | Coincidencia con el parámetro Variación del tamaño de la herramienta de pintura. |
| **Control (de tamaño)** | ■ | Coincidencia con el ajuste de presión de la herramienta de pintura para el parámetro Tamaño . |  |
| **Diámetro mínimo** | ■ | Coincidencia con el parámetro Tamaño mínimo de la herramienta de pintura. |  |
| **Escala de inclinación** | ✖ |  |  |
| **Variación del ángulo** | ■ | Coincidencia con el parámetro Variación del ángulo de la herramienta de pintura. |  |
| **Control (para Ángulo)** | ✖ |  |  |
| **Variación de redondez** | ■ | Se gestiona mediante el archivo de Substance &quot;Brush Maker Photoshop&quot;. |  |
| **Redondez mínima** | ■ | Se gestiona mediante el archivo de Substance &quot;Brush Maker Photoshop&quot;. |  |
| **Variación X Voltear** | ■ | Se gestiona mediante el archivo de Substance &quot;Brush Maker Photoshop&quot;. |  |
| **Variación Y Voltear** | ■ | Se gestiona mediante el archivo de Substance &quot;Brush Maker Photoshop&quot;. |  |
| **Proyección de pincel** | ✖ |  |  |
|  |  |  |  |
| Dispersión | **Dispersión** | ■ | Coincidencia con el parámetro Variación de posición de la herramienta de pintura. |
| **Ambos Ejes** | ■ | Coincidencia con el parámetro de eje de variación de posición de la herramienta de pintura. |  |
| **Control (para Dispersión)** | ✖ |  |  |
| **Recuento** | ■ | Compensada mediante el parámetro Espaciado de la herramienta de pintura. |  |
| **Variación del recuento** | ✖ |  |  |
| **Control (para Variación del recuento)** | ✖ |  |  |
|  |  |  |  |
| Textura | **Patrón de textura** | ✖ |  |
| **Invertir** | ✖ |  |  |
| **Escala** | ✖ |  |  |
| **Brillo** | ✖ |  |  |
| **Contraste** | ✖ |  |  |
| **Texturizar cada sugerencia** | ✖ |  |  |
| **Modo** | ✖ |  |  |
| **Profundidad** | ✖ |  |  |
| **Profundidad mínima** | ✖ |  |  |
| **Variación de la Profundidad** | ✖ |  |  |
| **Control (para variación de Profundidad)** | ✖ |  |  |
|  |  |  |  |
| Pincel doble | **Modo** | ✖ |  |
| **Tamaño** | ✖ |  |  |
| **Espaciado** | ✖ |  |  |
| **Dispersión** | ✖ |  |  |
| **Ambos Ejes** | ✖ |  |  |
| **Recuento** | ✖ |  |  |
|  |  |  |  |
| Dinámica de color | **Aplicar por sugerencia** | ✖ |  |
| **Variación frontal/de fondo** | ✖ |  |  |
| **Control (para variaciones F/B)** | ✖ |  |  |
| **Variación del tono** | ✖ |  |  |
| **Variación de saturación** | ✖ |  |  |
| **Variación del brillo** | ✖ |  |  |
| **Pureza** | ✖ |  |  |
|  |  |  |  |
| Traslado | **Variación de opacidad** | ■ | A juego con el parámetro Fusión de sellos de la herramienta de pintura establecido en &quot;Aclarar&quot;. |
| **Control (para opacidad)** | ■ | Coincidencia con el ajuste de presión de la herramienta de pintura para el parámetro Flujo. |  |
| **Mínimo (para el control de opacidad)** | ■ | Coincidencia con el parámetro Flujo mínimo de la herramienta de pintura. |  |
| **Variación del flujo** | ■ | Coincidencia con el parámetro Variación de flujo de la herramienta de pintura. |  |
| **Control (para flujo)** | ■ | Coincidencia con la configuración de presión de la herramienta de pintura para el parámetro Flujo (si es inferior a Opacidad). |  |
| **Mínimo (para el control de flujo)** | ■ | Coincidencia con el parámetro Flujo mínimo de la herramienta de pintura (si es inferior a Opacidad). |  |
| **Variación de humedad** | ✖ |  |  |
| **Control (para variación de humedad)** | ✖ |  |  |
| **Mínimo (para el control de humedad)** | ✖ |  |  |
| **Variación de la mezcla** | ✖ |  |  |
| **Control (para Mix)** | ✖ |  |  |
| **Mínimo (para el control de mezcla)** | ✖ |  |  |
|  |  |  |  |
| Pose del pincel | **Inclinación X** | ✖ |  |
| **Inclinación de reemplazo X** | ✖ |  |  |
| **Inclinación Y** | ✖ |  |  |
| **Inclinación Y De Anulación** | ✖ |  |  |
| **Rotación** | ✖ |  |  |
| **Anular rotación** | ✖ |  |  |
| **Presión** | ✖ |  |  |
| **Presión De Anulación** | ✖ |  |  |
|  |  |  |  |
| Otro | **Ruido** | ✖ |  |
| **Bordes húmedos** | ✖ |  |  |
| **Compilación** | ✖ |  |  |
| **Suavizado** | ■ | No coincide directamente, pero se puede controlar mediante la configuración de [ratón perezoso](../../lazy-mouse.md). |  |
| **Textura de Protect** | ✖ |  |  |
