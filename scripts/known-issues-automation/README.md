---
source-git-commit: 0376fe6500551442b28831d5742ecbbc9363ab19
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 1%

---
# Generador de problemas conocidos: Substance 3D Painter

Automatiza la generación del documento de marcado de problemas conocidos para Substance 3D Painter, publicado en:
`https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html`

Los problemas se originan en la épica de Jira `SBSFOUR-6267`. El script obtiene todos los problemas, filtra todo lo que ya se haya solucionado en la versión de destino y genera un archivo de marcado con formato listo para ejecutarse.

---

## Inicio rápido

En estos pasos se supone que ya ha completado la configuración única que se indica a continuación.

1. Conectarse a **GlobalProtect VPN**
2. Establezca `TARGET_VERSION` en su archivo `.env` a la versión para la que está generando documentos (p. ej. `12.0.3`)
3. Ejecute el script desde el directorio `scripts/known-issues-automation/`:

   ```
   python fetch_known_issues.py
   ```
4. Compruebe el resumen de resultados: informará de cuántos problemas se han recuperado y cuántos se han excluido
5. Copie el `known-issues.md` generado en `help/release-notes/known-issues.md`

> Si falta algún problema o es inesperado, inspeccione `raw_issues.json` para ver exactamente lo que Jira devolvió antes de aplicar el filtro.

---

## Configuración de una sola vez

### &#x200B;1. Instalar dependencias

```bash
pip install requests python-dotenv
```

### &#x200B;2. Crear el archivo `.env`

```bash
cp .env.example .env
```

### &#x200B;3. Obtener un token de acceso personal de Jira

1. Iniciar sesión en `https://jira.corp.adobe.com`
2. Vaya a su perfil → **Tokens de acceso personal** en la barra lateral izquierda
3. Haga clic en **Crear token**, asígnele un nombre y copie el valor generado

> Las PAT no caducan cuando finaliza la sesión del navegador, lo que las hace más fiables que las cookies de sesión para el acceso a API mediante scripts.

### &#x200B;4. Rellena tu archivo de `.env`

```
JIRA_PAT=your-personal-access-token
TARGET_VERSION=12.0.3
OUTPUT_FILE=known-issues.md
```

`TARGET_VERSION` es la versión de Substance 3D Painter para la que está generando la página de problemas conocidos. Controla los problemas corregidos que se excluyen. Consulte [Lógica de filtrado](#filtering-logic) más abajo.

---

## Estructura del repositorio

```
.
├── README.md                  # This file
├── fetch_known_issues.py      # Main script
├── .env.example               # Environment variable template (safe to commit)
├── .env                       # Your local credentials — never commit this
├── raw_issues.json            # Raw Jira dump from last run — gitignored
└── known-issues.md            # Generated output from last run — gitignored
```

---

## Referencia de Jira

| Campo | Valor |
|---|---|
| Instancia de Jira | `https://jira.corp.adobe.com` |
| Clave del proyecto | `SBSFOUR` |
| Epopeya de problemas conocidos | `SBSFOUR-6267` |

Todos los problemas conocidos deben estar vinculados a esta épica para que aparezcan en el documento generado. Si es necesario añadir o eliminar un problema de la página, actualice la imagen épica en Jira en lugar de editar el marcado manualmente.

---

## Cómo funciona el script

### Paso 1: Obtener

El script consulta la API REST de Jira mediante JQL:

```
"Epic Link" = SBSFOUR-6267 ORDER BY created ASC
```

Los resultados se paginan a 50 números por página. Se recuperan los siguientes campos para cada problema: `summary`, `issuetype`, `status`, `affectedVersions`, `fixVersions`, `labels`.

La autenticación usa un token de portador de `JIRA_PAT`. La instancia Jira corporativa utiliza un certificado SSL interno, por lo que la verificación del certificado está desactivada para estas solicitudes; se trata del comportamiento esperado en la red de Adobe.

### Paso 2: vertedero sin procesar

Antes de aplicar filtros o formatos, el script escribe `raw_issues.json`. Esta es una instantánea simplificada de cada problema que Jira devuelve, y siempre se genera independientemente de lo que suceda a continuación. Si el resultado parece incorrecto, inspeccione primero este archivo, que muestra exactamente los datos que Jira ha proporcionado.

### Paso 3 — Filtro

Los problemas se filtran utilizando dos reglas aplicadas a la vez:

1. **Filtro de estado**: solo `Backlog` y `Dev In Progress` problemas son problemas conocidos activos. Los problemas con el estado `Fixed` son candidatos a la exclusión, sujetos a la comprobación de la versión siguiente.

2. **Filtro de versión**: se excluye un problema de `Fixed` solo si una de sus versiones de corrección es menor o igual que `TARGET_VERSION`. Si la versión de la corrección es superior a `TARGET_VERSION`, el problema sigue apareciendo porque la corrección no se ha enviado para la versión que se está documentando.

Esto se encarga de los casos en los que se desarrollan dos versiones simultáneamente: un problema corregido en `12.1.0` sigue siendo un problema conocido de `12.0.3`.

Consulte [Lógica de filtrado](#filtering-logic) para ver la tabla de decisiones completa.

### Paso 4 — Categorías de análisis

Al principio de la cadena, se analizan las etiquetas de categoría en cada resumen de problemas:

- `[Shader] Some description` → categorías: `["Shader"]`, descripción: `"Some description"`
- `[Crash][Engine] Some description` → categorías: `["Crash", "Engine"]`, descripción: `"Some description"`
- `No brackets here` → ninguna categoría, tratada como no clasificada

La **categoría principal** es siempre la primera etiqueta. Determina la agrupación y la ubicación de la sección.

### Paso 5 — Agrupar y ordenar

Los problemas se organizan de la siguiente manera:

- Los problemas se agrupan por categoría principal
- Los grupos se ordenan por número de problemas, descendente (los grupos más grandes primero)
- Los grupos con más de un problema aparecen en la parte superior del documento
- Los grupos con un solo problema, además de los problemas sin categorizar, aparecen después de los grupos de varios problemas sin encabezado de sección
- Los problemas con `[Crash]` como categoría principal siempre se colocan en último lugar, en una sección `## Stability`

### Paso 6 — Formatear y escribir

El script genera `known-issues.md` con:

- YAML frontmatter (metadatos helpx)
- Encabezado `# Known issues` con un párrafo de introducción que asigna un nombre a la versión de destino
- Problemas con formato: `` * `[Category]` Description ``
- Problemas de varias categorías: `` * `[Category1]` `[Category2]` Description ``
- Líneas en blanco entre grupos de categorías
- Una sección `## Stability` al final para problemas de bloqueo

---

## Lógica de filtrado

| Estado | ¿Fijar conjunto de versiones? | Corrección de la versión frente al destino | ¿Incluido? |
|---|---|---|---|
| `Backlog` | — | — | Sí |
| `Dev In Progress` | — | — | Sí |
| `Fixed` | No | — | No (excluido conservadoramente) |
| `Fixed` | Sí | Fix version ≤ target | No (ya enviado) |
| `Fixed` | Sí | Fijar versión > destino | Sí (la corrección está en una versión futura) |

---

## Formato de salida

```markdown
---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html"
...
---

# Known issues

This page lists all the active known issues present in v12.0.3 of Substance 3D Painter:

* `[Engine]` Error when using Smart Materials if Texture Set has no tile 1001
* `[Engine]` Geometry mask shows artifacts at UV borders with instanced layers

* `[Shader]` user0 channel always can not be read as sRGB with specific shader

* `[Export]` GLTF exports at the wrong size
* `[Import]` Cannot import obj file with "nan" values

## Stability

* `[Crash]` Select "Export mesh" when mesh failed to load
```

**Nota de formato:** Las etiquetas de categoría usan un ajuste de comilla trasera — `` `[Category]` `` — no dobles marcas. El documento heredado mantenido manualmente contenía errores de doble acento grave; el script siempre produce el formato correcto.

---

## Resolución de problemas

**401 No Autorizado**
- Confirme que está conectado a **GlobalProtect VPN**
- Es posible que tu PAT haya caducado o se haya revocado: genera uno nuevo en `https://jira.corp.adobe.com/secure/ViewProfile.jspa` y actualiza tu `.env`

**`JIRA_PAT is not set`error**
- Asegúrese de que ha creado un archivo `.env` de `.env.example` y ha rellenado el token
- Confirme que está ejecutando el script desde el directorio `scripts/known-issues-automation/` para que `python-dotenv` pueda encontrar el archivo `.env`

**Faltan problemas en la salida**
- Marque `raw_issues.json`: si el problema no existe, no está vinculado a la épica `SBSFOUR-6267` en Jira
- Si el problema está en `raw_issues.json` pero no en la salida, el filtro lo excluyó: compruebe su estado y corrija la versión con respecto a su `TARGET_VERSION`

Advertencia de **`TARGET_VERSION`en tiempo de ejecución**
- El script se ejecutará, pero excluirá de forma conservadora todos los `Fixed` problemas si `TARGET_VERSION` no está establecido. Configúrelo siempre antes de generar el documento final.
