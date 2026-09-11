---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/shelf-issues/font-import.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo solucionar problemas de importación de archivos de fuentes en Substance 3D Painter para importar y utilizar correctamente los recursos de fuentes.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: No se puede importar el archivo de fuentes
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# No se puede importar el archivo de fuentes

Con la introducción del [recurso de texto](../../../painting/text-resource.md), el archivo de fuentes se recopila automáticamente al inicio. Los archivos de fuentes también se pueden importar manualmente.

En estos casos, pueden aparecer algunos mensajes de error:

* Al arrastrar y soltar un archivo en la interfaz de Painter.
* Cuando Painter está descubriendo fuentes en el disco (rastreo de biblioteca).

## Cómo solucionar el problema

Si aparece un mensaje de error sobre un <b>archivo dañado</b>, intente encontrar una versión alternativa del mismo y es posible que Painter pueda cargarlo. Tenga en cuenta que solo se admiten los formatos <b>.ttf</b> y <b>.otf</b>.

Si aparece un mensaje de error sobre un <b>problema de licencia</b>, la fuente simplemente no es compatible con Painter y no se puede importar.

### Introducción a Mensajes

|  |  |
| --- | --- |
| <b>Mensaje de error</b> | <b>Explicación</b> |
| Hay problemas en la biblioteca &quot;LIBRARYNAME&quot; que afectan a 4 archivo(s) de fuentes: FONTNAME, FONTNAME, FONTNAME,... | Este mensaje recopila una breve lista de nombres de archivo de fuentes que se han identificado que no se pueden importar dentro de Painter. Estos archivos se omitirán y no aparecerán en la ventana Activos. |
| Se han encontrado problemas de fuentes. Para obtener más información, visite https://... | Mensaje genérico que indica que se ha encontrado un problema con las fuentes. |
| No se puede importar FONTNAME debido a las restricciones de licencia. Para obtener más información, visite https://... | Painter debe poder incrustar fuentes en su archivo de proyecto para poder utilizarlas. Por lo tanto, las fuentes que no lo permiten (especificadas en sus metadatos) no se pueden importar. |
| No se puede importar FONTNAME porque el archivo está dañado o es de un tipo no compatible. Para obtener más información, visite https://... | Painter no puede leer el archivo de fuentes proporcionado. |
