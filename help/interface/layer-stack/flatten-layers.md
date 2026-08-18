---
title: Acoplar capas
description: ''
helpx_description: "Substance 3D Painter"
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/flatten-layers.html"
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%

---


# Acoplar capas

![](../../assets/v12_banner_flatten.jpg)

## Acoplar capas

El acoplado de capas permite condensar los datos de textura visibles de un grupo seleccionado en una sola capa. Esto puede ayudar a simplificar la pila de capas, mejorando el rendimiento y facilitando la administración de los proyectos.

>[!NOTE]
>
> Al utilizar la función Acoplar, se crea una nueva capa, pero no se elimina el grupo original de capas. En su lugar, el grupo de origen está desactivado, lo que deja la opción de eliminarlo o, alternativamente, guardarlo como un material inteligente para su edición posterior.

## Cómo acoplar capas

Para acoplar una serie de capas:

1. Seleccione las capas que desee.
1. Use <b>CTRL + G (CMD + G) </b> para agrupar la selección.
1. Use <b>CTRL + M (CMD + M)</b> para combinar la selección.

También puede acceder a estas opciones desde el menú contextual en lugar de usar métodos abreviados de teclado.

![](../../assets/v12_flatten_menu.jpg)

Cuando se acoplan capas, se crea una nueva capa de relleno con texturas acopladas y el grupo de origen se desactiva.

## Acoplar canales específicos

* En una capa de relleno, utilice el panel Propiedades para desactivar los canales que no desee acoplar. La información no se pierde cuando los canales están deshabilitados. Una vez que haya acoplado la capa, puede volver a activar los canales y los datos seguirán ahí
* En el caso de los grupos o las capas de pintura, puede utilizar los modos de fusión para desactivar canales:
  * En la parte superior de la pila de capas, seleccione el canal que desea desactivar.
  * Cambie el modo de fusión de la capa deseada a Desactivado.
  * Puede aplicar el mismo modo de fusión a todos los canales de una capa haciendo clic con el botón derecho en el modo de fusión y seleccionando &quot;Aplicar a todos los canales&quot;.

## Exporte mapas acoplados desde la pila de capas

Use <b>Exportar grupo acoplado a archivos</b> en el menú contextual de la pila de capas para exportar texturas rápidamente. Esta opción está disponible cuando se selecciona una capa o un grupo. Cuando se seleccionan varias capas o grupos, se gestionan como un lote, como si exportara cada uno de ellos uno por uno.

>[!NOTE]
>
> Al igual que con la función <b>Acoplar grupo </b>, los canales y capas vacíos o deshabilitados no se exportarán. Si se está utilizando una máscara de geometría, sólo se exportan los mosaicos UV activados dentro de la máscara de geometría.

### Administración de archivos

Al seleccionar <b>Exportar grupo acoplado a archivos</b>, tendrá la oportunidad de seleccionar una ubicación de carpeta para los archivos exportados.

Los nombres de los archivos exportados siguen el modelo del campo de nombre de archivo. El patrón predeterminado es:

* <b>$textureSet\_$layerName\_$srcMap(.$udim)</b>

Con este patrón, los mapas tendrán el nombre del conjunto de texturas, el nombre de la capa, el nombre del canal y, si se trata de un proyecto de mosaico UV, el número UDIM.

Si modifica el patrón, estará disponible de nuevo la próxima vez que se abra la ventana.

### Propiedades de archivo exportadas

Las propiedades de los archivos exportados se basan en los siguientes valores en el momento de la exportación:

* La resolución se basa en la resolución del conjunto de texturas.
* La profundidad de bits se basa en la profundidad de bits del canal en los ajustes del conjunto de texturas.

Las siguientes propiedades están codificadas y no se pueden cambiar:

* El relleno está bloqueado en 1px.
* El formato de archivo depende del canal que se exporta. Los mapas como height y normal suelen necesitar más profundidad de bits y se exportan como EXR, mientras que otros canales se exportan como PNG.
* Si solo se exporta una máscara, puede seleccionar el formato de exportación.

## ¿Cómo se genera la capa acoplada?

La función acoplar crea un mapa de bits por canal activado dentro de una nueva capa de relleno. La resolución se basa en la resolución del conjunto de texturas y la profundidad de bits viene determinada por los ajustes del conjunto de texturas.

El acoplado funciona cuando hay datos de textura dentro de un canal determinado. El acoplado no funcionará en una capa de pintura vacía y publicará un mensaje de error en el registro si no hay datos en la selección.

Solo se pueden acoplar las capas y los efectos visibles. Si algunas capas del grupo están desactivadas cuando el grupo se acopla, los efectos de estas capas no se incluirán en el resultado acoplado.

### Capas desactivadas

Solo se pueden acoplar las capas y los efectos visibles. Si algunas capas del grupo están desactivadas cuando el grupo se acopla, los efectos de estas capas no se incluirán en el resultado acoplado.

### Máscaras de capa y máscaras de geometría

Las máscaras se acoplan por separado de los datos de textura. Esto significa que, si acopla un grupo con una máscara, se generará un relleno acoplado y una máscara acopla.

Al utilizar una máscara de geometría, si solo se seleccionan algunos mosaicos UV dentro de la máscara de geometría, la capa alisada conservará esta selección. Los mosaicos UV que no se seleccionaron en la máscara de geometría se consideran vacíos y, por lo tanto, su texturizado no se conserva en el resultado alisado.

## Administrar contenido acoplado

>[!NOTE]
>
> Las imágenes acopladas se almacenan dentro del archivo de proyecto (.SPP). Esto significa que afectarán al tamaño del archivo de proyecto.

Las imágenes acopladas se etiquetan automáticamente como &quot;acopladas&quot;, por lo que puede buscarlas fácilmente en el panel Activos. También se almacenan automáticamente en la categoría Búsquedas guardadas &quot;Capas acopladas&quot;.

### Limpiar imágenes no utilizadas

La eliminación de imágenes no utilizadas del archivo de proyecto puede ayudar a reducir el tamaño del proyecto. En el panel Activos, puede eliminar imágenes desde el menú del botón derecho. O bien, para quitar todas las imágenes no utilizadas, usa <b>Archivo > Quitar recursos no utilizados</b>. Tenga en cuenta que esto no solo eliminará las imágenes acopladas, sino también cualquier recurso que no se esté utilizando en la pila de capas, las ranuras de mapas respaldados o en cualquier otro lugar de la interfaz de usuario.
