---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/effects/compare-mask.html"
breadcrumb-title: ''
description: Aprenda a utilizar el efecto Comparar máscara en Substance 3D Painter para crear máscaras basadas en operaciones de comparación de texturas.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Compare Mask
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Máscara de comparación
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---


# Máscara de comparación

![](../../assets/compare-mask.png)

Este efecto permite comparar de forma rápida y sencilla dos canales y, como resultado, producir una máscara. Este efecto solo está disponible para la máscara en capas.

A continuación se muestran los ajustes disponibles para este efecto:

| Configuración | Descripción |
| --- | --- |
| **Canal** | El canal que se va a comparar entre el origen y el destino desde el que se va a crear una máscara. Esta lista se basa en el canal disponible en la [configuración del conjunto de texturas](../../interface/texture-set/texture-set-settings.md). |
| **Comparar** | Hay tres parámetros disponibles aquí para elegir cómo se debe calcular la máscara. El menú desplegable del centro define la operación de comparación (menor que, dentro de la tolerancia, mayor que). <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/compare-mode.png"/></div> Los modos de origen y destino son:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Capas inferiores</strong> : Tenga en cuenta la versión acoplada de todas las capas inferiores a la actual.</li><li data-preserve-html="true"><strong>Esta capa</strong>: Tenga en cuenta solo esta capa.</li><li data-preserve-html="true"><strong>Esta máscara</strong>: Tenga en cuenta el contenido existente de la máscara (por ejemplo, si ya hay un efecto Relleno o un efecto Generador).</li><li data-preserve-html="true"><strong>Constante</strong>: Valor uniforme.</li></ul>Las operaciones son :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Menor que</strong> : Si el origen (menú desplegable de la izquierda) tiene valores más bajos que el destino (menú desplegable de la derecha), se generarán valores blancos en la máscara.</li><li data-preserve-html="true"><strong>Dentro de tolerancia</strong> : Si el origen (menú desplegable de la izquierda) tiene valores similares a los del destino (menú desplegable de la derecha), se generarán valores blancos en la máscara.</li><li data-preserve-html="true"><strong>Mayor que</strong> : Si el origen (menú desplegable de la izquierda) tiene valores más altos que el destino (menú desplegable de la derecha), se generarán valores blancos en la máscara.</li></ul> |
| **Constante** | Valor con el que comparar cuando el ajuste de comparación se establece en &quot;constante&quot;. |
| **Dureza** | Controla el smoothness y la dureza de la comparación de máscara resultante. |
| **Histograma de canales de origen** | Proporcione una vista de histograma del origen y el destino. Útil para saber si se superponen un poco o no se superponen en absoluto (si no se superponen, la máscara estará vacía).Para obtener más información sobre cómo funciona el histograma, consulte : [Niveles](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/atomic-nodes/levels). |

>[!NOTE]
>
> Es posible hacer clic con el botón derecho en una capa y elegir el método abreviado &quot;**Añadir máscara con la combinación de heightes**&quot; para agregar rápidamente este nuevo efecto en una capa. Este método abreviado también cambiará el canal de Height **modo de fusión** a &quot;**Normal**&quot; en lugar del valor predeterminado &quot;**Sobreexposición lineal (añadir)**&quot;.\
> ![](../../assets/compare-shortcut.png)
