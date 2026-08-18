---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/adding-resource-paths-by-editing-preferences-manually/editing-the-shelf-preferences-with-python.html"
breadcrumb-title: ''
description: Aprenda a editar las preferencias de estantería utilizando la creación de scripts de Python en Substance 3D Painter para la gestión automatizada de rutas de recursos.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding resource paths by editing preferences manually > Edit Shelf Preferences with Python
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Editar preferencias de la estantería con Python
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 2%

---


# Edición de las preferencias de la estantería con Python

A continuación se muestran ejemplos de secuencias de comandos de Python para modificar el Registro de Windows y manipular las rutas de acceso de recursos.

## Ruta de la clave del Registro

Consulte la siguiente tabla para utilizar la ruta de acceso de la clave del Registro correspondiente:

<table data-preserve-html="true"> <colgroup> <col/> <col/> <col/> </colgroup> <tbody> <tr> <th>Sistema</th> <th>Versión</th> <th>Ruta</th> </tr> <tr> <td rowspan="2"><p><strong>Windows</strong></p><p>(Registro)</p></td> <td><strong>7.2</strong> o posterior</td> <td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td>Heredada</td> <td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><p><strong>Mac</strong></p><p>(biblioteca)</p></td> <td><strong>7.2</strong> o posterior</td> <td>/Usuarios/[nombre de usuario]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td> </tr> <tr> <td>Heredada</td> <td>/Usuarios/[nombre de usuario]/Library/Preferences/com.substance3d.Substance Painter.plist</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td><strong>7.2</strong> o posterior</td> <td>/home/[nombre de usuario]/.config/Adobe/Adobe Substance 3D Painter.conf</td> </tr> <tr> <td>Heredada</td> <td>/home/[nombre de usuario]/.config/Allegorithmic/Substance Painter.conf</td> </tr> </tbody> </table>

## Adición de una nueva ruta

Agregar una ruta de acceso de recurso requiere comprobar cuál ya existe para incrementar la lista con una nueva.

El código siguiente agrega en la clave del Registro una nueva ruta de acceso de almacenamiento después de comprobar cuál es el número actual de ruta de acceso ya definida.

>[!NOTE]
>
> Es posible que la subclave **Shelf** (junto a **pathInfos**) no esté presente en el Registro. Para que aparezca, inicie la aplicación, abra las preferencias (Editar > Configuración) y, a continuación, haga clic en Aceptar y cierre la aplicación.

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

 

ShelfName = "myshelf" #Needs to be lowercase 

ShelfPath = "C:/Temp" 

ShelfStatus = "false" #false = not disabled 

 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

  

## Open parent registry key

Key = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ  ) 

 

## Iterate over each sub-key to retrieve the biggest Shelf number

SubKeyCount = winreg.QueryInfoKey( Key )[0] 

ShelfNumber = 0 

 

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 ShelfNumber = max( ShelfNumber, int(SubKeyName) ) 

 

ShelfNumber += 1 

 

## Create the new Key and add its values

NewKey = winreg.CreateKey( Key, str( ShelfNumber ) ) 

 

winreg.SetValueEx( NewKey, "disabled", 0, winreg.REG_SZ, ShelfStatus) 

winreg.SetValueEx( NewKey, "name", 0, winreg.REG_SZ, ShelfName) 

winreg.SetValueEx( NewKey, "path", 0, winreg.REG_SZ, ShelfPath) 

 

NewKey.Close() 

 

## Increment the Shelf path counter

Count = winreg.QueryValueEx( Key, "size" ) 

Key.Close() 

 

Key = winreg.OpenKeyEx( RegConnection, RegistryKeyName, 0, winreg.KEY_SET_VALUE  ) 

winreg.SetValueEx( Key, "size", 0, winreg.REG_DWORD, Count[0] + 1 ) 

Key.Close()
```


## Deshabilitar o habilitar una ruta de acceso de recursos

Cualquier ruta creada puede ser eliminada cuando ya no sea necesaria, pero también deshabilitada para la ruta predeterminada que no puede ser eliminada por completo.

El siguiente código analiza el Registro de Windows y deshabilita el espacio de almacenamiento predeterminado (denominado &quot;starter\_assets&quot;).

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

 

## Open registry key

Key    = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ ) 

SubKeyCount  = winreg.QueryInfoKey( Key )[0] 

 

## Iterate over each sub-key

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 SubKey = winreg.OpenKey( 

  RegConnection, 

  RegistryKeyName + "\" + SubKeyName, 

  winreg.KEY_READ ) 

 SubKeyValueCount = winreg.QueryInfoKey( SubKey )[1] 

 

## Read subkey values

 Values = [] 

 for i in range( SubKeyValueCount ) : 

  Values.append( winreg.EnumValue( SubKey, i ) ) 

 

## Note : Values is a table of tuples

 FoundKey = False 

 for Value in Values : 

  if Value[0] == "name" : 

   if Value[1] == "starter_assets" : 

    FoundKey = True 

 

 SubKey.Close() 

 

## Found the path ? Then we edit the Key

 if FoundKey : 

  print( " - Editing Windows Registry" ) 

 

## Re-Open key in edition mode

  SubKey  = winreg.OpenKey(   

   winreg.HKEY_CURRENT_USER, 

   RegistryKeyName + "\" + SubKeyName, 

   0, 

   winreg.KEY_SET_VALUE ) 

 

## Assign new value

  winreg.SetValueEx(SubKey, "disabled", 0, 1, "true" ) #use "false" to Enable that shelf path 

 

  SubKey.Close() 

 

## Finish

Key.Close()
```
