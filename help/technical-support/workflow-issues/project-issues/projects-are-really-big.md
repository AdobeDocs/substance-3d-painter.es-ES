---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/project-issues/projects-are-really-big.html"
breadcrumb-title: ''
description: Aprenda a reducir el tamaño de los archivos de proyecto de Substance 3D Painter para optimizar el rendimiento y los requisitos de almacenamiento.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Projects are really big
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Los proyectos son realmente grandes
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---


# Los proyectos son realmente grandes

El proyecto de Substance 3D Painter puede ser muy grande y ocupar mucho espacio en disco. Esta página explica por qué y cómo mitigarlo.

## ¿Qué tipo de recursos se almacenan en un proyecto?

Cada recurso o recurso utilizado durante la creación de texturas se almacena en el archivo de proyecto, entre los que se incluyen:

* **Malla de origen** (no es el archivo original, sino uno procesado)
* **Mapas de malla horneados**
* **Materiales** (como Materiales de Substance)
* **Mapas de bits** u otros recursos utilizados por cualquier trazo de capa/ajuste preestablecido/pincel.

Las mallas de alto contenido de poli no se incluyen en el proyecto. Simplemente están vinculados.

## ¿Por qué un proyecto almacena tantos recursos?

Almacenar todos los recursos utilizados hace que un proyecto sea completamente autónomo y se pueda mover fácilmente de un equipo a otro sin romperlo. El principal inconveniente es el tamaño de archivo potencialmente grande en el disco.

La decisión de tener todo incrustado en el archivo del proyecto se debe a que todo no es destructivo. Esto significa que el proyecto se &quot;vuelve a generar&quot; cuando se vuelve a abrir. Si falta un solo pincel o material de la estantería, el proyecto podría romperse y no podría regenerarse correctamente. Si se almacena un duplicado del recurso, se garantiza que el proyecto se pueda restaurar cuando se guardó.

## ¿Hay alguna forma de reducir el tamaño de un proyecto?

Hay algunas formas de reducir el tamaño de un proyecto:

### Limpiar recursos no utilizados

Cuando utilice muchos recursos en un proyecto, Substance 3D Painter los copiará. Por ejemplo, si ha utilizado un alfa para pintar algo. Si más adelante elimina la capa cuando se pintó el alfa, Substance 3D Painter no elimina automáticamente el recurso.

Para quitar los recursos no utilizados, use la acción **Limpiar** del [menú Archivo](https://substance3d.adobe.com/display/DRAFTPAINTER/File+menu) . A continuación, guarde el proyecto (esto activará la eliminación real del recurso).

Los recursos que todavía se utilizan en un proyecto no se pueden quitar. Esto significa que el conjunto de texturas deshabilitado sigue haciendo referencia a los recursos y evita que se eliminen. Para evitarlo, quite los conjuntos de texturas deshabilitados en la [ventana de reasignación de conjuntos de texturas](../../../interface/texture-set/texture-set-reassignment.md).

### Reducir la resolución del conjunto de texturas

Cuando se guarda un proyecto, el resultado final de la pila de capas de un conjunto de texturas se guarda en el proyecto. Esto permite conservar una previsualización en la ventana gráfica cuando se vuelve a abrir el proyecto sin tener que volver a calcular el conjunto de texturas. Sin embargo, cuanto mayor sea la resolución del conjunto de texturas, mayor será la caché de previsualización.

Para reducir el espacio en caché, simplemente cambie la resolución a un número inferior, como 512 por ejemplo. Dado que Substance 3D Painter no es destructivo, esta resolución se puede cambiar de nuevo más adelante sin perder calidad.

### Compactar el proyecto

Guardar un proyecto de forma incremental (mediante CTRL+S) puede fragmentar mucho el archivo del proyecto. Si bien no es un problema crítico, esto puede introducir espacio vacío en el archivo de proyecto, lo que puede aumentar el tamaño.

Use la función &quot;Guardar y compactar&quot; en el [menú Archivo](../../../interface/main-menu/file-menu.md) para volver a guardar el proyecto y eliminar el espacio vacío desperdiciado. Esta acción de guardar será más larga que una acción normal de guardar, pero puede reducir significativamente el espacio del archivo.

### Reducir el tamaño de los mapas de malla horneados

En general, el mayor culpable y la razón por la que un proyecto ocupa tanto espacio en el disco es porque los Mapas de malla horneados son muchos y grandes.

Para reducir el tamaño de Mapas de malla, hay algunas cosas que se pueden hacer :

* *Usar una resolución de cocción inferior.*\
  Si bien el mapa Normal puede beneficiarse de ser horneado en 4K, este podría no ser el caso para el mapa de posición que generalmente es solo acerca de degradados de color. Hornea en dos pases con dos resoluciones diferentes para mezclar tamaños de archivo diferentes.
* *Exporta las texturas y reduce manualmente su espacio.*\
  De forma predeterminada, Substance 3D Painter procesa todas las texturas como imágenes RGBA en 16 bits, incluidos los pasteles en escala de grises, como la Oclusión Ambiente.

  Para reducir las texturas de cocción para impresión, utilice este paso a paso:
  1. Deshabilite el ajuste &quot;Aplicar difusión&quot; en la ventana de Baker
  1. Establezca la &quot;Dilación con&quot; en un valor razonable (32 píxeles para una resolución de 2048, por ejemplo).
  1. Hornea todas tus texturas con la misma resolución
  1. Exporte las texturas al horno con el ajuste preestablecido de exportación &quot;Mapas de malla&quot; como PNG de 16 bits con el relleno definido en &quot;Sin relleno (paso a través)&quot;
  1. Abra cada mapa en un software de edición de fotos o Substance 3D Designer
  1. Reduzca la resolución de las texturas para las que parece ajustado. Asegúrese de cambiar la Oclusión ambiente, la curvatura y el Thickness de color a escala de grises.
  1. Guarde las nuevas versiones de textura como PNG de 16 bits.
  1. Vuelva a importar las texturas y sustitúyalas sobre las texturas de cocción originales en los ajustes del Conjunto de texturas.
  1. Utilice la acción Limpiar del menú Archivo para eliminar los mapas de malla antiguos.
  1. Utilice la acción Guardar y compactar del menú Archivo para comprimir el archivo de proyecto.\
     Después de todos estos pasos, la huella del proyecto debería reducirse significativamente.

Es importante que los mapas de malla permanezcan como mínimo texturas de 16 bits. Aunque las texturas de 8 bits pueden tener un tamaño menor, presentarán artefactos en los generadores de materiales y máscaras inteligentes. Recomendamos PNG porque es un formato de compresión sin pérdida, lo que significa que comprimirá las texturas sin introducir artefactos y también admite 16 bits.
