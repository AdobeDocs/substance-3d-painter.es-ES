---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/project-resources.html"
breadcrumb-title: ''
description: Accede a los recursos del proyecto y a la documentación técnica de Substance 3D Painter para mejorar tu flujo de trabajo y solucionar problemas.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Recursos del proyecto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Recursos y configuración del proyecto

La administración de los recursos del proyecto puede ayudar a establecer una buena base para el rendimiento del proyecto en Painter.

+++Reducir escala de mapas con bake
A veces, no todos los mapas con bake deben tener resoluciones 2k o 4k. No dude en hacer un bake un lote a 2k, luego vuelva a hacer a una resolución más baja para ver si hay una diferencia visual.

+++

+++Administrar mapas de bits importados
Las imágenes importadas pueden afectar drásticamente al rendimiento, por lo que es importante tener en cuenta lo que se importa. Si los conjuntos de texturas se establecen en 2k y no se exportan con una resolución más alta de todos modos, el uso de una imagen 8k no tendrá ningún impacto positivo: su calidad se limitará a 2k, ya que es la resolución del conjunto de texturas.

El formato también importa: EXR, HDR e incluso PNG pesan mucho más que un JPG, y puede que no todas las imágenes necesiten el nivel de calidad de un EXR (como el Color base o los detalles de Height, por ejemplo).

+++

+++Ajustar la configuración del sombreador
La calidad del specular en Ultra dará un resultado más preciso, pero el ajuste es costoso. Cuantos más efectos se activen a la vez en el sombreador, más pesado será el cálculo. Siempre que sea posible, divide los materiales complejos en otro conjunto de texturas con un sombreador independiente. Si el desplazamiento está activado, tenga cuidado con el parámetro teselación.

+++

+++Ajustar opciones de archivo
Utilice <b>Archivo > Guardar > Guardar y reduzca el archivo</b> <b>dimensionar </b> para vaciar datos innecesarios y usar <b>Quitar recursos no utilizados</b> para deshacerse de los archivos importados al proyecto que no se usen en ningún lugar del proyecto.

+++
