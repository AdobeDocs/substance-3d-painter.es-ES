---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/performances-guidelines/mesh-and-uv-setup.html"
breadcrumb-title: ''
description: Conozca las prácticas recomendadas sobre la configuración de mallas y UV en Substance 3D Painter para optimizar el rendimiento y la calidad de la textura.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Mesh and UV setup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configuración de malla y UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Configuración de malla y UV

Tomar unos minutos para preparar tu malla para Painter puede hacer que el proceso de texturizado sea más rápido y fácil.

+++Modelos de alto polirecuento
No hay un benchmark específico para el policarbonato que Painter pueda manejar, ya que depende en gran medida de las especificaciones de la máquina, la asignación de conjuntos de texturas y las propiedades de pila de capas, pero menos de 10 millones de polietilenos deberían manejarse bien si se tienen en cuenta las optimizaciones de pila de capas.

+++

+++Modelos de bajo polirecuento
Hay tal cosa como un poli demasiado bajo. Esto se debe a que el motor de textura utiliza los polígonos para saber qué parte de la malla debe procesarse para calcular los trazos de pincel. Las mallas con un recuento muy bajo de polímeros se pueden volver a procesar completamente incluso con trazos de pincel pequeños que pueden sobrecargar la GPU innecesariamente.

Por ejemplo, si se aplica texturizado a un solo plano cuádruple, es mejor subdividir la malla, especialmente cuando se pinta a mano con muchos trazos, ya que la información se extiende sobre más vértices.

+++

+++Dividir texturas en varios conjuntos de texturas
Lo mejor es dividir mallas más grandes con asignaciones de materiales más complejas en varios conjuntos de texturas. Los conjuntos de texturas le permiten asignar diferentes configuraciones a cada conjunto de texturas, como las propiedades de resolución y sombreado. Por ejemplo, si solo una parte de la malla utiliza translucidez o SSS, es mejor asignar otro conjunto de texturas y una instancia del sombreador diferente a esa parte. De este modo, estas propiedades más complejas no tienen que calcularse cuando no se utilizan.

+++

+++Mantén las Islas de UV unidas
Intenta mantener las Islas de UV vecinas en el espacio 3D unidas. Esto se aplica tanto al diseño del UDIM como al diseño del espacio UV clásico. Si tienen trazos de pintura o texturas compartidos, es más fácil calcularlos cuando están agrupados en la misma área del espacio UV, en lugar de si están en extremos opuestos.

El motor de textura funciona dividiendo una textura en fragmentos más pequeños para acelerar el cálculo. Esto significa que cada trazo solo actualiza los fragmentos que deben cambiarse, en lugar de actualizar toda la textura con cada trazo. Al mantener las Islas de UV vecinas cercanas entre sí, se minimiza el número de fragmentos que se verán afectados por un solo trazo.

+++

+++Evite tener demasiados objetos
El rendimiento debe seguir siendo cómodo al importar una malla que tenga menos de 8000 subobjetos. Si se sobrepasa este límite, el rendimiento de la ventana gráfica y de la pintura puede verse afectado. Si se alcanza este límite, se recomienda combinar objetos para reducir la sobrecarga de procesamiento.

+++
