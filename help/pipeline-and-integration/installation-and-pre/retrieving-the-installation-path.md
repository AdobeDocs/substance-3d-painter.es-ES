---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/retrieving-the-installation-path.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo recuperar la ruta de instalación de Substance 3D Painter para la integración de secuencias de comandos y canalizaciones.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Retrieving the installation path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Recuperación de la ruta de instalación
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 5%

---


# Recuperación de la ruta de instalación

Esta página reagrupa información sobre las formas de recuperar la ruta de instalación de la aplicación en función de la versión y la plataforma.

## Windows

### Escritorio de Creative Cloud

1. Abra el Editor del Registro de Windows (**regedit**).
1. Vaya a la clave del registro: ** HKEY\_LOCAL\_MACHINE\Software\Microsoft\Windows\CurrentVersion\App Rutas\**
1. Abra la subclave denominada **Adobe Substance 3D Painter.exe**
1. El valor de la clave contiene la ruta de acceso al ejecutable de la aplicación donde está instalada

>[!NOTE]
>
> Esta clave de registro solo está disponible desde la versión 7.2.\
>  Para versiones anteriores, la ruta de instalación se puede recuperar de las asociaciones de archivos en **HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\ Explorer\FileExts**.

### Substance 3D independiente

1. Abra el Editor del Registro de Windows (**regedit**).
1. Vaya a la clave del Registro: **HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall**
1. Busque la subclave que coincida con el ID de aplicación de la versión de la aplicación (consulte la tabla siguiente)
1. El valor de la clave contiene la ruta de la ubicación de instalación de la aplicación

| Versión | AppId |
| --- | --- |
| **Versión 1.x** | `{410F5B6E-A29C-4F43-9DE3-44A1357D6AF5}` |
| **Versión 2.x** | `{f42b7a996fa1d13a1d0a2e33eea2c0800bb5d1b8}` |
| **3.x (2017.x) a 7.1** | `{33C3E9E2-0675-4196-9019-28AB9C5E9BB0}` |
| **7.2 o posterior** | `{2a8bbb68-725b-477c-9194-60efc5ece348}` |

### Vapor

La aplicación se instala en la subcarpeta **steamapps/common/** de la carpeta de instalación de Steam.

## Mac

En Mac, la aplicación se instala de la siguiente manera:

| Versión | Ruta |
| --- | --- |
| **7.2 o posterior** | **/Applications/Adobe Substance 3D Painter.app** |
| **Heredado** | **/Applications/Substance Painter.app** |

## Linux

En Linux, el paquete rpm se instala en la siguiente ruta:

| Versión | Ruta |
| --- | --- |
| **7.2 o posterior** | **/opc/Adobe/Adobe\_Substance\_3D\_Painter** |
| **Heredado** | **/opc/Allegorithmic/Substance\_Painter** |
