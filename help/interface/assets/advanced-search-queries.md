---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/assets/advanced-search-queries.html"
breadcrumb-title: ''
description: Aprenda a crear consultas de búsqueda avanzadas en Substance 3D Painter para encontrar recursos específicos mediante criterios de búsqueda complejos.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Advanced search queries
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Consultas de búsqueda avanzada
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Consultas de búsqueda avanzada

Las consultas de búsqueda avanzada le permiten crear búsquedas complejas y reutilizarlas como [búsquedas guardadas](saved-searches.md).

Las consultas avanzadas se pueden utilizar en la barra de búsqueda y pueden contener:

1. **Ruta** : permite refinar el resultado de una búsqueda por una estructura de carpeta/carpeta.
1. **Uso**: Enumerar todos los posibles usos disponibles en la aplicación
1. **Consulta de texto** : Permitir agregar cualquier otro tipo de consulta libremente (como palabras clave personalizadas)

Se permiten varias selecciones al definir una nueva consulta de búsqueda.

## Ruta

La consulta de ruta permite refinar una consulta basada en una ruta. El panel **Filtrar por ruta** muestra todas las bibliotecas disponibles (que puedes añadir tú mismo mediante Edición > Configuración > Bibliotecas).\
Es posible utilizar la definición de ruta para filtrar por ruta de biblioteca personalizada o por subcarpetas específicas de la jerarquía.

## Uso

El uso define qué es un recurso y cómo utilizarlo en Substance 3D Painter. Algunos se pueden definir por el tipo de archivo del recurso.\
Por ejemplo:

* **pbr.glsl**: Un archivo de sombreador - solo se puede utilizar como un sombreador, y nada más.
* **effect.sbsar**: Un archivo de substance: puede ser un generador, un filtro o incluso un material, por lo que, si su uso no se establece en el gráfico original (en Designer), el usuario deberá indicarlo en Painter en el momento de la importación.

## Texto

La consulta de texto admite varios tipos de filtrado, algunos de los cuales son más avanzados que la interfaz normal.\
Se pueden habilitar escribiendo las palabras clave correctas.

* **Tipos de búsqueda disponibles** :
  * &quot; **n:** &quot; : name
  * &quot; **s:** &quot; : estante/biblioteca (incluye &quot;sesión&quot; y &quot;proyecto&quot;)
  * &quot; **p:** &quot; : ruta
  * &quot; **u:** &quot; : uso
* **Escapando** : es posible utilizar &quot; **\**&quot; antes del carácter del que se debe escapar o utilizar comillas, por ejemplo:
  * **a\ nombre\ con\ espacios**
  * **&quot;un nombre con espacios&quot;**
* **Atributos (o grupo) específicos** : para buscar en atributos específicos, anteponga &#39;o grupo&#39; a un especificador de tipo. Ejemplo :
  * **n:a,b,c,d** : nombre es a o b o c o d
* **Comportamiento de búsqueda** :
  * Para filtrar usos específicos, agregue la **palabra clave** específica a su búsqueda, por ejemplo: &quot;**imágenes** ambiente&quot;
  * Para agregar varias solicitudes, use una coma &quot;**,**&quot;, por ejemplo: &quot;cobalt **,** oro&quot; (si se usa una coma, la búsqueda solo mostrará un recurso que coincida con ambas palabras clave al mismo tiempo)
  * Para buscar un nombre exacto, utilice un signo de exclamación &quot;!&quot; al final, ejemplo :  **di!**  (devolverá **dirt** pero no **goteos**, esta palabra clave deshabilita la coincidencia aproximada)
  * Para excluir un patrón de una búsqueda, utilice un guion &quot;**-** &quot;, por ejemplo:  **u:image n:-normal** (devolverá imágenes que no contienen &quot;normal&quot;)
* **Funciones coincidentes (sufijo de patrón):**
  * **valor predeterminado** : coincidencia aproximada (difusa)
  * **contiene** : !
  * **regex**: #
  * **igual** : =
  * **empieza por** : ^
  * **termina por** : &amp;
