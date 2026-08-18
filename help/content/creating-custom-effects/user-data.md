---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/user-data.html"
breadcrumb-title: ''
description: Aprenda a utilizar los datos de usuario en efectos personalizados para Substance 3D Painter para pasar información personalizada a los efectos de sombreado.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > User data
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Datos del usuario
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 1%

---


# Datos del usuario

En esta página se describen las propiedades personalizadas (datos de usuario) que se pueden añadir en el gráfico del Substance para ejecutar comportamientos específicos.\
La configuración de los datos de usuario se suele aplicar a los nodos de entrada o salida de un gráfico para indicar cómo debe interpretarlos la aplicación. Esto permite solicitar que la entrada de un gráfico sea de cierta manera para aplicar efectos es un contexto conocido (ej: solicitar un espacio de color específico) o para indicar cómo se realizó una salida en caso de que la aplicación tuviera que aplicar conversiones adicionales posteriormente.

* La configuración de datos de uso se define como **key = value**
* Los valores de configuración múltiples están separados por un punto y coma ( **;** )

## Espacio de color

La configuración de **espacio de color** se puede usar para solicitar entradas de gráficos del Substance con un espacio de color específico o para definir una salida configurada de una determinada manera. Por ejemplo, se especifica el formato de la salida normal del mapa.

Sintaxis de ejemplo: **colorspace=$working**

Introducción a Contextos:

* **Botón Color**: Widget de botón de color en las propiedades de un gráfico de Substance.
* **Entrada/salida de gráfico**: nodo de entrada o salida de un gráfico conectado a un canal (por ejemplo: ColorBase).
* **Entrada de imagen**: entrada genérica de un gráfico, no relacionada con canales específicos.

>[!NOTE]
>
> Con la introducción de la gestión de color, han cambiado varios comportamientos relacionados con el ajuste de los espacios de color:
> 
> * En la tabla siguiente se enumeran primero los ajustes de espacio de color compatibles anteriores a la versión 8.1. La segunda sección es exclusiva para la versión 8.1 y posteriores.
> * En cuanto a los contextos en los que se puede utilizar la configuración de espacio de color, sólo desde la versión 8.1 puede el botón de color definir un espacio de color. En versiones anteriores se suponía que estaban en el espacio de visualización (sRGB).
> 
> Las transformaciones y el espacio de color **snorm** y **unorm** no deben mezclarse con formatos de textura de GPU, su propósito es diferente.

| ColorSpace | Disponibilidad de contexto | Descripción |
| --- | --- | --- |
| **auto** | Botón de color Entrada/salida de gráfico Entrada de imagen | Predeterminado. La aplicación decide la conversión del espacio de color que se va a realizar en función de las propiedades del nodo de entrada y de la imagen conectada a la entrada. |
| **lineal** | Botón de color Entrada/salida de gráfico Entrada de imagen | Estándar sRGB IEC 61966-2-1:1999 espacio de color con una curva de gamma/tono lineal. Solo disponible con el modo de administración de color **Heredado**. |
| **srgb** | Botón de color Entrada/salida de gráfico Entrada de imagen | Espacio de color estándar sRGB IEC 61966-2-1:1999. Solo disponible con el modo de administración de color **Heredado**. |
| **passthru** | Botón de color Entrada/salida de gráfico Entrada de imagen | Obsoleto. Se interpreta como **lineal** en el modo de administración de color heredado y como **raw** con OCIO/ACE. Debe reemplazarse por **raw**. |
| **snorm** | Entrada/salida de gráfico Entrada de imagen | Firmado normalizado. Solicitar que la imagen de entrada esté en el rango [0, 1]. Para imágenes de entrada de 8 bits, esto significa que el valor medio es 127. Para las entradas de imagen flotantes, el centro es de 0,5 y no realiza ninguna sujeción. |
| **normalxyzright** | Entrada/salida de gráfico Entrada de imagen | Formato de mapa de normales OpenGL. |
| **normalxyzleft** | Entrada/salida de gráfico Entrada de imagen | formato de mapa de normales de DirectX. |
|  |  |  |
| **uniformar** | Entrada/salida de gráfico Entrada de imagen | Entrada flotante, sin rango/sujeción. |
| **datos** | Botón de color Entrada/salida de gráfico Entrada de imagen | Normalizado o flotante sin firmar. Información sobre colores distintos. |
| **raw** | Botón de color Entrada/salida de gráfico Entrada de imagen | No se aplica ninguna transformación de color cuando se utiliza este ajuste. |
| **$standardsrgb** | Botón de color Entrada/salida de gráfico Entrada de imagen | Espacio de color estándar sRGB IEC 61966-2-1:1999. |
| **$working** | Botón de color Entrada/salida de gráfico Entrada de imagen | El espacio de color de trabajo depende de la configuración de gestión de color. Será idéntico a los datos para canales no gestionados de color y mono-canal (esténcil, alfa, máscara) |
| **$raw** | Botón de color Entrada/salida de gráfico Entrada de imagen | Alias de **raw**. |
| **$auto** | Botón de color Entrada/salida de gráfico Entrada de imagen | Alias de **auto**. |

## modo de Alpha

El valor **alpha** se puede usar para especificar cómo se combina el alfa de una entrada o salida de color (RGBA).

Sintaxis de ejemplo: **alfa=premultiplicado**

| Configuración | Descripción |
| --- | --- |
| recto | Solicite o defina el alfa como recto. |
| premultiplicado | Solicite o defina el alfa como premultiplicado. |
| ninguno | Passthrough, utilice el alfa dado tal cual. |

>[!NOTE]
>
> El canal **Opacidad** se considera **recto** de forma predeterminada.

## Color predeterminado de entrada de imagen

El color predeterminado de la entrada de imagen de un gráfico de Substance es negro con su alfa definido en 0. El valor **defaultcolor** permite definir un valor diferente cuando la entrada de imagen de un gráfico está vacía

Para especificar el color se pueden utilizar valores flotantes (rango [0, 1]) o valores enteros (rango [0, 255]). Cada valor de componente está separado por una coma, mientras que el valor de coma flotante utiliza un punto como separador decimal. Si un valor flotante no tiene punto, se considerará un entero.

Sintaxis de ejemplo:

* **defaultcolor=(1.0,0.5,0.0)**
* **defaultcolor=(0,128,255)**

## Relleno de entrada de imagen

De forma predeterminada, las entradas de imagen de una gráfica de Substance no tienen relleno, ya que el área fuera de la Isla de UV suele rellenarse con un color uniforme por motivos de rendimiento. El ajuste de relleno se puede usar para solicitar una dilatación infinita, que se puede usar para filtros para evitar crear costuras, por ejemplo.

Sintaxis de ejemplo: **p****adding=extend**

## Deshabilitar una salida de forma predeterminada

Al añadir una sustancia a una ranura (como la ranura de material de la herramienta de una capa de relleno), es posible especificar mediante el campo de texto de metadatos para no activar un canal específico :

* En un nodo de salida específico (como un material):  **disable=(true)**
* En un nodo de salida genérico (como un filtro):  **disable=(height,diffuse,specular)**

Al cargar la sustancia, este canal no se activará en la interfaz de usuario y, por lo tanto, no tendrá ningún efecto en la pila de capas. El usuario aún puede volver a activar el canal.

## Designación de una salida como máscara/alfa común

La salida de un gráfico de Substance se puede utilizar como canal alfa/máscara compartida en las otras salidas.

Hay dos formas de hacerlo:

* Cree un nodo de salida con el identificador **channels\_Alpha**
* O bien, agregue los siguientes datos de usuario en un nodo de salida específico:  **IsChannelsAlpha=true**

Pueden aplicarse algunas condiciones:

* Si existe un nodo de salida con el identificador **channels\_Alpha** y otras salidas no tienen los datos de usuario, este nodo se utilizará como máscara de canales.
* Si una salida tiene los datos de usuario, se usará como máscara de canales mientras no exista el nodo **channels\_Alpha**.
* Si existe un nodo **channels\_Alpha** y un nodo con los datos de usuario, se utilizará primero el nodo de salida **channels\_Alpha**.
* Si varios nodos tienen los datos de usuario, el primer nodo encontrado por la aplicación se utilizará como máscara de canales. El orden en el que se encuentran las salidas no está garantizado al mismo que el definido por el gráfico del Substance.

>[!NOTE]
>
> Esta configuración solo se aplica al gráfico de Substance utilizado en **modo de material**. No se aplica a filtros, generadores, etc.

## Definir modo de fusión predeterminado para salidas de material

Es posible definir cuál debe ser el modo de fusión de una salida específica en una gráfica de Substance al arrastrar y soltar materiales de la estantería en la ventana gráfica o la pila de capas.

* En un nodo de salida específico:  **blendingmode=normal**

Lista de modos de fusión admitidos:

* normal
* paso
* desactivar
* reemplazar
* multiplicar
* dividir
* inversedivide
* oscurecer
* aligerar
* lineardodge
* restar
* inversesubtract
* diferencia
* exclusión
* signeaddtion
* superponer
* pantalla
* quemadura lineal
* colorburn
* esquivar
* softlight
* luz intensa
* vividlight
* claraboya
* matiz
* saturación
* color
* valor
* normal, combinar
* detalle normal
* normalinversedetail
