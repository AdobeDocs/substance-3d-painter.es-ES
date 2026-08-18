---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/rendering-issues/blocky-artifacts-appear-on-textures-in-the-viewport.html"
breadcrumb-title: ''
description: Aprenda a corregir los defectos de bloque que aparecen en las texturas en la ventana gráfica de Substance 3D Painter para obtener una calidad visual limpia.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Blocky artifacts appear on textures in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Aparecen artefactos de bloque en las texturas de la ventana gráfica
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# Aparecen artefactos de bloque en las texturas de la ventana gráfica

A partir de la versión 2018.3.0, pueden aparecer en la ventana gráfica los siguientes tipos de artefactos:

![](../../../assets/viewport-artifacts.jpg){width="400px"}

Estos artefactos están relacionados con problemas con los controladores de la GPU de Nvidia.\
Para evitar los artefactos, debe desactivarse la compatibilidad con hardware de texturas virtuales dispersas.

Los controladores GeForce **Drivers 440.97** han **solucionado este problema** . Recomendamos actualizar a estos controladores y mantener el SVT habilitado para obtener un buen rendimiento.

Los nuevos controladores están disponibles en el sitio web de Nvidia: <https://www.nvidia.com/Download/index.aspx>

## Desactivación de la aceleración de hardware de texturas virtuales dispersas

### 1 - Inicie Substance 3D Painter y abra la Configuración

![](../../../assets/settings-34.png)

Abra la configuración principal en Editar > Configuración.

### 2 - Busque la sección llamada &quot;Texturas virtuales dispersas&quot;

![](../../../assets/svt-subsection.png)

Dentro de la sección &quot;General&quot;, desplácese hacia abajo y busque la subsección denominada &quot;Texturas virtuales dispersas&quot;

### 3 - Desmarque la configuración

![](../../../assets/uncheck-hardware.png)

Desactive la configuración &quot;Aceleración de soporte de hardware&quot; desmarcándola.

### 4 - Validar y reiniciar Substance 3D Painter

![](../../../assets/validate-1.png)

Valide el cambio haciendo clic en el botón &quot;Aceptar&quot;.

![](../../../assets/restart-3.png)

Reinicie Substance 3D Painter haciendo clic en el botón &quot;Sí&quot; para aplicar el cambio.
