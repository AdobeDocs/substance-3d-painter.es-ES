---
helpx_url: "https://helpx.adobe.com/es/substance-3d-painter/painting/presets/creating-particles-presets/overview-of-the-particle-editor.html"
breadcrumb-title: ''
description: Obtenga más información sobre el editor de partículas de Substance 3D Painter para crear ajustes preestablecidos de pincel de partículas personalizados para la pintura de texturas.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Overview of the particle editor
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Descripción general del editor de partículas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---


# Descripción general del editor de partículas

Esta página cubre varios aspectos del editor de partículas PopcornFX. Algunos de los títulos y parámetros de las ventanas pueden estar sujetos a cambios dependiendo de la versión del editor utilizado.

## Configuración de Viewport

### Cómo importar su propia malla

Copie y pegue la malla en la carpeta &quot;Mallas&quot; de su paquete. Luego en el Editor abra su malla y haga clic en &quot;Build&quot;.

Ahora, en su sistema de partículas, vaya a &quot;Backdrop&quot; en la vista de árbol, haga clic con el botón derecho en &quot;3D Layers&quot;, &quot;New Backdrop&quot;, &quot;CNEdEditorBackdrop\_Model3D&quot;, y seleccione su malla en &quot;resource model&quot;.

En Substance 3D Painter, la malla se escala para que esté dentro de un cuadro de tamaño [-1;1] en cada eje. Para obtener la escala correcta con Substance 3D Painter en el Editor, debe importar una malla que ya se haya escalado para que encaje en ese cuadro (de forma sencilla), o jugar con Escalas en el Editor.

Nota: solo se admite el formato de malla FBX.

#### Cómo mostrar la cuadrícula

Ctrl-G. Puede personalizar el color de la cuadrícula en &quot;Propiedades del editor&quot; &quot;GridColor&quot;.

## Emisor

### Cómo crear eventos &quot;OnCollide&quot;

El revólver físico maneja la colisión con mallas de fondo en la escena. En Substance 3D Painter el escenario será tu malla.

Primero, en el Evolver Físico, establezca &quot;WorldInteractionMode&quot; en &quot;OneWay&quot; para habilitar la colisión de partículas. A continuación, crea un evento llamado &quot;OnCollide&quot;, el Evolver Física lo activará en la colisión con la escena.

En Substance 3D Painter, la escena es el modelo en el que se está trabajando y todos los eventos denominados &quot;Al chocar&quot; serán reemplazados por el sistema de partículas del emisor del pincel actual.

#### Cómo disparar partículas desde la cámara

En la parte superior de la ventana gráfica, habilite el 4º botón &quot;Restringir se genera en el plano de la cámara&quot;.

Substance 3D Painter activará por defecto los emisores de la cámara.

#### Cómo emitir partículas en la parte superior como la lluvia

Desactive &quot;Restringir los inicios en el plano de la cámara&quot; si está activado.

Cree un Atributo de objeto llamado &quot;Global&quot;, ahora Substance 3D Painter generará sus partículas en el origen.

Para desovar en la parte superior de la malla, agregue una Caja de Sampler de formas o un CILINDRO, colóquelo en la parte superior y muéstrelo en su Script de desove.

Por ejemplo, con un Shape Sampler BOX llamado &quot;Spawn&quot;, añada esto a su Script Spawner:

*Posición = Spawn.samplePosition();*

## Receptor

### Cómo generar el emisor al crear o editar un receptor

Para acercarse aún más al flujo de trabajo de Substance 3D Painter mientras edita el receptor, puede configurar el editor para anular el sistema de partículas generado.

En la vista de árbol del receptor, seleccione &quot;Propiedades del editor&quot;, luego habilite &quot;UserOverSpawn&quot; y seleccione su emisor en &quot;OverSpawnEffect&quot;.

Aún debe abrir el emisor para configurar los eventos &quot;Al chocar&quot; para generar el receptor que está editando actualmente.

#### Cómo configurar campos de objetos

Esta es la descripción del campo de partículas que debe tener en el receptor:

*&quot;Tamaño&quot; float*

Multiplicador del tamaño de pincel en Substance 3D Painter.

*&quot;Opacidad&quot; float*

El multiplicador de la opacidad del pincel en Substance 3D Painter.

*&quot;UV&quot; float3*

Coordenada de textura en la malla de partículas.

En un Script Evolver, pruebe la &quot;malla&quot; de Shape Sampler con la coordenada paramétrica proporcionada por el Evolver de proyección:

UV = Mesh.sampleTexcoord(pCoords);

*&quot;Normal&quot; float3*

Normal de la superficie de malla debajo de las partículas.

En un script Evolver, pruebe la &quot;malla&quot; de Shape Sampler con la coordenada paramétrica dada por el revólver de proyección:

Normal = normalize(Mesh.sampleNormal(pCoords));

*&quot;Seed&quot; int*

Solo un valor generado aleatoriamente para Substance 3D Painter:

En un script Evolver, agregue:

Semilla = int(rand(0,20000000));

*&quot;pCoords&quot; int3*

No es utilizado por Substance 3D Painter, pero es indispensable para hacer la proyección de partículas en la malla y muestrear otros campos.

#### Cómo proyectar partículas en la malla

Añada un Evolver de proyección en el &quot;Estado\_0&quot; del receptor.

Cada fotograma, el Evolver de proyección, proyectará partículas en la superficie más cercana de un Sampler de formas.

El Evolver de proyección puede rellenar la coordenada paramétrica de la proyección en el campo de partículas especificado por &quot;OutputParametricCoordsField&quot; (consulte &quot;pCoords&quot;, campo de partículas).

Y puede reproyectar un vector en la superficie de la malla con &quot;ReprojectadoField&quot;.

Aquí, queremos proyectar partículas en la forma de Sampler &quot;Malla&quot;, rellenar las coordenadas paramétricas en el campo de partículas int3 &quot;Coord&quot;, y proyectar la &quot;Velocidad&quot; en la superficie también:

#### Cómo muestrear la malla

En Substance 3D Painter, todos los Muestreadores de formas denominados &quot;Mesh&quot; y &quot;ShapeType&quot; &quot;MESH&quot; se reemplazarán por la malla utilizada en Substance 3D Painter.<b>\
</b>

En el Editor, configúrelo en la misma malla que su fondo.

Para muestrear elementos de un script, escriba &quot;Mesh.sample~Something~(pCoords)&quot; en un script. Consulte la documentación siguiente:

<https://wiki.popcornfx.com/index.php/CParticleSamplerShape#Script_bindings>

Algunos fragmentos de código útiles que necesitará:

```
// UV is the texture coordinate of the particle on the mesh

// Must be after CParticleEvolver_Projection

UV = Mesh.sampleTexcoord(pCoords);

// Normal is the Normal of the surface on the mesh just below the particle

// Must be after CParticleEvolver_Projection

Normal = normalize(Mesh.sampleNormal(pCoords));
```


## Consejos generales

### Cómo importar emisor/receptor en Substance 3D Painter

En Substance 3D Painter, haz &quot;Archivo&quot; > &quot;Importar partículas&quot; o Ctrl-Alt-R y luego elige tu Emitter.pkfx o Receiver.pkfx en tu Pack.

Substance 3D Painter detectará automáticamente los requisitos (campos de partículas, eventos OnCollide) para decidir si su pkfx es un emisor, un receptor o no es compatible.

Ahora, debería ver su Emisor/Receptor en la Estantería.

#### Cómo depurar partículas con un tamaño de partícula viable

Como el campo de partículas &quot;Tamaño&quot; debe estar entre 0 y 1 para ser un multiplicador del tamaño del pincel en Substance 3D Painter, las partículas serán demasiado grandes en el Editor. Por lo tanto, añada un campo personalizado flotante &quot;BBSize&quot; establecido en 0.01 en el script de Spawner, para utilizarlo en el procesador de partículas de Billboard como el &quot;SizeField&quot; para ver mejor las partículas.

#### Cómo no meterse con el orden evolutivo

El orden de la evolución puede ser muy importante.

Por ejemplo, usted podría desear tener siempre sus 2 últimos evolucionadores para ser el Evolver de Proyección y luego el Evolver de Script que muestra el UV y Normal con los pCoords generados por el Evolver de Proyección.

Tenga en cuenta que el orden de los evolucionadores es literalmente el orden de ejecución dentro de un fotograma, y que Substance 3D Painter recopilará los valores de los campos de partículas y el final de cada fotograma.

#### Cómo muestrear el mapa normal de la malla

Substance 3D Painter reemplazará todos los Muestreadores de textura llamados &quot;NormalMap&quot; por el mapa normal de la malla (si se importan).

Esa es la única textura que puedes tener por ahora, el resto de texturas no serán accesibles desde Substance 3D Painter.

Una vez que haya añadido el Sampler de textura llamado &quot;NormalMap&quot;, puede probarlo en un script :

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerTexture>

Algunos fragmentos de código útiles:

```
// In Evolver Script convert the NormalMap texture in tangent space to world space normal

// /!\ the "Normal" particle field must always be the normal of the mesh not influenced by the normal map

// /!\ dont forget to initialize your particle fields in your Spawn Script

// otherwise pCoords and Normal will be invalid at the first update

float normalFactor = 1.0; // change the intensity of the normal map

float3 meshnormal = Normal;

float4 rawtangent = Mesh.sampleTangent(pCoords);

float3 binormal = normalize(cross(meshnormal, rawtangent.xyz) * rawtangent.w);

float3 tangent = normalize(cross(meshnormal, binormal));

float3 tsNormal = normalize(((NormalMap.sample(UV).xyz * 2.0 - 1.0).xyz) * float3(-normalFactor, normalFactor, 1));

float3 normal = normalize(tsNormal.x * tangent + tsNormal.y * binormal + tsNormal.z * meshnormal);
```


#### Cómo crear turbulencias

En el Editor, cree un Sampler de turbulencia.

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerProceduralTurbulence>

Luego tienes 2 maneras de muestrear la turbulencia y afectar las partículas:

##### La manera fácil

En el Evolver físico de la capa, defina &quot;VelocityFieldSampler&quot; en el nombre del Sampler de turbulencia y defina &quot;Arrastrar&quot; en un valor > 0.

##### La forma parametrizada

Para ajustar la turbulencia con los atributos, se muestrea el campo de velocidad generado por el Sampler de turbulencia en un script Evolver:

Crear 2 atributos de objeto:

* float &quot;TurbulencePower&quot; minmax: [0;5]
* float &quot;TurbulenceScale&quot; minmax: [0,001; 5] (debe ser > 0)

A continuación, cree 3 campos de objetos:

float &quot;TurbPower&quot; y float &quot;TurbScale&quot;

Para almacenar atributos en el script de generador:

* TurbScale = 1.0 / TurbulenceScale;
* TurbPower = TurbulencePower;

float3 &quot;VelocityField&quot; en modo de rotación.

Se utilizará como el &quot;VelocityField&quot; en el Evolver de Física (ya establecido de forma predeterminada en el campo &quot;VelocityField&quot;).

Así que antes de su Evolver Física, en un Script Evolver, pruebe su Turbulence Sampler llamado &quot;Turb&quot;:

VelocityField = Turb.sample(Position \* TurbScale) \* TurbPower;

#### Cómo utilizar correctamente dt, el tiempo delta

El tiempo delta es el tiempo de simulación en segundos entre cada actualización de fotograma. En el Editor, el tiempo delta se actualiza con el tiempo real transcurrido. En Substance 3D Painter se corrige el tiempo delta y cada actualización se inicia en cuanto termina la última.

Un juego que corre a 60 FPS tendrá un tiempo delta de 1/60= 0.016 segundos, así que intenta que tus pinceles corran alrededor de 0.016s de tiempo delta.

* Tiempo de los grandes deltas > 0.016s
* Actualización rápida de PRO

Como el tiempo entre actualizaciones es grande, el movimiento de las partículas será mayor, por lo que el pincel se ejecutará más rápido en Substance 3D Painter.

* Aproximación con

PopcornFX es una especie de gran sistema de discretización, por lo que más grande es el dt, más grandes serán las imprecisiones. Vea la implicación del gran delta de tiempo en las turbulencias: <http://www.popcornfx.com/wiki/index.php/CParticleEvolver_Physics#Dealing_with_turbulences_at_low_framerates>

* Estafas de estafa

Si el tiempo delta es grande, el movimiento de partículas entre los fotogramas también lo es. Por lo tanto, en Substance 3D Painter pueden aparecer pequeñas manchas en lugar de líneas rectas.

Esto se debe a que Substance 3D Painter dibujará un punto de trazo para cada partícula al final de cada fotograma y no dibujará líneas para cada partícula entre el último fotograma y el actual.

* Poco tiempo delta &lt; 0,016s
* Precisión PRO

Cuanto menor sea el tiempo delta, menor será la distancia entre los trazos del pincel, por lo que el dibujo será más nítido. Y la discretización de la simulación también será mejor.

* CON lento

Cuanto menor sea el tiempo delta, mayor será el número de actualizaciones necesarias para dibujar la misma distancia.

Consejos finales sobre los tiempos delta : una buena manera de obtener el dt de la derecha podría ser comenzar con uno grande (0,1 s) y luego disminuir paso a paso para obtener el resultado deseado.

#### Cómo exponer los parámetros de su sistema de partículas

Substance 3D Painter recopilará los atributos de partículas de los sistemas de partículas y los expondrá en los parámetros del pincel físico:

<http://www.popcornfx.com/wiki/index.php/Particle_effect_attributes>

En PopcornFX tiene la función denominada &quot;Atributos en evolución&quot; que le permite acceder a Atributo en scripts de evolución: no hagas eso. En su lugar, cree un campo de partículas y almacene los atributos en el script de generador, y luego use esos campos de partículas en los scripts de evolucionador. (esto podría solucionarse en el futuro)

#### Cómo detectar partículas problemáticas

Nunca debe tener partículas con valores de campo de partículas extraños, así que asegúrese de romper en problemático de vez en cuando:

<http://www.popcornfx.com/wiki/index.php/Particle_tips_BreakOnProblematicParticle>

#### Cómo resolver problemas de sistemas de partículas en Substance 3D Painter

En el directorio de instalación de Substance 3D Painter, debería encontrar un archivo llamado &quot;popcorn.htm&quot;. Este archivo contiene todos los registros de PopcornFX, echar un vistazo dentro para ver lo que podría suceder mal.

#### Cómo inicializar correctamente los campos de objetos

Para obtener los valores válidos de UV y Normal de pCoords desde el primer fotograma, añada esto a su Script Spawner:

<b>  
</b>

```
// PostEval() will be called after particles have been translated to their respective spawn locations

// so, PostEval() is executed in world space

function void PostEval()

{

// we need to initialize correctly the values needed by Substance 3D Painter:

pCoords = Mesh.projectParametricCoords(Position);

UV = Mesh.sampleTexcoord(pCoords);

Normal = normalize(Mesh.sampleNormal(pCoords));

}
```
