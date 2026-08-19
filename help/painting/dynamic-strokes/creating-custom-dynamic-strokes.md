---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/painting/dynamic-strokes/creating-custom-dynamic-strokes.html"
breadcrumb-title: ''
description: Aprenda a crear trazos dinámicos personalizados en Substance 3D Painter para diseñar comportamientos y efectos de trazos de pincel únicos.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Creating Custom Dynamic Strokes
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Creación de Trazos dinámicos personalizados
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Creación de Trazos dinámicos personalizados

Para crear Trazos dinámicos personalizados, hay dos opciones disponibles:

* Uso de un recurso de Substance existente para crear un nuevo pincel o herramienta preestablecida
* Cree un nuevo recurso de Substance desde cero (requiere [Substance 3D Designer](https://substance3d.adobe.com/display/SDDOC/Substance+Designer) ).

También se recomienda leer [Dynamic Stroke Performances](dynamic-stroke-performances.md) antes de crear archivos de Substance personalizados para evitar cualquier culpable.

## Reutilización de recursos existentes

Crear nuevos Trazos dinámicos desde cero puede resultar difícil. Un buen punto de partida puede ser usar los recursos existentes, ajustarlos y, a continuación, guardarlos como nuevos ajustes preestablecidos.

Encuentra recursos compatibles en la estantería que se ajusten a tus necesidades y echa un vistazo a nuestra página sobre [Ajustes preestablecidos](../presets/presets.md).

## Creación de archivos de Substance personalizados para Trazos dinámicos

A continuación se muestra una lista de los parámetros admitidos para Trazos dinámicos en Substance.

| Identificador de variable | Descripción |
| --- | --- |
| <b>Raíz aleatoria</b> | Si se cocina un archivo de Substance con la Raíz aleatoria expuesta, se podrá controlar con la función Trazo dinámico. |
| <b>stampIndex</b> | <b>Integer1</b> lo usará Substance 3D Painter al pintar el trazo de pincel. Los valores mínimo y máximo no tienen efecto, Substance 3D Painter los ignorará. |
| <b>stampCycleCount</b> | <b>Integer1</b> Painter leerá los valores de parámetro predeterminado, mínimo y máximo para mostrar el parámetro Stamp Cycle Count. Este parámetro controla cuántas variaciones únicas del Substance se crearán. |
| <b>$time</b> | Substance 3D Painter usará <b>Float1</b> al pintar el trazo de pincel en función del tiempo de pintura transcurrido (por trazo). Esta propiedad puede generar muchas variaciones Substance y, por lo tanto, puede afectar al rendimiento. |
| <b>strokeSpacing</b> | <b>float1</b> Valor de espaciado actual para todo el trazo pintado. |
| <b>strokeSize</b> | <b>float1</b> Valor de tamaño actual para todo el trazo pintado. |
| <b>stampStrokePosition</b> | <b>integer1</b> Se usa para especificar el inicio o el comienzo de un trazo. El valor final solo está disponible en el trazo de trazado, no mediante pintura manual. Posible valor:<ul data-preserve-html="true"> <li data-preserve-html="true">0 = medio</li> <li data-preserve-html="true">1 = inicio</li> <li data-preserve-html="true">2 = fin</li> </ul>Se puede deshabilitar usando la etiqueta de usuario isstrokepositionactive. |
| <b>distanceAlongCurve</b> | <b>float1</b> Distancia actual en la marca dada a lo largo de una ruta. Esta propiedad puede generar muchas variaciones Substance y, por lo tanto, puede afectar al rendimiento. Se puede deshabilitar con la etiqueta de usuario <b>iscurvedistanceactive</b>. |
| <b>distanceMaxCurve</b> | <b>float1</b> Longitud total de una ruta de acceso realizada con la herramienta ruta de acceso. Se puede deshabilitar con la etiqueta de usuario <b>iscurvedistanceactive</b>. |
| <b>pathCorner</b> | <b>entero1</b> Indica el tipo de esquina que está usando una cinta de opciones. Posible valor:<ul data-preserve-html="true"> <li data-preserve-html="true">0 = Sin esquina</li> <li data-preserve-html="true">1 = Esquina izquierda</li> <li data-preserve-html="true">2 = Esquina derecha</li> </ul> |
| <b>pathCornerAngle</b> | <b>float</b> Ángulo (en radianes) del vértice en una Ruta de lazo. Se puede utilizar para compensar o ajustar el aspecto de un vértice en función de un valor de ángulo preciso. |
| <b>patchLengthOnCurve</b> | <b>float</b> Tamaño de una sección (revisión) en una Ruta de lazo. Combinado con <b>distanceAlongCurve</b> y <b>distanceMaxCurve</b>, se puede usar para normalizar el tamaño de un parche, por ejemplo. |
