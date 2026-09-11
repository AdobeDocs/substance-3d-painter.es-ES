---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-declare-stacks-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de API del sombreador Declarar pilas de capas para Substance 3D Painter para crear pilas de capas de material personalizadas.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Declare Stacks - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Declarar pilas por capas - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%

---


# Declarar pilas por capas - API del sombreador

## Capas de materiales: declarar pilas editables

Una pila editable se define mediante un identificador único y una lista de canales de documento. Los posibles ID de canal son: *ambientocclusion* *anisotropyangle* *anisotropylevel* *basecolor* *blendingmask* *diffuse* *desplazamiento* *emisivo* *brillo* *height* *submarino* *metálico* ** opacidad ** reflexión ** rugosidad ** dispersión ** specular ** nivel especular ** transmisivo ** usuario0 ** usuario1 ** usuario2 ** usuario3} 7} *usuario4* *usuario5* *usuario6* *usuario7***

Ejemplo:

```
//:  stacks [ 

//:    { 

//:      "id": "Mask1", 

//:      "channels": [ 

//:        {"id": "opacity"} 

//:      ] 

//:    }, { 

//:      "id": "Mask2", 

//:      "channels": [ 

//:        {"id": "opacity"}, 

//:        {"id": "user0"} 

//:      ] 

//:    } 

//:  ]
```


Para enlazar un canal de una pila a un parámetro de muestra, coloque el identificador de pila delante de la etiqueta del canal:

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
