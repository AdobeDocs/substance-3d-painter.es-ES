---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/auto-update.html"
breadcrumb-title: ''
description: Aprenda a utilizar la actualización automática de recursos en Substance 3D Painter para mantener sus bibliotecas de recursos sincronizadas y actualizadas.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Actualización automática de recursos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---


# Actualización automática de recursos

![](../assets/banner_autoupdate.jpg)

La actualización automática de recursos, o <b>actualización automática</b>, es una característica de la [ventana Activos](../interface/assets/assets.md) que permite volver a cargar y actualizar los recursos cuando hay nuevas versiones disponibles. Este proceso se puede activar automática o manualmente en la interfaz, o mediante scripts de Python.

![](../assets/auto_update_menu.png)

## Tutorial

Puede ver un tutorial rápido para obtener una descripción general de la función:

## Activación de la actualización automática

![](../assets/auto_update_red_icon.png)

Para habilitar la <b>actualización automática</b>, simplemente ve a la parte inferior de la ventana Activos y haz clic en el icono de las flechas dobles. Se abrirá el menú de actualización automática con todos sus ajustes. A continuación, habilita una de las opciones disponibles en la sección <b>actualizaciones automáticas</b>.

### Actualizaciones automáticas

![](../assets/auto-update_auto_settings.png)

La configuración de las actualizaciones automáticas controla la frecuencia con la que la aplicación debe buscar actualizaciones y dónde.

| Configuración | Descripción |
| --- | --- |
| <b>Panel de activos</b> | Si se habilita, la actualización automática buscará activos para actualizar en todas las bibliotecas cargadas actualmente. Esto incluye el proyecto actual. Sin embargo, no actualizará los recursos utilizados en la pila de capas, la configuración de visualización, la configuración de sombreador, etc. |
| <b>Recursos utilizados en el proyecto</b> | Si está activada, la actualización automática buscará los activos que se van a actualizar y que el proyecto actual importa y utiliza actualmente. Esto se aplica a los recursos utilizados en la pila de capas, la configuración de visualización, la configuración de sombreador, etc. |
| <b>Actualizar cada x minutos</b> | Controlar la frecuencia con la que la aplicación busca una actualización de los recursos. Un retraso de 0 minutos activará una actualización cada pocos segundos. Tenga en cuenta que un retraso tan bajo puede crear problemas de rendimiento. |

>[!NOTE]
>
> Si las actualizaciones automáticas están habilitadas, la aplicación buscará automáticamente los cambios cada vez que vuelva a estar seleccionada.

### Actualizaciones manuales

![](../assets/auto-update_manual.png)

Las acciones de actualización manual son una forma cómoda de activar el sistema de actualización cuando se desee. Se pueden utilizar con o sin la configuración de actualización automática habilitada.

| Configuración | Descripción |
| --- | --- |
| <b>Actualizar el panel de activos</b> | Inicie el proceso de actualización automática. Comportarse de la misma manera que el <b>panel Activos</b> (ver arriba). |
| <b>Actualizar recursos usados en el proyecto</b> | Inicie el proceso de actualización automática. Se comportan de la misma manera que los <b>recursos utilizados en el proyecto</b> (ver arriba). |

## Configuración avanzada

![](../assets/auto-update_mismatch.png)

La configuración avanzada permite controlar el comportamiento del proceso de actualización.

| Configuración | Descripción |
| --- | --- |
| <b>Omitir recursos cuando sus parámetros no coinciden</b> | Si se habilita, el proceso de actualización automática evitará actualizar los recursos si la nueva versión no coincide con la versión anterior. Por ejemplo, si un material de Substance tiene parámetros que ya no existen en la nueva versión (porque se han eliminado o se les ha cambiado el nombre), el proceso de actualización omitirá el recurso y mantendrá la versión anterior. |

>[!NOTE]
>
> Para forzar la actualización de activos que no coinciden, puede deshabilitar la configuración <b>Omitir activos cuando su parámetro no coincide</b>.

## Actualizar estado y registro

![](../assets/auto-update_log.png)

Después de una actualización de los recursos (automática o manual), el resultado del proceso aparecerá en la pestaña <b>Activos</b> en la ventana <b>Registro</b>, donde se informará de las actualizaciones y los problemas correctos. Si un recurso no coincide (ver arriba), los detalles del problema se proporcionarán por recurso.

El registro se puede abrir rápidamente haciendo clic en el icono dedicado en la parte superior derecha del menú de actualización automática:

![](../assets/auto_update_log_icon.png)

>[!NOTE]
>
> Cuando aparecen uno o más problemas después de una actualización, el icono de registro mostrará un pequeño icono de advertencia.

Dependiendo de cómo vaya el proceso de actualización, pueden aparecer varios tipos de problemas:

| Problema | Descripción |
| --- | --- |
| <b>No se pudo actualizar en el panel Activos</b> | Este mensaje indica que un problema ha impedido que el sistema de actualización continúe. Expanda el nombre del recurso para obtener más información. |
| <b>(nombre de archivo).(formato) no existe. No se puede volver a cargar (nombre de recurso)</b> | Este mensaje significa que ya no se puede encontrar el archivo de origen de un recurso (ya sea porque se ha movido o porque se ha quitado). Una solución sencilla es volver a importar el recurso o reubicarlo en la ventana Activos (mediante el menú contextual). |

## Mensaje de proyecto antiguo

![](../assets/auto_update_old_project_dialog.png.img.png)

Al abrir un proyecto antiguo, una opción estará disponible dentro del mensaje emergente de advertencia para informar sobre el proceso de actualización automática. Esta es una forma cómoda de desactivar rápidamente el proceso de actualización automática en caso de que permaneciera activado antes de abrir el proyecto antiguo.
