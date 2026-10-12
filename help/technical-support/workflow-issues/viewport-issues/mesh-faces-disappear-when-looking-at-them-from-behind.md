---
breadcrumb-title: ""
description: Obtenga más información sobre cómo corregir la desaparición de caras de malla cuando se visualizan desde detrás en la ventana gráfica de Substance 3D Painter para obtener una visibilidad de malla adecuada.
title: Las caras de malla desaparecen al mirarlas desde atrás
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%
---

# Las caras de malla desaparecen al mirarlas desde atrás

De forma predeterminada, las mallas de la ventana gráfica pueden no mostrar la parte posterior de los polígonos de malla (cara posterior). Esto se debe a que son sacrificados por el sombreador actual.

Para mostrar la parte posterior de las caras, simplemente cambie el sombreador actual a **pbr-metal-rough-alpha-test** en la [configuración del Sombreador](../../../interface/shader-settings/shader-settings.md).
