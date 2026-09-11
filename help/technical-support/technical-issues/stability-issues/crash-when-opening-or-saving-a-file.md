---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-when-opening-or-saving-a-file.html"
breadcrumb-title: ''
description: Aprenda a corregir bloqueos de Substance 3D Painter al abrir o guardar archivos para una administración de proyectos fiable.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash when opening or saving a file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bloqueo al abrir o guardar un archivo
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# Bloqueo al abrir o guardar un archivo

Hay algunas razones por las que Substance 3D Painter se bloqueo en Windows al abrir un cuadro de diálogo de archivo. Esta página reagrupa los motivos y las soluciones a este problema.

## Conflictos de software

Algunos programas pueden agregar extensiones de shell personalizadas que pueden conducir a inestabilidades o bloqueos. Consulta la lista de [conflictos de software](../startup-issues/software-conflicts.md) para obtener más información.

## Extensiones de shell/temas personalizados

Los temas personalizados no son compatibles con nuestro entorno gráfico de usuario, por lo que se recomienda desinstalar el tema actual antes de utilizar Substance 3D Painter.

Los equipos **Alienware** / **Dell** integran de forma predeterminada algunas extensiones de shell que se sabe que son incompatibles con Substance 3D Painter. Se recomienda desinstalarlos. Aunque no conocemos exactamente todas las extensiones que son incompatibles, la mayoría de las veces corresponden a:

* DBROverlayIconBackuped.DBROverlayIconBackuped (Clase)
* DBROverlayIconNotBackuped.DBROverlayIconNotBackuped (Clase)

Puede ver qué extensiones están instaladas en el equipo mediante la herramienta siguiente. A continuación se muestra un procedimiento aproximado sobre cómo proceder:

1. Descargue e instale ShellExView desde NirSoft: <http://www.nirsoft.net/utils/shexview.html>
1. Ejecutar el programa
1. Haz clic en **Opción** y elige **Filtrar por tipo de extensión**
1. Seleccione **Controlador de superposición de iconos**
1. Debería ver las dos entradas de **Alien Respawn** .
1. Seleccione **both** y haga clic en el botón rojo para deshabilitarlos.
