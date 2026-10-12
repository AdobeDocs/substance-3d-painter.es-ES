---
breadcrumb-title: ""
description: Aprenda a automatizar la instalación de Substance 3D Painter para la implementación empresarial y los flujos de trabajo de integración de canalización.
title: Instalación automatizada
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%
---

# Instalación automatizada

Al utilizar el instalador independiente de Substance 3D, es posible instalar la aplicación en modo silencioso para facilitar la implementación.

Estamos usando **InnoSetup** para generar el instalador. El conjunto completo de parámetros que se pueden usar con el instalador está [disponible aquí](http://www.jrsoftware.org/ishelp/index.php?topic=setupcmdline).

## Instalación en modo silencioso mediante la línea de comandos

El indicador que se debe usar para realizar una instalación silenciosa es **/SILENT**. El indicador **/NCRC** también se puede usar para omitir el CRC (verificación) del paquete con el fin de acelerar el proceso.

Ejemplo:

```
SubstancePainter_Installer.exe /NCRC /SILENT /DIR="C:InstallationFolder"
```


>[!NOTE]
>
> La ruta de instalación debe utilizar una barra invertida para separar las carpetas; de lo contrario, el instalador no la reconocerá.
