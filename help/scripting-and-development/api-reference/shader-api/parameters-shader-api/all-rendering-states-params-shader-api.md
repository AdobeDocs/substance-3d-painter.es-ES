---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-rendering-states-params-shader-api.html"
breadcrumb-title: ''
description: Acceda a la referencia de la API del sombreador de parámetros Todos los estados de procesamiento de Substance 3D Painter para controlar los parámetros del estado de procesamiento.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Rendering States Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Todos los parámetros de estados de procesamiento - API del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 2%

---


# Todos los parámetros de estados de procesamiento - API del sombreador

## Ejemplos de estados de procesamiento

## Selec. cara posterior

Retirar caras:

```
//: state cull_face on
```


Dibujo de caras frontales y posteriores:

```
//: state cull_face off
```


## Fusión

Sin fusión, objetos completamente opacos:

```
//: state blend none
```


Modo de fusión estándar para el orden de recepción:

```
//: state blend over
```


Modo de fusión estándar para el orden de dibujo de atrás a adelante. Suponer que el color se premultiplica por alfa:

```
//: state blend over_premult
```


Modo de fusión aditivo:

```
//: state blend add
```


Modo de fusión multiplicativa:

```
//: state blend multiply
```


## Localidad de muestreo del sombreador

De forma predeterminada, los canales de documento se muestrean utilizando coordenadas de textura sin transformar para procesar optimizaciones durante la pintura.

Si aparecen artefactos, establezca el estado *no local* en *el* .

```
//: state nonlocal on 

 
```
