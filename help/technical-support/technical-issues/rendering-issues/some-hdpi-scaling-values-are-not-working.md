---
breadcrumb-title: ""
description: Obtenga información sobre cómo solucionar problemas de valor de escala HDPI en Substance 3D Painter para una compatibilidad de pantalla adecuada de alta resolución.
title: Algunos valores de escala HDPI no funcionan
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%
---

# Algunos valores de escala HDPI no funcionan

En Windows, es posible que algunos valores de escala HDPI (utilizados para escalar la interfaz en monitores con resoluciones altas) no funcionen correctamente.\
Esto se debe a que nuestro marco de trabajo de ventana (Qt) no los admite. No podemos solucionarlo hasta que lo administren realmente los proveedores del propio marco.

Por lo tanto, este es el comportamiento que puede encontrarse en función de su configuración :

* 120 PPP (**escala del 125%**): se representa como 96 PPP (**escala del 100%**)
* 144 PPP (**escala del 150%**): se representa como 192 PPP (**escala del 200%**)
* 168 PPP (**escala del 175%**): se representa como 192 PPP (**escala del 200%**)

Para obtener más información, consulte: <https://bugreports.qt.io/browse/QTBUG-55654>
