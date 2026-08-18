---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/preferences-and-application-data-location.html"
breadcrumb-title: ''
description: Obtenga información sobre las preferencias y las ubicaciones de datos de la aplicación para que Substance 3D Painter administre la configuración y los datos de usuario.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Preferences and application data location
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Preferencias y ubicación de datos de la aplicación
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 4%

---


# Preferencias y ubicación de datos de la aplicación

Esta página reagrupa información sobre dónde se almacenan las preferencias de la aplicación por versión y plataforma.\
Puede resultar útil saber dónde se almacenan las preferencias en caso de que desee agregar **shelfs personalizados** (para instalaciones de studios) o quitar estas preferencias para realizar una **instalación limpia** de la aplicación.

## Preferencias

Esta ruta es la ubicación de las preferencias de la aplicación (métodos abreviados guardados, rutas de activos/estanterías, diseño de la interfaz, etc.).

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>Sistema</th><th>Versión</th><th>Ruta</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>(Registro)</p></td><td><strong>7.2</strong> o posterior</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>Heredada</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>(biblioteca)</p></td><td><strong>7.2</strong> o posterior</td><td>/Usuarios/[nombre de usuario]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>Heredada</td><td>/Usuarios/[nombre de usuario]/Library/Preferences/com.substance3d.Substance Painter.plist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td><strong>7.2</strong> o posterior</td><td>/home/[nombre de usuario]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>Heredada</td><td>/home/[nombre de usuario]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

## Datos de aplicación

Esta ruta es la ubicación de los datos adicionales de la aplicación (miniaturas de recursos, archivo de registro, etc.).

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Platform</th><th>Versión</th><th colspan="2">Ruta</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> o posterior</td><td colspan="1">Datos de la aplicación (local)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Datos de la aplicación (itinerancia)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">Heredada</td><td colspan="1">Datos de la aplicación (local)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">Datos de la aplicación (itinerancia)</td><td colspan="1">C:\Users\[nombre de usuario]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="2">/Usuarios/[nombre de usuario]/Librería/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Heredada</td><td colspan="2">/Usuarios/[nombre de usuario]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="2">/home/[nombre de usuario]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Heredada</td><td colspan="2">/home/[nombre de usuario]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> Algunos de los directorios de las rutas mencionadas anteriormente pueden estar ocultos de forma predeterminada. Escriba la ruta de acceso manualmente en el explorador de archivos o muestre los archivos ocultos para verlos.
