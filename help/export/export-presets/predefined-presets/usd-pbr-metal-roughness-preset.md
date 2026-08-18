---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export/export-presets/predefined-presets/usd-pbr-metal-roughness-preset.html"
breadcrumb-title: ''
description: Aprenda a utilizar el ajuste preestablecido Exportar USDz (Apple AR) en Substance 3D Painter para exportar texturas para flujos de trabajo de Apple AR.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Export presets > Predefined Presets > USDz (Apple AR) Preset
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: USDz (Apple AR)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# Plantilla predefinida USDz (Apple AR)

>[!NOTE]
>
> Para exportar a USD con una Plantilla de salida personalizada, no utilice la plantilla USDz (Apple AR). En su lugar, utilice la Plantilla de salida que haya elegido y habilite <b>Exportar recurso USD</b> en la parte inferior de la <b>pestaña Configuración</b>.

La plantilla de salida predefinida USDz (Apple AR) exporta el recurso configurado para su uso con aplicaciones Apple AR.

Para utilizar la plantilla USDz (Apple AR):

1. Abra la ventana de exportación con <b>Archivo > Exportar texturas</b> o con el método abreviado de teclado <b>Ctrl + Mayús + E</b>.
1. En la <b>pestaña Configuración</b>, abre la <b>lista desplegable de Plantillas de salida</b> y selecciona <b>USDz (Apple AR)</b>.

![Imagen de la ventana de exportación que muestra el menú desplegable de plantillas de salida abierto y los USDz (Apple AR) seleccionados.](../../../assets/export-usd.png){zoomable="yes"}

Se crean y se guardan cinco archivos de textura (color base, metálico, normal, oclusión y rugosidad). Todos los archivos se guardan como JPG, excepto el mapa normal, que se guarda como PNG para evitar artefactos debido a la compresión con pérdida.

Además, se crean otros dos archivos con la extensión usdc y usdz:

A continuación se muestra un ejemplo del JadeToad abierto directamente en MacOS desde Finder:

![](../../../assets/usdz.png){width="400px"}

A continuación se muestra un ejemplo del archivo USDZ enviado a un iPhone, utilizando el modo AR para colocar el modelo JadeToad en un entorno real:

![](../../../assets/3d-usdz.jpg){width="500px"}
