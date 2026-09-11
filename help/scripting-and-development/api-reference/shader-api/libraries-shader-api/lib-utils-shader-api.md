---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-utils-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador de Lib Utils de Substance 3D Painter para utilizar funciones de utilidad en el desarrollo de sombreadores personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Utils - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilería Lib - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---


# Utilería Lib - API del sombreador

## Funciones de utilidad Allegorithmic

## Asignación de tonos

Estos son ejemplos de mapeado de tonos que puede usar en su sombreador. Painter no aplica ninguna asignación de tonos, excepto la opcional aplicada por Yebis. Si decides hacer alguna asignación de tonos en tu sombreador, se aplicará antes de la asignación de tonos Yebis.

Efectúe la asignación de tonos de la curva en S en función de los parámetros sigma y n.

```
vec3 tonemapSCurve(vec3 value, float sigma, float n) 

{ 

  vec3 pow_value = pow(value, vec3(n)); 

  return pow_value / (pow_value + pow(sigma, n)); 

}
```


## conversiones sRGB

Estas son las conversiones utilizadas en Painter. Puede anular la conversión lineal -> sRGB automática en la ventana gráfica colocando esta línea en su sombreador personalizado:

*#define DISABLE\_FRAMEBUFFER\_SRGB\_CONVERSION*

y realizar tu propia conversión personalizada.

Conversión de sRGB a color lineal. Versión escalar.

```
float sRGB2linear(float x) 

{ 

  return x <= 0.04045 ? 

    x * 0.0773993808 : // 1.0/12.92 

    pow((x + 0.055) / 1.055, 2.4); 

}
```


Conversión de sRGB a color lineal. Versión del RGB.

```
vec3 sRGB2linear(vec3 rgb) 

{ 

  return vec3( 

    sRGB2linear(rgb.r), 

    sRGB2linear(rgb.g), 

    sRGB2linear(rgb.b)); 

}
```


Conversión de sRGB a color lineal. Versión de RGB + Alpha.

```
vec4 sRGB2linear(vec4 rgba) 

{ 

  return vec4(sRGB2linear(rgba.rgb), rgba.a); 

}
```


Conversión de color de lineal a sRGB. Versión escalar.

```
float linear2sRGB(float x) 

{ 

  return x <= 0.0031308 ? 

      12.92 * x : 

      1.055 * pow(x, 0.41666) - 0.055; 

}
```


Conversión de color de lineal a sRGB. Versión del RGB.

```
vec3 linear2sRGB(vec3 rgb) 

{ 

  return vec3( 

      linear2sRGB(rgb.r), 

      linear2sRGB(rgb.g), 

      linear2sRGB(rgb.b)); 

}
```


Conversión de color de lineal a sRGB. Versión de RGB + Alpha.

```
vec4 linear2sRGB(vec4 rgba) 

{ 

  return vec4(linear2sRGB(rgba.rgb), rgba.a); 

}
```


Conversión de color de lineal a sRGB opcional. Versión escalar.

```
//: param auto conversion_linear_to_srgb 

uniform bool convert_to_srgb_opt; 

float linear2sRGBOpt(float x) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(x) : x; 

}
```


Conversión de color de lineal a sRGB opcional. Versión del RGB.

```
vec3 linear2sRGBOpt(vec3 rgb) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgb) : rgb; 

}
```


Conversión de color de lineal a sRGB opcional. Versión de RGB + Alpha.

```
vec4 linear2sRGBOpt(vec4 rgba) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgba) : rgba; 

}
```


Conversión de colores. Versión escalar.

```
uniform int output_conversion_method; 

float convertOutput(float x) 

{ 

 if (output_conversion_method == 0) return x; 

 else if (output_conversion_method == 1) return linear2sRGB(x); 

 else return sRGB2linear(x); 

}
```


Conversión de colores. Versión del RGB.

```
vec3 convertOutput(vec3 rgb) 

{ 

 if (output_conversion_method == 0) return rgb; 

 else if (output_conversion_method == 1) return linear2sRGB(rgb); 

 else return sRGB2linear(rgb); 

}
```


Conversión de colores. Versión de RGB + Alpha.

```
vec4 convertOutput(vec4 rgba) 

{ 

 if (output_conversion_method == 0) return rgba; 

 else if (output_conversion_method == 1) return linear2sRGB(rgba); 

 else return sRGB2linear(rgba); 

}
```


## Tramado

Estos son algunos elementos que ayudan a agregar tramado a los sombreadores.

Usar matriz de Bayer 8x8 para el modo de tramado

```
import lib-bayer.glsl 

 

float getDitherThreshold(uvec2 coords) 

{ 

  return bayerMatrix8(coords); 

} 

 

 

vec4 RGB2Gray(vec4 rgba) 

{ 

  float gray = 0.299 * rgba.r + 0.587 * rgba.g + 0.114 * rgba.b; 

  return vec4(vec3(gray), rgba.a); 

}
```


Eliminación de AO y sombras en superficies metálicas brillantes (cerca de espejos)

```
float specularOcclusionCorrection(float diffuseOcclusion, float metallic, float roughness) 

{ 

  return mix(diffuseOcclusion, 1.0, metallic * (1.0 - roughness) * (1.0 - roughness)); 

} 

 
```
