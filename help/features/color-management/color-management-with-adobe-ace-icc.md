---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/color-management/color-management-with-adobe-ace-icc.html"
breadcrumb-title: ''
description: Aprenda a utilizar la gestión de color ICC y de ACE de Adobe en Substance 3D Painter para obtener flujos de trabajo de color coherentes.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with Adobe ACE - ICC
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gestión de color con Adobe ACE - ICC
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Gestión de color con Adobe ACE - ICC

Esta página muestra la configuración de gestión de color relacionada con el Adobe Color Engine (ACE) para utilizar la imagen con perfiles ICC.

## Configuración del proyecto

![](../../assets/cm-ace.png)

La configuración del proyecto se puede establecer al crear un nuevo proyecto mediante la ventana [nuevo proyecto](../../getting-started/project-creation.md) o mediante la ventana [configuración del proyecto](../../interface/project-configuration.md).

>[!NOTE]
>
> Si se carga una variable de entorno (véase a continuación) o un archivo de ajustes preestablecidos, se desactivará la configuración de la interfaz de usuario.

Los ajustes disponibles son:

| Sección | Configuración | Descripción |
| --- | --- | --- |
| **Configuración** | **Administración de color** | Defina el motor que desea utilizar para administrar colores.Valores posibles:<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>Heredado</strong> (predeterminado): Utilice la corrección de color de gamma sRGB/sRGB lineal predefinida.</li> <li data-preserve-html="true"><strong>OpenColorIO</strong>: Utiliza OCIO integración.</li> <li data-preserve-html="true"><strong>ACE de Adobe</strong>: Adobe Color Engine, para admitir perfiles ICC.</li> </ul> |
|  | **Usar un archivo de ajuste preestablecido** | Si está activado, permita que se activen los ajustes de gestión de color a través de un archivo de configuración de json. |
|  | **Archivo de ajustes preestablecidos** | Ruta al archivo preestablecido, en formato json. Para obtener más información, consulte a continuación. |
|  |  |  |
| **Configuración de color** | **Espacio de color de trabajo** | Espacio de color utilizado por el motor para trabajar dentro de la aplicación. Éste es el espacio de color desde el que las texturas se pueden convertir a (importar) o desde (exportar).Los valores posibles son:<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>sRGB lineal IEC61966-2.1</strong> (predeterminado)</li> <li data-preserve-html="true"><strong>ACEScg ACE Espacio de trabajo AMPAS S-2014-004</strong></li> <li data-preserve-html="true"><strong>Lineal Adobe RGB (1998)</strong></li> </ul> |
|  | **Intento de renderizado** | Especifique el método utilizado para convertir el color entre espacios de color.Valores posibles:<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>Perceptual</strong></li> <li data-preserve-html="true"><strong>Saturación</strong> (predeterminado)</li> <li data-preserve-html="true"><strong>Cromático relativo</strong></li> <li data-preserve-html="true"><strong>Cromático absoluto</strong></li> </ul> |
|  |  |  |
| **Valores predeterminados del espacio de color de importación de mapa de bits** | **imágenes de 8 bits** | Espacio de color que se utiliza de forma predeterminada al importar archivos de imagen de 8 bits. |
|  | **imágenes de 16 bits** | Espacio de color que se utiliza de forma predeterminada al importar archivos de imagen de 16 bits. |
|  | **Imágenes de punto flotante** | Espacio de color que se utiliza de forma predeterminada al importar archivos de imagen HDR./EXR. |
|  | **Usar perfiles ICC incrustados cuando estén disponibles (recomendado)** | Si está activada, utilice los perfiles ICC desde el archivo de imagen para ajustar sus colores. |
|  |  |  |
| **Material del Substance** | **Espacio de color de material predeterminado** | Defina el espacio de color que se debe utilizar para los materiales de Substance con entrada/salida con gestión de color. |
|  |  |  |
| **Exportar espacio de color** | **imágenes de 8 bits** | Espacio de color que se utiliza de forma predeterminada al exportar archivos de imagen de 8 bits. |
|  | **imágenes de 16 bits** | Espacio de color que se utiliza de forma predeterminada al exportar archivos de imagen de 16 bits. |
|  | **Imágenes de punto flotante** | Espacio de color que se utiliza de forma predeterminada al exportar archivos de imagen HDR./EXR. |

## Uso de un archivo de ajustes preestablecidos

![](../../assets/cm-ace-env-var.png)

Es posible utilizar un archivo de ajustes preestablecidos (en formato json) para controlar la configuración de ACE al crear nuevos proyectos.

### Variable de entorno

La variable de entorno **PAINTER\_ACE\_CONFIG** se puede usar para especificar la ruta de un archivo de ajuste preestablecido. Si está presente, la aplicación siempre utilizará un archivo de ajustes preestablecidos para controlar la configuración de gestión de color. La configuración se deshabilitará en la interfaz.

Para obtener más información, consulte la página [Variables de entorno](../../pipeline-and-integration/configuration/environment-variables.md).

### Ejemplo preestablecido

A continuación se muestra un ejemplo de un archivo json que se puede utilizar como archivo de ajustes preestablecidos:

```
{ 

  "color settings": { 

    "working color space": "Linear Adobe RGB (1998)", 

    "rendering intent": "Saturation" 

  }, 

  "bitmap import color space defaults" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw", 

    "use embedded ICC profiles when available": false 

  }, 

  "substance material": { 

    "material color space default": "image P3" 

  }, 

  "export colors spaces" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw" 

  } 

} 
```
