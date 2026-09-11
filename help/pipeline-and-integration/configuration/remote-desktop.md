---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/remote-desktop.html"
breadcrumb-title: ''
description: Aprenda a configurar Substance 3D Painter para el acceso remoto al escritorio para habilitar los flujos de trabajo y la colaboración remotos.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Remote Desktop
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Escritorio remoto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---


# Escritorio remoto

Esta página describe soluciones y alternativas para que Substance 3D Painter pueda ejecutarse a través de Escritorio remoto (RDP) en Windows.

De forma predeterminada, el RDP en Windows se ejecuta en un contexto de OpenGL que no existe o que es demasiado bajo, lo que hace que la aplicación no pueda funcionar correctamente o que se produzca un bloqueo. Substance 3D Painter requiere un contexto de OpenGL 3.3. A continuación, se muestran soluciones para mitigar el problema, pero no hay garantías de que funcionarán, ya que el problema inicial depende de Windows y algunos controladores de GPU.

>[!NOTE]
>
> Las GPU NVIDIA Quadro pueden ejecutar la aplicación en modo RDP de forma predeterminada, mientras que las GPU Nvidia GeForce solo proporcionan un contexto OpenGL 1.4 (demasiado bajo para Substance 3D Painter). Es posible instalar un ejecutable para remediar esto, consulte: <https://developer.nvidia.com/designworks>

## Configuración de directivas de Windows

En Windows 10, puede ser necesario cambiar la **Directiva de grupo** para permitir que la GPU se ejecute en modo RDP.

Para ello:

1. Presione **Win + R** para abrir la ventana de ejecución
1. Escriba &quot;**gpedit.msc**&quot; y luego Intro
1. Vaya a **Directiva de equipo local\Configuración del equipo\Plantillas administrativas\Componentes de Windows\Servicios de Escritorio remoto\Host de sesión de Escritorio remoto\Entorno de sesión remota**
1. Habilite la opción **Usar el adaptador de gráficos predeterminado de hardware para todas las sesiones de Servicios de Escritorio remoto** .

## Comando TSCON de Windows

Si el cambio de directiva anterior no funciona, puede intentar usar la línea de comandos **tscon**. Este comando desconecta el equipo remoto y conecta uno nuevo al hardware físico (ratón, teclado, etc.). Simplemente ejecutando la aplicación y volviendo a conectar remotamente debería poder trabajar con la aplicación en la GPU.

1. Presione la tecla **Windows+R** para abrir la ventana **execute**.
1. Escriba **cmd** y pulse **Intro** .
1. En la línea de comandos, escriba y ejecute el comando siguiente:  **tscon 1 /dest:console**
1. Pulse Intro
1. En la línea de comandos, escriba el siguiente comando:  **iniciar &quot;Ruta/Al/Substance/Painter/Carpeta/Substance 3D Painter.exe&quot;** (asegúrese de cambiar la ruta para que coincida con su equipo)
1. Pulse Intro

Después de estos pasos, espere unos segundos para permitir el inicio de la aplicación y, a continuación, vuelva a conectarse a la sesión.

Es posible que tenga que ejecutar la línea de comandos de Windows en modo de administrador en caso de que este procedimiento no funcione.

## Alternativas

Si las sugerencias anteriores siguen sin funcionar, recomendamos utilizar soluciones alternativas, como VNC o Teamviewer, que admiten la GPU a través de conexiones remotas.
