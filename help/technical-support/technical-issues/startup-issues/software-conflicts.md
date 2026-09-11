---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/technical-support/technical-issues/startup-issues/software-conflicts.html"
breadcrumb-title: ''
description: Obtenga información sobre cómo resolver conflictos de software que impiden que Substance 3D Painter se inicie correctamente en el sistema.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Software conflicts
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Conflictos de software
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---


# Conflictos de software

Esta página contiene una lista de problemas conocidos con otro software que pueden bloquearse o impedir que Substance 3D Painter se ejecute correctamente.

| *Posible origen del conflicto* | *Problema* |
| --- | --- |
| **Antivirus/Antispyware** | El software antivirus o antispyware puede crear algunos de los problemas siguientes:<ul data-preserve-html="true"> <li data-preserve-html="true"><b> Falso positivo</b>: Painter se marca incorrectamente como virus o malware.</li> <li data-preserve-html="true"><b> Archivos bloqueados</b>: Painter no puede leer ni escribir archivos (exportación, creación de ajustes preestablecidos, etc.).</li> <li data-preserve-html="true"><b> Eliminación de archivo</b>: Painter no puede iniciarse o funcionar normalmente porque se han eliminado los archivos necesarios.</li> </ul>Si se produce una de estas situaciones, se recomienda desactivar temporalmente el antivirus para ver si es útil o añadir excepciones manualmente para Painter. |
| **AMD CrossFire y NVIDIA SLI** | Painter no admite varias configuraciones de GPU, lo que provoca bloqueos. Se recomienda desactivar esta función. |
| <b> Asistente de Autodesk </b> | La aplicación Asistente de Autodesk puede crear conflictos y hacer que la aplicación se convierta en un bloqueo al inicio o al abrir un archivo de proyecto. Actualice la aplicación de Autodesk para resolver el problema. |
| <b> ordenadores Alienware/Dell</b> | Consulte esta página para obtener más información: [Bloqueo al abrir o guardar un archivo](../stability-issues/crash-when-opening-or-saving-a-file.md). |
| **APFS de Paragon Software** | Este software puede registrar una ubicación en la variable de entorno Windows Path que puede bloquear la aplicación al iniciarse. Es posible que la desinstalación del software no sea suficiente y que la variable de entorno deba eliminarse manualmente. Ejemplo de ubicación problemática:  `C:Program Files (x86)Paragon SoftwareAPFS for Windowsï–›éŒ à €è¸€ì‡ì‡ç¿¹` |
| **Avecto** | La ejecución de una versión anterior de Avecto puede provocar ralentizaciones y bloqueos. Asegúrese de actualizarlo a la versión más reciente. |
| **Ajuste de GPU de Asus** | Este software puede causar problemas durante la compilación de sombreadores en Substance 3D Painter o incluso impedir que se inicie la compilación de sombreadores. Si se produce este problema, recomendamos desinstalar el software para ver si se soluciona el problema. |
| **Asus RAMCache** | Este software puede impedir que Substance 3D Painter se inicie correctamente o hacerlo inestable mientras se ejecuta. Recomendamos desactivar o instalar Asus RAMCache si tiene problemas de estabilidad. |
| **Asus Sonic Suite** | En equipos con una placa base ASUS, <b>Asus Sonic Suite</b> se puede instalar de forma predeterminada. La desinstalación de este software puede corregir algunos problemas de visualización o interfaz en Substance 3D Painter. |
| **Software de copia de seguridad en la nube** **(** OneDrive,**GDrive,** **Dropbox,** **Filestream, etc.)** | El software de copia de seguridad en la nube puede ser la fuente de numerosos bloqueos al guardar un proyecto. Si esto sucede, se recomienda trabajar en el archivo de proyecto y guardarlo en una carpeta no sincronizada y, en su lugar, volver a copiar los archivos de proyecto en la unidad de nube una vez que los cambios ya no se realicen. |
| **Chitubox** | Este software puede crear un conflicto y poner en bloqueo la aplicación al abrir un cuadro de diálogo de archivo (como abrir o guardar un proyecto). Puede deshabilitar la configuración <b>Habilitar vista previa en miniatura del modelo de escritorio</b> en las preferencias de Chitubox para evitar este problema. |
| **Pantalla Duet** | Se sabe que <b>Duet Display</b> crea problemas de controladores de GPU que pueden afectar al comportamiento de Substance 3D Painter. Se recomienda desinstalarlo. |
| **Google Chrome** | Google Chrome puede causar algunos bloqueos al ejecutarse junto con Substance 3D Painter. Para mejorar la estabilidad de Substance 3D Painter, se recomienda actualizar Google Chrome y los controladores de la GPU. Si se siguen produciendo bloqueos, desactive Aceleración de hardware en Google Chrome (que hará que Chrome deje de utilizar la GPU). |
| **Software de audio nahimic** | <b>Nahimic</b> puede congelar o bloqueo el Painter. Detenerlo puede ayudar, y actualizarlo también puede evitar problemas. Nahimic también ejecuta servicios en segundo plano que pueden interferir con la aplicación y que pueden necesitar ser detenidos o deshabilitados. |
| **Software De Vídeo Openshot** | <b>Openshot Video Software</b> puede crear un conflicto con Substance 3D Painter con las vistas previas de la estantería. La actualización de Openshot debería solucionar el problema. |
| **Pyinstaller** | Esta aplicación puede producir una configuración de entorno incorrecta, lo que provoca un error al iniciarse. Para obtener más información, consulte [Error al iniciar la aplicación debido a Qt](application-failed-to-start-because-of-qt.md). |
| **Rptr / Plays.tv** | <b>Rptr</b> (o <b>[Plays.tv](http://plays.tv/) </b>) se instala de forma predeterminada con algunos controladores de GPU. Este software puede crear inestabilidad y bloqueo la aplicación. Se recomienda desinstalar la aplicación. |
| **RGBFusion** | Este software puede crear conflictos con los controladores de la tableta gráfica, detener el proceso puede corregir temporalmente el problema o desinstalar RGBFusion para una solución permanente. |
