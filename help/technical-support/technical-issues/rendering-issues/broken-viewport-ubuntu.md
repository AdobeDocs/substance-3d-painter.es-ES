---
breadcrumb-title: ""
description: Obtenga información sobre cómo solucionar problemas de la ventana gráfica rota o que no responde en Ubuntu en Substance 3D Painter para una representación 3D adecuada.
title: La ventana gráfica aparece rota o no responde en Ubuntu
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%
---

# La ventana gráfica aparece rota o no responde en Ubuntu

Al ejecutar Painter desde Steam en Ubuntu a partir de la versión 11.1, la ventana gráfica puede aparecer rota o sin respuesta.

Esto está relacionado con el hecho de que Painter no se inicie con la GPU correcta asignada. En Ubuntu, la GPU integrada en lugar de la discreta puede terminar siendo seleccionada. Painter hereda esta configuración a través de Steam, lo que puede provocar problemas.

Existen algunas soluciones:

1. Ejecutar Steam desde un terminal. Esto forzará un contexto diferente y debería hacer que Steam y Painter se ejecuten en la GPU correcta.
1. Edite el método abreviado de Steam para deshabilitar la configuración <b>Ejecutar usando tarjeta gráfica exclusiva</b>. A continuación, ejecute Steam normalmente.

Para obtener más información, consulte [este problema de github](https://github.com/ValveSoftware/steam-for-linux/issues/9940).
