---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/license-issues/maintenance-is-expired-dialog-on-startup.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo resolver el cuadro de diálogo de mantenimiento caducado que aparece al iniciar Substance 3D Painter para la administración de licencias.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > License Issues > Maintenance is expired dialog on startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Cuadro de diálogo Mantenimiento caducado al inicio
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---


# Cuadro de diálogo Mantenimiento caducado al inicio

![](../../../assets/expired-mainteance-message.png)

Al iniciar la aplicación, puede aparecer un cuadro de diálogo con el mensaje &quot;Su mantenimiento actual ha caducado&quot;. Esta página muestra soluciones para evitar este cuadro de diálogo.

## Solución 1: actualizar el archivo de licencia

El mensaje de advertencia aparece porque el archivo de licencia es demasiado antiguo y debe actualizarse. Para ello, basta con **reactivar el producto** mediante el asistente de aplicaciones. El archivo de licencia también se puede descargar manualmente a través del sitio web de Substance 3D: <https://www.substance3d.com/>.

## Solución 2: edite la configuración de preferencias para ocultar el cuadro de diálogo

>[!NOTE]
>
> Se recomienda intentar actualizar el archivo de licencia antes de utilizar esta solución alternativa.

Otra solución es ocultar el mensaje de advertencia estableciendo una configuración específica.

Vaya a la ubicación de preferencias de la aplicación:

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>Sistema</th><th>Versión</th><th>Ruta</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>(Registro)</p></td><td><strong>7.2</strong> o posterior</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>Heredada</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>(biblioteca)</p></td><td><strong>7.2</strong> o posterior</td><td>/Usuarios/[nombre de usuario]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>Heredada</td><td>/Usuarios/[nombre de usuario]/Library/Preferences/com.substance3d.Substance Painter.plist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td><strong>7.2</strong> o posterior</td><td>/home/[nombre de usuario]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>Heredada</td><td>/home/[nombre de usuario]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

### Windows

Para definir la variable en Windows, siga estos pasos:

1. Abra el menú Inicio.
1. Busque **Regedit** para abrir el editor del Registro.
1. Vaya a la clave del Registro que aparece en la tabla anterior.
1. Haga clic en la clave del Registro denominada como software en la vista de árbol de la izquierda.
1. Haga clic con el botón derecho en el área vacía del panel derecho y elija **Nuevo > Valor de cadena**.
1. Asigne al nuevo valor el nombre **DisableLicenseWarningPopup** y presione Intro para validar.
1. Haga doble clic en el valor que acaba de crear.
1. Defina el campo Datos del valor en: **true**
1. Guarde el cambio.
1. Inicie la aplicación.

### MacOS

1. Abra una nueva ventana de **Finder**
1. Desplácese a la ruta que aparece en la tabla anterior.
1. Haga clic con el botón derecho en el archivo **plist** y elija **Abrir con > Xcode**.
1. En la parte superior de la lista, agregue una nueva clave denominada **DisableLicenseWarningPopup**
1. Establezca el tipo de clave en **cadena**
1. Establezca el valor de clave en **true**
1. Guarde y cierre el archivo.
1. Inicie la aplicación.

### Linux

Para definir la variable en Linux, siga estos pasos:

1. Vaya a la lista de rutas de la tabla anterior.
1. Abra el archivo **.conf** que se encuentra en la carpeta.
1. Agregue una nueva línea bajo la línea **[General]**
1. En la nueva línea, pegue el texto siguiente: **DisableLicenseWarningPopup=true**
1. Guarde el archivo.
1. Inicie la aplicación.
