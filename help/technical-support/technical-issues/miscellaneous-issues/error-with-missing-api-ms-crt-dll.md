---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/error-with-missing-api-ms-crt-dll.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo corregir los errores de DLL de api-ms-crt que faltan en Substance 3D Painter para obtener la compatibilidad adecuada con la biblioteca en tiempo de ejecución de Windows.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Error with missing api-ms-crt dll
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Error con la dll de api-ms-crt que falta
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Error con la dll de api-ms-crt que falta

Substance 3D Painter no se puede iniciar porque falta **api-ms-win-crt-runtime-l1-1-0.dll** en el equipo.\
Es muy probable que esto se deba a que la actualización KB2999226, que forma parte de **Visual C++ Redistributable** para Visual Studio 2015, no se pudo instalar.

## ¿Cómo se soluciona el problema?

### 1 - Compruebe que Windows esté actualizado

1. Abrir el menú Inicio
1. Seleccione Panel de control
1. Haga clic en **Windows Update**
1. Haga clic en **Buscar actualizaciones**
1. **Instalar** todas las actualizaciones disponibles.
1. Una vez instaladas las actualizaciones, **reinicie** el equipo.

Después del reinicio, repita los pasos anteriores hasta que no haya más actualizaciones disponibles.

### 2 - Instalar Visual C++ Redistributable

1. Descargue Visual C++ Redistributable :
   1. Para [Windows de 64 bits](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x64.exe)
   1. Para [Windows de 32 bits](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x86.exe)
1. Ejecute **vcredist\_x64.exe** (64 bits) o **vcredist\_x86.exe** (32 bits)
1. Seleccione Desinstalar y siga el procedimiento
1. Vuelva a ejecutar el ejecutable
1. Seleccione Instalar
