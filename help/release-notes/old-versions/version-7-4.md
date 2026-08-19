---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/release-notes/old-versions/version-7-4.html"
breadcrumb-title: ''
description: Consulte las notas de la versión 7.4 de Substance 3D Painter para obtener más información sobre las nuevas funciones, mejoras y correcciones de errores.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 7.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versión 7.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1910'
ht-degree: 0%

---


# Versión 7.4

**Substance 3D Painter 7.4** agrega compatibilidad con OpenColorIO con la introducción del nuevo flujo de trabajo de administración de color.

Fecha de publicación: *24 de noviembre de 2021*

## Funciones principales

### Nueva gestión de color

![](../../assets/banner-cm.jpg)

Esta versión presenta la administración de color con la compatibilidad de [OpenColorIO](https://opencolorio.org/) (OCIO para abreviar) versión 2.

Este nuevo flujo de trabajo permite gestionar y calibrar los colores desde la importación hasta la exportación, así como dentro del puerto de visualización, lo que permite hacer coincidir cualquier contenido en diferentes aplicaciones con mayor facilidad.

* **Configuración del proyecto**\
  Al crear un nuevo proyecto, ahora es posible activar la gestión de color. El proyecto existente también puede activar la gestión de color a través de la configuración del proyecto.\
  Para habilitar la administración de color, cambie de **Legacy** (predeterminado) a **OpenColorIO** y use una de las configuraciones predeterminadas o una personalizada.

  ![](../../assets/cm-settings.png){width="400px"}

* **Configuración de visualización del área de visualización**\
  En la parte superior de las vistas 2D y 3D hay dos controles para la gestión de color:\
  **Botón Color**: active o desactive la transformación de color de la ventana gráfica.\
  **Menú desplegable de transformación de visualización**: seleccione qué transformación de visualización desea utilizar para convertir los colores.

  ![](../../assets/cm-viewport.jpg){width="500px"}

* **Configuración del selector de color**\
  Cuando la gestión de color está activada, los selectores de color ofrecen nuevos controles. Los colores se editan en el espacio de color de trabajo especificado por la configuración.\
  Debajo de los reguladores de HSV/RGB se muestra el valor de color final, transformado desde el espacio de trabajo al espacio de color de visualización.

  ![](../../assets/color-picker-demo.png)

  ![](../../assets/cm-picker-display-value.png)

* **Importar mapas de bits y materiales de Substance con espacio de color personalizado**\
  Hay disponibles configuraciones dedicadas para especificar cómo se deben manejar los recursos, incluyendo cómo se debe interpretar la salida de materiales de Substance.\
  También es posible saber qué espacio de color está usando un recurso analizando su nombre de archivo.

  ![](../../assets/auto-color-space.png)

* **Configuración de exportación**\
  Al exportar texturas, los canales con gestión de color mostrarán en sus nombres de archivo el nombre del espacio de color utilizado con la ayuda de la nueva palabra clave **$colorSpace**.

  ![](../../assets/export-list-1.png){width="250px"}

  ![](../../assets/export-list-2_1.png)

>[!NOTE]
>
> Para obtener más información sobre cómo funciona la administración de color dentro de la aplicación, consulte la [página dedicada](../../features/color-management/color-management.md).

### Nuevo desacoplamiento de la ventana gráfica 2D y 3D

![](../../assets/banner-undock.jpg)

Las vistas 2D y 3D ahora se pueden desacoplar para moverlas a otro lugar. Por ejemplo, teniendo la vista 3D en una pantalla principal mientras la vista 2D se encuentra en otra pantalla.

Trabajar con una vista desacoplada es más fácil para organizar el diseño de la aplicación y estar al tanto de las cosas sin perder demasiada área de pintura.

* **Desacoplar una vista**\
  Para desacoplar una vista, simplemente abra el menú Ver y elija una de las dos opciones. Cada opción abre una nueva ventana con su vista dentro, mientras que la otra vista permanece acoplada dentro de la interfaz principal.

  ![](../../assets/undock-menu.png)

* **Intercambiar incluso con una vista no acoplada**\
  Mientras una vista no esté acoplada, la acción de intercambio del menú de vistas se puede utilizar para intercambiarlas.

  ![](../../assets/swap-undock.gif){width="500px"}

* **Compatible con la administración de color**\
  La vista desacoplada tiene su propia transformación de visualización de gestión de color, lo que facilita su administración en diferentes monitores.

  ![](../../assets/false-colors-undock.jpg){width="500px"}

### Nueva compatibilidad con SpaceMouse® de 3Dconnection

![](../../assets/spacemouse-banner.jpg)

**SpaceMouse®** es un dispositivo con conexión 3D que permite manipular la cámara de la ventanilla 3D de una manera más intuitiva y fácil. Ahora es compatible de forma nativa y directa plug and play con Painter.

Para obtener más información, consulte la [página de documentación](../../features/spacemouse-by-3dconnexion.md) dedicada.

>[!NOTE]
>
> * Disponible con la versión 7.4.2 y superior.
> * Asegúrese de instalar los controladores SpaceMouse® más recientes para beneficiarse del esquema de control de Painter.

### Nuevo contenido

![](../../assets/banner-content-4.jpg)

Se ha añadido un nuevo conjunto de activos al contenido predeterminado disponible con la aplicación:

* Nuevas pegatinas, herramientas preestablecidas y filtros (de **Käy Vriend**):
  * **Calcomanías**
    * Cicatriz recta simple
    * Parche de bolsillo normal
  * **Ajustes preestablecidos**
    * Cinta avanzada con cremallera
    * Parada avanzada de cremallera
    * Regulador avanzado de cremallera
    * Cordón de apriete
    * Cordón de apriete Ojete
    * Estrellas brillantes doradas
    * Fiesta de brillo
    * Puntos de brillo pastel
  * **Generador**
    * Inflar Encoger/Envolver

* Nuevos mapas de bits de suciedades (de **Emiel Sleegers**):
  * Suciedad Yeso de pintura
  * Yeso de suciedad descolorido
  * Pintura suciedad pelada
  * Humedad de la suciedad
  * Pelusa de suciedad
  * Suciedad Cobweb
  * Bush de suciedad
  * Suciedad Madera blanda
  * Papel suciedad rasgado
  * Suciedad agrietada profundamente
  * Suciedad Dust cepillado

### Desempaquetado automático de UV mejorado

![](../../assets/banner-uv-1.jpg)

El desempaquetado automático de UV se ha actualizado con una nueva opción que mejora el soporte de los modelos 3D con superficies extendidas.

Esta nueva configuración denominada **Evitar Islas de UV alargadas** aprovecha mejor el espacio UV dividiendo Islas de UV que podrían ser demasiado largas.

A continuación se muestra un ejemplo de esta nueva configuración sin usarla frente a usarla:

![](../../assets/uv-before-after.jpg){width="500px"}

### Scripts de Python mejorados

![](../../assets/banner-python-1.jpg)

La API de Python tiene un nuevo método que permite llamar a la API de Javascript.

Este nuevo método facilita la migración de complementos antiguos a la nueva API de Python. También desbloquea algunas características como la administración de **Baking** y **Shader** que aún no se han expuesto en Python.

Para ejecutar un comando Javascript desde Python, use la función **evaluation()** del nuevo submódulo **js**. Puede encontrar más información en la documentación de la API (disponible a través del menú Ayuda de la aplicación).

## Notas de la versión

### 7.4.2

*(Publicado El 8 De Marzo De 2022)*

**Agregado:**

* [SpaceMouse] [Windows] Compatibilidad con la conexión 3D de SpaceMouse en el área de visualización 3D para la navegación
* [SpaceMouse] [Windows] Métodos abreviados/teclas básicos para los modelos Pro y Enterprise SpaceMouse en la ventana gráfica 3D
* [SpaceMouse] [Windows] Icono de centro de rotación dedicado en la ventana gráfica 3D
* [Gestión de color] Utilice las funciones de la configuración de OCIO para cambiar la configuración predeterminada
* [Gestión de color] Gestión de color de la ventana de propiedades para widgets de color
* [Gestión de color] Gestión de color de la ventana de propiedades para la previsualización de materiales
* [Gestión de color] Gestión de color de muestras en el selector de color
* [Gestión de color] Añadir un ajuste para definir el espacio de color sRGB estándar
* [Gestión de color] Añadir el espacio de color sRGB estándar desde la configuración de OCIO en el selector de color Lista de selectores de visualización
* [Gestión de color] Mejoras en el menú de anulación del espacio de color
* [Gestión de color] Permita anular el espacio de color del mapa de entorno en Ajustes de visualización.
* [Gestión de color] Dibujo de degradados del selector de color en función de la visualización actual
* [Gestión de color] Fijar valores HDR de forma predeterminada en el editor de color
* [Gestión de color] Usar passthrough (sin espacio de color) para filtros en modo heredado
* [Gestión de color] Limitar la visualización de degradados en el editor de color para que coincidan con el rango [0-1]
* [Gestión de color] Ocultar el selector de visualización en el selector de color en el modo Heredado
* [Administración de color] Convertir el campo hexadecimal del selector de color siempre en espacio de color sRGB
* [Gestión de color] Desactivar el menú desplegable de visualización del selector de color para canales de datos
* [Optimización] La cuadrícula de deformación vuelve a calcular únicamente los mosaicos UV cubiertos
* [Exportar] Permite exportar proyectos de azulejo UV para Sketchfab, USD y glTF
* [Scripting]&#x200B;[Python] Permitir el cambio de la función de asignación de tonos

**Corregido:**

* [Sketchfab] Al actualizar el modelo existente, se crea un nuevo modelo
* [Sketchfab] Bloqueo al buscar un modelo actualizado anteriormente
* Bloqueo al exportar a USD
* Bloqueo al crear una nueva instancia de sombreado en Máscara de geometría o cuando la geometría está oculta
* [Ventana Importar recurso] Bloqueo al cambiar el tipo de recursos importados
* Los mapas de malla normales se invierten cuando se utilizan en la pila de capas
* [Substance] No se tiene en cuenta el modo de fusión de datos de usuarios
* [Gestión de color] Los mapas de bits con espacio de color en el nombre de archivo se importan como secuencias de mosaico UV
* [Gestión de color] Las salidas con gestión de color del gráfico del Substance están en un espacio de color incorrecto
* [Gestión de color] La herramienta Relleno poligonal muestra un color incorrecto
* [Gestión de color] El asignador de tonos ACES se aplica a los canales en modo solo
* [Gestión de color] La previsualización de la iluminación de la esfera de la herramienta no está gestionada por color
* [Administración de color] [Exportar] Los mapas convertidos aplican una conversión incorrecta
* [Scripting]&#x200B;[Python]&#x200B;[Gestión de color] Los proyectos creados con plantillas y variables de entorno OCIO están en modo heredado
* [Scripting] [Python] No se puede utilizar la función de evaluación de JavaScript al inicio
* [Oferta de Adobe 3D] No se puede iniciar Painter si se utiliza la configuración regional con idiomas no admitidos de forma predeterminada

**Problemas conocidos:**

* Conexión 3D con SpaceMouse no compatible en MacOS
* [UI] Barra de desplazamiento horizontal con administración de color que aparece en algunos casos en la ventana de nuevo proyecto
* [Panaderos] El ajuste &quot;Normal promedio&quot; no tiene efecto en los proyectos de azulejo UV
* [Mac M1] Los materiales inteligentes no se muestran correctamente
* [Gestión de color] Los recursos utilizados en el modo de proyección no se administran por color en la superposición

### 7.4.1

*(Publicado El 14 De Diciembre De 2021)*

**Agregado:**

* [Gestión de color] Usar función de datos en nombres de archivo exportados
* [Gestión de color] Expanda la sección Gestión de color de forma predeterminada cuando OCIO está seleccionado en las nuevas ventanas de configuración de proyecto y proyecto
* [Gestión de color] Añadir ACES a un asignador en modo heredado
* [Gestión de color] Ajustar los valores de configuración predeterminados
* [Gestión de color]&#x200B;[Exportar] Rellenar $colorSpace en nombres de archivo para canales de datos
* [Exportar] Exportar proyecto de azulejo UV a Stager
* [Interoperabilidad] No disponible para las ediciones Steam y Substance
* [Interoperabilidad] Permitir el envío de un proyecto de mosaico UV a Stager

**Corregido:**

* [MacOS] [Bloqueo] Painter no se inicia con Catalina
* [Administración de color] [Bloqueo] Bloqueo aleatorio al reproducir con administración de color/tipo de datos en el canal de usuario
* [Gestión de color] Recursos utilizados como escala de grises en la máscara visualización del espacio de color nuevo menú
* [Gestión de color] El canal del usuario es más oscuro en la ventana gráfica en el modo heredado + vista en solitario
* [Gestión de color] El mapa Env siempre es lineal cuando se utiliza en iRay
* [Gestión de color] El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
* [Gestión de color] El selector de color se interrumpe en el interior de un Substance en modo heredado
* [Gestión de color] Al cambiar entre vistas de canal solo en la ventana gráfica, no se muestra con el espacio de color correcto al utilizar el menú desplegable
* [Gestión de color] La exportación aplica la conversión incorrecta en canales de usuario con gestión de color en modo heredado
* Los trazos realizados en la máscara de vista solo no se muestran al volver a la vista de material
* [Exportar] Los mapas convertidos no se exportan como canales con gestión de color
* [Conjunto de texturas] Falta la información sobre herramientas con el nombre original en los canales de usuario con nombre cambiado
* [Steam] Faltan archivos al comprobar su integridad con Steam

**Problemas conocidos:**

* [Mac M1] Los materiales inteligentes no se muestran correctamente

### 7.4.0

*(Publicado El 24 De Noviembre De 2021)*

**Agregado:**

* [Gestión de color] Compatibilidad con la gestión de color OpenColorIO versión 2
* [Gestión de color] Añadir ajustes de gestión de color a los ajustes del proyecto
* [Gestión de color] Ventana de advertencia sobre los cambios de configuración de la gestión de color al abrir un proyecto
* [Gestión de color] Mostrar un mensaje de error si se selecciona un archivo de configuración de OCIO no válido
* [Gestión de color] Permite anular la configuración con la variable de entorno OCIO
* [Gestión de color] Varias configuraciones OCIO integradas de forma predeterminada en la aplicación
* [Gestión de color] Extraer nombre de espacio de color del nombre de archivo de mapa de bits importado
* [Gestión de color] Permita anular el espacio de color con un espacio de color desde la configuración de la ventana Propiedades
* [Gestión de color] Añadir opciones de gestión de color en Configuración del conjunto de texturas
* [Gestión de color]&#x200B;[Ventana] Permitir la gestión de color de vistas 2D y 3D por separado
* [Gestión de color] Cargar y convertir mapa de entorno en el espacio de color de trabajo
* [Gestión de color] Ajuste el selector de color y el editor con el espacio de color actual
* [Gestión de color] Permite seleccionar el espacio de color de transformación de visualización en la ventana gráfica con un nuevo menú desplegable.
* [Gestión de color] Aplicación de la transformación de visualización con resultados de procesamiento de Iray
* [Gestión de color] Exportar texturas con diferentes espacios de color
* [Gestión de color] [Python] Aplicación de la configuración de gestión de color de la variable de entorno (OCIO) a proyectos nuevos
* [Ventana gráfica] Permite desacoplar la ventana gráfica 2D o 3D
* [Auto Unwrap] Nueva opción para evitar islas alargadas
* [Scripting Python] Llamar a funciones de JavaScript desde la API de Python
* [Nueva ventana de proyecto] Hacer que la sección de mapas importados sea contraíble
* [Proyección]&#x200B;[Deformar] Permite ocultar las normales como una opción en los ajustes de Deformación
* [Contenido] 11 nuevos mapas de suciedades
* [Contenido] 8 nuevos ajustes preestablecidos de herramientas (cremallera, cordón de apriete, brillo)
* [Contenido] 8 materiales nuevos (cicatriz, bolsillo, ...)
* [Contenido] 1 generador nuevo (inflar encogimiento)

**Problemas conocidos:**

* [Mac M1] Los materiales inteligentes no se muestran correctamente
* [Administración de color] [Bloqueo] Bloqueo aleatorio al reproducir con administración de color/tipo de datos en el canal de usuario
* [Gestión de color] El selector de color no selecciona el valor adecuado para el canal de datos en el modo heredado
* [Gestión de color] [Iray] Guardar el renderizado en EXR o TIFF mientras la Gestión de color está activada en la ventana gráfica siempre se guarda en lineal
* [Administración de color] Los recursos utilizados como escala de grises en la máscara muestran un menú de espacio de color incorrecto
* [Gestión de color] [Iray] El mapa Env siempre es lineal cuando se usa en Iray
* [Gestión de color] [Exportar] Los mapas convertidos no se exportan como canales con gestión de color
* [Gestión de color] [Exportar] La exportación ignora si el canal del usuario tiene gestión de color o no está en modo heredado
