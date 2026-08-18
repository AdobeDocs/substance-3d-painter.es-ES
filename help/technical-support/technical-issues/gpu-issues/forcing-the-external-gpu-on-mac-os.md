---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/forcing-the-external-gpu-on-mac-os.html"
breadcrumb-title: ''
description: Obtenga más información sobre cómo obligar a Substance 3D Painter a utilizar una GPU externa en macOS para mejorar el rendimiento de procesamiento.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Forcing the external GPU on Mac OS
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Forzar la GPU externa en el sistema operativo Mac
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---


# Forzar la GPU externa en el sistema operativo Mac

En Mac OS Mojave, es posible especificar por aplicación el uso de la GPU externa. El rendimiento y la estabilidad de Substance 3D Painter pueden mejorar si se habilita esta configuración.

Para obtener más información, consulte la [documentación de Apple](https://support.apple.com/en-us/HT208544).

Para activarla:

1. Cierre Substance 3D Painter si está en ejecución.
1. Seleccione Substance 3D Painter en el Finder; se encuentra en la carpeta **Aplicaciones****.**
1. Pulse **Comando-I** o haga clic con el botón derecho en la aplicación **Substance 3D Painter** y elija **Obtener información**.
1. En la nueva ventana, habilite la configuración **Preferir GPU externa**.
1. Reinicie Substance 3D Painter.

>[!NOTE]
>
> Esta configuración no será visible si no hay una eGPU conectada o si la versión actual de MacOS es demasiado antigua.
