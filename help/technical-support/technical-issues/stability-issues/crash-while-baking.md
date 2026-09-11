---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-while-baking.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo corregir bloqueos de Substance 3D Painter durante las operaciones de hace un bake para obtener flujos de trabajo fiables de hace un bake de texturas.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash while baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bloqueo al hacer un bake
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Bloqueo al hacer un bake

Substance 3D Painter puede producir bloqueos durante el proceso de hace un bake en algunas configuraciones. Esta página reagrupa una lista de problemas conocidos y cómo mitigarlos.

## Bloqueo con Hacer un bake vista previa

De forma predeterminada, Substance 3D Painter muestra en la ventana gráfica el estado en curso de hacer un bake una textura. En algunos equipos, esta característica puede provocar inestabilidad.

Para desactivarla:

1. Use **Editar > Configuración** para abrir la configuración principal
1. En **General**, se desplaza hacia abajo hasta la sección denominada **Opciones de horneado** .
1. Desmarque o deshabilite la opción **Habilitar proceso de procesamiento de vista previa en vivo** .

## Choque con el Trazado de rayos de GPU

En algunas GPU con controladores inestables, el proceso de procesamiento puede producir bloqueos debido a la función Trazado de rayos de GPU.

Para desactivarla:

1. Use **Editar > Configuración** para abrir la configuración principal
1. En **General**, se desplaza hacia abajo hasta la sección denominada **Opciones de horneado** .
1. Desmarque o deshabilite la opción **Habilitar Trazado de rayos de GPU** .

## Bloqueo con CPU Ryzen

La aplicación puede entrar en bloqueo durante el proceso de hacer un bake en alguna configuración del equipo que se ejecuta con una CPU Ryzen. Una actualización del BIOS suele solucionar el problema.

Esto se relaciona con los cálculos multiproceso. Muchos constructores de placas madre han publicado nuevas actualizaciones de BIOS para solucionar este problema, por lo que recomendamos aplicar la actualización. Para obtener más información, consulte el manual de la placa base y el sitio web del constructor.

## Archivos Assbin incompatibles

De forma predeterminada, al hacer un bake, las mallas de alta densidad se preprocesan en archivos **\*.assbin** para acelerar la reconfiguración más adelante. En algunos casos excepcionales, estos archivos pueden producir bloqueos en la aplicación si se han generado con una versión diferente. Simplemente eliminarlos debería resolver el problema, ya que se regenerarán.
