---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/layer-instancing.html"
breadcrumb-title: ''
description: Aprende a usar la creación de instancias de capas en Substance 3D Painter para reutilizar capas en varios conjuntos de texturas de forma eficaz.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Layer instancing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Creación de instancias de capas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Creación de instancias de capas

**Creación de instancias de capas** permite sincronizar parámetros de capa entre varias capas y [Conjuntos de texturas](../texture-set/texture-set.md) mientras se puede generar un resultado dependiente de la malla.

Cuando se crea una instancia de capa, la capa original (o capa de origen) se utiliza para replicar parámetros en todas las instancias existentes. **Solo se puede modificar la capa de origen**.

>[!WARNING]
>
> Cualquier acción de pintura (trazos de pincel, relleno de polígono, etc.) solo funcionará en el conjunto de texturas donde se encuentra la capa de origen. Otros conjuntos de texturas que tengan una instancia de esta capa simplemente descartarán las acciones de pintura.

## Creación de una instancia de capa

Para crear una instancia de capa:

1. Seleccione cualquier capa existente
1. Copie la capa (**CTRL+C**)
1. Pégala como una instancia (usa **CTRL+MAYÚS+V** o haz clic con el botón derecho para abrir el menú contextual y elige **Pegar como instancia**)

![](../../assets/paste-as-layer-instance.png)

>[!NOTE]
>
> Las instancias se pueden crear desde cualquier capa, incluidos **grupos**. Crear instancias de una carpeta puede ser una forma sencilla de replicar varias capas en varios conjuntos de texturas. Al añadir capas dentro de una carpeta de instancias, también se replicarán en instancias existentes.

Una vez creada una instancia, la capa de origen y destino mostrará un nuevo icono. Este icono es un botón que se puede utilizar para navegar entre una capa de origen y sus instancias con mayor facilidad, sin tener que cambiar manualmente entre conjuntos de texturas (véase a continuación).

| Nombre | Icono |
| --- | --- |
| **Capa sin instancias** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/non-instanced.png"/></div> |
| **Origen de instancia** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/instance-source.png"/></div> |
| **Destino de instancia** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/instance-target.png"/></div> |

## Creación de una instancia entre conjuntos de texturas

Es posible crear una instancia de capa en varios conjuntos de texturas en una sola acción, evitando copiarla/pegarla manualmente.

Para crear una instancia en varios conjuntos de texturas:

1. Seleccione cualquier capa existente
1. Haga clic con el botón derecho en la capa para abrir el menú contextual
1. Elija **Crear instancias entre conjuntos de texturas**
1. En la nueva ventana, compruebe qué conjuntos de texturas necesitan para recibir una instancia.
1. Haga clic en Aceptar para validar y crear las instancias.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/instance-across-texture-sets.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/instance-across-texture-sets-dialog.png)

</td>
</tr>
</table>

>[!NOTE]
>
> El signo de exclamación situado junto al nombre de un conjunto de texturas indica que el canal **no coincide**. Esto significa que si se crea una instancia en estos conjuntos de texturas, no se procesará correctamente porque falta un canal.

## Cambiar entre una instancia y su origen

Dado que una instancia **solo** puede actualizarse **editando el origen** (por razones técnicas), es obligatorio seleccionar la capa de origen para editar sus propiedades.\
Esto se puede hacer haciendo clic en el botón **propiedades de instancia** en la capa de la pila de capas.

![](../../assets/instance-properties-optim.gif)

Al hacer clic en un botón de propiedades de instancia, cambiará la **ventana de propiedades** de la herramienta o capa actual a **una lista** que muestra una capa de origen y sus instancias.\
Al hacer clic en **cualquier elemento** de la lista, automáticamente **salta a esta capa** . Esto **cambiará** automáticamente los **conjuntos de texturas seleccionados** al correcto también.

El uso de la lista **árbol de instancias** es la mejor manera de **pasar rápidamente** de una instancia a su origen mientras se ven las **dependencias** al mismo tiempo.

## Ciclos de instancias (y cómo resolverlos)

Los ciclos son instancias que se utilizan en la propia capa de origen, ya sea directa o indirectamente. El motor de Substance 3D Painter no puede calcular los ciclos **&#x200B;**&#x200B;y, por lo tanto, debe **deshabilitarlos** hasta que se corrijan o quiten.

Ejemplo:\
![](../../assets/instance-cycle-optim.gif)

En este ejemplo, la instancia de la capa de origen se mueve dentro de ella (porque es una carpeta). La instancia se rompe porque para generar sus parámetros necesitamos consultar los parámetros desde el origen, que depende de los parámetros de la instancia. Esto crea un ciclo que no se puede resolver automáticamente. La instancia se desactiva.

La única forma de corregir un ciclo es **mover** la instancia fuera de la carpeta o **eliminarla**.

Las instancias de capa se pueden utilizar en las capas de origen siempre que la propia instancia haga referencia a una capa de origen diferente.
