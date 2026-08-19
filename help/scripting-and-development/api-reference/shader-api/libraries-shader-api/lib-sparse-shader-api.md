---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-sparse-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador Lib Sparse de Substance 3D Painter para trabajar con el muestreo de texturas dispersas en sombreadores personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Sparse - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Sparse - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Lib Sparse - API del sombreador

## lib-sparse.glsl

Este archivo proporciona funciones útiles para garantizar la corrección de muestreo de texturas dispersas (ARB\_sparse\_texture). Permite muestrear solo una parte de las texturas realmente presentes en la memoria de vídeo.

**Funciones públicas:** *getSparseCoord* *getSparseCoordLod0* *textureSparseQueryLod* *textureSparse*

**Estructuras públicas:** *SamplerSparse* *SparseCode*

La macro *FEATURE\_SPARSE\_TEXTURE* solo se define si está habilitada la extensión de textura virtual dispersa.

Si está activado, procese las búsquedas de textura adicionales para subir a la pirámide mipmap si faltan texeles.

```
## ifdef FEATURE_SPARSE_TEXTURE

//: param auto material_lod_check_needed 

uniform bool material_lod_check_needed = false; 

//: param auto material_lod_mask 

uniform usampler2D material_lod_mask; 

## endif // FEATURE_SPARSE_TEXTURE

//: param auto uvtile_reference_sampler 

uniform sampler2D uvtile_reference_sampler; 

//: param auto uvtile_size 

uniform vec2 uvtile_size; 

//: param auto uvtile_inverse_size 

uniform vec2 uvtile_inverse_size; 

//: param auto uvtile_lod_bias 

uniform float uvtile_lod_bias;
```


Sampler y estructura de información de texturas dispersas

Se utiliza para consultar todos los uniformes relacionados con sampler con un solo enlace automático

```
struct SamplerSparse { 

  sampler2D tex; 

  vec4 size; // width, height, 1/width, 1/height 

  bool is_set; // a boolean indicating whether the texture is in the texture set or not 

  uvec3 lod_mask_select; // masking operations description allowing to retrieve loaded mipmaps information 

};
```


Coordenadas de muestreo dispersas

Almacenar las coordenadas UV y la máscara Ld dispersa en cuanto a materiales

```
struct SparseCoord { 

  vec2 tex_coord; 

  vec2 dfdx; 

  vec2 dfdy; 

  float lod; 

  uint material_lod_mask; 

}; 

 

 

## if defined(SHADER_FRAGMENT)
```


Estructura de coordenadas de textura de compilación usada por la función de muestreo *textureSparse()* (debe llamarse desde el sombreador de fragmentos)

Ejemplo: *SparseCoord uv1coord = getSparseCoord(input.multi\_tex\_coord[1]);*

```
SparseCoord getSparseCoord(vec2 tex_coord) { 

  SparseCoord res; 

  res.tex_coord = tex_coord; 

  res.dfdx = dFdx(tex_coord); 

  res.dfdy = dFdy(tex_coord); 

## ifdef FEATURE_SPARSE_TEXTURE

  res.material_lod_mask = material_lod_check_needed ? 

    textureLod(material_lod_mask,tex_coord,0.0).r : 

    0u; 

  res.lod = getLodFromReferenceSampler(tex_coord); 

## endif // FEATURE_SPARSE_TEXTURE

  return res; 

} 

## endif
```


Estructura de coordenadas de textura de compilación usada por la función de muestreo *textureSparse()* Versión de muestreo de nivel base (se puede usar si el sombreador de fragmentos está fuera)

```
SparseCoord getSparseCoordLod0(vec2 tex_coord) { 

  SparseCoord res; 

  res.tex_coord = tex_coord; 

  res.dfdx = vec2(0.0); 

  res.dfdy = vec2(0.0); 

## ifdef FEATURE_SPARSE_TEXTURE

  res.material_lod_mask = material_lod_check_needed ? 

    textureLod(material_lod_mask,tex_coord,0.0).r : 

    0u; 

  res.lod = 0.0; 

## endif // FEATURE_SPARSE_TEXTURE

  return res; 

} 

 

## if defined(SHADER_FRAGMENT)
```


Calcular el nivel de detalle que se utilizará para tomar muestras de una textura dispersa

Subir la pirámide mipmap si faltan texeles Devuelve LoD ANTES de aplicar el sesgo LoD

```
float textureSparseQueryLod(SamplerSparse sampler, SparseCoord coord) { 

## ifdef FEATURE_SPARSE_TEXTURE

  float lodfix = coord.lod; 

  if (material_lod_check_needed) { 

    lodfix = getFixedSparseLod(getTextureLodMask(sampler.lod_mask_select, coord.material_lod_mask), lodfix); 

  } 

  return lodfix-uvtile_lod_bias; 

## else // FEATURE_SPARSE_TEXTURE

  return textureQueryLod(sampler.tex, coord.tex_coord).y-uvtile_lod_bias; 

## endif // FEATURE_SPARSE_TEXTURE

} 

## endif // SHADER_FRAGMENT
```


Calcular los derivados que se usarían para tomar muestras de una textura dispersa

Sube a la pirámide mipmap si faltan texeles

```
void textureSparseQueryGrad(out vec2 dfdx, out vec2 dfdy, SamplerSparse sampler, SparseCoord coord) { 

## ifdef FEATURE_SPARSE_TEXTURE

  if (material_lod_check_needed) { 

    float lodfix = getFixedSparseLod(getTextureLodMask(sampler.lod_mask_select, coord.material_lod_mask), coord.lod); 

    if (coord.lod!=lodfix) { 

      // Fix dfdx dfdy, take account offset, no more anisotropy 

      vec2 ddfix = exp2(lodfix-uvtile_lod_bias) * uvtile_inverse_size; 

      dfdx = vec2(ddfix.x,0.0); 

      dfdy = vec2(0.0,ddfix.y); 

      return; 

    } 

  } 

## endif // FEATURE_SPARSE_TEXTURE

  dfdx = coord.dfdx; 

  dfdy = coord.dfdy; 

}
```


Realiza una búsqueda de textura en una textura dispersa y sube los niveles de mapa MIP si es necesario

Esta función reemplaza el estándar *texture(sampler2D, vec2)* para recuperar texeles de una textura dispersa

```
vec4 textureSparse(SamplerSparse sampler, SparseCoord coord) { 

  vec2 dfdx,dfdy; 

  textureSparseQueryGrad(dfdx, dfdy, sampler, coord); 

  return textureGrad(sampler.tex, coord.tex_coord, dfdx, dfdy); 

}
```


Dada una textura, realiza búsquedas optimizadas de varias texturas con pequeños desplazamientos

Estamos proporcionando versiones alternativas de este ayudante para un máximo de N=4

```
void textureSparseOffsets(SamplerSparse sampler, SparseCoord coord, vec2 offsets[N], out vec4 results[N]) { 

  vec2 dfdx,dfdy; 

  textureSparseQueryGrad(dfdx, dfdy, sampler, coord); 

  for(int i = 0; i < N; ++i) { 

    results[i] = textureGrad(sampler.tex, coord.tex_coord + offsets[i], dfdx, dfdy); 

  } 

} 

 
```
