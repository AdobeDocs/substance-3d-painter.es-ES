---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/scripts-and-plugins/creating-a-javascript-plugin.html"
breadcrumb-title: ''
description: Aprenda a crear complementos de JavaScript para Substance 3D Painter para ampliar la funcionalidad y automatizar los flujos de trabajo personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Creating a Javascript plugin
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Creación de un complemento de Javascript
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 1%

---


# Creación de un complemento de Javascript

Esta guía paso a paso describe cómo crear un plugin simple que permite exportar la máscara de la capa seleccionada actualmente en un proyecto.

El objetivo del plugin de esta guía es exportar todos los canales del conjunto de texturas actual dentro de un proyecto como texturas individuales.

## 1 - Ir a la carpeta de complementos

Para añadir un nuevo plugin de Javascript, debe crearse una carpeta en la carpeta de plugins de Substance 3D Painter.

Para tener acceso a la carpeta **plugins**, vaya a:

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>Platform</th> <th>Versión</th> <th>Ruta</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong> o posterior</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Heredada</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong> o posterior</td> <td colspan="1">/Usuarios/nombre_usuario/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Heredada</td> <td colspan="1">/Usuarios/nombre_usuario/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td colspan="1"><strong>7.2</strong> o posterior</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>Heredada</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

### 2 - Crear la carpeta del complemento

El nombre de un complemento se basa en el nombre de su carpeta principal.

Para este ejemplo, solo tiene que crear una nueva carpeta denominada **export-texturas** dentro de la carpeta plugins.

### 3 - Creación de los archivos del plugin

Abra la carpeta recién creada y cree dos archivos de texto vacíos (bloc de notas):

* **main.qml**
* **toolbar.qml**

La extensión de archivo qml es una extensión de Javascript para scripts creados para el lenguaje QML Qt. Permite ejecutar código JavaScript pero también crear interfaces de usuario personalizadas.

El archivo **main.qml** es obligatorio; es el primer archivo que buscará la aplicación para cargar el complemento. Sin embargo, se pueden crear archivos adicionales con cualquier nombre, lo que permite dividir un script en partes para facilitar la administración. En este caso, **toolbar.qml** se usará para describir el aspecto de un botón que el complemento agregará a la interfaz.

### 4 - Contenido de script

Abra los archivos de script en un editor de texto como el Bloc de notas++ y pegue los siguientes fragmentos de código. Eche un vistazo a los comentarios del código para obtener más detalles.

**toolbar.qml**

```
import QtQuick 2.7 

import AlgWidgets 2.0 

import AlgWidgets.Style 2.0 

 

AlgButton 

{ 

 tooltip: "" 

 iconName: "" 

 text: "Export Textures" 

}
```


**main.qml**

```
// Default includes, to acces Qt/QML 

// and Substance 3D Painter APIs 

import QtQuick 2.7 

import Painter 1.0 

 

// Root object for the plugin 

PainterPlugin 

{ 

 // Disable update and server settings 

 // since we don't need them 

 tickIntervalMS: -1 // Disabled Tick 

 jsonServerPort: -1 // Disabled JSON server 

 

 // Implement the OnCompleted function 

 // This event is used to build the UI 

 // once the plugin as been loaded by Substance 3D Painter 

 Component.onCompleted: 

 { 

  // Create a toolbar button 

  var InterfaceButton = alg.ui.addToolBarWidget("toolbar.qml"); 

 

  // Connect the function to the button 

  if( InterfaceButton ) 

  { 

   InterfaceButton.clicked.connect( exportTextures ); 

  } 

 } 

 

 // Custom function called by the Button, 

 // this is the core of the plugin 

 function exportTextures() 

 { 

  // Catch errors in the script during execution 

  try 

  { 

   // Verify if a project is open before  

   // trying to export something 

   if( !alg.project.isOpen() ) 

   { 

    return; 

   } 

 

   // Retrieve the currently selected Texture Set (and sub-stack if any) 

   var MaterialPath = alg.texturesets.getActiveTextureSet() 

   var UseMaterialLayering = MaterialPath.length > 1 

   var TextureSetName = MaterialPath[0] 

   var StackName = "" 

 

   if( UseMaterialLayering ) 

   { 

    StackName = MaterialPath[1] 

   } 

 

   // Retrieve the Texture Set information 

   var Documents = alg.mapexport.documentStructure() 

   var Resolution = alg.mapexport.textureSetResolution( TextureSetName ) 

   var Channels = null 

 

   for( var Index in Documents.materials ) 

   { 

    var Material = Documents.materials[Index] 

 

    if( TextureSetName == Material.name ) 

    { 

     for( var SubIndex in Material.stacks ) 

     { 

      if( StackName == Material.stacks[SubIndex].name ) 

      { 

       Channels = Material.stacks[SubIndex].channels 

       break 

      } 

     } 

    } 

   } 

 

   // Create the export settings 

   var Settings = { 

    "padding":"Infinite", 

    "dithering":"disbaled", // Hem, yes... 

    "resolution": Resolution, 

    "bitDepth": 16, 

    "keepAlpha": false 

   } 

 

   // Build the base of the export path 

   // Files will be located next to the project 

   var BasePath = alg.fileIO.urlToLocalFile( alg.project.url() ) 

   BasePath = BasePath.substring( 0, BasePath.lastIndexOf("/") ); 

 

   // Export the each channel 

   for( var Index in Channels ) 

   { 

    // Create the stack path, which defines the channel to export 

    var Path = Array.from( MaterialPath ) 

    Path.push( Channels[Index] ) 

 

    // Build the filename for the texture to export 

    var Filename = BasePath + "/" + TextureSetName 

 

    if( UseMaterialLayering ) 

    { 

     Filename += "_" + StackName 

    } 

 

    Filename += "_" + Channels[Index] + ".png" 

 

    // Perform the export 

    alg.mapexport.save( Path, Filename, Settings ) 

    alg.log.info( "Exported: " + Filename ) 

   } 

  } 

  catch( error ) 

  { 

   // Print errors in the log window 

   alg.log.exception( error ) 

  } 

 } 

} 
```


Una vez hecho esto, guarde y cierre el archivo.

### 5 - Carga y habilitación del plugin

Inicie Substance 3D Painter; de forma predeterminada, los nuevos complementos se cargan y habilitan automáticamente.

Abra un proyecto y haga clic en el botón de interfaz de usuario creado por el plugin para exportar los canales del conjunto de texturas seleccionado actualmente:

![](../../assets/button-plugin.png)

Para activar o desactivar un complemento, utilice el menú JavaScript situado en la parte superior de la interfaz:

![](../../assets/disable-plugin.png)
