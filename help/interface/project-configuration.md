---
helpx_url: 'https://helpx.adobe.com/es/substance-3d-painter/interface/project-configuration.html'
breadcrumb-title: ''
description: Aprenda a configurar los ajustes del proyecto en Substance 3D Painter para configurar la resolución de textura, los canales y las propiedades del proyecto.
helpx_creative_field: ''
helpx_description: Painter > Interface > Project configuration
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Configuración del proyecto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 3e4ef9bd5897f042b01d6c0819ec06cc21ba208a
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 3%

---


# Configuración del proyecto

![](../assets/project-configuration-full.png)

La ventana Configuración del proyecto dispone de controles para modificar la configuración del proyecto. La configuración del proyecto se establece generalmente al crear un nuevo proyecto, pero a veces puede ser necesario realizar cambios en esta configuración más adelante en el proyecto.

## Malla 3D

Si se han realizado cambios en la malla 3D o en el archivo de malla, puede volver a importar la malla mientras mantiene los demás datos del proyecto. Compruebe **Reimportar malla** y asegúrese de que se está importando el archivo correcto.

La reimportación de la malla suele ser útil cuando se necesita:

* Actualizar la topología del modelo 3D
* Actualizar las coordenadas UV
* Agregar o quitar [conjuntos de texturas](texture-set/texture-set.md)

| **Parámetro** | **Descripción** |
| --- | --- |
| **Malla 3D** | Indica la ruta de acceso al archivo de modelo 3D. Use el **botón Seleccionar** para cambiar el archivo de origen del proyecto. |
| **Volver a importar malla** | Si se habilita, el archivo de malla se volverá a importar al hacer clic en Aceptar en la parte inferior de la interfaz. Este parámetro se comprueba automáticamente si el botón Seleccionar se utiliza para especificar un archivo de malla diferente del archivo de malla original. |

>[!NOTE]
>
> Si los ID de material cambian o se les cambia el nombre al volver a importar la malla del proyecto, los conjuntos de texturas anteriores del proyecto pueden desactivarse, lo que da la apariencia de texturas que faltan. Esto se puede solucionar con la [Ventana de reasignación](texture-set/texture-set-reassignment.md) de la **Lista de conjuntos de texturas**.

## Configuración del proyecto

Esta sección controla varias configuraciones relacionadas con el proyecto:

<table>
  <tr>
    <th><em>Configuración</em></th>
    <th><em>Descripción</em></th>
  </tr>
  <tr>
    <td><strong>Formato de mapa de normales</strong></td>
    <td>Define el formato del mapa normal utilizado para la malla en la ventana gráfica. Este parámetro solo afecta a los <a href="shader-settings/shader-settings.md">sombreadores</a> en la ventana gráfica y a los mapas de malla en los <a href="../baking/baking.md">panaderos</a>. La pila de capas es independiente. Valor recomendado para aplicaciones comunes:<br><br><ul><li><strong>Unidad</strong>: OpenGL</li><li><strong>Motor irreal</strong>: DirectX</li><li><strong>Maya</strong>: OpenGL</li><li><strong>3DS Max</strong>: DirectX</li><li><strong>Mezclador</strong>: OpenGL</li></ul></td>
  </tr>
  <tr>
    <td><strong>Calcular espacio tangente por fragmento</strong></td>
    <td>Determina cómo calcular y mostrar mapas normales en la ventana gráfica para sombreado e iluminación. Si se activa, la tangente y los valores binormales de la malla se calcularán por píxel en lugar de por vértice.<br>Valor recomendado para aplicaciones comunes:<br><br><ul><li><strong>Unidad</strong>: Deshabilitado (habilitado si se usa HDRP)</li><li><strong>Motor irreal</strong>: Activado</li></ul></td>
  </tr>
</table>

>[!NOTE]
>
> Para cambiar el formato normal o el cálculo de la tangente es necesario volver a hornear los mapas de malla para garantizar que el aspecto en las ventanas gráficas sea correcto.

### Configuración específica de tipo de archivo

Cuando se selecciona un formato de malla USD, otros ajustes específicos del tipo de archivo quedan disponibles.

![](../assets/image2023-1-30-11-16-6.png){width="473px"}

<table>
  <tr>
    <th><em>Parámetro</em></th>
    <th><em>Descripción</em></th>
  </tr>
  <tr>
    <td><strong>Alcance y variantes</strong></td>
    <td>Seleccione una parte específica de un archivo USD. De forma predeterminada, se establece en "Root", lo que significa que se utilizará todo el archivo USD en el proyecto de Painter. <strong>Cambiar...</strong> abre una nueva ventana que muestra el contenido del USD. Si se detectan variantes, puede seleccionar una variante específica para cargarla en el proyecto.<br><br>Nota:<br><ul><li>Solo la selección de variante de modelado tendrá algún impacto.</li><li>Las variantes anidadas dentro de variantes no se detectan actualmente.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Nivel de subdivisión</strong></td>
    <td>Se aplica a la geometría que tiene subdivisión. Especifique cuánto se debe subdividir la malla para aplicar texturas en Painter. Si subdivision se establece explícitamente en 'none' dentro del archivo USD, esta configuración estará atenuada. La subdivisión se aplica después del desenvolvimiento UV, por lo que no alteraría la forma de los UV de la malla.</td>
  </tr>
  <tr>
    <td><strong>Encuadre</strong></td>
    <td>Se aplica a los USD en los que se detecta la animación. Seleccione el marco que se cargará en el proyecto de Painter. Si no hay ninguna animación en el archivo USD seleccionado, esta configuración está atenuada.</td>
  </tr>
</table>

## Ajustes de azulejos UV

Esta sección tiene controles para alternar el uso de UDIM en el proyecto. No es posible cambiar esta configuración después de crear el proyecto, pero puede ver la configuración del proyecto aquí. Para obtener más información, consulte la [documentación de mosaicos UV](../features/uv-tiles/uv-tiles.md).

## Configuración de importación

Estos ajustes controlan cómo se importará la malla seleccionada:

| *Configuración* | *Descripción* |
| --- | --- |
| **Importar cámaras** | Si se habilita, las cámaras presentes en el archivo de malla también se importarán y estarán disponibles en la ventana gráfica 3D. |
| **Conservar posiciones de trazos en la malla** | Este ajuste controla cómo se vuelven a calcular los trazos de pincel después de importar una nueva malla 3D. Se recomienda mantener esta configuración habilitada en la mayoría de los casos. Para obtener más información, consulte la documentación de [Reproyección UV](../features/uv-reprojection.md). |
| **Desempaquetar automáticamente** | Desempaquetado automático de UV. Haga clic en el botón Opción para configurar el proceso. Para obtener más información, consulte la [documentación sobre el desajuste automático de UV](../features/automatic-uv-unwrapping.md). |

### configuración de tamaño físico

Ajuste el [Tamaño físico](../features/physical-size.md) de la malla importada.

| *Configuración* | *Descripción* |
| --- | --- |
| **Usar escala de unidad interna del archivo de malla** | Si la malla se ha creado con medidas físicas precisas, deje esta opción seleccionada para mantener el mismo tamaño físico en Painter. |
| **Escala de unidad personalizada** | Si la malla no se ha creado teniendo en cuenta el tamaño físico, utilice esta opción para personalizar el tamaño de la malla. Deberá conocer el tamaño físico deseado y el tamaño en unidades de la malla importada para determinar este valor. |
| **Cambiar la escala de la capa de relleno a Tamaño físico al asignar materiales** | Cuando se activa, las capas de relleno y los efectos cambian automáticamente el método de escala a Tamaño físico al asignar un material que tiene propiedades de Tamaño físico. |

### Ajustes de gestión de color

Esta sección controla la configuración relativa a la conversión de colores. Para obtener más información, consulte la documentación de [Administración de color](../features/color-management/color-management.md).
