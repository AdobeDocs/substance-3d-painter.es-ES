---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/performances-guidelines/gpu-drivers.html"
breadcrumb-title: ''
description: Obtenga más información sobre la VRAM de GPU y los requisitos de controlador para que Substance 3D Painter optimice el rendimiento y la estabilidad del procesamiento.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > GPU Drivers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Controladores y VRAM de GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Controladores de GPU

No podemos garantizar el rendimiento sin el uso de controladores recomendados. Deben evitarse los controladores que no sean WHQL.\
Los controladores de GPU son como cualquier software, y cada nueva versión puede presentar problemas de rendimiento. Si se producen problemas después de actualizar a una versión más reciente del controlador, se recomienda bajar los controladores a una versión anterior.

## Configuración de controladores NVIDIA

Algunas configuraciones predeterminadas de NVIDIA pueden afectar al rendimiento. Se recomienda crear un perfil y deshabilitar los siguientes parámetros (establézcalos en desactivados) :

* Threaded Optimization
* Sincronización vertical

## Cómo otras aplicaciones pueden utilizar la GPU

Substance 3D Painter no es el único que trabaja con la GPU, pero otras aplicaciones hacen lo mismo. Casi cualquier aplicación 3D utilizará la GPU y la VRAM para ejecutarse, incluidas las que se utilizan habitualmente junto con Painter, como Blender, Maya, Unreal Engine, Unity, C4D y otras. Una solución para garantizar un buen rendimiento al tiempo que se mantienen abiertas estas aplicaciones es asegurarse de que Substance 3D Painter se inicie primero para solicitar su propia asignación de VRAM. Aun así, algún software puede adquirir algunas partes del VRAM de forma dinámica y puede seguir en conflicto con Substance 3D Painter incluso si se inicia después de Painter.

En general, cuanto más VRAM Painter tenga acceso a, más rápido se ejecutará, por lo que intente minimizar la cantidad de VRAM que utilizan otras aplicaciones que se ejecutan al mismo tiempo que Painter.

## Cantidad de VRAM de GPU y ancho de banda

Substance 3D Painter depende en gran medida de la GPU para realizar la mayoría de sus cálculos. Por esta razón es importante tener una GPU que cumpla con los [requisitos del sistema](../../getting-started/system-requirements.md).

Painter funciona transfiriendo texturas a la memoria de la GPU (VRAM) para realizar los cálculos (como operaciones de fusión para crear las texturas finales). Sin embargo, si el VRAM comienza a llenarse, las texturas no utilizadas se transferirán de nuevo a la RAM del equipo para liberar espacio VRAM. Substance 3D Painter escribe y lee GB de datos cuando trabaja. Esto significa que tanto la capacidad del VRAM (cantidad) como la velocidad del ancho de banda al realizar transferencias son importantes. Puede utilizar herramientas como [MSI AfterBurner](https://www.msi.com/page/afterburner) para supervisar este comportamiento.

>[!NOTE]
>
> Se sabe que <b>Nvidia GTX 970</b> tiene un diseño problemático con respecto a su memoria GPU que afecta a Substance 3D Painter. Los últimos 500 MB de los 4 GB funcionan a un ritmo más lento que los 3,5 GB restantes. Si Substance 3D Painter funciona con esos últimos 500 MB, el rendimiento se puede reducir hasta 10 veces (respecto a lo que medimos). Para obtener más detalles técnicos, consulte : <https://www.pcper.com/news/Graphics-Cards/NVIDIA-Responds-GTX-970-35GB-Memory-Issue>
