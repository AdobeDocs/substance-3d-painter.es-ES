---
title: Corrección de sesgo
description: Aprenda a utilizar la corrección de sesgo para corregir defectos hechos un bake al utilizar un flujo de trabajo de alto a bajo nivel de poly en Substance 3D Painter.
source-git-commit: db1c8daa33389f21699c53b0d6555c153fbc66d6
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---


# Corrección de sesgo

<table>
  <tr style="border: 0;">
    <td style="border: 0; width: 35%" valign="top"><img src="../assets/baking/skew-correction-example.png" alt=""/></td>
    <td style="border: 0; width: 65%" valign="top">A veces, al hacer un bake a baja polietileno desde un modelo de alta polietileno, es posible que los detalles aparezcan deformados o sesgados. Esto suele ocurrir cuando las normales de la jaula y las normales de la superficie no se alinean bien. La hace un bake automática proyecta el nivel de poly alto en el nivel de poly bajo basándose en estos valores normales, por lo que si son incorrectos, la hace un bake produce resultados deficientes.<br>Afortunadamente, la corrección de sesgo (o la asignación de sesgo) está disponible para ayudar a corregir este tipo de artefacto.La corrección de sesgo de <br>Skew le permite pintar valores directamente en la malla de baja densidad para redirigir la proyección utilizada durante el horneado sin necesidad de crear una jaula personalizada.</td>
  </tr>
</table>

>[!NOTE]
>
> La corrección de sesgo se pinta dentro del **modo de Hacer un bake** y se almacena por conjunto de texturas.

## Pintar correcciones de sesgo

El dibujo con corrección de sesgo le permite ajustar manualmente las normales de la superficie de la malla específicamente para hacer un bake. Aunque puedes hacer correcciones de sesgo de pintura sin hacer un bake, puede ayudar a [hacer un bake primero tus mapas de malla](how-to-bake-mesh-maps.md).

![](../assets/baking/mode_select_buttons.png)

*Cambiar al modo de hacer un bake para obtener acceso a la configuración de corrección de sesgo.*

>[!IMPORTANT]
>
> La pintura con corrección de sesgo requiere los siguientes ajustes:
>
> * Es necesario seleccionar una escena High Poly. La pintura de sesgo solo está disponible al hacer un bake de alta a baja poli; Si se ha marcado **Usar malla de poli baja como malla de poli alta**, la pintura de corrección de sesgo **no** estará disponible.
> * **La jaula** se debe establecer en **basada en la distancia**.
> * **Se debe comprobar el promedio de normales**.

Con la configuración anterior, puedes hacer clic en **corrección de sesgo de Pintura** en el **panel de configuración común** para empezar a pintar. Cuando entras por primera vez en el modo de pintura de corrección de sesgo, **Auto-rebake** se activará automáticamente para el canal normal. Si lo prefieres, puedes desactivar **Volver a hacer automáticamente** o cambiar el canal seleccionado en el [**panel bakeres de mapa de malla**](../interface/baking-panels/mesh-map-bakers.md).

![](../assets/baking/skew-correction-menu.png)

### Herramientas de pintura

Al pintar correcciones de sesgo, puedes usar muchas de las herramientas y métodos abreviados a los que estás acostumbrado en el modo de pintura, incluidas las herramientas **Borrador** y **Relleno poligonal**.

* Puedes cambiar entre **Pincel**, **Borrador** y **Relleno poligonal** desde la barra de herramientas, o usar el [método abreviado estándar](../interface/settings/shortcuts.md) del modo de pintura.
* Al usar las herramientas Pincel o Borrador, puede ajustar el tamaño, flujo, opacidad y espaciado del pincel con los parámetros situados en la parte superior de la **Ventana gráfica**. También puede usar el [método abreviado de teclado](../interface/settings/shortcuts.md) correspondiente cuando esté disponible.

### Protección de los bordes

La protección de bordes ignora la corrección de sesgo pintada cerca de los bordes para mantener un degradado suave de normales de superficie. Puede alternar **Protección de bordes** en la sección **Corrección de sesgo**. Cuando **Corrección de bordes** está habilitado, puedes ajustar la distancia del borde y el contraste del borde para lograr resultados óptimos.

* Distancia de borde: Controle la distancia desde el borde hasta la que surte efecto la protección del borde.
* Contraste de bordes: Controle el degradado de protección de bordes. El bajo contraste produce un degradado más suave.

>[!TIP]
>
> Los valores de **Distancia de borde** y **Contraste de borde** dependen del tamaño de la malla. Para mallas con detalles muy pequeños en comparación con el tamaño de malla, puede ser más fácil introducir manualmente valores pequeños, en lugar de utilizar los reguladores.

>[!NOTE]
>
> La protección de bordes se basa en el mapa de malla de **bordes definidos**, que está vinculado a la geometría de la malla, no a los bordes UV.

### Visualización de vectores de sesgo

De forma predeterminada, cuando comience a pintar correcciones de sesgo, las normales de la superficie de malla se visualizarán en **Ventana gráfica** como líneas rojas, amarillas y verdes. Puedes modificar el aspecto de estas líneas o desactivarlas por completo en la sección **Vectores de sesgo** del **menú Visualizaciones** que aparece en **Ventana gráfica.**

![](../assets/baking/visualizations_menu.png)

* **Longitud de vectores**: Ajuste la longitud de las líneas en la ventana gráfica. Las líneas más largas pueden facilitar la comprensión de la dirección del vector.
* **Densidad UV de vectores**: Cambie el número de líneas a través de la superficie de la malla. Los vectores se colocan en el espacio UV, por lo que si la malla tiene una densidad de texel incoherente, el número de vectores por unidad de superficie variará según el tamaño del polígono en el mapa UV.
* **Opacidad de vectores**: Haz que los vectores sean más o menos transparentes.

El color de los vectores indica la cantidad de corrección de sesgo aplicada en cada posición del vector.

* Los vectores rojos indican que no hay corrección de sesgo; se utilizan las normales de superficie por defecto.
* Los vectores verdes indican que las normales de la superficie se corrigen completamente y son directamente perpendiculares a la superficie.

![](../assets/baking/skew-correction-painting.gif)*Pintar con un valor de flujo bajo proporciona un control preciso sobre la intensidad de la corrección de sesgo.*

## Optimizar el rendimiento

### Organizar UV

**La rehorneación automática** está optimizada para intentar limitar la rehorneación al área afectada por cada trazo de pincel al pintar correcciones de sesgo. Cuando se pintura un trazo, **Auto-rebake** dibuja un cuadro delimitador alrededor del trazo en el espacio UV y rehace todo lo que hay dentro del cuadro. Esto significa que si el trazo solo cubre una pequeña sección de espacio UV, solo se rehorneará una pequeña área, haciendo que la operación sea muy eficiente.

Sin embargo, si el trazo cruza dos Islas de UV en lados opuestos del espacio UV, incluso un trazo pequeño puede requerir retocar toda la textura, negando la optimización.

Como resultado, recomendamos organizar los UV de malla para que las Islas de UV cercanas entre sí en el espacio 3D también estén cercanas entre sí en el espacio UV. Esto mejora el rendimiento de **reprocesamiento automático**.

### Definir alineación en UV

En general, las correcciones de sesgo de pintura con **Proyección > Alineación** establecidas en UV tienen más rendimiento. Para cambiar la **alineación**:

1. Seleccione **Corrección de sesgo de Pintura** y equipe el **Pincel** o el **Borrador**.
1. Haga clic con el botón derecho en **Ventana gráfica** para abrir el **panel de configuración del pincel**.
1. Desplácese hacia abajo hasta **Proyección**.
1. Establezca **Alignment** en **UV**.

Con **Alignment** establecido en **UV**, es más difícil realizar trazos suaves en las costuras de las Islas de UV, sin embargo, esto suele ser menos importante al pintar correcciones de sesgo que al texturizar la malla.

>[!NOTE]
>
> Los parámetros del **Pincel** y el **Borrador** se almacenan por separado. Para maximizar el rendimiento de ambas herramientas, deberá establecer la **alineación** para cada una de ellas de forma individual.

## Correcciones de sesgo y la pila de deshacer

Hacer un bake y pintar comparten un único historial de deshacer. El cambio entre el modo de Hace un bake y el modo de pintura es en sí mismo un paso imposible de hacer, y la activación o desactivación de la corrección de sesgo también se puede deshacer. Cuando se deshace una acción al hacer un bake en el modo de pintura, el modo Hacer un bake se vuelve a abrir automáticamente antes de que se deshagan esos pasos, por lo que nunca se deshace una acción fuera del modo en el que ocurrió.