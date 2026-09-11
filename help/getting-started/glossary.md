---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/getting-started/glossary.html"
breadcrumb-title: ''
description: Acceda al glosario de Substance 3D Painter para comprender los términos y conceptos clave utilizados en toda la documentación.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Glossary
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Glosario
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2131'
ht-degree: 6%

---


# Glosario

Substance 3D Painter es una aplicación 3D que se basa en una gran cantidad de técnicas y palabras clave técnicas que pueden ser difíciles de entender al principio.\
En esta página se enumeran las palabras clave más comunes utilizadas por la aplicación, junto con una breve explicación del concepto subyacente.

| *Palabra clave* | *Definición* |
| --- | --- |
| **Alineación** | La alineación es cómo se orientará un pincel hacia la malla 3D al pintar. |
| **Alpha** | Un alfa es una máscara que se puede utilizar para pintura detalles o formas complejas, por ejemplo, un código de barras o un logotipo. |
| **Hacer un bake** | Un hacer un bake (o hacer un bake) se refiere a la acción de calcular información desde una malla 3D y guardarla en una Textura basada en la información UV de una malla. |
| **Profundidad de bits** | La profundidad de bits es la cantidad de información que se puede almacenar en una textura (por color). Cuanto mayor sea el número, mejor será la precisión de la información. Sin embargo, el rendimiento disminuye con números altos al realizar cálculos. |
| **Pincel** | Un pincel es una herramienta para pintar en una malla. Un pincel se define mediante varios parámetros que controlan su comportamiento (como el tamaño y la opacidad). |
| **Cámara** | La cámara es el objeto que permite controlar la posición y la dirección de dónde se mira en una ventana gráfica 3D o 2D. |
| **Canal** | Un canal es una textura con un comportamiento específico. Algunos canales se utilizan para definir el color de un material, mientras que otros se utilizan para controlar el comportamiento de la luz sobre una superficie. |
| **Clonar** | El clon es una herramienta que se utiliza para replicar parte de la textura/pintura en otra ubicación. |
| **Contenido/máscara** | El contenido y la máscara hacen referencia a las dos propiedades principales de una capa. El contenido es la pintura real almacenada en los canales contenidos en una capa, mientras que la máscara se utiliza para mostrar u ocultar el contenido. Una máscara negra es igual a un contenido invisible. |
| **Difusión** | La difusión es una forma de generar información fuera de la Isla de UV de una malla. Funciona mediante el sangrado de los últimos píxeles situados cerca del borde de una isla de UV, creando colores desenfocados. |
| **Dilatación / Relleno** | Partiendo de la misma idea que la difusión, la dilatación es una forma de generar información fuera de la Isla de UV mediante la ampliación de los colores de los píxeles. |
| **Efecto** | Un efecto es un elemento que puede añadirse a una capa, ya sea en el contenido o en la máscara. Substance 3D Painter admite varios tipos de efectos, como filtros. |
| **Entorno** | Un entorno es una imagen que se utiliza para calcular la iluminación de una escena; suele ser una textura HDR. que representa una amplia gama de información de color. |
| **Exportar** | La acción de exportar es la forma de generar texturas aplanadas a partir de la pintura realizada dentro de la aplicación. Las texturas creadas a partir de la exportación se pueden utilizar en otras aplicaciones. |
| **FOV / Campo de visión** | El FOV es la extensión del mundo observable por la cámara. |
| **Rellenar** | El relleno es una acción (que puede ser un efecto o una capa) que puede cargar un color, una textura o incluso un material sobre toda la malla 3D. |
| **Filtro** | Un filtro es un efecto Substance que puede modificar la información anterior. Por ejemplo, un filtro de desenfoque suavizará una imagen anterior. Los filtros también pueden ser más complejos y modificar un material completo. |
| **Filtrado** | Los filtros hacen referencia a la forma en que se muestran las texturas dentro de una ventana gráfica 3D. Los más comunes son los más cercanos (los píxeles se leen tal cual, haciendo que una imagen aparezca de forma muy aproximada) y los bilineales (los píxeles se interpolan, haciendo que una imagen aparezca borrosa de cerca). |
| **GPU** | La GPU (unidad de procesamiento gráfico) es la parte de un equipo que realiza cálculos rápidos para producir imágenes. |
| **Generador** | Un generador es un Substance que genera nueva información/imágenes, normalmente basándose en texturas adicionales. Por ejemplo, algunos generadores de máscaras utilizan la textura hecha un bake para crear máscaras complejas. |
| **Histograma** | Un histograma es una representación gráfica de la distribución de los valores de color. Se utiliza para visualizar cómo se equilibran los colores dentro de una imagen entre sombras, tonos medios e iluminaciones. |
| **Iray** | Iray es un procesador de trazador de trayectorias creado por NVIDIA, que se utiliza para proyectar una iluminación realista sobre la malla 3D. Dado que se trata de un procesador avanzado, se ha diseñado para crear imágenes atractivas y no para utilizarse en trabajo en tiempo real. |
| **Variación** | La variación es una propiedad del pincel que produce un comportamiento aleatorio al pintar. |
| **Capa** | Una capa es un elemento que contiene varios canales con propiedades adicionales, como un modo de fusión y una opacidad. |
| **Pila de capas** | Una pila de capas es un lugar en el que se pueden gestionar y organizar las capas. Las capas se organizan de abajo hacia arriba. La capa inferior se dibujará primero y, a continuación, cada capa superior se agregará una por una encima de la otra. |
| **Ratón perezoso** | El ratón perezoso es un comportamiento de la herramienta Pincel. Ralentiza la ruta del pincel para mejorar la precisión al pintar y crea un retardo o desplazamiento entre el cursor del ratón y la pintura real. |
| **Nivel** | Un nivel es un efecto que permite controlar una información de rango o color/escala de grises mediante un histograma. Se puede utilizar para invertir el color o oscurecer/aclarar el color, por ejemplo. |
| **Registro** | Un registro es un archivo de texto donde se escribe información del software, normalmente relacionada con el equipo que ejecuta la aplicación. |
| **Malla de poli alta/baja** | Una malla de poli baja y una alta son malla 3D, una es con una baja densidad de polígonos, mientras que la otra es con una mayor cantidad de policonte (a menudo 100 veces más grande). Por lo general, la información de malla alta se hace un bake a la malla baja. |
| **Material** | Un material define las propiedades para representar una materia específica. En una malla 3D, el material también se utiliza para definir grupos de caras de polígono. |
| **Malla** | Una malla es un objeto 3D definido por información múltiple. En Substance 3D Painter, una malla se define por polígonos (normalmente triángulos). Se puede crear una malla en una aplicación de modelado 3D como **Blender** o **Autodesk Maya** . |
| **Mapa de malla** | Un mapa de malla es un mapa creado a partir de una malla que contiene información relativa a la malla. Puede ser una información de posición o una información de oclusión, por ejemplo. |
| **Mapa-Mp** | Un mapa mip es una textura precalculada, que normalmente se presenta como una secuencia de imágenes cada vez con una resolución inferior a la de la textura original. |
| **Modo** | Un modo se refiere a la configuración de la interfaz que da acceso a un conjunto específico de herramientas y controles dependiendo del modo. |
| **Ruido** | Un ruido es una imagen de procedimiento y aleatoria, que normalmente representa formas orgánicas y valores de color/escala de grises. |
| **Normal** | Una normal es una textura especial que deforma el comportamiento de una luz en la superficie de una malla 3D para simular detalles que no existen en la geometría. |
| **OpenGL / DirectX** | OpenGL y DirectX son una interfaz de programación de aplicaciones (API) utilizada para procesar información 2D y 3D. También definen el formato de mapa de normales. |
| **Ortográfico** | Una proyección Ortográfica es un medio para representar objetos tridimensionales en dos dimensiones en las que todas las líneas de proyección son ortogonales al plano de proyección. |
| **PBR / PBS** | La representación basada en la física (PBR por sus siglas en inglés) o el Sombreado basado en la física (PBS por sus siglas en inglés) es un modelo de gráficos de ordenador que busca representar los gráficos de una manera que modele con mayor precisión el flujo de luz en el mundo real. |
| **Empaquetado** | El empaquetado es la acción de almacenar varias imágenes dentro de una textura. Dado que las texturas se componen de canales rojos, verdes y azules separados, pueden almacenar información diferente que se puede leer de forma independiente en otra aplicación. |
| **Partículas** | Las partículas son un tipo de herramienta que genera trazos de pincel basados en propiedades físicas u otros comportamientos complejos. |
| **Perspectiva** | Perspectiva es una representación aproximada de un objeto o escena que el ojo humano ve sobre una superficie plana (como una pantalla). Es una simulación de profundidad y escala. |
| **Píxel / Texel** | Un píxel es un punto de una imagen, es el elemento más pequeño posible que contiene información de color. Cuanto mayor sea la resolución, más píxeles estarán disponibles para permitir una mejor definición y más detalles. Los texeles son píxeles dentro de una textura. |
| **Complemento** | Los plugins son funciones de programación (a menudo expresadas a través de scripts) que se pueden añadir al software, ampliando las posibilidades de la aplicación. |
| **Proceso posterior** | Un proceso posterior es un efecto visual aplicado en la pantalla una vez que se ha procesado la imagen 3D, a menudo para simular un comportamiento especial como la corrección del color o la floración. |
| **Procedimiento** | Procedimiento es un término para describir los procesos generados por un equipo a partir de una serie de parámetros. Puede ser simplemente resultados matemáticos como números o imágenes complejas. |
| **Proyección** | Una proyección es la acción de aplicar desde un punto de vista específico (como la cámara) una imagen/objeto a la superficie de la malla 3D. |
| **Resolución (potencia de 2)** | La resolución define el tamaño de una textura en sus ejes X e Y (o la anchura y el height). A menudo en una potencia de 2 escala (2, 4, 8, 16... 512, 1024, 2048...) porque está optimizado para cálculos en una GPU. |
| **Secuencias de comandos** | La creación de scripts es la acción o el uso de un comando específico a través de un formato de archivo basado en texto para ejecutar comportamientos específicos. |
| **Shader** | Un sombreador define el comportamiento de un material cuando recibe información de iluminación. Algunos sombreadores pueden ser simples (como el sombreado de caricatura) o más avanzados (como el sombreado de piel que simula la absorción de la luz en una superficie). |
| **Plataforma** | Un estante es la ubicación en la aplicación donde se organizan los recursos de varios tipos. Puede pasar de imágenes sencillas a herramientas más complejas. |
| **Máscara inteligente** | Las máscaras inteligentes se comportan como materiales inteligentes, pero en lugar de ser capas, son efectos definidos para generar máscaras basadas únicamente en la malla 3D actual. |
| **Material inteligente** | Un material inteligente es un grupo de capas guardadas como un archivo. El material inteligente se puede adaptar a cada proyecto en Substance 3D Painter, lo que permite crear materiales que cambiarán en función de la malla 3D actual. |
| **Difuminado** | El difuminado es una herramienta para sangrar, esparcir o mezclar colores. Se suele utilizar para suavizar los píxeles. |
| **Galería de símbolos** | Una galería de símbolos es una imagen alineada con la pantalla y utilizada con una proyección de cámara para realizar una pintura en la malla 3D. |
| **Substance** | Un Substance es un formato de archivo que permite generar textura en función de un conjunto de parámetros (que implican cálculos procedimientos). Estos parámetros se pueden modificar para crear variaciones. |
| **Simetría** | La simetría es una opción de una herramienta que permite la pintura en dos lugares al mismo tiempo en el espejo. |
| **Plantilla** | Una plantilla es un conjunto de opciones predefinidas que se utilizan al crear un nuevo proyecto. Por ejemplo, puede definir la resolución predeterminada o la configuración de haga un bake predeterminada. |
| **Proporción de texto** | La proporción de texel es la regla que compara el tamaño de una Isla de UV (2D) y la geometría de la malla 3D relacionada con ella. Una buena proporción de texel significa un despliegue uniforme de la geometría en 2D. Esto es importante para mantener el aspecto y la calidad de la pintura/texturización coherentes en la malla 3D. |
| **Textura** | Una textura es un fichero que contiene píxeles con dos dimensiones definidas por una resolución. Los píxeles pueden ser de escala de grises o de color. Cuando están coloreados, los píxeles pueden tener una información de transparencia (si es compatible con el formato de archivo). |
| **Conjunto de texturas** | En Substance 3D Painter, un conjunto de texturas representa una parte de una malla que tiene UV específicos sobre los que pintar. El conjunto de texturas se crea por cada material único detectado al importar una malla 3D. |
| **Tilling** | La inclinación es la repetición de una textura donde las costuras no son visibles en los bordes, se supone que simula un plano infinito. Ejemplo : césped o pavimentos. |
| **Herramienta** | Una herramienta hace referencia a una acción que permite interactuar con la malla 3D, a menudo para pintura o aplicar efectos. |
| **Barra de herramientas** | La barra de herramientas es la ubicación en la que están disponibles todos los métodos abreviados de iconos de las herramientas. |
| **UDIM** | UDIM es una forma de dividir las UV de una malla 3D en varios rangos para aumentar la resolución general de la textura. |
| **UV** | Los UV son información definida en una malla 3D que indica cómo se puede desdoblar para convertirse en una forma plana. Esta información se utiliza para proyectar una textura en una malla 3D. Substance 3D Painter solo permite la pintura en el rango 0-1, que representa el tamaño de una textura. Otros intervalos solo se admiten a través del sistema de UDIM. |
| **VRam** | La VRam es la memoria de la GPU (tarjeta gráfica), que se utiliza para almacenar información y textura al realizar cálculos. Cuanto más VRam, mejor para trabajar con Substance 3D Painter. |
| **Ventana** | El área de visualización es el lugar donde se muestra la escena 3D o 2D en la pantalla. Aquí también es donde es posible interactuar con las herramientas y la malla 3D controlando la cámara. |
