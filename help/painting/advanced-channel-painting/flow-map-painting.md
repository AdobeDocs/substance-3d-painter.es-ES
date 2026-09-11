---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/flow-map-painting.html"
breadcrumb-title: ''
description: Aprenda a pintura mapas de flujo en Substance 3D Painter para controlar la dirección del flujo de material y los efectos anisotrópicos.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Flow Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pintura de mapa de flujo
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Pintura de mapa de flujo

Se ha previsto un canal dedicado, pero mientras tanto, mediante el canal Normal y algunos parámetros de pincel es posible pintura de mapas de flujo en Substance 3D Painter.

## Paso 1 : Crear el mapa de normales

Cree una textura de mapa de normales de 16 por 16 píxeles. El color debe ser 128, 255, 128, que debe dar el siguiente color: ![](../../assets/up-dx.png)\
(Este color es el equivalente a un vector que mira hacia arriba, en DirectX)

## Paso 2 : Añadir canal normal

En tu proyecto de Substance 3D Painter, añade un canal **Normal** mediante la **configuración del conjunto de texturas** si este canal aún no existe.

## Paso 3 : Configuración del pincel

Active la función Seguir trazado en los parámetros del pincel. Cargue la textura de mapa de normales (paso 1) en la ranura del canal normal. Deshabilite los otros canales.

![](../../assets/brush-settings-1.png){width="300px"}

## Paso 4 : ¡pintura!

Al pintar en la malla con el ajuste Seguir trazado activado, los trazos de pincel dibujarán direcciones hacia el mapa de normales.

![](../../assets/painting-1.png){width="700px"}
