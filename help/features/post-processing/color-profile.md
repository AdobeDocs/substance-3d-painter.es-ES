---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/post-processing/color-profile.html"
breadcrumb-title: ''
description: Aprenda a utilizar el posprocesamiento del perfil de color en Substance 3D Painter para aplicar transformaciones de gradación de color y LUT.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Color Profile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Perfil de color
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---


# Perfil de color

![](../../assets/doc-lut-example.jpg){width="700px"}

Substance 3D Painter permite asignar **perfiles de color** a los **puntos de visión** cargando texturas **LUT**.\
Se puede utilizar un perfil de color para calibrar el color final de la pantalla de modo que coincida con un destino, como una cámara específica. A menudo, un perfil manipula los colores cambiando el brillo, la gamma, el contraste o incluso el equilibrio de color.

>[!NOTE]
>
> **LUT** significa &quot;**tabla de consulta**&quot;. Es una forma optimizada de realizar la gradación de color como efecto posterior. Se utiliza una LUT para compensar la diferencia entre un origen y un resultado.\
>  Substance 3D Painter usa **LUT 3D** almacenadas como **textura 2D** (flotante) de cualquier resolución posible (los valores predeterminados son **2048x128 píxeles** ). Esto significa que el cubo que almacena las operaciones de color se separa en sectores que se muestran uno al lado del otro. Para obtener más detalles técnicos, consulte el artículo **GPU Gem** : <http://http.developer.nvidia.com/GPUGems2/gpugems2_chapter24.html>

## Uso de un perfil de color

Un perfil de color se puede cargar a través de la ventana Configuración de visualización.\
Marque la casilla de verificación &quot;**Activar perfil de color**&quot; para afectar al puerto de visualización y habilitar un perfil de color.

![](../../assets/color-profile-ui.png)

* Cuando &quot;Activar perfil de color&quot; está **deshabilitado**, la representación de la ventana gráfica se realiza en **sRGB** para la vista de material (y lineal para algunos canales específicos)
* Cuando &quot;Activar perfil de color&quot; está **habilitado**, la representación de la ventana gráfica se realiza en **Lineal/Raw** para cada vista (incluidos los canales individuales)

Si se carga una textura LUT en la ranura del recurso, se utilizará para manipular la representación de la ventana gráfica cuando esté en **modo Material** .\
De lo contrario, el procesamiento se mostrará como Lineal/Raw (por ejemplo, con vistas de canales solo).

La configuración de **punto blanco** se puede usar para cambiar la asignación de tonos de la imagen de entrada (antes de que surta efecto la LUT).\
Por ejemplo, si está viendo el sol, el valor debe ser mayor que 1 (valor predeterminado). Para obtener una exposición perfecta, el punto blanco debe ajustarse al valor superior de la imagen.

La fórmula de punto blanco es la siguiente:

```
float Value = 1.0f / WhitePoint; // Value from the user interface 

float3 Output = clamp( HDR.rgb * Value, 0.0f, 1.0f );
```


Es posible aplicar una asignación de tonos específica antes de utilizar el perfil de color. Consulte las funciones disponibles en [Asignación de tonos](tone-mapping.md).\
Substance 3D Painter no procesa el color de entrada más que a través de la configuración de punto blanco. Por ejemplo, no se aplica ninguna LUT de Shaper.

## Creación de perfiles de color

Substance 3D Painter desplazará la ventana gráfica a la representación **Lineal** cuando esté habilitada la opción &quot;**Activar perfil de color**&quot;. Esto significa que, cuando se aplica una LUT, es necesario convertir el color de un perfil lineal al destino deseado.

### Método 1 : Modificación de la LUT de identidad

La edición de la LUT de identidad se puede realizar en un software que admita texturas <b>flotantes</b> de 32 bits, como <b>Substance 3D Designer</b>. Descargue la LUT de identidad como punto de partida para crear un nuevo perfil:

[Descargar color\_profile\_linear.exr](https://github.com/AdobeDocs/painter-python-api/raw/refs/heads/main/static/misc/color_profile_linear.exr)

### Método 2 : Uso de E/S de OpenColor para generar una Textura LUT

Instale las herramientas **OpenColor IO**. A continuación, descargue el Ejemplo de configuración de OCIO, disponible aquí : <http://opencolorio.org/downloads.html>\
Desde allí, ejecute el programa **ociolutimage** con los siguientes argumentos:

```
ociolutimage --generate --cubesize 64 --config nuke-default/config.ocio --colorconvert linear srgb --output lutLinearToSRGB.exr
```


**Nota**: También es posible modificar la LUT de identidad con **E/S OpenColor** mediante el programa **ocioconvert** para aplicar la conversión de color a esta LUT.

### Importación de un nuevo perfil de color

Simplemente abra la ventana de importación (o arrastre y suelte la LUT en el estante). Al importar la textura LUT en Substance 3D Painter, asegúrese de asignar el &quot;**colorlut**&quot; **usage** al nuevo recurso. De lo contrario, el recurso no será visible correctamente en el estante.

Para obtener más información, consulte la documentación sobre la importación de nuevos recursos : [Agregando recursos mediante la ventana de importación](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/adding-content-via-the-import-window-151584824.html)
