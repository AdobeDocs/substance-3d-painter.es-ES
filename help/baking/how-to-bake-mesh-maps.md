---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/baking/how-to-bake-mesh-maps.html"
breadcrumb-title: ''
description: Aprenda a hacer un bake mapas de malla en Substance 3D Painter para generar oclusión ambiental, curvatura y otras texturas basadas en geometría.
helpx_creative_field: ""
helpx_description: Painter > Baking > How to bake mesh maps
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Cómo hacer un bake mapas de malla
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---


# Cómo hacer un bake mapas de malla

El modo de hacer un bake dedicado de Substance 3D Painter facilita hacer un bake mapas de malla que pueden potenciar materiales inteligentes increíbles y otras herramientas. Siga leyendo o vea el vídeo siguiente para aprender a empezar a hacer un bake con Substance 3D Painter.

## 1 - Cambiar a modo de hacer un bake

De forma predeterminada, Painter se inicia en el modo de pintura al crear o abrir un proyecto. Para poder hornear mapas de malla, debe cambiar al modo de horneado. Utilice una de las siguientes opciones para cambiar al modo de Hacer un bake:

* Use el <b>botón de modo de Hacer un bake</b> (<b>icono de Croissant</b>) en la barra de herramientas contextual en la parte superior derecha de la ventana gráfica

  ![](../assets/croissant-icon.png)

  >[!NOTE]
  >
  > A veces, el <b>botón de modo de Hacer un bake</b> se puede ocultar detrás de otros paneles, según el diseño del área de trabajo.
* Use el menú Modo y seleccione <b>Hacer un bake mapas de malla.\
  </b>
* Utilice el método abreviado <b>F8</b>.

### 2 - Seleccionar conjuntos de texturas y Mosaicos de UV

Dentro de la <b>lista Conjunto de texturas</b>, use la casilla de verificación junto a cada conjunto de texturas (y número de Mosaicos de UV si existe) para seleccionar las partes que desea hacer un bake:

![](../assets/texture-set-list-baking-selection.png)

### 3 - Seleccionar bakeres

Dentro de la ventana Bakeres de mapa de malla, utilice las casillas de verificación para seleccionar los mapas que desea que se hagan un bake:

![](../assets/mesh-map-bakers-selection.png)

### 4 - Cambiar la configuración común

En el panel bakeres del mapa de malla, haga clic en los ajustes comunes para cambiar los ajustes, como la resolución del mapa con bake, la anchura de dilatación y los parámetros de poly altos, que se comparten en todos los mapas:

![](../assets/common-settings.png)

En la configuración común, puede definir los archivos que se van a utilizar como mallas de alta definición. La selección de mallas de alta definición permite definir cómo se genera la jaula para las mallas:

* Según la distancia: Inflar los vértices lejos de la malla a una distancia uniforme a través del modelo para crear una jaula.
* Automático (experimental): Painter analizará su malla y generará una jaula automáticamente, tratando de mantener la jaula cerca de la superficie sin crear intersecciones para obtener los mejores resultados.
* Archivo personalizado: Importe un archivo que haya creado para utilizarlo como jaula. Tenga en cuenta que los archivos importados deben tener el mismo número de vértices que la malla base para que funcione correctamente.

Si no va a hacer un bake desde una malla de alto contenido de poli, active la casilla de verificación <b>Usar malla de bajo contenido de poli como malla de alto contenido de poli</b>.

### 5 - Ajuste de la jaula

Hay diferentes opciones disponibles para ajustar la jaula en función del método de jaula que esté utilizando. Con una jaula basada en la distancia, puede ajustar las distancias frontal y trasera para minimizar la cantidad de intersección entre la jaula y su malla.

![](../assets/cage-distance.gif)

>[!NOTE]
>
> Aparecen manchas rojas cuando la jaula se cruza con la geometría del modelo. Una jaula que se intersecta generalmente conduce a artefactos y problemas en el área que se intersecta.

### 6 - Iniciar el proceso de hacer un bake

En la parte inferior de la ventana gráfica, haga clic en el botón Hacer un bake para iniciar el proceso de hacer un bake.

![](../assets/bake-button.png)

### 7 - Inspect muestra el registro de Hace un bake de errores

Una vez finalizado el proceso de hace un bake, puede consultar la ventana Registro de Hace un bake para comprobar si se ha informado de algún error.

Si los hay, utilice la flecha situada junto al mensaje de error para ver la configuración de baker correspondiente:

![](../assets/bake-failed.png)
