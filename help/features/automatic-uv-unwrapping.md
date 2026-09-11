---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/automatic-uv-unwrapping.html"
breadcrumb-title: ''
description: Aprenda a utilizar el desajuste UV automático en Substance 3D Painter para generar diseños UV para sus modelos 3D automáticamente.
helpx_creative_field: ""
helpx_description: Painter > Features > Automatic UV Unwrapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Desempaquetado automático de UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# Desempaquetado automático de UV

![](../assets/auto-unwrap-update-810.jpg)\
El desajuste automático de UV permite generar Islas de UV automáticamente al importar un modelo 3D. Se puede utilizar para realizar pinturas en modelos 3D que no tengan UV existentes.

## Activación del desajuste automático de UV

![](../assets/uv-new-project.png)

Al crear un nuevo proyecto o volver a importar una malla en un proyecto existente, asegúrese de que esté marcada la opción &quot;Desenvolvimiento automático&quot;. Si está desactivado, el proceso se omitirá y las UV de malla permanecerán tal cual.

## Ajustes de desajuste UV

![](../assets/unwrap-settings.png)

Al importar una malla y utilizar el proceso de desajuste, están disponibles los siguientes ajustes. Algunas configuraciones están disponibles a través del botón Opciones en la interfaz.

| Sección | ***Configuración*** | ***Descripción*** |
| --- | --- | --- |
| **Desempaquetar secuencia** | **Costuras** | Controla si las costuras (bordes de Isla de UV) se deben generar solo para mallas que no las tienen o que siempre se regeneran.Valores posibles:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Generar datos que faltan </strong> (predeterminado): Se generarán costuras para las mallas que las pierdan.</li><li data-preserve-html="true"><strong> Volver a calcular todo </strong> : Se generarán costuras para todas las mallas.</li></ul> |
| **Islas de UV** | Controla si el desenvolvimiento UV debe generarse a partir de mallas sin UV o para cualquier malla. Valores posibles:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Generar datos que faltan </strong> (predeterminado): Se generará el desempaquetado UV para las mallas que faltan UV.</li><li data-preserve-html="true"><strong> Volver a calcular todo </strong> : Se generará el desenvolvimiento UV para todas las mallas.</li></ul> |  |
| **Empaquetado** | Controla el empaquetado/disposición de las Islas de UV de las mallas.Valores posibles:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Generar datos que faltan </strong> (predeterminado): islas de UV de empaquetado para mallas a las que les faltaban UV.</li><li data-preserve-html="true"><strong> Volver a calcular todo </strong> : empaca todas las Islas de UV.</li></ul> |  |
|  |  |  |
| **Personalización del diseño** | **Tamaño de margen** | Define el espaciado entre las Islas de UV. Esta configuración aplica un porcentaje general independiente de la resolución.Valores posibles:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> No hay margen </strong> : 0 %</li><li data-preserve-html="true"><strong> Pequeño </strong> (predeterminado): 0,2 %</li><li data-preserve-html="true"><strong> Medio </strong> : 0,5 %</li><li data-preserve-html="true"><strong> </strong> grande : 1 %</li></ul> |
|  | **Orientación de la Isla de UV** | Controlar la orientación de las Islas de UV durante el proceso de empaquetado.Valores posibles:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sin restricciones</strong> (predeterminado): no se aplica ninguna restricción para calcular la orientación.</li><li data-preserve-html="true"><strong>Alinear con malla 3D</strong>: restringir la Isla de UV para que se oriente hacia la dirección de la malla</li></ul> |
|  |  |  |
| **Mosaicos de UV** | **Número máximo de Mosaicos de UV** | Si el flujo de trabajo de Mosaicos de UV está habilitado, esta configuración determina el número máximo de mosaicos que se producirán para distribuir en las Islas de UV. |
|  |  |  |
| **Optimización** | **Evitar Islas de UV alargadas** | Si se activa, este proceso dividirá las Islas de UV que se consideren demasiado largas para mejorar el uso del espacio de textura.Ejemplo de antes (arriba) y después (abajo): <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r10-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../assets/uv-before-after.jpg" width="400px"/></div> |

## Limitaciones conocidas

A continuación se muestra una lista de limitaciones relacionadas con el proceso de desempaquetado:

* El procesamiento de mallas de polietileno altas puede tardar mucho tiempo.
* Los vértices en las mismas coordenadas exactas se combinan
* La generación de UV puede fallar en algunas partes de la malla en algunos casos raros
* Proporción de texel no uniforme o muy distorsionada en una sola Isla de UV en algunos casos
* Proporción de textura no uniforme entre conjuntos de texturas
* La isla de UV generada puede ser muy alargada y no encajar en el espacio UV en algunos casos
* Es posible que las caras degeneradas o las caras de malla no triangular con bordes pequeños o superpuestos no se desenvuelvan con UV
