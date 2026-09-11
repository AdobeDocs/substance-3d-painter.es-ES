---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/scripting-and-development/api-reference/shader-api/changelog-shader-api.html"
breadcrumb-title: ''
description: Consulte el registro de cambios de Substance 3D Painter API del sombreador para realizar un seguimiento de las actualizaciones, las nuevas funciones y los cambios a lo largo del tiempo.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Changelog - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Changelog - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 3%

---


# Changelog - API del sombreador

## Changelog

## 2018.3.2

* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md): Las funciones de muestreo utilizan derivados de textura en lugar de nivel de mapa MIP simple. Es un requisito para el apoyo del muestreo de anisotropía. Las firmas de las funciones de muestreo no se modifican.
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): la función *getParallaxOffset* ha cambiado para usar derivados de textura

## 2018.3.0

* Agregue una nueva biblioteca [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) para ayudar a visualizar el resaltado de speculares anisotrópicos
* Agregue una nueva biblioteca [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) para ayudar a canalizar el muestreo ocupándose de la disponibilidad de mipmaps
* Actualice las interfaces de las bibliotecas de sombreador para que se encarguen de este muestreo seguro
* **Rechazo**: Las funciones anteriores basadas en las coordenadas de textura vec2 y el muestreador de textura han quedado obsoletas (utilice firmas nuevas)
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): Agregue una función *applyParallaxOffset* para simplificar el uso del efecto de oclusión de paralaje
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md): Agregar un generador de valores aleatorios de Blue Noise y alternativas temporales
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md): Dividir todos los ayudantes de muestreo de canal para tener ayudantes de interpretación y muestreo de valor

## 2018.2.0

* **Cambio de API del sombreador de superficie**: la firma de la función *shade* ha cambiado, consulte [surface-sombreador.glsl](shaders-shader-api/surface-shader-shader-api.md)
* La función *shadeShadow* ya no se usa y se puede quitar de forma segura de los sombreadores de superficie personalizados
* Para obtener más información, agregue compatibilidad con la dispersión subsuperficial, consulte [surface-sombreadores.glsl](shaders-shader-api/surface-shader-shader-api.md) y [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md)
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md): se quitó la función *pbrComputeBRDF*. Consulte el ejemplo [pbr-metal-rough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) para saber cómo usar la biblioteca ahora
* Se han añadido nuevos parámetros del motor: *textura\_blue\_noise*, *aspect\_ratio*, *camera\_vp\_matrix\_inverse*, *environment\_exposure*, *environment\_rotation*, *fovy*, *main\_light* y *screen\_size*. Consulte [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md) para obtener más información
* Agregue los metadatos *description* para proporcionar información sobre herramientas para parámetros de sombreador personalizados

## 2017.4.2

* Corregir sombreadores que faltan en muestras de documentación (sombreadores pixelados y de tonos)
* Corregir tramado para alta resolución
  * [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md): **bayerMatrix8()** devuelve valores válidos para coords > 4k

## 2017.4.1

* Fijar sombreadores recubiertos de pbr
  * [lib-vectors.glsl](libraries-shader-api/lib-vectors-shader-api.md): Las salidas de **tangentSpaceToWorldSpace()** y **worldSpaceToTangentSpace()** ahora están normalizadas

## 2017.4.0

* Reflejo de specular incorrecto en la Vista 2D para determinadas mallas

## 2017.3.1

* Tramado más barato

## 2017.2.0

* Quitar la normalización tbn interpolada para que coincida con el Substance Designer y los bakeres
* [Ventana gráfica] Reemplace la mesa Hammersley por una espiral de Fibonacci

## 2.6.0

* Corrección de los modos de fusión y de selección de sombreadores
* Retrabaja el tramado. Ahora, si tenemos un renderizado lineal, lo aplicamos después del perfil de color

## 2.5.0

* Añadir compatibilidad con perfiles de color (LUT) en las ventanas gráficas (conversión sRGB opcional)
* Añadir tramado a la opacidad en los sombreados
* Añadir asignación de oclusión de paralaje a sombreadores PBR
* Adición de una forma de ocultar los parámetros personalizados de la interfaz de usuario de sombreador predeterminada
* Adición de un vínculo a la lista de etiquetas de canal en la documentación del sombreador de capas
* Reemplazar la etiqueta &#39;channel\_ao&#39; por &#39;channel\_ambientocclusion&#39;
* [Ventana gráfica] Algunos mapas de normales tienen valores sujetos que aparecen como artefactos
* Corregir canales disponibles en documentos de sombreadores
* Permitir definir una interfaz de usuario de sombreador personalizada
* Adición de una interfaz de usuario de sombreador personalizada estándar para sombreadores de capas de materiales
* Los archivos de interfaz de usuario personalizados ahora se buscan en relación con una carpeta de sombreadores/interfaz de usuario personalizada en los estantes (como el mdl)
* Utilizar el canal de specular level en los sombreadores predeterminados
* Solucionar el ejemplo de parámetros de sombreador vec3
* Actualizar Painter al perfil principal de OpenGL

## 2.4.0

* Corrija la diferencia entre el mapa de normales combinado exportado y el mostrado en la ventana gráfica

## 2.2.0

* Se ha añadido compatibilidad con texturas sin enlace en material genérico para texturas que no son de documento.
* Actualizar la documentación personalizada de reguladores de sombreador
* Permitir definir la precisión de paso de los reguladores
* Documentación para control dinámico de capas de materiales

## 2.1.1

* Añada una función &#39;RGB2Gray&#39; en lib-utils

## 2.1.0

* Permitir definir grupos para parámetros de sombreador y materiales/máscaras
* Añadir los canales que faltan en la documentación (&#39;ao&#39;, &#39;diffuse&#39;, &#39;specularlevel&#39;)

## 2.0.4

* Función normal de desempaquetado incorrecta con valores alfa bajos
* Permitir la lectura de colores de vértices de malla en sombreadores personalizados
* [Viewport] Mapa de entorno Estirado en algunos equipos

## 2.0.0

* Permitir anular los mapas adicionales de Normal/AO por canal dedicado
* Cambie la función Height2Normal para utilizar el método Sobel
* Añadir la posibilidad de definir un mdl por sombreador
* Añadir una nueva carpeta mdl en el estante
* Añadir ajustes preestablecidos de canal difuso y de specular level
* Actualización de la documentación para la asignación de tonos
* Corrección de reflejos en el modo ortográfico
* Se ha corregido el error de blanco vertical que aparecía en una ubicación específica del mapa de envios
* Permitir definir &#39;default\_color&#39; para parámetros de textura

## 1.7.0

* Permitir tomar muestras de texturas externas (de la estantería)

## 1.6.0

* Exponer la función de asignación de gamma y tono para permitir anularlas
* Exponer varias texcocords

## 1.5.0

* Añadir número de línea y nombre de archivo en el informe de errores de sombreador

## 1.4.1

* Todas las conversiones sRGB siguen el estándar sRGB, excepto las realizadas en los sombreados que tienen una aproximación cercana
* El canal de height al Mapa de normales se convierte en un espacio de color incorrecto

## 1.4.0

* Añadir canal de oclusión ambiental
* Añadir nuevo flujo de trabajo para la edición normal
* Añada sintaxis de expresión &#39;or&#39; para parámetros automáticos relacionados con la textura
* Corrección de sombreadores pbr para Intel gpu en OSX

## 1.3.4

* Permitir interpolar binormales en fragmentos de sombreador
* Corregir espacio tangente Mikkt

## 1.3.3

* Corrección de armónicos esféricos que producen una intensidad de luz negativa
* El cálculo de la exposición es diferente del Substance Designer (y corrija el regulador de exposición)
* Las sombras no deben ser visibles en superficies 100 % metálicas

## 1.3.0

* Agregar función de sombra
* Añadir soporte para opacidad (&#39;alpha\_test&#39; y &#39;alpha\_blend&#39;)

## 1.2.0

* Posibilidad de definir los estados de OpenGL necesarios en sombreadores personalizados
* Corrección de bitangentes invertidos
* Añadir compatibilidad para el canal normal

## 1.0

* Añadir compatibilidad con sombreadores personalizados
