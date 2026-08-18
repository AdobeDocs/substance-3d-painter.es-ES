---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/broken-viewport-ubuntu.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo solucionar problemas de la ventana gráfica rota o que no responde en Ubuntu en Substance 3D Painter para una representación 3D adecuada.
helpx_creative_field: ""
helpx_description: Viewport appears broken or unresponsive on Ubuntu
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La ventana gráfica aparece rota o no responde en Ubuntu
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---


# La ventana gráfica aparece rota o no responde en Ubuntu

Al ejecutar Painter desde Steam en Ubuntu a partir de la versión 11.1, la ventana gráfica puede aparecer rota o sin respuesta.

Esto está relacionado con el hecho de que Painter no se inicie con la GPU correcta asignada. En Ubuntu, la GPU integrada en lugar de la discreta puede terminar siendo seleccionada. Painter hereda esta configuración a través de Steam, lo que puede provocar problemas.

Existen algunas soluciones:

1. Ejecutar Steam desde un terminal. Esto forzará un contexto diferente y debería hacer que Steam y Painter se ejecuten en la GPU correcta.
1. Edite el acceso directo de Steam para deshabilitar la configuración <b>Ejecutar usando tarjeta gráfica dedicada</b>. A continuación, ejecute Steam normalmente.

Para obtener más información, consulte [este problema de github](https://github.com/ValveSoftware/steam-for-linux/issues/9940).
