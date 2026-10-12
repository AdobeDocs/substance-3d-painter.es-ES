---
breadcrumb-title: ""
description: Obtenga información sobre cómo corregir bloqueos de Substance 3D Painter al trabajar con GPU sobreaceleradas para un rendimiento estable de la aplicación.
title: Bloqueo al trabajar con GPU sobreacelerada
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%
---

# Bloqueo al trabajar con GPU sobreacelerada

Las GPU sobreaceleradas a menudo pueden ser más inestables porque se ejecutan en frecuencias no diseñadas inicialmente por el constructor de la GPU. Si la GPU está sobreacelerada y tiene problemas de estabilidad, le recomendamos que vuelva a las frecuencias predeterminadas de fábrica durante un tiempo.

## GPU Nvidia

En las GPU de NVIDIA, a partir de los controladores 35.82, es posible deshabilitar temporalmente la sobreaceleración de GPU habilitando un modo de depuración en la configuración de los controladores. Esto permite comprobar y determinar los problemas relacionados con las tarjetas gráficas.

Para habilitar el modo de depuración:

1. Abra el **Panel de control de NVIDIA** (haga clic con el botón derecho en el escritorio).
1. Haga clic en el menú **Ayuda**.
1. Haga clic en **Modo de depuración**.

>[!NOTE]
>
> El modo de depuración puede no estar disponible si la GPU es una tarjeta de referencia. Solo estará disponible si la GPU se ejecuta en relojes no estándar o con una BIOS modificada. En este caso, se recomienda desactivar manualmente el overclocking.
