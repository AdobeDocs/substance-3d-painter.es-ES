---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/pipeline-and-integration/configuration/command-lines.html"
breadcrumb-title: ''
description: Aprenda a utilizar argumentos de línea de comandos con Substance 3D Painter para la integración de automatización, secuencias de comandos y canalización.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Command lines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Líneas de comandos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# Líneas de comandos

Esta página muestra varias líneas de comandos que se pueden utilizar al iniciar la aplicación para crear o abrir proyectos, por ejemplo.\
Estas líneas de comandos se pueden utilizar de la siguiente manera:

```
"Adobe Substance 3D Painter.exe" --command [option] 
```


## Lista de comandos

| Comando | Descripción |
| --- | --- |
| **—help** **-?** **-h** | Muestra información acerca de qué línea de comandos están disponibles y cómo utilizarlas. |
| **—version** **-v** | Mostrar la versión actual de Substance 3D Painter. |
| **—mesh** | Malla para cargar en un proyecto.Ejemplo:  `// Create a new project with a specific mesh   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj"       // Update a mesh inside an existing project   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj" "E:/MyMeshFolder/Project.spp"` |
| **—mesh-map** | Mapas con bake asociados a la malla (AO, Normal, Curvatura). Se puede especificar varias veces. Nomenclatura : TextureSetName\_AdditionalMapSlot<ul data-preserve-html="true"> <li data-preserve-html="true">Oclusión ambiental = <strong> <em> oclusión_ambiente </em> </strong></li> <li data-preserve-html="true">Curvatura = <strong> Curvatura <em> </em> </strong></li> <li data-preserve-html="true">Normal = <strong> <em> base_normal </em> </strong></li> <li data-preserve-html="true">Espacio Mundial Normal = <strong> <em> world_space_normals </em> </strong></li> <li data-preserve-html="true">Posición = <strong> Posición <em> </em> </strong></li> <li data-preserve-html="true">Thickness = <strong> <em> thickness </em> </strong></li> <li data-preserve-html="true">Id. = <em> Id. <strong> </strong> </em></li> </ul>Ejemplo:  `"Adobe Substance 3D Painter.exe" --mesh "E:/MyMeshFolder/MyMesh.obj" --mesh-map " E:/MyMeshFolder/DefaultMaterial_ambient_occlusion.png"` |
| **: dividido por audio** | Cree un conjunto de texturas por azulejo UDIM. |
| **—export-path** | Ruta de exportación predeterminada en la que se exportarán los resultados del proyecto. |
| **—vram-budget** | Anule el presupuesto de memoria de vídeo (VRAM) definido por el motor de Substance 3D Painter. La &quot;cantidad&quot; está en megabytes.    Ejemplo:  `// Set the VRam budget to 2GB   "Adobe Substance 3D Painter.exe" --vram-budget 2048` |
| **—disable-version-verification** | No comprobar si hay una nueva versión de la aplicación disponible al iniciarse |
| **—enable-remote-scripting** | Permite ejecutar comandos de secuencias de comandos desde fuera de la aplicación. Consulte [Control remoto con secuencias de comandos](../../scripting-and-development/scripts-and-plugins/remote-control-with-scripting.md) para obtener más información. |
