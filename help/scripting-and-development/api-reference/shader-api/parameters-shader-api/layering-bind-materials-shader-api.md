---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-bind-materials-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador de materiales de enlace de capas de Substance 3D Painter para enlazar materiales en flujos de trabajo de capas.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Bind Materials - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Materiales de enlace de capas - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# Materiales de enlace de capas - API del sombreador

## Capas de materiales: enlazar materiales como parámetros de sombreador

Un material se define mediante un &#39;id&#39; de identificador único. Parámetros adicionales:

* &#39;predeterminado&#39;: nombre de recurso material por defecto que se va a utilizar.
* &#39;tamaño&#39;: el tamaño de textura de los mapas de material.
* &#39;grupo&#39;: el grupo de la interfaz de usuario del widget de selección de material.

Ejemplo:

```
//:  materials [ 

//:    { 

//:       "id": "Material1", 

//:       "default": "Concrete 044", 

//:       "size": 512, 

//:       "group": "Material 1" 

//:    }, { 

//:       "id": "Material2", 

//:       "default": "Leaves elm", 

//:       "size": 1024, 

//:       "group": "Material 2" 

//:    } 

//:  ]
```


Para enlazar un canal de un material a un muestreador, defina un parámetro automático con el identificador del material seguido de la etiqueta del canal (consulte los canales disponibles en [all-engine-params.glsl](all-engine-params-shader-api.md)):

```
//: param auto Material1.channel_basecolor 

uniform sampler2D basecolor_tex1; 

//: param auto Material1.channel_metallic 

uniform sampler2D metallic_tex1; 

//: param auto Material1.channel_roughness 

uniform sampler2D roughness_tex1; 

 

//: param auto Material2.channel_basecolor 

uniform sampler2D basecolor_tex2; 

//: param auto Material2.channel_metallic 

uniform sampler2D metallic_tex2; 

//: param auto Material2.channel_roughness 

uniform sampler2D roughness_tex2; 

 
```
