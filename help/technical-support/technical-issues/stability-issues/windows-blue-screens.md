---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/stability-issues/windows-blue-screens.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo evitar errores de pantalla azul de Windows al utilizar Substance 3D Painter para un funcionamiento estable del sistema.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Windows Blue Screens
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Windows Blue Screens
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---


# Windows Blue Screens

En Windows, las [Pantallas azules de la muerte (BSOD)](https://en.wikipedia.org/wiki/Blue_screen_of_death) suelen estar relacionadas con errores de hardware o controladores. Substance 3D Painter en sí no es responsable de esos BSOD, pero puede arrojar algo de luz sobre un problema con el propio ordenador debido a lo intensiva que es la aplicación. En el caso de Substance 3D Painter, se puede producir un BSOD debido a los siguientes problemas.

## Controladores de GPU inestables

Substance 3D Painter depende en gran medida de la GPU para realizar sus distintos cálculos. Los controladores de la GPU pueden ser a veces inestables o presentar regresiones. Se recomienda mantener la GPU actualizada para obtener las correcciones más recientes y las mejoras de rendimiento. Consulte: [La GPU tiene controladores obsoletos](../gpu-issues/gpu-has-outdated-drivers.md).

### Instalación inestable de Windows

Windows puede ser inestable después de algunas actualizaciones. Utilice las herramientas de diagnóstico proporcionadas con Windows para detectar cualquier error potencial en el sistema.

Se recomienda ejecutar **Administración y mantenimiento de imágenes de implementación** (DISM) y la herramienta **Comprobador de archivos del sistema** (SFC). DISM es útil para recuperar los archivos de reemplazo necesarios para SFC con el fin de corregir los archivos del sistema dañados o que faltan.

Ejecutando **DISM** :

1. Abra el **menú Inicio**
1. Buscar **símbolo del sistema**
1. **Haga clic con el botón derecho** en el resultado y elija &quot;**Ejecutar como administrador**&quot;
1. Escriba el comando siguiente :  **DISM /Online /Cleanup-Image /RestoreHealth**
1. Presione **Intro**

Ejecutando **SFC** :

1. Abra el **menú Inicio**
1. Buscar **símbolo del sistema**
1. **Haga clic con el botón derecho** en el resultado y elija &quot;**Ejecutar como administrador**&quot;
1. Escriba el comando siguiente :  **sfc /scannow**
1. Presione **Intro**

Reinicie el equipo después de ambos comandos para aplicar las actualizaciones.

Para obtener más información sobre este tema, consulte:  [Usar la herramienta Comprobador de archivos de sistema para reparar los archivos del sistema que faltan o que están dañados](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system)

### Falta de espacio en disco

Desde la introducción de [Texturas virtuales dispersas](../../../features/sparse-virtual-textures.md) en Substance 3D Painter, la aplicación ahora usa el disco para almacenar texturas en la memoria caché mientras trabaja. Si el sistema se queda sin espacio, esto puede llevar a inestabilidad.

Hay dos soluciones fáciles para este problema:

* Libere espacio en el disco para dejar más espacio en el sistema de caché.
* Mueva el directorio de caché a otra unidad con más espacio. Esta ubicación se puede cambiar entrando en la configuración principal de la aplicación, consulte la configuración [&#x200B; &quot;Archivos temporales&quot;](https://docs.substance3d.com/display/SPDOC/General) .

### Disco defectuoso (HDD o SSD)

Como se ha mencionado en el punto anterior, el sistema de caché depende en gran medida del disco. Si la unidad de disco es defectuosa, esto puede hacer que el sistema sea inestable al intentar escribir o leer datos.

Para detectar si un disco es defectuoso, puede ejecutar CHKDSK en Windows:

1. Abra el **menú de estrellas**
1. Seleccione **Equipo / Este equipo**
1. **Haga clic con el botón derecho** en el disco duro y elija **Propiedades.**
1. Cambie a la pestaña **Herramientas**.
1. Haga clic en **Comprobar / Comprobar ahora** en **Comprobación de errores** .

### Memoria defectuosa

Una memoria defectuosa (RAM) puede provocar inestabilidad en el sistema si un programa no puede leer o escribir en la memoria de forma segura. Para comprobar la integridad de la memoria, se recomienda ejecutar **MemTest**.

Consulte [esta guía](https://www.memtest86.com/technical.htm) sobre cómo instalar y usar MemTest.
