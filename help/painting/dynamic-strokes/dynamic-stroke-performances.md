---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/painting/dynamic-strokes/dynamic-stroke-performances.html"
breadcrumb-title: ''
description: Obtenga más información sobre las consideraciones de rendimiento de los trazos dinámicos en Substance 3D Painter para optimizar la representación y la capacidad de respuesta de los trazos de pincel.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Dynamic Stroke Performances
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Rendimiento de trazo dinámico
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 0%

---


# Rendimiento de trazo dinámico

Para los Trazos dinámicos, el rendimiento del Substance es muy importante, ya que el Substance se puede regenerar muchas veces en un período muy corto. Si el cálculo de un Substance es demasiado pesado, puede crear latencia y, por lo tanto, se entrecorta y se congela al pintar. Todo eso puede terminar creando una mala experiencia de pintura. Esta página reagrupa información y recomendaciones sobre el uso de la función Trazo dinámico.

## El cálculo de trazos dinámicos puede ser pesado

También es importante saber que el cálculo puede tener un impacto en diferentes contextos:

* **Al pintar** : El trazo dinámico se genera (en función de su configuración) al pintar. Una configuración incorrecta puede hacer que la pintura sea lenta y lenta.
* **Al volver a abrir un proyecto** : Incluso si el proceso de pintura salió bien, todavía existe la posibilidad de que el cálculo se detenga al abrir un proyecto, lo que hace que los proyectos sean más largos de lo habitual. Esto se debe a que el proceso de pintura inicial salió bien porque el cálculo se extendió en el tiempo; sin embargo, sucede casi todo a la vez al abrir un proyecto. Esto significa que un proyecto podría solicitar la creación de miles de Substance únicos si el trazo dinámico no se ha configurado correctamente.
* **Consumo de memoria**: Generar muchas variaciones para una gráfica Substance podría terminar consumiendo mucha memoria (porque estas generaciones son volátiles a medida que se hacen sobre la marcha).

## Uso de los ajustes Variaciones y Espaciado

Si bien es fácil implementar efectos impresionantes o avanzados dentro del propio Substance, a veces puede ser más beneficioso mantenerlo simple y usar en su lugar configuraciones nativas de los parámetros de herramientas de Substance 3D Painter. Estos ajustes son mucho más rápidos de calcular para el motor de pintura :

* **Variación** : Estos parámetros permiten crear aleatoriedad muy barato cambiando algunos atributos sin volver a calcular el Substance (como el ángulo, la posición y la opacidad).
* **Espaciado** : Cuanto menor sea el espaciado, más sellos se crearán al pintar un trazo. A veces no es necesario un trazo de pincel continuo y el uso de un espaciado grande también puede ayudar a ver mejor el alfa/material utilizado.

## Cuándo y qué tipo de Aleatorio utilizar

La Raíz aleatoria es una gran manera de generar singularidad. El problema es que la generación puede ser costosa y en el caso de la función de Trazo dinámico puede ocurrir muy a menudo si no se retoca correctamente. Es importante entender cuándo usar la Raíz aleatoria y cuándo evitarla y preferir un método alternativo para obtener el mejor intercambio entre los elementos visuales y el rendimiento :

* **Raíz aleatoria por sello** : En este caso, se creará una nueva generación única de Substance para cada sello. Esto está bien para crear uñas únicas en un tablón de madera, por ejemplo, pero no si está creando rastros de tinta/pintura.
* **Raíz aleatoria por trazo** : Se crea una Raíz aleatoria exclusiva para el trazo de pincel actual. Esto resulta útil cuando se tienen pocos sellos, pero se necesita un nuevo conjunto de variaciones con cada trazo (como un efecto de spray).
* **Raíz aleatoria estática**: El Substance se genera una vez y nunca cambiará. Óptimo para actuaciones, pero tal vez demasiado restrictivo dependiendo de sus necesidades.

¿Qué pasa con **Time** ($time) ?\
El tiempo puede ser útil para crear aspectos muy específicos, pero en realidad es una de las variables más caras de usar en un gráfico de Substance. La razón es que es muy difícil obtener valores similares de un trazo de pincel a otro, por lo que el motor de pincel probablemente generará nuevas variaciones todo el tiempo. Evite esto si puede, utilice el espaciado y el índice de sello en su lugar, lo que combinado puede dar lugar a resultados similares.

## Uso de StampIndex y StampCycleCount

**StampIndex** es el identificador de un sello individual dentro de un trazo de pincel. De forma predeterminada, comienza en 0 y aumenta en 1 por cada nuevo sello. **StampCycleCount** permite limitar la cantidad de índices únicos e indica a Substance 3D Painter que recicle o reutilice los gráficos de Substance ya generados. Cuando el ID actual alcance el límite, Substance 3D Painter comenzará de nuevo desde 0 y creará un bucle.

La mejor solución para tener aleatoriedad y mantener un buen rendimiento es, por lo tanto, aprovechar el recuento cíclico con lo siguiente:

* **StampIndex como RandomSeed** : Al crear un gráfico de Substance es posible definir la Raíz aleatoria como Absoluta. Al hacerlo, puede darle un valor personalizado que puede ser el índice de sello. Esto creará una versión de gráfico de Substance única para cada sello dentro del trazo.
* **Combinado con StampCycleCount** : en realidad, puedes crear un conjunto limitado de nuevas variaciones y luego reutilizarlas.
* **Inicio aleatorio** : Si el recuento cíclico se define para que comience a partir de un valor aleatorio en lugar de 0, esto significa que se utilizará obtener una versión de Substance diferente al principio para cada trazo dentro del grupo de gráficas ya generadas.

## Desactivación del cálculo basado en valores de parámetros

Substance 3D Painter no puede determinar al ajustar un parámetro que puede dar como resultado el mismo resultado, simplemente porque el cálculo está oculto en el gráfico del Substance. Esto es básicamente una caja negra.

Para mejorar el rendimiento al ajustar parámetros y pintar con Trazos dinámicos, es posible especificar cuándo se deben generar nuevas instancias de gráficos mediante valores condicionales en los campos de datos de usuario del gráfico de Substance.

Los valores posibles son:

| *Variable* | *Uso* |
| --- | --- |
| **IsStampIndexActive** | Se utiliza para determinar si el índice de sello debe cambiar durante la pintura. |
| **IsRandomSeedActive** | Se utiliza para determinar si la Raíz aleatoria debe cambiar durante la pintura. |
| **IsTimeActive** | Se utiliza para determinar si el tiempo ($time) debe incrementarse durante la pintura. |

Por ejemplo:

```
IsRandomSeedActive=input.roundness_jitter>0 || input.flip_x_jitter || input.flip_y_jitter
```


En este caso, la velocidad aleatoria solo se cambiará si el parámetro de gráfico (identificador) **roundness\_jitter** es mayor que 0 o si están habilitadas las opciones booleanas **flip\_x\_jitter** o **flip\_y\_jitter**. Si no se cumple la condición, el gráfico no se regenerará. Los parámetros de gráfico deben ir precedidos de &quot;**entrada.**  &quot; para ser reconocido.
