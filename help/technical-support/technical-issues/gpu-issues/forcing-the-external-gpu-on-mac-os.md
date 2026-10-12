---
breadcrumb-title: ""
description: Obtenga más información sobre cómo obligar a Substance 3D Painter a utilizar una GPU externa en macOS para mejorar el rendimiento de procesamiento.
title: Forzar la GPU externa en el sistema operativo Mac
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%
---

# Forzar la GPU externa en el sistema operativo Mac

En Mac OS Mojave, es posible especificar por aplicación el uso de la GPU externa. El rendimiento y la estabilidad de Substance 3D Painter pueden mejorar si se habilita esta configuración.

Para obtener más información, consulte la [documentación de Apple](https://support.apple.com/en-us/HT208544).

Para activarla:

1. Cierre Substance 3D Painter si está en ejecución.
1. Seleccione Substance 3D Painter en el Finder; se encuentra en la carpeta **Aplicaciones**&#x200B;**.**
1. Pulse **Comando-I** o haga clic con el botón derecho en la aplicación **Substance 3D Painter** y elija **Obtener información**.
1. En la nueva ventana, habilite la configuración **Preferir GPU externa**.
1. Reinicie Substance 3D Painter.

>[!NOTE]
>
> Esta configuración no será visible si no hay una eGPU conectada o si la versión actual de MacOS es demasiado antigua.
