---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/interface/settings/libraries-configuration.html"
breadcrumb-title: ''
description: Aprenda a configurar bibliotecas en la configuración de Substance 3D Painter para administrar rutas de recursos y organización de recursos.
helpx_creative_field: ""
helpx_description: Painter > Interface > Settings > Libraries configuration
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configuración de bibliotecas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 1%

---


# Configuración de bibliotecas

![](../../assets/settings-libraries.png)

Esta sección permite especificar rutas de acceso personalizadas a carpetas de recursos adicionales y en qué ubicación deben guardarse los recursos de forma predeterminada.

## Rutas predeterminadas

De forma predeterminada, se predefinen dos rutas:

| Nombre | Ubicación |
| --- | --- |
| **tus\_assets** | Esta ruta se encuentra en la carpeta Documentos del perfil de usuario actual. Aquí es donde los recursos, como los ajustes preestablecidos, se crean de forma predeterminada desde la aplicación. (Se denomina &quot;estantería&quot; en las versiones anteriores). |
| **starter\_assets** | Esta ruta se encuentra en la carpeta de instalación de la aplicación. Contiene los recursos predeterminados. (Se denomina &quot;alegorithmic&quot; o &quot;substance&quot; en versiones anteriores). |

El botón de opción **default** se utiliza para definir en qué ruta se guardará el nuevo contenido (como los ajustes preestablecidos de pincel, los ajustes preestablecidos de material o los Materiales inteligentes).

## Adición de una nueva ruta

>[!NOTE]
>
> Sólo se puede crear o modificar una ruta de acceso si no hay ningún proyecto abierto.

| Configuración | Descripción |
| --- | --- |
| **Nombre** | Nombre que se utilizará para hacer referencia a la ruta de la interfaz (por ejemplo, al hacer clic con el botón secundario en un recurso). Este nombre también define el nombre de la ubicación interna para que los recursos realicen un seguimiento si están actualizados o no, por lo que se recomienda no cambiar este nombre una vez definido. |
| **Ruta** | Ubicación real donde se encuentran (o estarán) los recursos en el disco. |
| **Botón de signo más**  <div><img data-preserve-html="true" src="../../assets/shelf-button.png" width="30"/></div> | Al hacer clic en este botón, se añadirá la ruta definida por el nombre y la configuración de la ruta a la lista siguiente.Al agregar una nueva ruta, se creará automáticamente la estructura de subcarpetas necesaria para organizar los datos y los recursos. Para saber dónde colocar los recursos, consulte:  [Agregando contenido al estante](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/adding-content-to-the-shelf-142213317.html). |
| **Botón menos**   <div><img data-preserve-html="true" src="../../assets/shelf-remove.png" width="30"/></div> | Al hacer clic en este botón delante de un trazado, se eliminará de la lista. Los recursos ya no se mostrarán en la interfaz de [Assets](../assets/assets.md).  **Nota:** Las rutas predeterminadas no se pueden quitar, pero se deshabilitarán y sus recursos se ocultarán en su lugar. |
