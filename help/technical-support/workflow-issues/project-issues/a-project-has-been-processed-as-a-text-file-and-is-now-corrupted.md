---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/workflow-issues/project-issues/a-project-has-been-processed-as-a-text-file-and-is-now-corrupted.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo recuperar archivos de proyecto de Substance 3D Painter dañados que se han procesado como archivos de texto.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Corrupted project file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Archivo de proyecto dañado
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---


# Un proyecto se ha procesado como archivo de texto y ahora está dañado

En ocasiones, puede aparecer el siguiente error al cargar un proyecto :

```
[Hdf5Archive] Archive 'project.spp' appears to have been processed as a text file and is irremediably corrupted. 

[Project management] The selected project 'project.spp' isn't valid!
```


Este error significa que el proyecto se ha modificado fuera de Substance 3D Painter y **no se puede volver a leer correctamente** .\
Suele ocurrir cuando un software de control de versiones (como **Perforce** ) procesa el proyecto de Substance 3D Painter **como un archivo de texto en lugar de un archivo binario** . La única solución es agregar una nueva regla/excepción al software de control de versiones para forzar el procesamiento de **archivos spp como binarios** . Para obtener más información sobre **Perforce** , consulte la documentación dedicada : <https://www.perforce.com/perforce/r16.1/manuals/cmdref/p4_typemap.html>
