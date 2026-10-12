---
breadcrumb-title: ""
description: Aprenda a corregir las previsualizaciones de recursos vacías y de estanterías en Substance 3D Painter para restaurar la funcionalidad de visualización de miniaturas.
title: Las vistas previas de activos (o estantes) están vacías
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%
---

# Las vistas previas de activos (o estantes) están vacías

Este problema puede deberse a otro software. Consulte: [Conflictos de software](../startup-issues/software-conflicts.md).

Si no es posible determinar qué software está actualizando o desinstalando, busque una variable de entorno denominada &quot;QT\_PLUGIN\_PATH&quot; y quítela.

**En Windows:**

1. Abra **Sistema** en el Panel de control.
1. En la ficha Avanzadas, haga clic en **Variables de entorno**
1. Busque la variable denominada **&quot;QT\_PLUGIN\_PATH&quot;**
1. **Quitarlo**
1. **Reiniciar** el equipo
