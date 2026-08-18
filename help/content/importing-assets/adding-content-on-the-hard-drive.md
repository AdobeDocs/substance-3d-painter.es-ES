---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/importing-assets/adding-content-on-the-hard-drive.html"
breadcrumb-title: ''
description: Aprenda a agregar contenido de su disco duro a Substance 3D Painter para expandir su biblioteca de recursos con archivos locales.
helpx_creative_field: ""
helpx_description: Painter > Content > Importing assets > Adding content on the hard drive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Adición de contenido en el disco duro
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 2%

---


# Adición de contenido en el disco duro

Es posible agregar recursos a sus bibliotecas colocando el nuevo contenido directamente en el disco duro en la ubicación correcta.

De forma predeterminada, se proporciona una carpeta predeterminada para los activos de usuario en la que puede agregar su nuevo contenido, ya sea a través de la interfaz de la aplicación o soltándolo manualmente en la siguiente ubicación. Esta biblioteca predeterminada también se utiliza al crear nuevos ajustes preestablecidos, como pinceles, herramientas, materiales inteligentes, etc. Para obtener más información, consulte la documentación de [Ajustes preestablecidos](../../painting/presets/presets.md).

## ¿Dónde colocar los activos?

A continuación, se muestran las ubicaciones de la biblioteca predeterminada **Your Assets**, donde se crea su propio contenido personalizado de forma predeterminada:

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Platform</th><th>Versión</th><th>Ruta</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> o posterior</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Heredada</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="1">/Usuarios/nombre_usuario/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Heredada</td><td colspan="1">/Usuarios/nombre_usuario/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Heredada</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!WARNING]
>
> Los **activos de inicio** que se incluyen con la aplicación se encuentran en la carpeta de instalación y se reemplazan en cada nueva versión. No recomendamos colocar contenido personal en esta ubicación, ya que se **borrará con cada actualización** e incluso puede causar problemas de permisos de lectura/escritura.\
> Es mejor usar la ubicación de **Tus activos** u otra ubicación personalizada. Para obtener más información sobre cómo agregar una ubicación de biblioteca personalizada, vea [Agregar una nueva biblioteca](../../interface/assets/adding-a-new-library.md).

## Formatos de archivo y usos

Puede importar diferentes tipos de archivos a la biblioteca de Substance 3D Painter. Colocándolos en las carpetas designadas (como *alphas*, *colorluts*, *effects*...) asignará un tipo de uso al activo, por lo que es importante elegir la carpeta correcta al añadir nuevo contenido. Tenga en cuenta que si agrega una ubicación de biblioteca personalizada, se crearán automáticamente las carpetas adecuadas en esa ubicación.

| *Formato de archivo* | *Uso* | *Carpeta* |
| --- | --- | --- |
| **SBSAR** | Material de Substance | activos / Materiales |
| **SBSAR** | Filtros | activos/efectos |
| **SBSAR** | Generadores | activos / Generadores |
| **PNG, TGA, JPEG, etc.** | Textura o Alpha | activos / Texturas **o** Estante / Alpha |
| **HDR, EXR** | Entorno o Lut de color | activos / Entornos **o** Shelf / Colorlut |
| **GLSL** | Sombreador | activos / Shaders |
| **SPPR** | Pincel preestablecido | activos / Ajustes preestablecidos / Pincel |
| **SPPR** | Ajuste preestablecido de objetos | activos / Ajustes preestablecidos / Partículas |
| **SPPR** | Ajustes preestablecidos de material | activos / Ajustes preestablecidos / Materiales **o** activos / Materiales |
| **SPPR** | Herramienta preestablecida | activos / Ajustes preestablecidos / Herramientas |
| **SPSM** | Materiales inteligentes | activos / Materiales inteligentes |
| **SPMSK** | Máscara inteligente | activos / Máscaras inteligentes |
| **SPEXP** | Exportar ajuste preestablecido | Shelf / Export-presets |

>[!NOTE]
>
> A partir de la versión 7.2.0, las carpetas y categorías personalizadas se pueden utilizar en una biblioteca. Se podrá acceder a ellos en la ventana Activos a través de [Filtrar por ruta de acceso](../../interface/assets/filter-by-path.md) o [Rastros](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/navigating-in-the-shelf-147095659.html).

>[!WARNING]
>
> Los archivos **SBS** (no SBSAR) no se pueden usar directamente; deben exportarse como SBSAR desde Substance 3D Designer.
