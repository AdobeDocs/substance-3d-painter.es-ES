---
breadcrumb-title: ""
description: Acceda a la referencia de la API del sombreador de parámetros Todos los estados de procesamiento de Substance 3D Painter para controlar los parámetros del estado de procesamiento.
title: Todos los parámetros de estados de procesamiento - API del sombreador
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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


## localidad de muestreo de sombreador

De forma predeterminada, los canales de documento se muestrean utilizando coordenadas de textura sin transformar para procesar optimizaciones durante la pintura.

Si aparecen artefactos, establezca el estado *no local* en *el* .

```
//: state nonlocal on 

 
```
