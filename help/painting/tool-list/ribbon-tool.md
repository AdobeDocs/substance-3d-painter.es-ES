---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/ribbon-tool.html"
breadcrumb-title: ''
description: Utilice la herramienta Cinta de opciones de Substance 3D Painter para crear trazos de pintura similares a una cinta a lo largo de trazados para pintar texturas decorativas.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ruta de lazo
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 2%

---


# Ruta de lazo

![](../../assets/banner_ribbon.jpg)

La herramienta <b>Trayectoria de la cinta de opciones </b>te permite crear patrones que se deforman a lo largo de una curva definida por puntos en la superficie del modelo 3D. La cinta de opciones también se puede utilizar para escribir texto a lo largo de una curva.

La herramienta Cinta de opciones se puede seleccionar en el menú Herramienta Trazado de la barra de herramientas:

![](../../assets/ribbon_menu.png)

O mediante el botón <b>Tipo de ruta</b>:

![](../../assets/ribbon_path_type.png)

## Información general

La herramienta Ruta de lazo se diferencia de la herramienta Pintar a lo largo del trazado en la forma de dibujar imágenes y materiales.

Mientras que con la herramienta basada en Pintura/Pincel se repite una imagen varias veces en un trazado, con la cinta de opciones, la imagen se repite a lo largo del trazado y se deforma para seguir sus curvas. Los componentes individuales de un pincel se denominan <b>stamps</b>, mientras que los de la cinta de opciones se denominan <b>patches</b>.

![](../../assets/ribbon_comparison.jpg)

## Configuración

### Tamaño

![](../../assets/ribbon_ui_size.png)

| Parámetro | Descripción |
| --- | --- |
| <b>Ancho del trazo</b> | Controla la anchura global del trazo actual. |

### Opacidad

![](../../assets/ribobn_ui_opacity.png)

| Parámetro | Descripción |
| --- | --- |
| <b>Opacidad del trazo</b> | Controlar la opacidad final del trazo actual. |

### Trazo

![](../../assets/ribbon_ui_stroke.png)

| Parámetro | Descripción |
| --- | --- |
| <b>Orientación de la imagen</b> | Defina la dirección de la imagen de entrada. Esta dirección controla cómo se coloca la imagen en el trazado. |
| <b>Voltear imagen</b> | Voltee la imagen a lo largo del eje o la anchura del trazado. |
| <b>Esquina</b> | Defina cómo deben aparecer los vértices nítidos (tangentes divididas) en el trazado. Los comportamientos posibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Unión angular</b>: esquina aguda/puntiaguda</li> <li data-preserve-html="true"><b>Unión redondeada</b>: esquina lisa/redonda</li> <li data-preserve-html="true"><b>Unión biselada</b>: esquina cuadrada/plana</li> <li data-preserve-html="true"><b>Cortar combinación</b>: vuelva a iniciar el trazado. Este modo creará una nueva ruta con secciones dedicadas de inicio/fin.</li> </ul>A continuación se muestra el aspecto de las esquinas, en orden:  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_copy_1489087363_row-1k52rbi-column-6c32r7q_image" src="../../assets/ribbon_corners_small.jpg"/></div> |
| <b>Omitir finaliza cuando se cierra</b> | Si se activa, las secciones de inicio/fin se eliminarán cuando se cierre un trazado para crear un bucle continuo. Esto se aplica tanto a los desvíos de estiramiento como a los trazos dinámicos. |

### Estiramiento y Mosaico

![](../../assets/ribbon_ui_stretch.png)

La Ruta de lazo puede utilizar dos modos diferentes para controlar cómo se repite y estira una imagen a lo largo de un trazado:

* <b>Estirar a lo largo de la ruta</b>: (valor predeterminado) la imagen que se repite a lo largo del trazado se estirará para ajustarse a la longitud del trazado
* <b>Mantener relación de aspecto</b>: la relación de aspecto de la imagen que se repita a lo largo del trazado se conservará. Si la imagen es demasiado larga en comparación con el trazado, se recortará.

#### Estirar a lo largo de la ruta

![](../../assets/ribbon_ui_stretch_along.png)

| Parámetro | Descripción |
| --- | --- |
| <b>Estirar solo entre desplazamientos</b> | Si está activada, mantiene intactas las secciones inicial y final de una imagen mientras se estira el centro. Use los parámetros <b>Desplazamiento inicial</b> y <b>Desplazamiento final</b> para definir el tamaño de estas secciones. La sección central se calculará automáticamente en función del inicio/fin.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_copy_122891642_row-3t12rpd-column-6c32r7q_image" src="../../assets/ribbon_stretch_guides_path.png"/></div> |
| <b>Modo de segmentación</b> | Define cómo se repite una imagen a lo largo del trazado. Los valores posibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Ninguno</b>: la imagen no se repetirá. Se estirará a lo largo de todo el camino.</li> <li data-preserve-html="true"><b>Automático</b>: (predeterminado) la imagen se repite automáticamente un determinado número de veces en función de su tamaño y la anchura del trazo.</li> <li data-preserve-html="true"><b>Personalizado</b>: la imagen se repite el número de veces definido por el parámetro <b>Tiling amount</b>.</li> </ul> |
| <b>Cantidad de segmentación</b> | Especifique cuántas veces se repite una imagen en el modo de mosaico <b>Personalizado</b>. |
| <b>Reflejar cada 2º mosaico</b> | Voltee la imagen utilizada a lo largo de la longitud del trazado cada segunda repetición. |
| <b>Factor de proporción de aspecto</b> | Estire o comprima la proporción de aspecto de la imagen actual. |

#### Conservar relación de aspecto

![](../../assets/ribbon_ui_ratio.png)

| Parámetro | Descripción |
| --- | --- |
| <b>Proporción</b> | Defina cómo se escala la imagen conservando su proporción:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Ajustar al ancho de la ruta</b>: (predeterminado) Escale la imagen para que se ajuste a la anchura del trazado. Esto puede provocar que la imagen se recorte si es demasiado larga.</li> <li data-preserve-html="true"><b>Ajustar a longitud de ruta</b>: Adapte la dimensión de la imagen para que quepa un número exacto a lo largo del trazado, manteniendo aproximadamente la proporción.</li> </ul> |
| <b>Quitar mosaicos recortados</b> | Si se activa, se eliminarán las repeticiones a lo largo del trazado que no puedan ser totalmente visibles (si se han recortado). Esta configuración está deshabilitada si la configuración <b>Proporción</b> está establecida en <b>Ajustar a la longitud de la ruta</b>. |
| <b>Modo de segmentación</b> | Define cómo se repite una imagen a lo largo del trazado. Los valores posibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Ninguno</b>: la imagen no se repetirá. Se estirará a lo largo de todo el camino.</li> <li data-preserve-html="true"><b>Automático</b>: (predeterminado) la imagen se repite automáticamente un determinado número de veces en función de su tamaño y la anchura del trazo.</li> <li data-preserve-html="true"><b>Personalizado</b>: la imagen se repite el número de veces definido por el parámetro <b>Tiling amount</b>.</li> </ul> |
| <b>Reflejar cada 2º mosaico</b> | Voltee la imagen utilizada a lo largo de la longitud del trazado cada segunda repetición. |
| <b>Alineación</b> | Defina dónde debe comenzar la imagen a lo largo del trazado. Los valores posibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Alinear al principio</b>: la imagen se dibuja a partir del primer punto del trazado.</li> <li data-preserve-html="true"><b>Alinear en el centro</b>: la imagen se dibuja en el centro del trazado.</li> <li data-preserve-html="true"><b>Alinear al final</b>: la imagen se dibuja a partir del último punto del trazado.</li> </ul> |
| <b>Factor de proporción de aspecto</b> | Estire o comprima la proporción de aspecto de la imagen actual. |

### Fusión de canales

![](../../assets/ribobn_ui_blending.png)

Esta sección controla el resultado de la fusión cuando el trazado se superpone a sí mismo.

| Parámetro | Descripción |
| --- | --- |
| <b>Alpha</b> | Controla cómo se mezcla la sección <b>Alpha</b> de la Ruta de lazo en las regiones en las que se superpone a sí misma, lo que afecta a la intensidad de la fusión de todos los demás canales. Los valores posibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normal</b>: utiliza el alfa del segmento superior.</li> <li data-preserve-html="true"><b>Aclarar (máx.)</b>: (predeterminado) utiliza el valor alfa máximo, conservando el segmento más opaco.</li> <li data-preserve-html="true"><b>Sobreexposición lineal (Agregar)</b>: añade la alfa de los segmentos para acumularlos, lo que da como resultado un valor más saturado.</li> </ul> |
| <b>Normal</b> | Define cómo se mezcla el canal <b>Normal</b> en las regiones donde la ruta se superpone a sí misma. Los valores posibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normal</b>: usa el resultado del segmento superior.</li> <li data-preserve-html="true"><b>Combinación de mapa normal</b>: (predeterminado) combinar los segmentos con la misma intensidad.</li> <li data-preserve-html="true"><b>Detalles del mapa normal</b>: considere el segmento superior como detalles adicionales, mientras que las regiones inferiores conservarán su intensidad.</li> </ul>Esta configuración es independiente del modo de fusión <b>Normal</b> definido para toda la capa, que se aplica después de la propia fusión de superposición automática del trazado. <b>Nota</b>: este ajuste se desactiva si el canal es de un color uniforme. Sólo es compatible con mapas de bits y recursos de Substance. |
| <b>Height</b> | Define cómo se mezcla el canal <b>Height</b> en las regiones donde la ruta se superpone a sí misma. Los valores posibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normal</b>: usa el resultado del segmento superior.</li> <li data-preserve-html="true"><b>Sobreexposición lineal (Agregar)</b>: añade segmentos a la vez que conserva su intensidad original.</li> <li data-preserve-html="true"><b>Oscurecer (mín.)</b>: mantenga solo el valor más oscuro/más bajo de los segmentos superpuestos.</li> <li data-preserve-html="true"><b>Luz (máx.)</b>: (predeterminado) mantenga el valor más claro/más alto de los segmentos superpuestos.</li> <li data-preserve-html="true"><b>Pantalla</b>: similar a <b>Doge lineal</b>, pero ofrece un resultado menos saturado.</li> </ul>Esta configuración es independiente del modo de fusión <b>Height</b> definido para toda la capa, que se aplica después de la propia fusión de superposición automática del trazado. <b>Nota</b>: este ajuste se desactiva si el canal es de un color uniforme. Sólo es compatible con mapas de bits y recursos de Substance. |

Ejemplo de cómo puede verse el modo de fusión con el canal de height:

![](../../assets/ribbon_blend_modes_height.jpg)

## Texto e imágenes no cuadradas

Cuando se usa un [recurso de texto](../text-resource.md) o una imagen con una proporción no cuadrada, se ajustará automáticamente para ajustarse a la Ruta de lazo.

Este comportamiento permite escribir texto o repetir imágenes como patrones de recorte a lo largo de un trazado.

![](../../assets/ribbon_text_along_path.gif)

![](../../assets/ribbon_non-square.jpg)
