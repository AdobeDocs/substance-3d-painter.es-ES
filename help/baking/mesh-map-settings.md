---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/baking/mesh-map-settings.html'
breadcrumb-title: ''
description: Aprenda a configurar los ajustes del mapa de malla en Substance 3D Painter para controlar los parámetros hechos un bake y la calidad de salida.
helpx_creative_field: ''
helpx_description: Substance 3D Painter
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Configuración del mapa de malla
user-guide-description: ''
user-guide-title: ''
source-git-commit: 7b5f6e6c9623cb51253b6e49c8dbcbb22856418c
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 10%

---


# Configuración del mapa de malla

<b>El panel de configuración del mapa de malla</b> está disponible en modo de Hacer un bake y tiene controles para preparar la malla para hacer un bake. Para ajustar la configuración del mapa de malla para un mapa determinado, seleccione el mapa en el <b>panel bakeres del mapa de malla</b>. Cada mapa de malla puede tener diferentes configuraciones disponibles. En la parte superior del panel Bakeres de mapa de malla hay disponible una colección de <b>configuraciones comunes </b>compartidas por todos los mapas de malla.

Cualquier configuración que se comparta entre los mapas de malla aparecerá en la página Configuración común, en lugar de en cada mapa de malla individual.

## Ajustes comunes

La página Configuración común contiene controles que afectan al modo en que se hacen un bake todos los mapas de malla.

### Configuración de salida

| Configuración | Función |
| --- | --- |
| Tamaño de salida | Defina la resolución X e Y de los mapas de malla generados. Haga clic en el candado para permitir resoluciones que no sean cuadradas. |
| Anchura de dilatación | Ajuste hasta dónde se extiende la información hecha un bake más allá de los límites de las Islas de UV. |
| Aplicar difusión | Active esta casilla para aplicar la difusión a los bordes de la información generada. |

### Parámetros de malla poligonal alta

| Configuración | Función |
| --- | --- |
| Utilice Malla de poli baja como malla de poli alta | Active este ajuste para hacer un bake mapas en función de la malla del proyecto. |
| Mallas de alta definición | Añada mallas de poli altas a su proyecto para crear desde una malla de poli alta hasta una malla de poli baja en su proyecto. Se pueden importar varias mallas. |
| Jaula | Determine cómo se genera la jaula de haga un bake.<ul data-preserve-html="true"> <li data-preserve-html="true">Según la distancia: Inflar los vértices lejos de la malla a una distancia uniforme a través del modelo para crear una jaula.</li> <li data-preserve-html="true">Automático (experimental): Painter analizará su malla y generará una jaula automáticamente, tratando de mantener la jaula cerca de la superficie sin crear intersecciones para obtener los mejores resultados.</li> <li data-preserve-html="true">Archivo personalizado: Importe un archivo que haya creado para utilizarlo como jaula. Tenga en cuenta que los archivos importados deben tener el mismo número de vértices que la malla base para que funcione correctamente.</li> </ul> |
| Ignorar cara posterior | Alterne si se omiten las caras posteriores al hacer un bake. Esto puede ayudar a reducir los artefactos, pero también puede causar errores en determinados casos límite. |
| Coincidencia | Cambiar la forma en que el Baker determina si se deben incluir objetos al hornear:<ul data-preserve-html="true"> <li data-preserve-html="true">Siempre: Incluya todas las mallas de polietileno altas que se golpean dentro de la jaula mientras hace un bake.</li> <li data-preserve-html="true">Por nombre de malla: Para cada jaula, solo haga un bake mallas con el sufijo de malla correspondiente.</li> </ul> |
| Sufijo de malla de baja definición | Cuando utilice Coincidir por nombre de malla, utilice este sufijo para definir mallas de poli bajo. |
| Sufijo de malla poligonal alta | Cuando utilice Coincidir por nombre de malla, utilice este sufijo para definir mallas de poli altas y hacer que coincidan con la malla de poli baja correspondiente. |
| Suavizado | Ajuste la cantidad de suavizado en los mapas generados. |

#### Corrección de sesgo

| Configuración | Descripción |
| --- | --- |
| **Corrección de sesgo de Pintura** | Entra en el modo de pintura de corrección de sesgo. |
| **Protección de bordes** | Active la protección de bordes para enmascarar los valores de corrección de sesgo pintados cerca de los bordes definidos. |
| **Distancia de borde** | Controlar la distancia que se extiende la protección de los bordes desde los bordes duros |
| **Contraste de borde** | Controle la nitidez con la que el degradado de protección de bordes pasa de una protección completa a una protección nula. |

## Configuración del mapa de ID

| Configuración | Función |
| --- | --- |
| Origen de color | Cambie cómo se determinan los colores hechos un bake del mapa de ID:<ul data-preserve-html="true"> <li data-preserve-html="true">Color de vértice</li> <li data-preserve-html="true">Color de material</li> <li data-preserve-html="true">ID de archivo</li> <li data-preserve-html="true">ID de malla/poligrupo</li> </ul> |
| Generador de color | Cuando utilice el ID de archivo o el ID de malla/Poligrupo como origen de color, determine cómo se generan los colores:<ul data-preserve-html="true"> <li data-preserve-html="true">Aleatorio</li> <li data-preserve-html="true">Cambio de tono</li> <li data-preserve-html="true">Escala de grises</li> </ul> |

## Ajustes del mapa de oclusión ambiental

| Configuración | Función |
| --- | --- |
| Rayos secundarios | Cambiar el número de rayos secundarios. Más rayos pueden producir mejores resultados a costa de un mayor tiempo de procesamiento. |
| Distancia mínima del oclusor | Ajusta la distancia mínima que deben recorrer los rayos para alcanzar la geometría de alta polimerización e impactar en el mapa AO resultante. |
| Distancia máxima del oclusor | Los rayos que se extiendan más allá de esta distancia sin golpear la malla de polietileno alta no se consideran ocluidos y no afectarán al mapa AO. |
| En relación con el cuadro delimitador | Cuando esta casilla está activada, otros ajustes que hacen referencia a la distancia se basan en el cuadro delimitador de la malla del proyecto. Por lo tanto, una distancia de 1 es igual al tamaño del cuadro delimitador. |
| Ángulo de extensión | Ajuste el rango de angular de los rayos generados. Un ángulo de pliegue más alto permite que una superficie se oculte más fácilmente mediante una geometría que no esté posicionada perpendicularmente a la superficie. |
| Distribución | Selecciona cómo se distribuyen los rayos. |
| Ignorar cara posterior | Cambiar si las caras posteriores se consideran objetos ocluidos. |
| Oclusión automática | Seleccione las mallas que deben afectar a la oclusión ambiental de la malla actual. |
| Atenuación | Cambie la forma en que la oclusión se atenúa mediante la distancia del oclusor. |
| Plano de suelo | Active esta opción para crear un plano de tierra que actúe como un oclusor. |
| Desplazamiento del plano del suelo | Cambie la posición del plano de tierra. |

## Ajustes del mapa de curvatura

| Configuración | Función |
| --- | --- |
| Método | Elija cómo generar el mapa de curvatura. |
| Rayos secundarios | Ajuste cuántos rayos secundarios se utilizan para generar el mapa de curvatura. Más rayos secundarios pueden producir mejores resultados a costa de un mayor tiempo de procesamiento. |
| Radio de muestreo | Ajuste hasta dónde busca el baker para calcular la curvatura del punto actual. |
| Relativo al cuadro delimitador | Cuando esta opción está activada, todas las distancias se basan en el tamaño del cuadro delimitador de la malla. |
| Intersección automática | Elija qué objetos se tendrán en cuenta al determinar la curvatura. |
| Asignación de tonos automática (por mosaico de UV) | Deje esta opción marcada para ajustar automáticamente los mapas de curvatura de mapa de tonos por mosaico UV. |
| Mínimo de asignación de tonos | Si la asignación de tonos automática está desactivada, ajuste el valor mínimo de asignación de tonos. |
| Máximo de asignación de tonos | Si la asignación de tonos automática está desactivada, ajuste el valor máximo para la asignación de tonos. |

## Configuración del mapa de posición

| Configuración | Función |
| --- | --- |
| Modo | Seleccione si desea generar un mapa de posición de todos los ejes o sólo calcular la posición de un eje seleccionado. |
| Eje | Si se selecciona el modo de eje único, utilice este ajuste para elegir el eje que se va a calcular. |
| Tipo de normalización | Cambie cómo se normalizan los valores de posición, ya sea con un Cuadro delimitador, una Esfera delimitadora o desactive la normalización. |
| Escala de normalización | Cambiar lo que se considera los límites máximos del espacio de posición. |

## Ajustes de mapa de grosor

| Configuración | Función |
| --- | --- |
| Rayos secundarios | Cambiar el número de rayos secundarios. Más rayos pueden producir mejores resultados a costa de un mayor tiempo de procesamiento. |
| Distancia mínima del oclusor | Ajuste la distancia mínima que deben recorrer los rayos para alcanzar una geometría de poli alta e impactar en el mapa de espesor resultante. |
| Distancia máxima del oclusor | Los rayos que se extiendan más allá de esta distancia sin golpear la malla de polietileno alta se consideran no ocluidos y no afectarán al mapa de espesor. |
| En relación con el cuadro delimitador | Cuando esta casilla está activada, otros ajustes que hacen referencia a la distancia se basan en el cuadro delimitador de la malla del proyecto. Por lo tanto, una distancia de 1 es igual al tamaño del cuadro delimitador. |
| Ángulo de extensión | Ajuste el rango de angular de los rayos generados. Un ángulo de pliegue más alto permite que una superficie se oculte más fácilmente mediante una geometría que no esté posicionada perpendicularmente a la superficie. |
| Distribución | Selecciona cómo se distribuyen los rayos. |
| Oclusión automática | Seleccione las mallas que deben afectar al thickness de la malla actual. |
| Normalización | Cambie cómo se normalizan los valores de thickness. |

## Ajustes del mapa de altura

| Configuración | Función |
| --- | --- |
| Normalización | Cambie cómo se normalizan los valores de height. |
| Divisor de escala | Si Normalización se establece en Manual, utilice este regulador para ajustar el divisor de escala y la normalización del mapa de altura. |

## Ajustes de asignación de normales dobladas

| Configuración | Función |
| --- | --- |
| Rayos secundarios | Cambiar el número de rayos secundarios. Más rayos pueden producir mejores resultados a costa de un mayor tiempo de procesamiento. |
| Distancia mínima del oclusor | Ajusta la distancia mínima que deben recorrer los rayos para alcanzar una geometría poli alta e impactar en el mapa de normales dobladas resultante. |
| Distancia máxima del oclusor | Los rayos que se extienden más allá de esta distancia sin golpear la malla de polietileno alta se consideran no ocluidos y no afectarán el mapa de normales dobladas. |
| En relación con el cuadro delimitador | Cuando esta casilla está activada, otros ajustes que hacen referencia a la distancia se basan en el cuadro delimitador de la malla del proyecto. Por lo tanto, una distancia de 1 es igual al tamaño del cuadro delimitador. |
| Ángulo de extensión | Ajuste el rango de angular de los rayos generados. Un ángulo de pliegue más alto permite que una superficie se oculte más fácilmente mediante una geometría que no esté posicionada perpendicularmente a la superficie. |
| Distribución | Selecciona cómo se distribuyen los rayos. |
| Ignorar cara posterior | Elija si desea tratar las caras posteriores como oclusivas. |
| Oclusión automática | Seleccione qué mallas deben afectar a las normales dobladas de la malla actual. |
