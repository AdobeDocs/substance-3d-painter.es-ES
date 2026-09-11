---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/pipeline-and-integration/resource-management/preferences-and-content-migration.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo migrar preferencias y contenido en Substance 3D Painter al actualizar o cambiar a un sistema nuevo.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Preferences and content migration
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Preferencias y migración de contenido
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---


# Preferencias y migración de contenido

Esta página describe cómo migrar datos desde las preferencias y Shelf/Assets para utilizarlos en las nuevas versiones.

Después del lanzamiento de la versión 7.2, las preferencias y la ubicación de la estantería han cambiado para que sean comunes en las distintas versiones de la aplicación (Substance 3D independiente, Steam y Creative Cloud Desktop). Este cambio significa que las preferencias anteriores y los recursos personalizados **ahora se omiten** de forma predeterminada (**pero no se pierden**). Dado que **Shelf** ha pasado a llamarse **Assets**, la migración implica algunos pasos que se detallan a continuación.

## Migración de recursos de activos y plataformas

La ubicación de recursos del usuario predeterminado ha cambiado, lo que significa que cualquier contenido que se haya colocado en la carpeta Documentos ahora se omite en las nuevas versiones de la aplicación. Para restaurar este contenido, solo tiene que mover los archivos de una ubicación a la otra.

### Dónde encontrar el contenido

La ruta de estante o de recursos se puede encontrar en las siguientes ubicaciones:

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Platform</th><th>Versión</th><th>Ruta</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> o posterior</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Heredada</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="1">/Usuarios/nombre_usuario/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Heredada</td><td colspan="1">/Usuarios/nombre_usuario/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> o posterior</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Heredada</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

### Cómo migrar el contenido del estante

El contenido antiguo de Shelf son solo archivos en el disco, por lo que migrarlos solo se trata de colocar estos archivos en el lugar correcto.

1. Cierre la aplicación
1. Vaya a la antigua carpeta de estante
1. Copie o corte las subcarpetas (alfas, procedimientos, materiales, etc.)
1. Vaya a la nueva carpeta Activos
1. Pegue las subcarpetas que copió anteriormente dentro de la carpeta Activos y, si se le solicita, sobrescriba.

Ahora reinicie la aplicación, el contenido debe aparecer en la ventana Activos.

>[!NOTE]
>
> Asegúrese de copiar las subcarpetas y no sólo la carpeta principal de los recursos. Se ha cambiado el nombre de la carpeta principal de **shelf** a **assets**, por lo que copiar solo la carpeta principal no hará que los recursos estén visibles para la aplicación.

### Cómo migrar los ajustes preestablecidos de la estantería

Los ajustes preestablecidos de la estantería se guardan dentro de un archivo de configuración. Para migrar estos ajustes preestablecidos:

1. Cierre la aplicación
1. Vaya a la antigua carpeta de estante
1. Copie o corte el archivo Shelf.ini
1. Vaya a la nueva carpeta Activos
1. Pegue el archivo y sobrescriba el existente

Ahora reinicie la aplicación, las búsquedas guardadas deben aparecer en la sección dedicada o en la ventana Activos.

## Migración de preferencias

Se recomienda volver a ajustar manualmente la configuración de la aplicación desde la interfaz. Esta es la forma más segura de migrar la información sin introducir problemas de compatibilidad.

De lo contrario, consulte la página siguiente para saber dónde se encuentran ahora las preferencias: [Preferencias y ubicación de datos de la aplicación](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html).
