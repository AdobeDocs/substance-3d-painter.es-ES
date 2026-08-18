---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador de Substance 3D Painter para crear sombreadores personalizados y ampliar las funciones de representación.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---


# API del sombreador

![](../../../assets/header-shader.jpg)

Substance Painter utiliza sombreadores para procesar materiales en su ventana gráfica en tiempo real. Es posible escribir sombreadores personalizados para implementar nuevos comportamientos o simplemente hacer que la ventana gráfica coincida con otros procesadores.

Se pueden encontrar sombreadores adicionales para Substance Painter en el [Substance share](https://share.allegorithmic.com/libraries?by_category_type_id=6).

>[!NOTE]
>
> El API del sombreador también está disponible directamente desde la aplicación, en el menú **Ayuda > Documentación > API del sombreador**.

## Referencia de sombreado

## Changelog

* [Archivo de registro de cambios completo](changelog-shader-api.md)

## Preparación

En Substance Painter, puede escribir sus propios sombreadores en *GLSL*. Le permitimos escribir sólo una *parte* del sombreador de fragmentos, que a veces se denomina *sombreador de superficies*. Sin más preámbulos, vamos a presentar el sombreador de superficie Substance Painter &quot;Hello world&quot;:

```
void shade(V2F inputs) { 

  diffuseShadingOutput(vec3(1.0, 0.0, 1.0)); 

}
```


Ahora, si guardas este fragmento en un archivo *.glsl* y lo cargas en Substance Painter soltándolo en la pestaña de sombreado de tu estantería, ahora puedes usarlo y ver un hermoso color rosa uniforme en tu malla.

## Sombreado de superficie

* [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)

## Datos proporcionados por el motor (¿o cómo accedo a mis canales?)

En Substance Painter, puede acceder a los parámetros del motor de procesamiento (canales del documento, texturas adicionales, datos relacionados con la cámara, etc.). A continuación se muestra una lista exhaustiva de todos los parámetros proporcionados por el motor:

* [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md)

## Configuración del motor (¿o cómo se especifican los estados de procesamiento?)

En algunos casos, puede que desee utilizar una configuración de procesamiento específica (sacrificio, fusión, localidad de muestreo, etc.) para un efecto. Algunos estados de procesamiento se exponen y se pueden establecer en el sombreado. A continuación se muestra una lista exhaustiva de todos los estados de procesamiento expuestos :

* [all-rendering-states-params.glsl](parameters-shader-api/all-rendering-states-params-shader-api.md)

## Ajustes personalizados (¿o cómo puedo ajustar mi sombreador?)

Es habitual tener ajustes personalizados en un sombreador. Para ello, hemos introducido una forma de especificar ajustes personalizados en los sombreadores de Substance Painter. A continuación se muestra una lista exhaustiva de todos los tipos de ajustes de sombreado personalizados :

* [all-custom-params.glsl](parameters-shader-api/all-custom-params-shader-api.md)

## Bibliotecas incrustadas

Para evitar escribir mucho código repetitivo en todos los sombreados, hemos creado una pequeña pero práctica biblioteca de funciones útiles. **Ten en cuenta que no puedes editarlo ni crear el tuyo propio en este momento.**

* [lib-alpha.glsl](libraries-shader-api/lib-alpha-shader-api.md) : contiene ayudantes relacionados con la opacidad
* [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md) : contiene ayudantes de matriz de bayer
* [lib-define.glsl](libraries-shader-api/lib-defines-shader-api.md) : contiene constantes matemáticas útiles
* [lib-emissive.glsl](libraries-shader-api/lib-emissive-shader-api.md) : contiene ayudantes de propiedades emisoras
* [lib-env.glsl](libraries-shader-api/lib-env-shader-api.md) : contiene ayudantes relacionados con el mapa de entorno
* [lib-normal.glsl](libraries-shader-api/lib-normal-shader-api.md) : contiene ayudantes relacionados con el mapa normal (y mapa de height generado mapa normal)
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md) : contiene ayudantes de representación basados en la física
* [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) : contiene ayudantes de representación anisotrópicos basados físicamente
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md) : contiene ayudantes de asignación de oclusión de parallax
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md) : contiene utilidades aleatorias (secuencias de baja discrepancia)
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md) : contiene ayudantes de captadores de canal
* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) : contiene ayudantes seguros de muestreo de texturas ligeras
* [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md) : contiene ayudantes de dispersión subsuperficial
* [lib-utils.glsl](libraries-shader-api/lib-utils-shader-api.md) : contiene funciones de utilidad de color (conversiones sRGB, asignación de tonos)
* [lib-vectors.glsl](libraries-shader-api/lib-vectors-shader-api.md) : contiene vectores comunes ayudantes

## Metadatos

Puede declarar información adicional no necesaria para dar alguna pista al sistema de procesamiento. Esta es la sintaxis:

```
//: metadata { 

//:   "key1":"value1", 

//:   "key2":"value2" 

//: }
```


Las claves admitidas son:

* **interfaz de usuario personalizada**: Reemplace la interfaz de usuario de parámetros de sombreado estándar por una vista personalizada escrita como módulo QML (consulte la documentación de scripts). La ruta de acceso puede ser absoluta o relativa a una de las carpetas *custom-ui* de la estantería.
* **mdl**: defina el material del molde Iray que se utilizará con el sombreador. La sintaxis de la ruta es la siguiente: *mdl::folder1::folder2::mdl\_filename::material\_name* donde *folder1::folder2::mdl\_filename* es la ruta de acceso dentro de una de las carpetas *mdl* del estante a un archivo mdl y *::material\_name* es el nombre de un material declarado dentro de este archivo mdl. (ej.: &quot;mdl&quot; : &quot;mdl::alg::materials::físicamente\_metálico\_roughness::físicamente\_metálico\_roughness&quot;)

## Ejemplos de sombreadores (¡sí, por fin!)

Para obtener una idea de lo que parece un sombreador real, aquí hay algunos ejemplos de sombreador, ordenados por complejidad creciente:

* [pixelated.glsl](shaders-shader-api/pixelated-shader-api.md) : un sombreador de pixelado
* [toon.glsl](shaders-shader-api/toon-shader-api.md) : un sombreador de tonos
* [pbr-metal-rough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) : el sombreador PBR predeterminado incrustado en Substance Painter

## Control dinámico de capas de materiales

El Control dinámico de capas de materiales es un flujo de trabajo específico en el que los materiales se mezclan dentro de un sombreado y el usuario puede editar dinámicamente las máscaras de fusión en Substance Painter. Para activar este flujo de trabajo, existen dos nuevas funcionalidades:

* declarar pilas editables a partir de una definición de sombreado: [capas\_declare\_stacks.glsl](parameters-shader-api/layering-declare-stacks-shader-api.md)
* enlazar materiales como parámetros de sombreado: [capas\_bind\_materials.glsl](parameters-shader-api/layering-bind-materials-shader-api.md)
