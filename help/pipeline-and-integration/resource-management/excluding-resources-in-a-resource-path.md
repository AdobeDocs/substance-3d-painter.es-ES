---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/pipeline-and-integration/resource-management/excluding-resources-in-a-resource-path.html"
breadcrumb-title: ''
description: Aprenda a excluir recursos específicos de las rutas de recursos en Substance 3D Painter para una mejor organización de la plataforma.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Excluding resources in a resource path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Excluir recursos de una ruta de acceso de recurso
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---


# Excluir recursos de una ruta de acceso de recurso

Esta página explica cómo configurar un archivo omitido para especificar recursos y carpetas que se omitirán durante el proceso de rastreo de la ventana [Assets](../../interface/assets/assets.md). Permite evitar que se muestren recursos no deseados.

>[!NOTE]
>
> Esta funcionalidad está disponible desde la versión 7.2.3.

## Creación de un archivo omitido

Vaya a la ubicación de la carpeta de recursos en la que desee ocultar los recursos. A continuación, cree un archivo con el nombre siguiente:

```
.ignore_assets_pt
```


>[!NOTE]
>
> Tenga en cuenta que el nombre de archivo debe empezar por un punto.

Debe tener este aspecto una vez creado:

![](../../assets/ignore-file-location.png)

## Ejemplo

El siguiente contenido de archivo descartará cualquier recurso y carpeta que no sean las carpetas de biblioteca predeterminadas:

```
## exclude all

* 

 

## re-include library directories

!alphas 

!colorluts 

!effects 

!emitters 

!environments 

!export-presets 

!generators 

!materials 

!presets 

!procedurals 

!receivers 

!shaders 

!smart-masks 

!smart-materials 

!templates 

!textures
```


## Reglas y directrices

En la tabla siguiente se muestran las reglas generales que se aplican al archivo omitido.

>[!NOTE]
>
> La coincidencia de patrones del archivo omitido distingue mayúsculas de minúsculas, independientemente del comportamiento del sistema operativo.

| Regla | Descripción | Ejemplo |
| --- | --- | --- |
| **Línea en blanco** | Línea vacía que no coincide con nada. Se puede utilizar como separador para facilitar la lectura. |  |
| **Separador de directorios** | La barra diagonal se utiliza como separador de directorios. Los separadores pueden ocurrir al principio, al medio o al final de un patrón de búsqueda.Si hay un separador al principio o en el medio (o ambos) del patrón, el patrón es relativo al nivel de directorio del propio fichero de ignorar. De lo contrario, el patrón también puede coincidir en cualquier nivel por debajo del nivel de archivo omitir. Si hay un separador al final del patrón, se ignorará, el patrón seguirá coincidiendo tanto con los ficheros como con los directorios. | `folder/filename.extension   folder/sub-folder` |
| **Línea de comentarios** | Una línea que comienza con el signo de número (o hash) sirve como comentario. | `# This is a comment` |
| **Asterisco** | Un asterisco equivale a cualquier cosa menos a una barra diagonal. | `# Match anything starting with Alpha   alpha*   # Match any file with given extension   *.jpg` |
| **Intervalo de caracteres** | Se puede especificar un intervalo de caracteres entre corchetes para que coincida con el nombre de la carpeta y el nombre de archivo.<ul data-preserve-html="true"> <li data-preserve-html="true"><b>[abc]</b>: Coincidir con un carácter de la lista dada</li> <li data-preserve-html="true"><b>[a-c]</b>: Coincidir con un carácter del intervalo especificado</li> <li data-preserve-html="true"><b>[ !abc]</b>: Coincidir con un carácter no incluido en la lista dada</li> <li data-preserve-html="true"><b>[ !a-c]</b>: Coincidir con un carácter que no se encuentre en el intervalo especificado</li> </ul>El rango y la lista también pueden ser números con el formato <b>[0-9]</b>. | `# Exclude any UDIM image in PNG   *_[0-9][0-9][0-9][0-9].png` |
| **Carácter de escape** | Indique caracteres literales que, de otro modo, se ignorarían o se usarían como reglas. | `# This is a comment   [#]This/Is/A/Path` |
| **Espacios finales** | Los espacios finales se omiten a menos que se escapen. | `# Match a subfolder with trailing space   folder/subfolder[ ]` |
| **Prefijo De Exclamación** | Prefijar un motivo con un signo de exclamación permite negarlo.Cualquier archivo coincidente excluido por un patrón anterior se volverá a incluir. No es posible volver a incluir un archivo si se excluye un directorio principal de dicho archivo. El rastreo no enumera los directorios excluidos por motivos de rendimiento, por lo que los patrones de los archivos contenidos no tienen efecto, independientemente de dónde estén definidos. | `# Re-include specific file   !my_file_name.png` |
