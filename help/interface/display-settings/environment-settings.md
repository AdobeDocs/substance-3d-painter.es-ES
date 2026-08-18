---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/interface/display-settings/environment-settings.html"
breadcrumb-title: ''
description: Aprenda a configurar los ajustes del entorno en Substance 3D Painter para controlar la iluminación y el fondo para la previsualización del material.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Environment settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configuración del entorno
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---


# Configuración del entorno

Esta sección de **Configuración de visualización** controla la iluminación en la ventana gráfica.

## Entorno

![](../../assets/env-settings.png)

| *Configuración* | *Descripción* |
| --- | --- |
| **Mapa de entorno** | Textura del mapa de entorno que se utilizará para iluminar la escena. Se puede encontrar en la ventana [Assets](../assets/assets.md) mediante el ajuste preestablecido &quot;Environment&quot;.Haga clic en el botón para abrir un mini-estante y elegir un mapa de entorno diferente. |
| **Omitir espacio de color del mapa de entorno** | Si el proyecto actual usa [Administración de color](../../features/color-management/color-management.md), esta configuración se puede habilitar para invalidar el espacio de color del mapa de entorno. |
| **Opacidad del entorno** | Controla la visibilidad/opacidad de las texturas del entorno en el fondo de la ventana gráfica. Esta configuración no afecta a la iluminación de la escena. |
| **Exposición del entorno** | El valor de exposición (EV) es un número que representa una luminancia de escena fija. Este ajuste permite desplazar el valor de luminancia predeterminado.Este ajuste debe permanecer en 0 cuando se trabaja con los mapas de entorno proporcionados con la aplicación. Texturizar un activo con un valor de exposición incorrecto podría provocar problemas de calibración del color en otras aplicaciones. |
| **Rotación de entorno** | Controla la rotación horizontal de la textura del entorno. Resulta útil para girar la iluminación de la escena y cambiar la reacción del objeto. Se puede controlar con un [acceso directo](../settings/shortcuts.md). |
| **Desenfoque de entorno** | Controla la nitidez o desenfoque de la textura del entorno en el fondo de la ventana gráfica. Esta configuración no afecta a la iluminación. |
| **Alineación de entorno** | Controla cómo la textura del entorno gira en torno al modo 3D dentro del área de visualización. Este ajuste se puede utilizar para iluminar áreas bajo el modelo 3D cuando se configura en local.Valores posibles:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Mundo</strong> (predeterminado): el entorno se alinea con la escena y gira alrededor del eje superior del modelo 3D.</li><li data-preserve-html="true"><strong>Local</strong>: el entorno se alinea con la cámara y gira alrededor del eje superior de la cámara.</li></ul> |

## Sombras

![](../../assets/shadow-2.png)

| *Configuración* | *Descripción* |
| --- | --- |
| **Sombras** | Activar o desactivar el procesamiento de sombras en la ventana gráfica. |
| **Modo de cálculo** | Controla la rapidez con la que se calculan las sombras.<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Intensivo </strong> : Calcula rápido, pero puede bloquear el procesamiento de la ventana gráfica.</li><li data-preserve-html="true"><strong> Promedio </strong> : Promedio del modo Intensivo y Ligero.</li><li data-preserve-html="true"><strong> </strong> ligero : (predeterminado) Calcule las sombras lentamente durante unos segundos, pero no ralentiza el rendimiento de la ventana gráfica.</li></ul> |
| **Opacidad de las sombras** | Controla la cantidad de sombras que serán visibles en la escena. |
