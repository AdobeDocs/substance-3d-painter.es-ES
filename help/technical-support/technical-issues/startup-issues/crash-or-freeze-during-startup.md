---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/startup-issues/crash-or-freeze-during-startup.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo solucionar bloqueos y bloqueos al iniciar Substance 3D Painter para iniciar una aplicación estable.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Crash or freeze during startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bloqueo o congelación durante el inicio
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---


# Bloqueo o congelación durante el inicio

En esta página se enumeran los problemas conocidos y sus soluciones relacionados con la aplicación que no se inicia correctamente.

## Conflictos de software

Consulte la página siguiente para obtener una lista de todos los programas conocidos que pueden crear conflictos: [Conflictos de software](software-conflicts.md).

## Ejecución en una GPU incorrecta

Si la aplicación no se inicia en la GPU correcta, podrían producirse problemas de estabilidad. Consulte esta página para obtener más información: [Painter no se inicia en la GPU correcta](../gpu-issues/painter-doesn-t-start-on-the-right-gpu.md).

## Controladores de GPU obsoletos

El uso de controladores de GPU antiguos puede provocar bloqueos o bloqueos. Se recomienda utilizar los controladores de GPU más recientes cuando estén disponibles. Consulte: [La GPU tiene controladores obsoletos](../gpu-issues/gpu-has-outdated-drivers.md).

## Pantalla en blanco y sin respuesta

Si la aplicación se bloquea al iniciarse en Windows (lo que lleva a una pantalla en blanco), puede ser por varias razones:

* Una aplicación externa está creando un conflicto. Consulte [Conflictos de software](software-conflicts.md) para saber cuáles.
* Algunas ventanas de la aplicación se abrieron en otro monitor. Restaurar la interfaz a su diseño predeterminado permite iniciar la aplicación normalmente:
  1. Abra el editor del Registro (**regedit** en el menú Inicio)
  1. Vaya a las preferencias de la aplicación (consulte: [Preferencias y ubicación de datos de la aplicación](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html))
  1. Expanda la clave **Adobe Substance 3D Painter**
  1. Seleccione la clave **Main Window 2018** y elimínela
  1. Reinicie la aplicación

## Bloqueo debido a una ruta incorrecta del sistema/ruta de Python

La aplicación comprueba la ruta del sistema para cargar los módulos de Python y la configuración del entorno. Si el sistema tiene una configuración incorrecta, puede provocar un bloqueo durante el arranque.

En Windows:

1. Abra el menú **Inicio**
1. Busque y seleccione el **Sistema (Panel de control)**
1. Haga clic en **Configuración avanzada del sistema**
1. Haga clic en **Variables de entorno**
1. En **Variables del sistema**, busque la variable **PATH**

A continuación, puede editar la variable para verificar su contenido. Por ejemplo, si la variable contiene este tipo de caracteres, provocará un bloqueo

```
ï–›éŒ à €è¸€ì‡ì‡ç¿¹
```


## Actualizaciones de Windows 10

Algunas actualizaciones de Windows 10 a veces pueden crear inestabilidad. Utilice las herramientas de diagnóstico proporcionadas con Windows para detectar cualquier error potencial en el sistema.

Se recomienda ejecutar **Administración y mantenimiento de imágenes de implementación** (DISM) y la herramienta **Comprobador de archivos del sistema** (SFC). DISM es útil para recuperar los archivos de reemplazo necesarios para SFC con el fin de corregir los archivos del sistema dañados o que faltan.

Ejecutando **DISM** :

1. Abrir el menú Inicio
1. Buscar símbolo del sistema
1. Haga clic con el botón derecho en el resultado y elija &quot;Ejecutar como administrador&quot;
1. Escriba el comando siguiente :  **DISM /Online /Cleanup-Image /RestoreHealth**
1. Pulse Intro

Ejecutando **SFC** :

1. Abrir el menú Inicio
1. Buscar símbolo del sistema
1. Haga clic con el botón derecho en el resultado y elija &quot;Ejecutar como administrador&quot;
1. Escriba el comando siguiente :  **sfc /scannow**
1. Pulse Intro

Reinicie el equipo después de ambos comandos para aplicar las actualizaciones.

Para obtener más información sobre este tema, consulte:  [Use la herramienta Comprobador de archivos de sistema para reparar los archivos del sistema que faltan o que están dañados](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system).

## Bloqueo al iniciar en versiones anteriores

En Windows, es posible que la versión 2018 (4.x) o una anterior no se inicie porque uno de los archivos dll proporcionados con la carpeta de instalación es demasiado antiguo para el sistema operativo. Este bloqueo se puede corregir reemplazando manualmente el archivo por una versión más reciente.

Para ello:

1. Vaya a la carpeta de instalación del Substance Painter.
1. Cambie el nombre del archivo <b>libay32.dll</b> en <b>backup\_libay32.dll</b>.
1. Descargue el siguiente archivo: [actualizado\_libeay32.zip](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/182266673/225968681/1/1644000679697/updated-libeay32.zip).
1. Extraiga el archivo dll del archivo zip en la carpeta de instalación (junto al archivo Substance Painter.exe ).
1. Inicie la aplicación.
