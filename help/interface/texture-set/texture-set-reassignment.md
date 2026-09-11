---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/texture-set/texture-set-reassignment.html"
breadcrumb-title: ''
description: Aprenda a reasignar conjuntos de texturas en Substance 3D Painter para reorganizar las asignaciones de mallas y la asignación de texturas.
helpx_creative_field: ""
helpx_description: Painter > Interface > Texture Set > Texture Set reassignment
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Reasignación de conjunto de texturas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# Reasignación de conjunto de texturas

![](../../assets/txtset-reassignment-window.png)

La ventana Reasignación de conjunto de texturas permite cambiar la asignación de pila de capas a una parte diferente de la malla de la escena. Esto resulta útil, por ejemplo, después de importar una nueva malla a un proyecto existente en el que algunos conjuntos de texturas se desactivan. Esto sucede porque la pila de capas se asignó a un material que ya no existe. Con la ventana de reasignación es posible recuperar esa pila de capas (consulte &quot;Restauración de conjuntos de texturas desactivados&quot; a continuación).

Para acceder a la ventana Reasignación de conjuntos de texturas, ve a la ventana [Lista de conjuntos de texturas](texture-set-list.md) y elige **Configuración > Reasignar conjuntos de texturas**.

La ventana se divide en tres secciones:

* **Conjuntos De Texturas Deshabilitados** : Muestra todos los conjuntos de texturas que no se utilizan actualmente.
* **Conjuntos De Texturas Del Proyecto** : Muestra todos los conjuntos de texturas asignados actualmente a un material de malla.
* **Materiales de malla** : Enumere los materiales de malla del proyecto.

La ventana también tiene botones adicionales que realizan las siguientes acciones:

* **Deshacer** : Volver al estado anterior de la ventana
* **Rehacer** : Vuelva a aplicar el cambio que se ha deshecho.
* **Aplicar** : Cierre la ventana y realice las reasignaciones.
* **Cancelar** : Cierre la ventana y descarte los cambios que estén en curso.

## Reasignación de conjuntos de texturas

![](../../assets/reassign-existing-sets.gif)

La reasignación de conjuntos de texturas se puede realizar simplemente arrastrando y soltando los botones.

## Restauración de conjuntos de texturas desactivados

![](../../assets/reassign-disabled-sets.gif)

Un conjunto de texturas se puede desactivar cuando ya no está asociado a un material de malla.\
Esto puede ocurrir al importar una nueva malla a un proyecto en el que los nombres de los materiales difieren entre el proyecto y la nueva malla.

Para restaurar un conjunto de texturas, simplemente **intercambia** su posición con una en la lista &quot;**Conjuntos de texturas del proyecto**&quot;.

## Eliminación de conjuntos de texturas deshabilitados

![](../../assets/reassign-delete-sets.gif)

Al hacer clic en la **cruz** junto a un conjunto de texturas en la lista **Conjuntos de texturas deshabilitados**, se **marcará para su eliminación**.\
La eliminación se producirá al hacer clic en el botón **Aplicar** situado en la parte inferior de la ventana.

>[!WARNING]
>
> Esta acción no se puede deshacer una vez que la ventana se cierra con el botón &quot;Aplicar&quot;.
