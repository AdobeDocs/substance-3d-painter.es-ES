---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/exporting-the-log-file.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo exportar archivos de registro de Substance 3D Painter para solucionar problemas y para obtener asistencia técnica.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Exporting the log file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exportación del archivo de registro
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%

---


# Exportación del archivo de registro

Esta página explica cómo encontrar el archivo de registro de la aplicación y cómo compartirlo para solicitar asistencia.

## Recuperando el archivo de registro

Existen dos formas de obtener el archivo de registro:

### Exportación del archivo de registro desde la aplicación

El archivo de registro se puede exportar directamente desde la aplicación en el menú **Ayuda** y seleccionando la acción **Exportar registro**.

![](../assets/screenshot-20210622-195334.png)

### Recuperar el archivo de registro manualmente en el disco

Si la aplicación no se inicia, no será posible exportar el archivo de registro. Afortunadamente, el archivo de registro se puede ubicar manualmente en el disco. Vaya a la carpeta que coincida con su sistema operativo a continuación y recupere el archivo **log.txt** manualmente.

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Platform</th><th>Versión</th><th colspan="2">Ruta</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> o posterior</td><td colspan="1">Datos de la aplicación (local)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Datos de la aplicación (itinerancia)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">Heredada</td><td colspan="1">Datos de la aplicación (local)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">Datos de la aplicación (itinerancia)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="2">/Usuarios/[nombre de usuario]/Librería/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Heredada</td><td colspan="2">/Usuarios/[nombre de usuario]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="2">/home/[nombre de usuario]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Heredada</td><td colspan="2">/home/[nombre de usuario]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> Algunos de los directorios de las rutas mencionadas anteriormente pueden estar ocultos de forma predeterminada. Escriba la ruta de acceso manualmente en el explorador de archivos o muestre los archivos ocultos para verlos.

## Adjuntar el archivo de registro a un mensaje de la comunidad para obtener asistencia

Al escribir un mensaje, utilice el área de datos adjuntos para insertar el archivo de registro:

![](../assets/screenshot-20210708-113456.png)
