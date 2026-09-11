---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/masking-and-effects.html"
breadcrumb-title: ''
description: Aprenda a usar máscaras y efectos en Substance 3D Painter pila de capas para controlar la visibilidad de las capas y aplicar efectos de capa.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Masking and effects
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Máscara y efectos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 5%

---


# Máscara y efectos

## Enmascaramiento

Las capas se pueden enmascarar para mostrar/aplicar su contenido solo en partes específicas de la textura. La máscara funciona como un parámetro de intensidad sobre el contenido de la capa. Una máscara de una capa siempre está en escala de grises, independientemente del contenido que se utilice para realizar la pintura sobre ella (por lo tanto, cualquier color se convertirá en un valor de escala de grises antes de pintarse).

Puede añadir una máscara con el menú del botón derecho o con el botón dedicado :

![](../../assets/layer-mask.gif)

Posibles operaciones en máscaras :

* Puedes visualizar la máscara haciendo **ALT + clic izquierdo del ratón** en su miniatura. Cambiará la ventana gráfica a una vista aislada de la máscara desde esta capa. Esta operación también está disponible a través de la configuración del visor.
* Puede deshabilitar temporalmente una máscara haciendo **MAYÚS + clic izquierdo del ratón** en su miniatura. Vuelva a hacer la misma operación para volver a habilitarla. Esta operación también está disponible a través del menú del botón derecho (&quot;alternar máscara&quot;).
* Puedes copiar el contenido de una máscara a otra haciendo **clic con el botón derecho > Copiar contenido de máscara** en la miniatura y, a continuación, haciendo **clic con el botón derecho > Pegar en máscara** en la miniatura de la segunda máscara.
* Puede invertir el fondo de la máscara haciendo **clic con el botón derecho > Invertir fondo de máscara**. Esto resulta útil si desea evitar la destrucción de los efectos asociados a una máscara.

>[!WARNING]
>
> Si se vuelve a añadir una máscara o se elimina, se destruirá la máscara y todos los efectos asociados a ella.

Es posible crear una máscara inmediatamente al crear una capa de relleno (mediante arrastrar y soltar) si se presiona la tecla **CTRL** :

![](../../assets/mask-material-optimized.gif)

## Efectos

Los efectos son operaciones especiales que se pueden editar en cualquier momento. Los efectos se pueden colocar en una máscara o en el contenido de una capa.\
Sin embargo, los efectos son más apropiados para uno para el otro. Por ejemplo, los &quot;generadores&quot; son apropiados para las máscaras.

La línea debajo de cada miniatura de una capa indica si existen efectos. Gris es igual a sin efectos, rojo es igual a al menos un efecto. Hay una pila de efectos por máscara y por contenido.

![](../../assets/effect.gif)

Para obtener más información, [consulte la página dedicada](../../features/effects/effects.md).

## Máscaras inteligentes

Las máscaras inteligentes son una forma de guardar una máscara y su efecto para reutilizarlas fácilmente en otras capas u otros proyectos. Para crear una máscara inteligente, solo tienes que hacer clic con el botón derecho sobre una máscara y elegir &quot;**Crear máscara inteligente**&quot;.\
Al arrastrar y soltar una máscara inteligente en una capa, se creará una máscara negra si aún no existe; de lo contrario, la lista de efectos se combinará con la existente. Es posible sobrescribir por completo la lista de efectos manteniendo presionado &quot;**CTRL**&quot; al colocar la máscara inteligente.

![](../../assets/smart-mask-new-optimized.gif)

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/smart-mask-add-optimized.gif)

</td>
<td style="border: 0;" valign="top">

![](../../assets/smart-mask-overwrite-optimized.gif)

</td>
</tr>
</table>
