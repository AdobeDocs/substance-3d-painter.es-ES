---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/performances-guidelines/layer-management.html"
breadcrumb-title: ''
description: Conozca las prácticas recomendadas de administración de capas en Substance 3D Painter para optimizar el rendimiento y mantener los proyectos organizados.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Layer management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Administración de capas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---


# Administración de capas

Painter calcula la pila de capas desde la parte inferior a la superior. Por lo tanto, si realiza cambios en la capa superior de la pila, Painter solo tendrá que calcular los cambios de dicha capa. Sin embargo, si realiza un cambio en una capa situada en la parte inferior de la pila, Painter debe calcular todas las capas superiores a dicha capa para calcular el resultado final.

Existen varias opciones que puede utilizar para reducir el coste de rendimiento de realizar cambios en las capas inferiores de la pila:

+++Uso de máscaras de geometría
Las máscaras de geometría son tu mejor herramienta de optimización. Siempre que pueda aislar una parte de la malla en la que trabajar, hágalo enmascarando capas o carpetas. Las máscaras geométricas funcionan aislando bien por UDIM o por parte de malla, de modo que las áreas que no están en la máscara no se procesan, lo que mejora el rendimiento. Como ventaja, también puede aislar visualmente esas partes en la ventana gráfica para facilitar el texturizado.

Puedes [obtener más información sobre las máscaras de geometría con este tutorial](https://www.youtube.com/watch?v=TGASuIGSUns) o haciendo referencia a la documentación](../../interface/layer-stack/geometry-mask.md).[

+++

+++Ocultar capas
Para evitar ralentizaciones al realizar cambios en un nivel inferior de la pila de capas, puede ocultar capas sobre la capa editada hasta que haya terminado de realizar los ajustes. Painter no procesa las capas ocultas, por lo que si todas las capas superiores están ocultas, es como si estuviera editando la capa superior de la pila. De esta manera, las capas superiores solo se calcularán una vez, cuando las muestre, en lugar de después de cada cambio que realice.

+++

+++Desactivación de capas
Al igual que al ocultar capas, el modo de fusión desactivado evitará que se calculen las capas. Puede resultar útil definir capas de bajo impacto para desactivar el modo de fusión, al tiempo que se modifican áreas en las que no son importantes.

+++

+++Usar carpetas
Intente agrupar capas siempre que sea posible, ya que las carpetas actúan como un punto de almacenamiento en caché invisible. Si realiza cambios por debajo o por encima de una carpeta determinada, no se volverán a calcular todas las capas de la carpeta de forma individual, sino que se volverá a calcular el resultado de su grupo.

+++

+++Limitar el uso de filtros cerca de la parte superior de la pila de capas
Los filtros pueden ser costosos. Si es necesario utilizar un filtro cerca de la parte superior de la pila de capas, utilice máscaras de geometría para reducir el coste de rendimiento.

+++

+++Limitar el uso del modo de fusión de paso a través
El paso a través se utiliza con frecuencia con filtros o capas de trazo de pincel. Es un modo de fusión costoso porque mira todas las capas inferiores y transforma su resultado, en lugar de reemplazar el resultado como el modo de fusión normal. Siempre que utilice el paso a través, intente combinarlo con carpetas y máscaras de geometría para minimizar el impacto en el rendimiento.

+++

+++Mantenga pequeña la profundidad de proyección
Con cualquier herramienta o modo que tenga un ajuste de profundidad de proyección (deformación, plano, trazado, etc.), mantenga el valor de profundidad de proyección lo más pequeño posible. Cuanto más se extiende la profundidad de proyección, menor es su rendimiento.

+++

+++Tenga cuidado con los pinceles que tienen trazos dinámicos
Los pinceles y las herramientas con una etiqueta naranja tienen un parámetro dinámico. Este parámetro dinámico se puede establecer en &quot;Ilimitado&quot;, lo que significa que cada sello de un trazo será único. Esto puede tener un impacto considerable en el rendimiento si se utilizan cientos o miles de trazos de pincel. En la mayoría de los casos, es difícil notar la diferencia después de 16-32 variaciones, por lo que, en términos generales, ir más allá de eso es poco probable que tenga mucho impacto visual.

[Obtenga más información sobre los trazos dinámicos en la documentación.](../../painting/dynamic-strokes/dynamic-strokes.md)

+++

+++Trabajar con una resolución de textura más baja
Disminuir la resolución de los documentos es la forma más rápida de mejorar el rendimiento. Duplicar la resolución supone un mapa 4 veces más grande, por lo que pasar de 1k a 2k supone hasta 4 veces más de coste de rendimiento. Como resultado, a menudo es útil trabajar con una resolución más baja durante el mayor tiempo posible.

+++

+++Definir pegatinas en modo de proyección plana
El modo de pegatina predeterminado es Deformar, pero a menos que realmente esté deformando la pegatina moviendo sus puntos, cambiarla al modo Planar es mucho menos costoso.

+++
