---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/adding-saved-searches-manually.html"
breadcrumb-title: ''
description: Aprenda a añadir manualmente búsquedas guardadas en Substance 3D Painter para acceder rápidamente a los filtros de recursos de uso frecuente.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding saved searches manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Adición manual de búsquedas guardadas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 2%

---


# Adición manual de búsquedas guardadas

Las consultas de búsqueda de activos (o búsquedas guardadas) se pueden definir editando un archivo de configuración. Esta página explica cómo.

## Ubicación del archivo de configuración

Para agregar consultas guardadas personalizadas, vaya a la carpeta Documentos del usuario y abra el archivo **Shelf.ini**.

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>Platform</th> <th>Versión</th> <th>Ruta</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong> o posterior</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Heredada</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong> o posterior</td> <td colspan="1">/Usuarios/nombre_usuario/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Heredada</td> <td colspan="1">/Usuarios/nombre_usuario/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td colspan="1"><strong>7.2</strong> o posterior</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>Heredada</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

## Ejemplo

A continuación se muestra un ejemplo de contenido que se puede incluir en el archivo de configuración:

```
[filters] 

size=4 

1name=Grunge 

1query="u:basematerial=,smartmaterial=,smartmask=,texture=,procedural=,brush=,alpha= grunge" 

2name=Procedural 

2query="u:procedural=" 

3name=Environment 

3query="u:environment=" 

4name=Default Filters 

4query="p:/allegorithmic/^ u:filters="
```


Así es como funciona la sintaxis:

* **Tamaño**: determina el número de ajustes preestablecidos personalizados que la aplicación debe leer y cargar.
* **Número**: al inicio de la línea define el ajuste preestablecido actual al que se dirige (p. ej.:  **1/**).
* **Consulta**: (después del número) define los términos de búsqueda reales utilizados. En el ejemplo, usa **u:** para los usos, **p:** para las rutas o una cadena para un término de búsqueda. El contenido de la consulta debe estar entre comillas. Para obtener información sobre los términos que se pueden usar, [consulte esta página](../../interface/assets/advanced-search-queries.md).
* **Nombre**: el nombre del ajuste preestablecido.
