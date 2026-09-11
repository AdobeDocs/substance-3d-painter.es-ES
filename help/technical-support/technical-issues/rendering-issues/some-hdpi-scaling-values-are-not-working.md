---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/rendering-issues/some-hdpi-scaling-values-are-not-working.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo solucionar problemas de valor de escala HDPI en Substance 3D Painter para una compatibilidad de pantalla adecuada de alta resolución.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Some HDPI scaling values are not working
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Algunos valores de escala HDPI no funcionan
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
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
