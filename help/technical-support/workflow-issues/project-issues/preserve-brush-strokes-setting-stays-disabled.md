---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/project-issues/preserve-brush-strokes-setting-stays-disabled.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo corregir la configuración de conservar trazos de pincel desactivada en Substance 3D Painter para conservar los trazos de pincel correctamente.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Preserve brush strokes setting stays disabled
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La opción Conservar trazos de pincel permanece desactivada
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# La opción Conservar trazos de pincel permanece desactivada

Debido a un error desafortunado introducido en Substance 3D Painter 1.5 (parcialmente corregido en 1.7), algunos proyectos han perdido metadatos relacionados con la malla. Por lo tanto, este error hace que la opción &quot;Conservar posiciones de trazos en malla&quot; de la ventana [Configuración del proyecto](../../../interface/project-configuration.md) esté deshabilitada.

Para resolver el problema, deben seguirse algunos pasos específicos :

* Abra el proyecto con el problema en Substance 3D Painter 1.7 o superior
* Vaya a Editar > Configuración del proyecto
* Seleccione y vuelva a importar la malla original que utilizó en el proyecto actual (no la versión actualizada)
* Valide y deje que Substance 3D Painter calcule las capas, nada debe cambiar si es la misma malla
* Vaya de nuevo a Editar > Configuración del proyecto
* La opción &quot;Conservar posiciones de trazos en la malla&quot; ahora debería estar activada de nuevo, lo que le permite importar la nueva malla
