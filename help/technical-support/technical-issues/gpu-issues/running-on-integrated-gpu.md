---
breadcrumb-title: ""
description: Aprenda a configurar Substance 3D Painter para utilizar una GPU dedicada en lugar de gráficos integrados para obtener un mejor rendimiento.
title: Ejecución en GPU integrada
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%
---

# Ejecución en GPU integrada

![](../../../assets/integrated-gpu.png){width="500px"}

Puede suceder que algunos equipos estén configurados de forma predeterminada para ejecutarse en un chipset integrado en lugar de en una GPU dedicada.\
Dado que el rendimiento en el chipset integrado es muy bajo, recomendamos utilizar una GPU dedicada. Puede aparecer una ventana emergente que le avisa al respecto.

Con una GPU NVIDIA, el cambio a la GPU NVIDIA depende de los perfiles de la aplicación. Si una aplicación no tiene dicho perfil, puede asignar la tarjeta gráfica manualmente:

1. Haga clic con el botón derecho en el escritorio y seleccione Panel de control de NVIDIA **o**. Vaya al Panel de control y busque Panel de control de NVIDIA
1. En **Configuración 3D** , vaya a **Administrar configuración 3D**
1. En la pestaña **Configuración del programa**, agregue un nuevo perfil para **Substance 3D Painter**
1. Cambie la configuración del procesador de gráficos preferido a Procesador NVIDIA de alto rendimiento
