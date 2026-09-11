---
breadcrumb-title: ''
description: Revisa todos los cambios y actualizaciones en las versiones de Substance 3D Painter para realizar un seguimiento de la evolución y las mejoras de las funciones a lo largo del tiempo.
title: ZBrush a Painter Bridge
user-guide-description: ''
user-guide-title: ''
source-git-commit: c50b48e520277293b9ddef466baf8e27db4891ab
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---


# ZBrush a Painter Bridge

A partir de ZBrush 2026.2.0 (actualización de Maxon One de abril de 2026) y Substance 3D Painter 12.0.2 (versión Steam y CC), es posible enviar modelos directamente desde ZBrush a Painter a través de un plugin instalado automáticamente con la última versión de ZBrush.

![Imagen promocional que muestra un recurso representado mientras está superpuesto por el mismo recurso en Zbrush y en Painter.](../../assets/zbrush_promotional.png)

Con el plugin Substance Bridge, no es necesario pasar por el largo proceso de exportar archivos independientes de baja y alta poli, importarlos en Painter y configurar y ejecutar hagas un bake.

Para empezar a utilizar el puente de Zbrush a Painter:

1. Asegúrese de tener instalada al menos la versión 2026.2.0 de ZBrush.
1. Habilite el complemento en Painter asegurándose de que esté marcada la opción **Python > zbrush_painter_plugin**.
1. Desde ZBrush, **Enviar a Painter** está disponible en **Textura > Puente de Substance**

![Imagen del complemento Substance Bridge en ZBrush](../../assets/zbrush_painterSendTo.png)

## Configuración

Puede configurar las siguientes opciones para la creación automática de proyectos en Painter:

| Configuración | Descripción |
| --- | --- |
| Enviar a Painter | Envía el modelo a Substance 3D Painter con la configuración actual aplicada. Cada clic crea un nuevo proyecto de Substance desde cero. |
| **Subherramientas** | |
| Todo | Envía todas las subherramientas independientemente de la visibilidad. Ya sea que el globo ocular esté encendido o apagado, todo se envía. |
| Visible | Envía sólo las subherramientas con el icono de ojo activado en la lista de subherramientas. |
| Activo | Envía únicamente la SubTool seleccionada actualmente |
| Enviar PolyPaint | Convierte PolyPaint en un mapa de textura y lo aplica como capa de relleno en Substance, donde puede realizar pinturas sobre él y fusionarlo con él. |
| Suavizar normales | Suaviza las normales tangentes al exportar, de modo que las mallas faceteadas aparecen suaves en Substance, al igual que la forma en que las procesan los motores de juegos. Desactive esta opción para ver las facetas reales de la geometría. |
| Hacer un bake mapas automáticamente | Ejecuta automáticamente los algoritmos de hace un bake de Substance cuando llega el modelo, generando mapas de normales, oclusión ambiental, curvatura y otros mapas de detalle a partir de la comparación de malla alta/baja. |
| Forzar Desenvolvimiento automático UV | Activa el algoritmo de desajuste UV de Substance en cada subherramienta que llega. Si el modelo ya dispone de UV adecuados, deje esta opción desactivada, ya que los sobrescribe. |
| Nivel de subdivisión | Controla los niveles de subdivisión que se envían. Actual sólo envía el nivel mostrado. Bajo y alto envía los niveles más bajo y más alto para hacer un bake y es la opción recomendada para la mayoría de los flujos de trabajo. |
| Conjuntos de texturas | Controla cómo se divide el espacio UV en Substance: Por SubTool (un conjunto de texturas por SubTool) o Por PolyGroup (un conjunto de texturas por PolyGroup dentro de cada SubTool). |

Cuando Painter reciba el modelo, si la opción hacer un bake automáticamente está activada, se iniciará haciendo un bake. La subdivisión más baja del modelo es la malla importada como la malla de baja densidad, y la subdivisión más alta se utiliza como la de alta densidad para hacer un bake los detalles. ZBrush puede manejar un número mucho mayor de polígonos que Painter, así que asegúrese de que la malla de poli bajo tiene un tamaño de trabajo óptimo (esto dependerá de la máquina, pero menos de 1 millón es mejor).

Los conjuntos de texturas de Painter representan asignaciones de materiales. Un conjunto de texturas es igual a un espacio UV.

* Por subherramienta crea un conjunto de texturas para cada subherramienta (todas las partes de la subherramienta compartirían el mismo espacio UV), que es la opción más sencilla.
* Por grupoPoly crea un conjunto de texturas por grupoPoly dentro de cada subherramienta, lo que proporciona un control más preciso sobre las asignaciones de materiales.

>[!NOTE]
>
>Con la versión Steam de Painter, Painter debe estar abierto para recibir el modelo ZBrush.


## Recursos adicionales

[Vea este vídeo](https://www.youtube.com/watch?v=fLkkwV4BzrU) para ver el puente en acción, o acceda a la [documentación de ZBrush](https://help.maxon.net/zbr/en-us/Default.htm#html/reference-guide/texture/substance-bridge/substance-bridge.html?Highlight=painter) para obtener más información.
