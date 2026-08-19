---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/workflow-issues/export-issues/my-exported-opacity-map-is-totally-black.html"
breadcrumb-title: ''
description: Aprenda a corregir los mapas de opacidad exportados que aparecen totalmente en negro en Substance 3D Painter para una exportación de transparencia adecuada.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > My exported opacity map is totally black
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mi mapa de opacidad exportado es totalmente negro
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%

---


# Mi mapa de opacidad exportado es totalmente negro

Cuando se crea un proyecto nuevo, el color predeterminado procede del sombreado y no de las texturas. Por lo tanto, cuando exporte todas las partes que no haya pintado, se mostrarán negras con un valor alfa establecido en 0 (porque no hay datos en estas partes).

La forma más sencilla de solucionar este problema es colocar una capa de relleno en la parte inferior de la pila de capas : rellenará todas las coordenadas UV con un color predeterminado, que es idéntico al color predeterminado del sombreado.
