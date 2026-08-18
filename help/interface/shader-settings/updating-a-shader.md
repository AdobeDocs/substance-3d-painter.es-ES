---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/interface/shader-settings/updating-a-shader.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo actualizar sombreadores personalizados en Substance 3D Painter para aplicar cambios de sombreado y volver a cargar archivos de sombreado.
helpx_creative_field: ""
helpx_description: Painter > Interface > Shader settings > Updating a shader
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Actualización de un sombreado
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---


# Actualización de un sombreado

En ocasiones, puede ser necesario actualizar el sombreado utilizado por un proyecto para corregir problemas o aprovechar las funciones más recientes. Esta página describe cómo hacerlo.

A continuación se muestra un método paso a paso sobre cómo actualizar el sombreado de un proyecto:

* **Actualizar un sombreado mediante la ventana del sombreado**
* **Actualizar un sombreado mediante el complemento Resource Updater**

Si un proyecto usa un **sombreador personalizado** (no incluido de forma predeterminada en Substance 3D Painter), consulta la página [Sombreador personalizado](https://substance3d.adobe.com/display/DRAFTPAINTER/Shader+API) para obtener una guía sobre cómo actualizarlo.

## Actualizar un sombreado mediante la ventana de sombreado

### 1 - Abra la ventana Configuración del sombreado

La ventana **Configuración de sombreado** está disponible a la derecha de forma predeterminada en la barra de herramientas de Dock.

![](../../assets/shader-settings-window.png)

### 2 - Haga clic en el botón de sombreado y seleccione el sombreado actualizado

Haga clic en el botón de sombreado (debajo del botón de deshacer/rehacer) y busque el sombreado que coincida con el que ya se utilizó.

![](../../assets/shader-mini-shelf.png)

### 3 - Se actualiza el sombreador

Una vez cargado el nuevo sombreado, se debe quitar la mención **outdated** y el modelo 3D debe aparecer normalmente en la ventana gráfica.

![](../../assets/updated-shader.png)

## Actualizar un sombreado mediante el complemento Resource Updater

### 1 - Abra el actualizador de recursos

Dirígete a la izquierda de la interfaz para buscar la barra de herramientas **Complementos** y haz clic en el icono **Actualizador de recursos**.

![](../../assets/resource-icon.png)

### 2 - Cambiar a la ficha Sombreado

En la nueva ventana que apareció, haga clic en la pestaña &quot;Shader&quot; para mostrar el sombreado presente en el proyecto actual.

![](../../assets/shader-tab.png)

### 3 - Busque el sombreador y actualícelo

En la ficha Sombreador debería aparecer una lista de todos los usuarios de recursos de sombreador del proyecto actual. Los sombreadores **obsoletos** son visibles con un **fondo rojo** . Haga clic en el botón &quot;actualizar&quot; junto a un recurso para actualizarlo.

![](../../assets/update-shader-click.gif)
