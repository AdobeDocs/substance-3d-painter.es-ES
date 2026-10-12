---
breadcrumb-title: ""
description: Acceda a la referencia de API del sombreador Declarar pilas de capas para Substance 3D Painter para crear pilas de capas de material personalizadas.
title: Declarar pilas por capas - API del sombreador
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%
---

# Declarar pilas por capas - API del sombreador

## Capas de materiales: declarar pilas editables

Una pila editable se define mediante un identificador único y una lista de canales de documento. Los posibles ID de canal son: *ambientocclusion* *anisotropyangle* *anisotropylevel* *basecolor* *blendingmask* *diffuse* *desplazamiento* *emisivo* *brillo* *height* *submarino* *metálico* **&#x200B; opacidad &#x200B;** reflexión **&#x200B; rugosidad &#x200B;** dispersión **&#x200B; specular &#x200B;** nivel especular **&#x200B; transmisivo &#x200B;** usuario0 **&#x200B; usuario1 &#x200B;** usuario2 **&#x200B; usuario3&rbrace; 7&rbrace; *usuario4* *usuario5* *usuario6* *usuario7***

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


Para enlazar un canal de una pila a un parámetro de muestra, añada el identificador de la pila al prefijo de la etiqueta del canal:

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
