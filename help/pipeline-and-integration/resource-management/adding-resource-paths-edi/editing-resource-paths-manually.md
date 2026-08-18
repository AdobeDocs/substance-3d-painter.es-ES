---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/adding-resource-paths-by-editing-preferences-manually/editing-resource-paths-manually.html"
breadcrumb-title: ''
description: Aprenda a editar manualmente las rutas de acceso de recursos en las preferencias de Substance 3D Painter para personalizar las ubicaciones de recursos de estantería.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding resource paths by editing preferences manually > Editing resource paths manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Edición manual de rutas de recursos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 1%

---


# Edición manual de rutas de recursos

Esta página es una guía sobre cómo editar las preferencias para añadir o eliminar rutas de recursos sin iniciar la aplicación.

## Ubicación de preferencias

Las ubicaciones de recursos se administran con las preferencias de la aplicación, que pueden cambiar según la plataforma:

<table data-preserve-html="true"> <colgroup> <col/> <col/> <col/> </colgroup> <tbody> <tr> <th>Sistema</th> <th>Versión</th> <th>Ruta</th> </tr> <tr> <td rowspan="2"><p><strong>Windows</strong></p><p>(Registro)</p></td> <td><strong>7.2</strong> o posterior</td> <td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td>Heredada</td> <td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><p><strong>Mac</strong></p><p>(biblioteca)</p></td> <td><strong>7.2</strong> o posterior</td> <td>/Usuarios/[nombre de usuario]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td> </tr> <tr> <td>Heredada</td> <td>/Usuarios/[nombre de usuario]/Library/Preferences/com.substance3d.Substance Painter.plist</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td><strong>7.2</strong> o posterior</td> <td>/home/[nombre de usuario]/.config/Adobe/Adobe Substance 3D Painter.conf</td> </tr> <tr> <td>Heredada</td> <td>/home/[nombre de usuario]/.config/Allegorithmic/Substance Painter.conf</td> </tr> </tbody> </table>

## Adición de una ruta en Windows

En Windows, las rutas se pueden administrar a través del Registro de Windows:

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/reg-shelf-pathinfos.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/reg-content.png)

</td>
</tr>
</table>

1. Haga clic en **Inicio > Ejecutar** o pulse **Windows + R** .
1. Escriba &quot;**regedit**&quot; (sin las comillas) en el cuadro de diálogo y pulse **Aceptar**.
1. Navegue en la vista de árbol a la izquierda de la ventana **Editor del Registro** y vaya a la clave del Registro mencionada anteriormente.
1. **Agrega una clave** debajo de **pathInfos** con un **número** como nombre. Aumente el número en función de las claves existentes (a partir de 1).
1. Haga **clic con el botón derecho del ratón** > **new** > **Valor de cadena** en la parte derecha de la ventana. Asígnele el nombre **disabled** y establezca el valor en **false**.
1. Haga **clic con el botón derecho del ratón** > **new** > **Valor de cadena** en la parte derecha de la ventana. Asígnele el nombre **name** e introduzca el nombre del estante personalizado.
1. Haga **clic con el botón derecho del ratón** > **new** > **Valor de cadena** en la parte derecha de la ventana. Asígnele el nombre **path** y establezca el valor en path donde se encuentra el estante.
1. No olvide incrementar en 1 la clave &quot;**size**&quot; dentro de &quot;**pathInfos**&quot;.
1. Cierre la ventana.
1. Inicie la aplicación.

Es posible definir la nueva ruta de acceso como la predeterminada (donde se crean nuevos recursos, como los ajustes preestablecidos) cambiando el valor de la entrada **writableShelf** por el nombre de la nueva ubicación.

![](../../../assets/default-shelf.png)

## Adición de una ruta en Linux

En **Linux** se pueden crear rutas adicionales a través del archivo de configuración de preferencias de la aplicación del usuario, almacenado en el directorio principal (consulte.

1. Vaya a la ruta mencionada anteriormente.
1. Abra el archivo **Substance 3D Painter.config**
1. Desplácese hacia abajo hasta la sección **[Shelf]**

Añada una nueva ruta de estante incrementando el último número visible, por ejemplo:

```
pathInfos2disabled=false  

pathInfos2name=custom_resources 

pathInfos2path=/home/Username/Documents/custom_path 

writableShelf=custom_resources
```


Use la variable **writableShelf** para especificar qué ruta será la predeterminada (donde se crean nuevos recursos, como los ajustes preestablecidos).

Guarde los cambios y reinicie la aplicación.
