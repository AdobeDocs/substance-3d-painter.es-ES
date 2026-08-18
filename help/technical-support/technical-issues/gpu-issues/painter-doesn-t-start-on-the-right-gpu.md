---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/painter-doesn-t-start-on-the-right-gpu.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo configurar Substance 3D Painter para que se inicie en la GPU correcta para obtener un rendimiento y una compatibilidad óptimos.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Painter doesnt start on the right GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Painter no se inicia en la GPU derecha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---


# Painter no se inicia en la GPU correcta

En Windows, es posible que la aplicación no utilice la GPU adecuada al iniciarse, lo que puede provocar problemas de rendimiento y estabilidad. A continuación se muestra una lista de problemas comunes y sus soluciones para asegurarse de que el software funciona con la GPU correcta.

Para saber qué GPU se usa, puedes comprobar el [archivo de registro](../../exporting-the-log-file.md).

## Windows

### Configuración de los cables del monitor

En Windows, la GPU asignada a una aplicación depende del monitor en el que se ejecuta la aplicación. Esto se debe a que los cables del monitor están vinculados directamente a la salida de la propia GPU. La aplicación puede iniciarse en una GPU incorrecta, por lo tanto, si el monitor en el que se inicia está vinculado a la salida gráfica de la placa base en lugar de a la de la propia tarjeta gráfica. En ese caso, es probable que Windows utilice la GPU integrada en lugar de la GPU dedicada.

<b>Para solucionar este problema</b>: solo tiene que corregir la configuración del cable desconectando el monitor vinculado a la placa base y vinculándolo a las salidas de la GPU.

### Instalación incorrecta del controlador de GPU

Si los controladores de la GPU no están instalados correctamente, la aplicación no podrá acceder a la GPU dedicada y tendrá que volver a la GPU integrada.

<b>Para solucionar este problema</b>: desinstale los controladores de la GPU actuales, realice una limpieza y vuelva a instalar los controladores de la GPU después de reiniciar el equipo.

### Configuración de perfil de controlador de GPU Nvidia

En algunos equipos, como los portátiles, la aplicación puede ejecutarse en la GPU integrada en lugar de la GPU Nvidia dedicada de forma predeterminada. Con una GPU NVIDIA, el cambio a la GPU derecha depende de los perfiles de aplicación. Si una aplicación no tiene dicho perfil, puede asignar uno manualmente.

<b>Para solucionar este problema</b>:

1. Haga clic con el botón derecho en el escritorio y seleccione Panel de control de NVIDIA <b>o</b>. Vaya al Panel de control y busque Panel de control de NVIDIA
1. En <b>Configuración 3D</b>, vaya a <b>Administrar configuración 3D</b>
1. En la pestaña <b>Configuración del programa</b>, agregue un nuevo perfil para <b>Substance 3D Painter</b>
1. Cambie la configuración del procesador de gráficos preferido a Procesador NVIDIA de alto rendimiento

### Configuración de rendimiento de Windows

Es posible que Windows haya establecido una configuración de GPU incorrecta para la aplicación debido a la configuración predeterminada de rendimiento y consumo de energía.

<b>Para solucionar este problema: </b>Siga el paso a paso que se indica a continuación para invalidar la configuración de GPU predeterminada.

1. Abra la configuración de pantalla haciendo clic con el botón derecho en su escritorio :

   ![](../../../assets/settings-33.png)
1. Vaya a la parte inferior de la ventana en la página de inicio y haga clic en &quot;Configuración de gráficos&quot; :

   ![](../../../assets/graphics-settings.png)
1. Haga clic en el botón &quot;Examinar&quot; y localice el ejecutable de Substance 3D Painter :

   ![](../../../assets/browse-16.png)
1. Una vez añadida la aplicación, haga clic en el botón &quot;Opciones&quot; :

   ![](../../../assets/options-19.png)
1. Elija el ajuste &quot;Alto rendimiento&quot; y haga clic en el botón &quot;Guardar&quot;

   ![](../../../assets/specs.png)

## Linux

### Desactive &quot;Prefiere GPU no predeterminada&quot;

Al ejecutar Painter desde un acceso directo de escritorio o a través de Steam, asegúrese de que la configuración <b>PrefersNonDefaultGPU</b> dentro del archivo <b>\*.desktop</b> esté establecida en <b>false</b>.

Esta configuración puede inducir a error y hacer que se utilice o se fuerce la GPU integrada en lugar de la discreta y más potente. Para obtener más información [vea esta discusión](https://github.com/ValveSoftware/steam-for-linux/issues/9940).

### Forzar GPU específica mediante la variable de entorno DRI\_PRIME

De forma predeterminada, Painter utilizará la primera GPU indicada por la API de gráficos Vulkan; sin embargo, esta GPU podría ser la incorrecta (podría ser la GPU integrada la primera), lo que provocaría un rendimiento deficiente. La variable de entorno DRI\_PRIME se puede utilizar para forzar la GPU de su elección. Para obtener más información, [consulte la documentación de la wiki de Arch](https://wiki.archlinux.org/title/PRIME#For_open_source_drivers%E2%80%94PRIME). También puede consultar la [documentación de Mesa](https://docs.mesa3d.org/envvars.html#envvar-DRI_PRIME).
