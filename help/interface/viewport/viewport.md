---
helpx_url: 'https://helpx.adobe.com/es/substance-3d-painter/interface/viewport.html'
description: Aprenda a utilizar la ventana gráfica de Substance 3D Painter para visualizar sus modelos y texturas 3D durante el proceso de pintura.
helpx_description: Painter > Interface > Viewport
title: Área de visualización
source-git-commit: 7b5f6e6c9623cb51253b6e49c8dbcbb22856418c
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 2%

---


# Área de visualización

![](../../assets/viewports-progress.jpg){width="600px"}

La ventana gráfica es donde se muestra la malla 3D y sus texturas. Aquí también es donde es posible pintar en la superficie de la malla 3D.

## Información general

El mirador se divide en cuatro partes:

* **Barra de herramientas contextual**: esta barra de herramientas se encuentra en la parte superior de la ventana gráfica y ofrece acceso directo a varias propiedades en función del contexto actual (por ejemplo, parámetros de pincel al pintar).
* **Vista 3D**: esta vista muestra la malla 3D desde un ángulo específico, definido por una cámara.
* **vista 2D**: esta vista muestra el desajuste UV de la malla 3D para el [conjunto de texturas](../texture-set/texture-set-list.md) seleccionado actualmente.
* **Barra de progreso**: esta barra gris/verde en la parte inferior de la ventana gráfica aparece cuando hay un cálculo en curso (por ejemplo, cuando el motor está generando texturas).

Para obtener más información, consulte las páginas dedicadas:

* [Vista 2D](2d-view.md)
* [Vista 3D](3d-view.md)
* [Gestión de cámaras](camera-management.md)

Las vistas 3D y 2D se pueden ajustar para mostrar información adicional o diferente mediante la [configuración de la pantalla](../../interface/display-settings/display-settings.md).

## Controles de navegación de ventana

Los controles para desplazarse por la ventana gráfica son similares en las vistas 2D y 3D.

<table>
  <tr>
    <th>Tipo de movimiento</th>
    <th>Método abreviado</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td>Orbitar/rotar<br></td>
    <td><strong>Alt + clic izquierdo</strong></td>
    <td><ul><li>Vista 3D: Orbitar la cámara alrededor de la posición del cursor.</li><li>Vista 2D: Gire el espacio UV alrededor de la posición del cursor.</li></ul></td>
  </tr>
  <tr>
    <td>Panorámica</td>
    <td><strong>Alt + clic central</strong></td>
    <td>Mueva la cámara hacia arriba, hacia abajo, hacia la izquierda o hacia la derecha.</td>
  </tr>
  <tr>
    <td>Zoom/efecto de cámara Dolly</td>
    <td><strong>Alt + clic derecho</strong></td>
    <td>Acerque o aleje el zoom de las mallas/UV.</td>
  </tr>
</table>

>[!NOTE]
> Tanto en las vistas 2D como en 3D, puedes ajustar a ángulos ortogonales al orbitar o rotar con **Alt + Mayús + clic izquierdo**.

## Cambio Del Diseño

El diseño predeterminado coloca la vista 3D a la izquierda y la vista 2D a la derecha. Hay algunos parámetros disponibles en la **Barra de herramientas contextual** que permiten cambiar el diseño:

<table>
  <tr>
    <th><em>Configuración</em></th>
    <th><em>Descripción</em></th>
  </tr>
  <tr>
    <td><strong>Modo de ventana gráfica</strong><br>![](../../assets/viewport-viewmode.png)</td>
    <td>Estos ajustes controlan el diseño de la ventana gráfica:<br><ul><li><strong>3D/2D</strong> (predeterminado): mostrar las vistas 3D y 2D en la ventana gráfica</li><li><strong>Solo 3D</strong>: maximice la vista 3D y oculte la vista 2D.</li><li><strong>Solo 2D</strong>: maximiza la vista 2D y oculta la vista 3D.</li><li><strong>Intercambiar 3D/2D</strong>: cambie el orden en el que se muestran las vistas. Si la vista 3D estaba a la izquierda, estará a la derecha después de elegir esta acción.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Modo de perspectiva</strong><br>![](../../assets/viewport-camera-projection.png)</td>
    <td>Estos ajustes controlan cómo aparecerá la malla 3D en la vista 3D:<br><ul><li><strong>Vista de perspectiva</strong> (predeterminada): muestra la malla 3D tal y como la vería el ojo humano o una cámara.</li><li><strong>Vista ortográfica</strong>: muestra la malla 3D, ya que cada dirección mide la misma longitud.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Modo de rotación de cámara</strong><br>![](../../assets/viewport-camera-axis.png)</td>
    <td>Esta configuración controla cuántos ejes puede rotar la cámara de la ventanilla.<br><ul><li><strong>Rotación gratuita</strong>: la cámara gira sobre los ejes X, Y y Z.</li><li><strong>Rotación restringida</strong> (predeterminado): la cámara gira únicamente en los ejes X e Y (sin desplazamiento).</li></ul></td>
  </tr>
  <tr>
    <td><strong>Modo de procesamiento</strong><br>![](../../assets/viewport-rendering.png)</td>
    <td>Cambie al <a href="../../features/iray-renderer/iray-renderer.md">modo de representación</a>.</td>
  </tr>
</table>
