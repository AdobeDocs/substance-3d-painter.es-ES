---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-engine-params-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador Todos los Parámetros del Motor de Substance 3D Painter para controlar los parámetros de sombreador a nivel del motor.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Engine Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Todos los parámetros del motor - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Todos los parámetros del motor - API del sombreador

## Ejemplos de parámetros del motor

## Parámetros de textura

Substance Painter utiliza un sistema de textura virtual dispersa (SVT) para mostrar texturas en la ventana gráfica.

Para obtener más información sobre este sistema, consulta la [documentación en línea](../../../../features/sparse-virtual-textures.md).

Este sistema tiene repercusiones en la forma de escribir código de sombreador. Proporcionamos ayudantes para simplificar su uso con la estructura *SamplerSparse* y las funciones de búsqueda de texturas (consulte [lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)).

Uso básico:

```
// Defines the SamplerSparse structure 

import lib-sparse.glsl 

 

//: param auto TEXTURE_TAG 

uniform SamplerSparse uniform_tex;   // Texture sampler and its information
```


Los parámetros de textura permiten utilizar el operador &#39;or&#39; para definir una reserva:

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform SamplerSparse uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2
```


Donde *TEXTURA\_TAG* es una de las etiquetas descritas a continuación.

### Etiquetas de canales del documento

Todas estas texturas están **premultiplicadas** y **dilatadas** para evitar problemas de costuras.

**Canales del conjunto de texturas**

*channel\_ambientocclusion* *channel\_anisotropyangle* *channel\_anisotropylevel* *channel\_basecolor* *channel\_blendingmask* *channel\_diffuse* *channel\_desplazamiento* *channel\_emisivo* *channel\_brillo* *channel\_height 9&rbrace;* canal\_ior **&#x200B; canal\_metálico &#x200B;** canal\_normal **&#x200B; canal\_opacidad &#x200B;** canal\_reflexión **&#x200B; canal\_rugosidad &#x200B;** canal\_dispersión **&#x200B; canal\_specular &#x200B;** canal\_nivel especular *38&rbrace;canal\_transmisivo***

**Canales de usuario**

*canal\_usuario0* *canal\_usuario1* *canal\_usuario2* *canal\_usuario3* *canal\_usuario4* *canal\_usuario5* *canal\_usuario6* *canal\_usuario7*

### Mapas de malla

*texture\_ambientocclusion* : Mapa de Oclusión ambiental\
*texture\_curvature* : Mapa de curvatura\
*texture\_id* : Mapa de ID\
*textura\_normal* : Mapa normal de espacio tangente\
*textura\_normal\_ws* : Mapa normal del espacio mundial\
*texture\_position* : Mapa de posición espacial mundial\
*textura\_thickness* : mapa de thickness

## Parámetros de textura adicionales

Uso básico:

```
//: param auto TEXTURE_TAG 

uniform sampler2D uniform_tex;   // The texture itself 

 

//: param auto TEXTURE_TAG_size 

uniform vec4 uniform_tex_size;   // The size of the texture (width, height, 1/width, 1/height)
```


Los parámetros de textura permiten utilizar el operador &#39;or&#39; para definir una reserva:

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform sampler2D uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2 

 

//: param auto TEX_TAG_1_size or TEX_TAG_2_size 

uniform vec4 uniform_tex_size; // if TEX_TAG_1 exists then TEX_TAG_1_size else TEX_TAG_2_size
```


Donde *TEXTURA\_TAG* es una de las etiquetas descritas a continuación.

*textura\_azul\_noise* : Una textura de ruido azul\
*textura\_entorno* : Mapa del entorno, **mip-mapped**, use [lib-env.glsl](../libraries-shader-api/lib-env-shader-api.md) para usar este

## Otros parámetros

*aspect\_ratio* : *float* que contiene la proporción de anchura / height *de la ventana gráfica*

```
//: param auto aspect_ratio 

uniform float uniform_aspect_ratio;
```


*camera\_view\_matrix* : un *mat4* que representa la transformación del espacio mundial al espacio de la cámara

```
//: param auto camera_view_matrix 

uniform mat4 uniform_camera_view_matrix;
```


*camera\_view\_matrix\_it* : versión de transposición inversa de *camera\_view\_matrix*

```
//: param auto camera_view_matrix_it 

uniform mat4 uniform_camera_view_matrix_it;
```


*camera\_vp\_matrix\_inverse* : inverso de la matriz *proyección \* camera\_view\_matrix*

```
//: param auto camera_vp_matrix_inverse 

uniform mat4 uniform_camera_vp_matrix_inverse;
```


*entorno\_exposición* : un *float* que representa la exposición de envmap

```
//: param auto environment_exposure 

uniform float uniform_environment_exposure;
```


*entorno\_max\_load* : *float* representa la profundidad de la pirámide mip-map de envmap

```
//: param auto environment_max_lod 

uniform float uniform_max_lod;
```


*entorno\_rotation* : un *float* que representa la rotación del envmap alrededor del eje superior\
el valor está en el rango [0,1] y debe asignarse al rango [0, 2\*pi]

```
//: param auto environment_rotation 

uniform float uniform_environment_rotation;
```


*frente*: un *entero* que indica las caras representadas (-1: caras posteriores, 0: indefinido, 1: caras frontales)\
el valor 0 significa que puede confiar con seguridad en la variable integrada glsl *gl\_FrontFacing*

```
//: param auto facing 

uniform int uniform_facing;
```


*fovy* : un *flotador* que representa el campo de visión de la cámara a lo largo del eje Y

```
//: param auto fovy 

uniform float uniform_fovy;
```


*is\_2d\_view* : un *bool* que indica si la representación se realiza para el Vista 2D o no

```
//: param auto is_2d_view 

uniform bool uniform_2d_view;
```


*is\_Perspectiva\_proyección* : un *bool* que indica si la proyección es ortográfica o de Perspectiva

```
//: param auto is_perspective_projection 

uniform bool uniform_perspective_projection;
```


*main\_light* : un *vec4* que indica la posición de la luz principal en el entorno

```
//: param auto main_light 

uniform vec4 uniform_main_light;
```


*mvp\_matrix* : *mat4* que representa la matriz de proyección de la vista de modelo

```
//: param auto mvp_matrix 

uniform mat4 uniform_mvp_matrix;
```


*scene\_original\_radius* : un *float* que representa el radio de la esfera delimitadora de la escena antes de su normalización

```
//: param auto scene_original_radius 

uniform float uniform_scene_original_radius;
```


*screen\_size* : un *vec4* que contiene datos de tamaño de pantalla *(ancho, height, 1/ancho, 1/height)*

```
//: param auto screen_size 

uniform vec4 uniform_screen_size;
```


*world\_camera\_direction* : un *vec3* que representa la orientación mundial de la cámara

```
//: param auto world_camera_direction 

uniform vec3 uniform_world_camera_direction;
```


*world\_eye\_position* : un *vec3* que representa la posición del ojo mundial

```
//: param auto world_eye_position 

uniform vec3 uniform_world_eye_position; 

 
```
