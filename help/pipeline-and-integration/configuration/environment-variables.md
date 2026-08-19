---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/pipeline-and-integration/configuration/environment-variables.html"
breadcrumb-title: ''
description: Aprenda a utilizar variables de entorno en Substance 3D Painter para configurar el comportamiento de la aplicación y la integración de canalización.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Environment variables
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Variables de entorno
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 3%

---


# Variables de entorno

Esta página muestra variables de entorno que se pueden utilizar para anular el comportamiento predeterminado de la aplicación.

| Variable | Descripción | Versión |
| --- | --- | --- |
| **SUBSTANCE\_PAINTER\_LICENSE** | Valor: Ruta directa a un archivo de licencia.Permite anular la ubicación predeterminada del archivo de licencia. Ejemplo : si el archivo de licencia está en **H:/allegorithmic/licenses/substance\_painter.key**, los datos de la variable deben ser **&quot;H:/allegorithmic/licenses/substance\_painter.key&quot;**.  **Nota:** Use SUBSTANCE\_PAINTER\_2\_LICENSE en su lugar para una versión anterior a la 3.x (2017.x). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALLEGO\_LICENSE\_IDLE\_DELAY** | Valor: 7200Especifique el tiempo en segundos antes de liberar una licencia de licencia en el caso de una configuración de varios usuarios. El valor predeterminado es de 2 horas (7200s). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_SKIP\_CHECK\_FOR\_UPDATES** | Valor : 0 o 1 (1 = Desactivar comprobación de actualizaciones)Permite omitir la comprobación de actualizaciones cuando se inicia la aplicación. Deshabilite el panel Novedades . | <ol data-preserve-html="true"><li data-preserve-html="true">2.2</li></ol> |
| **SUBSTANCE\_PAINTER\_SVT\_HARDWARE\_ACCELERATION** | Valor: 0 o 1 (1 = Activado) Utilice la función Dispersión en la GPU. Si la GPU o el sistema operativo no admiten esta configuración, se omitirá. Para configuraciones de hardware compatibles, consulte la documentación : [Texturas virtuales dispersas](../../features/sparse-virtual-textures.md)Esta variable invalida el parámetro disponible en la ventana [Configuración](../../interface/settings/settings.md). | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_TEMP\_LOCATION** | Valor: Ruta de acceso directa a una carpetaDefine dónde debe escribir el Substance Painter sus archivos temporales (incluida la caché SVT). Esta variable invalida el parámetro disponible en la ventana [Configuración](../../interface/settings/settings.md). | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_PREVIEWS\_MEMORY\_BUDGET** | Valor: 500Define la cantidad de memoria (Ram) que la aplicación puede utilizar para cargar y almacenar previsualizaciones temporales desde la ventana Activos. Cuando se alcanza el límite del presupuesto, se descargan las previsualizaciones antiguas. Este valor solo controla la visualización de las previsualizaciones en la ventana Activos.El valor se define en megabytes. El valor predeterminado es 500 MB. | <ol data-preserve-html="true"><li data-preserve-html="true">2</li></ol> |
| **SUBSTANCE\_PAINTER\_PLUGINS\_PATH** | Ubicación de los complementos adicionales de Python. | 6.1 |
| **PYTHONPATH** | Módulos adicionales de Python para cargar con la integración de Python de la aplicación. Para obtener más información, consulte [Carga de módulos externos de Python](https://helpx.adobe.com/es/substance-3d/unlisted/documentation/spdoc/loading-external-python-modules-205363420.html). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **OCIO** | Ruta de acceso a un archivo **config.ocio** que se usará para controlar la configuración de [administración de color](../../features/color-management/color-management.md) con OpenColorIO.  **Nota:** Esta variable de entorno tiene prioridad sobre la variable **PAINTER\_ACE\_CONFIG**. | <ol data-preserve-html="true"><li data-preserve-html="true">4</li></ol> |
| **PAINTER\_ACE\_CONFIG** | Ruta de acceso a un archivo json que se usará para establecer la configuración de [administración de color](../../features/color-management/color-management.md) con ACE de Adobe. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_DISABLE\_SPECIFIC\_FEATURES** | Deshabilite varias funcionalidades dentro de las aplicaciones:<ul data-preserve-html="true"><li data-preserve-html="true">Vínculos a recursos externos (ayuda, páginas web, ejemplos, etc.)</li><li data-preserve-html="true">Desactivar comprobaciones de actualizaciones</li><li data-preserve-html="true">Deshabilitar el envío de estadísticas de uso</li><li data-preserve-html="true">Desactivar exportación a Substance share</li><li data-preserve-html="true">Desactivar los paneles Bienvenido y Novedades</li></ul> | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_DEBUG\_FPS** | Mostrar dentro de la ventana gráfica un contador de cuántos fotogramas por segundo procesa la ventana gráfica. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_PAINTER\_VRAM\_BUDGET** | Especifique la cantidad de memoria de GPU que puede utilizar Painter. Esto define un presupuesto global en MB. Por ejemplo, para definir un límite de 4 GB, utilice el valor 4000. También se puede utilizar un argumento de línea de comandos para realizar la misma acción. Consulte [Líneas de comandos](command-lines.md). | <ol data-preserve-html="true"><li data-preserve-html="true">2.1</li></ol> |
