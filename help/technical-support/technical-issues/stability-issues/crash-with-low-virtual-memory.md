---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-with-low-virtual-memory.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo solucionar los bloqueos de Substance 3D Painter causados por una memoria virtual baja para garantizar un rendimiento estable de la aplicación.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash with low virtual memory
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bloqueo con poca memoria virtual
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Bloqueo con poca memoria virtual

Substance 3D Painter puede ser inestable si el archivo de **paginación** ( **intercambio** de memoria/ **memoria virtual**) está establecido con un valor **demasiado bajo** .\
Se recomienda dejar que el sistema operativo maneje estas configuraciones (lo que normalmente ocurre de forma predeterminada). Substance 3D Painter requiere un **mínimo** de **16 GB** de memoria virtual para funcionar correctamente.

## ¿Cómo cambiar el tamaño de la memoria virtual en Windows?

>[!NOTE]
>
> Para cambiar el tamaño de la memoria virtual en Windows será necesario reiniciar el equipo.

Acceda a la configuración de memoria virtual con los siguientes pasos

1. Haga clic con el botón derecho en el icono **Equipo/Este equipo** y elija **Propiedades**
1. Seleccione &quot;**Configuración avanzada del sistema**
1. Haga clic en el botón **Configuración** de la sección **Rendimiento**
1. Haga clic en la pestaña **Avanzado**
1. Haga clic en **Cambiar** en la sección **Memoria virtual**

Ahora es posible hacer lo siguiente:

* Marque la casilla de verificación **Administrar automáticamente el tamaño del archivo de paginación para todas las unidades**

**o**

* Seleccione el disco duro donde desea cambiar el tamaño de la memoria virtual, elija **Tamaño administrado por el sistema** y haga clic en el botón **Establecer**.

**Automático:**

![](../../../assets/virtual-memory-default.png)

**Manual:**

![](../../../assets/virtual-memory-settings.png)
