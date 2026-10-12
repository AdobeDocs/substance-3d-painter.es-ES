---
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%
---
# Eliminar metadatos de HelpX heredados

Con Python 3.10 o posterior, ejecute los siguientes comandos desde la raíz del repositorio:

```shell
python remove_helpx_metadta.py 1 <path>
python remove_helpx_metadta.py 2 <path>
```

El modo `1` es un ensayo: muestra los archivos coincidentes e informa del número de archivos
archivos digitalizados, archivos con coincidencias y campos de metadatos coincidentes sin cambiar los archivos.
El modo `2` quita esos campos e informa de los recuentos de eliminación. Omitir `<path>` a
examinar la carpeta actual. Trazados de citas que contengan espacios.

El script analiza de forma recursiva `.md` archivos (no distingue entre mayúsculas y minúsculas) y elimina los archivos de nivel superior
Campos de materia frontal YAML cuyos nombres comienzan por `helpx`, incluido su multilínea
valores. Conserva otros metadatos, comentarios, líneas en blanco, contenido de marcado,
codificación y finales de línea. No quita `helpx` referencias en el cuerpo.
Revise la ejecución en seco antes de usar el modo `2`; eliminación edita archivos en su lugar sin
crear copias de seguridad. Los errores de archivo y las frentes no cerradas se notifican y generan
un estado de salida distinto de cero. Los archivos con contenido frontal no cerrado se dejan sin cambios.