---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/plugins/autosave.html"
breadcrumb-title: ''
description: Aprenda a utilizar el complemento Autoguardar en Substance 3D Painter para guardar automáticamente sus proyectos a intervalos regulares.
helpx_creative_field: ""
helpx_description: Painter > Features > Plugins > Autosave
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Autoguardar
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---


# Autoguardar

![](../../assets/autosave-details.png){width="500px"}

Los complementos de autoguardado permiten **crear copias de seguridad** del proyecto abierto actualmente. Crea un archivo en el lateral mientras no modifica el proyecto actual.

Los archivos de copia de seguridad se ubicarán en tres posibles ubicaciones:

* Si se ha guardado el proyecto actual, las copias de seguridad estarán junto a él.
* Si el proyecto nunca se ha guardado (sin título), las copias de seguridad se guardarán en la carpeta de autoguardado de la carpeta Documentos del usuario. ( **Documentos/Allegorithmic/Substance 3D Painter/autosave** )
* Si se ha activado la configuración de anulación, las copias de seguridad se ubicarán en la ruta facilitada en la configuración.

*Hay disponible un botón de posponer en la interfaz para retrasar el autoguardado.*

## ¿Cómo se activa el guardado automático?

El autoguardado se basa en un temporizador interno, una vez que el temporizador ha terminado, comienza el proceso de autoguardado.\
El botón de posponer se activará cuando esté cerca del final del temporizador, lo que permite retrasar el autoguardado durante unos pocos minutos.

Todos los valores basados en el tiempo se pueden modificar a través de la ventana de configuración.

## ¿Cómo se desactiva el autoguardado?

Si, por cualquier razón, es necesario desactivar el proceso de autoguardado, se puede hacer a través del menú del complemento. Para ello, haz clic en el menú **Complementos** > **Autoguardar** > **Deshabilitar**.

## Configurar el guardado automático

Para configurar el comportamiento de autoguardado, haz clic en el menú **Complementos** > **Autoguardado** > **Configurar**.

* **Intervalo de autoguardado en minutos** : indica el tiempo de espera entre cada autoguardado.
* **Número de archivos de guardado automático** : la cantidad máxima de archivos de copia de seguridad creados para un proyecto determinado.
* **Intervalo de inactividad en minutos** : cuánto tiempo se retrasará el autoguardado al hacer clic en el botón de posponer.
* **Tiempo de advertencia antes de guardar en segundos**: cuánto falta para que el botón posponer esté activo y la barra de progreso esté visible antes del desencadenador de autoguardar.

>[!NOTE]
>
> El temporizador de guardado automático se detendrá si:
> 
> * El motor está haciendo un cálculo
> * Las texturas se están exportando
> * La ventana de configuración está abierta
> * El proyecto se está guardando

En la parte inferior de la ventana es posible reemplazar la ubicación predeterminada de los archivos de copia de seguridad.\
Cuando la opción &quot;**Guardar siempre en el siguiente directorio**&quot; está habilitada, todo el archivo de copia de seguridad se ubicará en la carpeta especificada (la ruta predeterminada es la carpeta Documentos del usuario).
