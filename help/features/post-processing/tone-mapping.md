---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/features/post-processing/tone-mapping.html"
breadcrumb-title: ''
description: Aprenda a utilizar el posprocesamiento de asignación de tonos en Substance 3D Painter para ajustar la exposición y la gradación de color en la ventana gráfica.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Tone Mapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Asignación de tonos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---


# Asignación de tonos

![](../../assets/tone-mapping.png)

Los parámetros de Asignación de tonos permiten controlar cómo se escalarán los colores para que se muestren en la pantalla. Estos ajustes pueden resultar útiles para redistribuir los colores debido a su amplia gama de valores (que puede superar lo que la pantalla actual puede mostrar).

>[!NOTE]
>
> Substance 3D Painter emite **HDR.** colores (Alto rango dinámico) (en el espacio de gamma lineal), pero la mayoría de las pantallas solo permiten visualizar colores **LDR** (bajo rango dinámico). Para asignar el rango de HDR al rango de LDR, se debe realizar una conversión. Este es el principio de la asignación de tonos.

| *Configuración* | *Descripción* |
| --- | --- |
| **Exposición** | Ajusta el HDR. el procesamiento del espacio produce resultados antes de aplicar efectos de deslumbramiento o realizar la asignación de tonos. |
| **Gamma** | Valor de gamma para la corrección de gamma. |
| **Función** | Función que se utiliza para asignar el rango de HDR al rango de LDR.  Las funciones disponibles son:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Automático </strong> : La función de mapa de tonos se selecciona automáticamente. El valor predeterminado es <strong> Sensitométrico </strong> . </li><li data-preserve-html="true"><strong> Lineal </strong> : El color de salida no se fija de 0 a 1 solo para este tipo. Esto es óptimo para cuando se implementa algún efecto en el espacio HDR. en el lado de la aplicación después de aplicar los efectos. <br/>No recomendamos esto a menos que tenga alguna razón específica para usarlo, porque los componentes de alta luminancia se perderán por completo y las iluminaciones se apagarán si se utiliza la asignación lineal como salida de pantalla final tal cual.</li><li data-preserve-html="true"><strong> LinearSat </strong> : Es casi igual que <strong> Lineal </strong> , excepto que el color de salida está sujeto. Además, la síntesis de destellos es un poco más suave que <strong> Lineal </strong> .</li><li data-preserve-html="true"><strong> Sensitométrico </strong> : Función predeterminada cuando se realiza el procesamiento de escenas en el espacio HDR.</li><li data-preserve-html="true"><strong> Reinhard </strong> : Esto da como resultado una asignación más gradual que <strong> Sensitométrica </strong> y un contraste ligeramente bajo. En consecuencia, hace que la resolución de los componentes de alta luminancia sea alta y que las variaciones de luminancia de las partes brillantes se reproduzcan más intensamente.</li><li data-preserve-html="true"><strong> ReinhardLum </strong> : Tipo para implementar el mapa de tonos <strong> de Reinhard </strong> con la luminancia como referencia y manteniendo la saturación original (intensidad: RGB). Asigna únicamente la información de luminancia al espacio LDR y, a continuación, reproduce la saturación original. La saturación en el espacio HDR. también se mantiene después de la asignación de tonos.</li><li data-preserve-html="true">Registro </strong> de <strong> : Esto da como resultado una asignación aún más gradual que <strong> Reinhard </strong> y un contraste bajo. Hace que la resolución de los componentes de alta luminancia sea alta y que las variaciones de luminancia de las partes brillantes sean más intensas.</li><li data-preserve-html="true">LogLum </strong> de <strong> : Tipo para implementar el mapa de tonos del espacio logarítmico con la luminancia como referencia y mantener la saturación original (intensidad: RGB). De este modo, solo se asigna la información de luminancia al espacio logarítmico y, a continuación, se reproduce la saturación original. La saturación en el espacio HDR. también se mantiene después de la asignación de tonos.</li></ul> |
| **Factor de asignación** | Esto controla el nivel máximo de luminancia (brillo) en el espacio HDR que se asigna al espacio LDR final en el proceso de asignación de tonos. Los colores son más brillantes que el HDR especificado. La luminancia del espacio no se puede representar en el espacio LDR, lo que provoca iluminaciones apagadas. En términos concretos, este valor es la luminancia (después de la escala de exposición) en el espacio HDR. que se asigna al valor de luminancia máximo (1,0) en el espacio LDR. En el modo de renderizado HDR, cuanto menor sea este valor, mayor será el contraste y mayor la probabilidad de que las iluminaciones se estropeen. Por el contrario, si se especifican valores más altos, se obtiene un contraste más bajo y se reduce la probabilidad de iluminaciones apagadas. En el modo de representación LDR, cuando se realiza una reasignación al espacio HDR para aplicar un efecto, el rango de luminancia se expande hasta el valor especificado en **Factor de asignación** . Por el contrario, la luminancia **Factor de asignación** se asigna a la luminancia LDR máxima durante la asignación de tonos.Es decir, especifica el factor de escala de rango dinámico aplicado a los resultados de procesamiento LDR para la aplicación de efectos. Al establecer este valor en alto, se enfatizan las regiones brillantes en los efectos.  **Nota:** Esta configuración no tendrá efecto (se omitirá) si la **función** está establecida en cualquiera de las siguientes en HDR modo de representación:  **Lineal**, **LinealSat** o **Sensitométrica** . |
