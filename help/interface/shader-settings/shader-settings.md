---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/shader-settings.html"
breadcrumb-title: ''
description: Aprenda a configurar los ajustes del sombreado en Substance 3D Painter para personalizar la representación del material y el aspecto visual.
helpx_creative_field: ""
helpx_description: Painter > Interface > Shader settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configuración del sombreador
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 5%

---


# Configuración del sombreador

![](../../assets/shader-settings.png)

La ventana **Shaders Settings** permite controlar los parámetros del sombreado (y del molde Iray) y los parámetros de desplazamiento de geometría.

Un sombreado es una función que define el aspecto que debe tener un objeto al interactuar con luces y sombras en las ventanas gráficas. En esta aplicación, los sombreadores se utilizan para saber cómo leer los canales del conjunto de texturas y procesar la malla 3D en las ventanas gráficas.

## Deshacer archivo de sombreado y pila

![](../../assets/shader-undo.png)

Esta sección de la ventana Ajustes del sombreado controla los parámetros principales al manipular los sombreadores.\
La pila Deshacer/Rehacer del sombreado es independiente del [Historial](https://substance3d.adobe.com/display/DRAFTPAINTER/History) principal para no crear conflictos al pintar.

Si el archivo de sombreado está marcado como &quot;Desactualizado&quot;, se recomienda actualizarlo cuando sea posible. Consulte :  [Actualizando un sombreador](https://substance3d.adobe.com/display/DRAFTPAINTER/Updating+a+Shader)

| *Configuración* | *Descripción* |
| --- | --- |
| **Deshacer** | Revertir/Cancelar un cambio de archivo de sombreado o cualquier modificación de parámetros de sombreado |
| **Rehacer** | Aplique de nuevo un cambio cancelado mediante la herramienta Deshacer. |
| **Archivo de sombreado** | Botón que muestra el archivo de sombreado actual utilizado. Haga clic en el botón para abrir una mini-estantería y elegir un sombreador diferente. |
| **Nombre de instancia** | Nombre de la instancia del sombreador. |
| **Restaurar valores predeterminados** | Restaure todos los parámetros del sombreado a sus valores predeterminados (tal como están en el archivo del sombreado). |

### Instancia de sombreado

Una instancia de sombreado es un sombreado basado en un archivo de sombreado original pero con parámetros personalizados. Una instancia de sombreado se puede compartir entre conjuntos de texturas y un conjunto de texturas puede tener una instancia de sombreado única.

**Por ejemplo:** un proyecto puede usar un sombreador base, mientras que un conjunto de texturas usa un sombreador personalizado para admitir la opacidad.

Para crear y administrar instancias de sombreado, consulte la ventana [Lista de conjuntos de texturas](../texture-set/texture-set-list.md).

## Parámetros de sombreado

![](../../assets/shader-parameters-1.png)

Los parámetros de sombreado dependen del archivo de sombreado cargado actualmente.

## Desplazamiento y teselación

![](../../assets/disp-parameters.png)

Desplazamiento y Mosaico son dos funcionalidades que se pueden utilizar para modificar la forma de un objeto y agregar más detalles.

* **Desplazamiento**: Empuje o desvíe la geometría en función de un canal de entrada.
* **Mosaico**: Subdivide la geometría para densificarla. Más densidad significa que el espaciado entre polígonos es más corto, lo que proporciona detalles más precisos.

En la bandeja hay disponible un filtro denominado &quot;**Height a normal**&quot; que se puede usar para obtener el mapa normal final (en caso de que la conversión nativa no sea lo suficientemente sólida).

### Desplazamiento

A continuación se muestra la configuración del Desplazamiento:

| *Configuración* | *Descripción* |
| --- | --- |
| <b> Canal de origen </b> | Canal en el que se basa la deformación de la malla. El valor predeterminado es Height, pero también se puede establecer en Desplazamiento. |
| <b>Unidad de escala</b> | Seleccione cómo se define la escala de desplazamiento:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normalizado: La escala de Desplazamiento </b>es relativa al tamaño del cuadro delimitador de la malla.</li> <li data-preserve-html="true"><b>Escena: La escala de Desplazamiento </b>es relativa a las unidades del archivo de escena importado.</li> <li data-preserve-html="true"><b>Tamaño físico (cm)</b>: La escala de desplazamiento se mide en cm en función del tamaño físico del objeto.</li> </ul> |
| <b> Cantidad de escala</b> | Controla la cantidad de deformación aplicada a la malla del proyecto en función de la unidad de escala seleccionada. |

>[!NOTE]
>
> Tanto la configuración de la <b>escena</b> como la del <b>Tamaño físico (cm) de la unidad de escala requieren que el modelo importado se haya preparado para las mediciones de tamaño físico. </b>Si las unidades no están configuradas correctamente en el archivo importado, o si el tipo de archivo importado no admite las unidades de tamaño físico, el desplazamiento seguirá funcionando, pero es posible que no proporcione los resultados adecuados para sus necesidades.

### Teselación

A continuación se muestran los ajustes de Teselación:

| *Configuración* | *Descripción* |
| --- | --- |
| **Modo de subdivisión** | Determina cómo se calcula la cantidad de subdivisión. Las configuraciones disponibles son:<ul data-preserve-html="true"><li data-preserve-html="true"> Uniforme (predeterminado) </li><li data-preserve-html="true"> Longitud del borde </li></ul> |
| **Recuento de subdivisiones** | (Modo Uniforme)De 1 a 32. Un valor alto produce más polígonos, lo que proporciona más detalles, pero puede introducir problemas de rendimiento. |
| **Longitud máxima** | (Longitud de borde de modo)1 / Valor. Cada borde del polígono se divide hasta que cada segmento sea igual o menor que este número, siendo 1/1 el tamaño de la escena. |
