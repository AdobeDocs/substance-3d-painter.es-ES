---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/effects/filter.html"
breadcrumb-title: ''
description: Aprenda a utilizar efectos de filtro en Substance 3D Painter para aplicar filtros de procesamiento de imágenes y ajustes de textura.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Filtro
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# Filtro

Los efectos de filtro son sustancias que transforman el contenido de una capa o máscara.

## ¿Cómo se aplica un filtro?

Según el tipo de filtro, se debe crear un efecto de filtro en el contenido o la máscara de una capa.\
Hay dos formas de aplicar un filtro, la cual se utiliza depende de cómo se vaya a utilizar el filtro.

## Aplicar manualmente un filtro.

En el siguiente ejemplo, se aplica un filtro de desenfoque al contenido de una capa, pero se utiliza más comúnmente para aplicar filtros a máscaras :

### 1 - Añadir un efecto de filtro

Para empezar, seleccione el contenido de una capa (miniatura izquierda) y, a continuación, haga clic en el botón del efecto (o haga clic con el botón derecho para abrir el menú contextual).\
Seleccione la opción &quot;**agregar filtro**&quot; en la lista.

![](../../assets/add-filter.gif)

### 2 - Seleccione el filtro en la ventana de propiedades

En la ventana de propiedades, los parámetros o el filtro están actualmente vacíos. Solo está disponible el botón de selección.\
Haga clic en el botón para abrir el mini-estante y seleccionar el filtro deseado, aquí elegimos el filtro de desenfoque.

![](../../assets/filter-select-shelf.gif)

## Arrastrar y soltar un filtro desde el estante

Este método solo está diseñado para filtros que deben aplicarse a toda la pila de capas. Establecerá automáticamente todos los [modos de fusión](../../interface/layer-stack/blending-modes.md) del canal. No funciona para aplicar filtros a una máscara.

### 1 - Abra el área Filtros de la estantería

En la estantería, haz clic en la sección &quot;Filtros&quot; de la izquierda.

![](../../assets/shelf-filters.gif)

## 2 - Arrastre y suelte el filtro

Selecciona el filtro que quieres usar en la estantería. Arrástralo y suéltalo en tu pila de capas, asegurándote de que se coloca en la ubicación correcta (evita soltarlo en grupos no deseados, por ejemplo).

![](../../assets/filter-dragdrop.gif)

Observe cómo en el ejemplo anterior el filtro eliminado ya tiene un modo Fusión de paso a través. Esto se aplica a todos los canales del documento.

## Adición de nuevos tipos de filtros

Todos los filtros son Substance, que se pueden crear con Substance 3D Designer.\
Como inicio rápido, Substance 3D Designer proporciona plantillas listas para usar en Substance 3D Painter.

Para obtener más información, consulte esta página : [Creando efectos personalizados](../../content/creating-custom-effects/creating-custom-effects.md)
