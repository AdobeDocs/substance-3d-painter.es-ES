---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/getting-started/activation-and-licenses.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo activar Substance 3D Painter y administrar licencias para empezar a utilizar la aplicación para pintar texturas.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Activation and licenses
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Activación y licencias
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---


# Activación y licencias

Esta página contiene información sobre cómo activar y administrar sus licencias para que pueda empezar a usar Painter.

## Proceso de activación por tipo de aplicación

El proceso de activación depende de dónde haya comprado Painter o tenga acceso a él:

| Tipo de aplicación | Proceso de activación |
| --- | --- |
| Escritorio de Creative Cloud | Consulte la página dedicada en la [documentación de HelpX](https://helpx.adobe.com/es/download-install/using/download-creative-cloud-apps.html). En caso de que haya algún problema, la [documentación del Creative Cloud](https://helpx.adobe.com/es/creative-cloud/user-guide.html) puede proporcionar respuestas adicionales. |
| Vapor | Inicie el producto directamente desde su biblioteca de Steam. |
| Substance 3D independiente | Consulte el proceso de activación que se describe a continuación. |

## Pasos de activación independiente

### El asistente de activación

El asistente de activación aparece en una determinada versión heredada de Substance 3D Painter.

Si tiene un archivo de licencia vitalicia descargado del sitio web de Substance 3D antes del 30 de septiembre de 2022, todavía puede utilizarlo para activar las versiones elegibles de Substance 3D Painter a través del Asistente de activación. [Encontrarás más información sobre las licencias y cuentas de Substance heredadas aquí.](https://substance3d.adobe.com/faq-end-of-life-accounts/)

![](../assets/activation-wizard.png){width="350px"}

El Asistente para la activación tiene 3 opciones:

* <b>Evaluar este producto</b>: Las pruebas heredadas ya no están disponibles. En su lugar, [puede iniciar una versión de prueba de 30 días para cada aplicación de Substance 3D aquí](https://www.adobe.com/es/products/substance3d/free-trial-download.html?msockid=35568f9be2b964ec22d09c04e3eb65af) o con Creative Cloud Desktop.
* <b>Activar usando un archivo de licencia</b>: active el producto con un archivo de licencia (<b>\*.key</b>) descargado de la página de su cuenta en el sitio web de Substance 3D antes del 30 de septiembre de 2022.
* <b>Activar usando tu cuenta</b>: Las cuentas de sustancias heredadas ya no se pueden utilizar para la activación.

>[!WARNING]
>
> Para instalar el archivo de licencia con el Asistente de activación, asegúrese de ejecutar Painter como administrador y desactive temporalmente el antivirus.

### Activación manual

Puede activar manualmente Substance Painter colocando el archivo license.key en la carpeta siguiente:

>[!NOTE]
>
> Asegúrese de que el archivo se llama **license.key**; de lo contrario, la aplicación no podrá encontrarlo.

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Platform</th><th>Versión</th><th colspan="2">Ruta</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> o posterior</td><td colspan="1">Datos de la aplicación (local)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Datos de la aplicación (itinerancia)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">Heredada</td><td colspan="1">Datos de la aplicación (local)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">Datos de la aplicación (itinerancia)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="2">/Usuarios/[nombre de usuario]/Librería/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Heredada</td><td colspan="2">/Usuarios/[nombre de usuario]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="2">/home/[nombre de usuario]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Heredada</td><td colspan="2">/home/[nombre de usuario]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> Algunos de los directorios de las rutas mencionadas anteriormente pueden estar ocultos de forma predeterminada. Escriba la ruta de acceso manualmente en el explorador de archivos o muestre los archivos ocultos para verlos.

### Variable de entorno

Puede invalidar la ubicación en la que Painter comprueba el archivo **license.key** con una [variable de entorno](../pipeline-and-integration/configuration/environment-variables.md).
