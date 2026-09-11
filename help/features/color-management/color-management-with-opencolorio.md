---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/color-management/color-management-with-opencolorio.html"
breadcrumb-title: ''
description: Aprenda a usar la gestión de color OpenColorIO en Substance 3D Painter para obtener flujos de trabajo de color uniformes entre canalizaciones.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with OpenColorIO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gestión de color con OpenColorIO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 8%

---


# Gestión de color con OpenColorIO

Esta página muestra la configuración de gestión de color relacionada con OpenColorIO (OCIO).

## Configuración del proyecto

![](../../assets/project-settings-3.png)

La configuración del proyecto se puede establecer al crear un nuevo proyecto mediante la ventana [nuevo proyecto](../../getting-started/project-creation.md) o mediante la ventana [configuración del proyecto](../../interface/project-configuration.md).

>[!NOTE]
>
> Si la variable de entorno **OCIO** está presente y especifica un archivo de configuración válido, anulará y deshabilitará la configuración en la interfaz de usuario.

Los ajustes disponibles son:

<table data-preserve-html="true" style="width: 99.9039%;"><colgroup><col style="width: 12.512%;"/><col style="width: 21.1742%;"/><col style="width: 66.3122%;"/></colgroup><tbody><tr><th style="width: 12.5%;">Sección</th><th style="width: 21.1538%;">Configuración</th><th style="width: 66.25%;">Descripción</th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>Configuración</strong></td><td style="width: 21.1538%;"><strong>Gestión de colores</strong></td><td style="width: 66.25%;"><p>Defina el motor que desea utilizar para administrar colores.</p><p>Valores posibles:</p><ul><li><strong>Heredado</strong> (predeterminado): Utilice la corrección de color de gamma sRGB/sRGB lineal predefinida.</li><li><strong>OpenColorIO</strong>: Utiliza OCIO integración.</li><li><strong>ACE de Adobe</strong>: Adobe Color Engine, para admitir perfiles ICC.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>Configuración de OpenColorIO</strong></td><td style="width: 66.25%;"><p>El archivo de configuración que se debe utilizar para controlar la configuración de gestión de color.</p><p>Valores posibles:</p><ul><li><strong>Substance</strong> (predeterminado): usa Gamma lineal como espacio de trabajo.</li><li><strong>ACE 1.0.3</strong>: utilice ACEScg como espacio de trabajo.</li><li><strong>ACE 1.2</strong>: utilice ACEScg como espacio de trabajo.</li><li><strong>Personalizado</strong>: utilice un fichero de configuración personalizado.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>Archivo de configuración</strong></td><td style="width: 66.25%;">Ruta de acceso al archivo de configuración de OCIO. Deshabilitado si el modo de configuración no está establecido en <strong>Personalizado</strong>.</td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="2" style="width: 12.5%;"><strong>Configuración de color</strong></td><td style="width: 21.1538%;"><strong>Espacio de color de trabajo</strong></td><td style="width: 66.25%;">Espacio de color utilizado por el motor para trabajar dentro de la aplicación. Es el espacio de color desde el que se pueden convertir las texturas (importar) o desde (exportar).</td></tr><tr><td colspan="1"><strong>Espacio de color sRGB estándar</strong></td><td colspan="1"><p>El espacio de color que coincide con el espacio de color [estándar sRGB](https://en.wikipedia.org/wiki/SRGB) (IEC 61966-2-1:1999).</p><p>Este espacio de color se utiliza en varios lugares dentro de la aplicación:</p><ul><li>Para convertir un conjunto de colores en el campo hexadecimal del selector de color.</li><li>Para guardar y cargar muestras de color en el selector de color.</li><li>Para que aparezca como Pantalla en la lista del selector de color.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="4" style="width: 12.5%;"><strong>Valores predeterminados del espacio de color de importación de mapa de bits</strong></td><td style="width: 21.1538%;"><strong>Imágenes de 8 bits</strong></td><td style="width: 66.25%;">Espacio de color que se utiliza de forma predeterminada al importar archivos de imagen de 8 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Imágenes de 16 bits</strong></td><td style="width: 66.25%;">Espacio de color que se utiliza de forma predeterminada al importar archivos de imagen de 16 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Imágenes de punto flotante</strong></td><td style="width: 66.25%;">Espacio de color que se utiliza de forma predeterminada al importar archivos de imagen HDR./EXR.</td></tr><tr><td style="width: 21.1538%;"><strong>Detección autom. de espacios de color</strong></td><td style="width: 66.25%;"><p>Permite definir el espacio de color de los recursos en función de ajustes específicos.</p><p>Valores posibles:</p><ul><li><strong>Deshabilitado</strong>: para utilizar la configuración de color predeterminada, omita la configuración de recursos.</li><li><strong>Analizar nombre de archivo</strong> (predeterminado): utilice OCIO [convención de nomenclatura](https://opencolorio.readthedocs.io/en/latest/guides/authoring/rules.html?highlight=filename#strictparsing) para extraer el nombre del espacio de color utilizado por el recurso.</li><li><strong>Usar reglas de archivos de configuración</strong>: utilice la configuración OCIO para determinar cómo asignar espacios de color. Este parámetro tiene prioridad sobre la configuración anterior del espacio de color del archivo de imagen.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td style="width: 12.5%;"><strong>material de Substance</strong></td><td style="width: 21.1538%;"><strong>Valor predet. del espacio de color de material</strong></td><td style="width: 66.25%;"><p>Defina el espacio de color que se debe utilizar para los materiales de Substance con entrada/salida con gestión de color (consulte a continuación la lista de canales).</p></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>Exportar espacios de color</strong><br/><br/><br/></td><td style="width: 21.1538%;"><strong>Imágenes de 8 bits</strong></td><td style="width: 66.25%;">Espacio de color que se utiliza de forma predeterminada al exportar archivos de imagen de 8 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Imágenes de 16 bits</strong></td><td style="width: 66.25%;">Espacio de color que se utiliza de forma predeterminada al exportar archivos de imagen de 16 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Imágenes de punto flotante</strong></td><td style="width: 66.25%;">Espacio de color que se utiliza de forma predeterminada al exportar archivos de imagen HDR./EXR.</td></tr></tbody></table>

### OpenColorIO roles

Las siguientes funciones son compatibles y permiten cambiar la selección predeterminada de espacios de color:

| Nombre de función | Descripción |
| --- | --- |
| **substance\_3d\_painter\_standard\_srgb** | Función para especificar el espacio de color que coincide con el estándar [sRGB](https://en.wikipedia.org/wiki/SRGB) (IEC 61966-2-1:1999). |
| **substance\_3d\_painter\_bitmap\_import\_8bit** | Función para especificar el espacio de color utilizado para importar imágenes de 8 bits. |
| **substance\_3d\_painter\_bitmap\_import\_16bit** | Función para especificar el espacio de color utilizado para importar imágenes de 16 bits. |
| **substance\_3d\_painter\_bitmap\_import\_floating** | Función para especificar el espacio de color utilizado para importar imágenes HDR. |
| **substance\_3d\_painter\_substance\_material** | Función para especificar el espacio de color utilizado para los canales con gestión de color en materiales de Substance. |
| **substance\_3d\_painter\_bitmap\_export\_8bit** | Función para especificar el espacio de color utilizado al exportar texturas de 8 bits. |
| **substance\_3d\_painter\_bitmap\_export\_16bit** | Función para especificar el espacio de color utilizado al exportar texturas de 16 bits. |
| **substance\_3d\_painter\_bitmap\_export\_floating** | Función para especificar el espacio de color utilizado al exportar texturas HDR. |

>[!NOTE]
>
> Las configuraciones OCIO proporcionadas con la aplicación se pueden utilizar como ejemplos sobre cómo utilizar estas funciones específicas.
