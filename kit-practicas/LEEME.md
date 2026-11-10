# Kit de prácticas del curso de agentes de IA

Universidad de Málaga, curso 2026-27

Aquí están todos los materiales de las prácticas de las dos sesiones.
**Todos los datos son ficticios o simulados**, así que puedes equivocarte sin miedo.
En la Sesión 1 trabajamos con **Antigravity**, el agente de Google, con **R** y
con **Overleaf**, y usamos **Claude** como segunda opinión. Nadie tiene que
pagar nada.

---

## Antes de empezar

1. Descomprime el kit en una carpeta fácil de encontrar (por ejemplo, el Escritorio).
2. Guarda el `.zip` original. Si algo sale mal, lo vuelves a descomprimir y empiezas de cero.

## Con Antigravity (Sesión 1)

1. Instala R (cran.r-project.org) y, desde R o RStudio, los paquetes `readxl` y
   `knitr` con `install.packages(c("readxl", "knitr"))`.
2. Instala Antigravity (antigravity.google/download) y entra con tu cuenta de
   Google de la universidad o con una personal de Gmail.
3. Abre esta carpeta como proyecto. En la barra de la izquierda, **New
   Project** (la carpeta con un signo más), **Add Folder**, elige
   `kit-practicas` y pulsa **Create**.
4. En **Settings > General > Global Permissions > Permission Preset**, elige
   **Request Review**. Así el agente te pedirá permiso antes de ejecutar
   cualquier orden en tu ordenador. Leer y escribir ficheros dentro de esta
   carpeta no pide permiso, y por eso se trabaja sobre copias.

## Con Claude (segunda opinión y Sesión 2)

En el navegador (claude.ai) no hace falta instalar nada. Abre un chat nuevo y
adjunta los ficheros de la práctica con el botón **+** o arrastrándolos. Para la
práctica de la carpeta desordenada, adjunta `02-carpeta-desordenada/Descargas.zip`.

En la aplicación de escritorio de Claude, con la extensión **Filesystem**,
Claude puede trabajar sobre esta carpeta y te pide permiso antes de cada acción.
En **Ajustes > Extensiones > Explorar extensiones**, instala Filesystem y elige
como carpeta permitida **solo esta carpeta** (`kit-practicas`).

## Si tienes Claude Code

Abre una terminal dentro de `kit-practicas` y escribe `claude`. El kit trae una
configuración (`.claude/settings.json`) para que empiece en **modo Manual**, en el
que te pedirá permiso antes de crear, cambiar o mover nada, y no podrá borrar con
`rm`.

---

## Que te dure el uso

- Una conversación nueva para cada práctica (salvo la 4, que sigue en la de la 3).
- Mejor un encargo bien pensado que cinco intentos.
- **El día de clase, no uses los agentes antes de la sesión.**

## Qué hay en cada carpeta

| Carpeta | Práctica | Sesión |
|---|---|---|
| `01-presupuestos/` | Prácticas 3, 4 y 5 (seis Excel con los presupuestos de 20 municipios) y reto A del mini-proyecto | 1 y 2 |
| `02-carpeta-desordenada/` | Práctica 6 (Ordena el caos) | 2 |
| `03-encuesta/` | Mini-proyecto, reto B (La voz de los estudiantes) | 2 |
| `04-documentos/` | Práctica 8 (Instrucciones escondidas) | 2 |
| `05-calculadora/` | Mini-proyecto, reto C (La calculadora del IFRU) | 2 |
| `06-skill-informe/` | Práctica 7 (Tu primera Skill) | 2 |
| `plantillas/` | Encargo, normas de la casa (`CLAUDE.md`) y bitácora | 1 y 2 |
| `prompts.md` | Todos los encargos de los cuadernos, para copiar y pegar | 1 y 2 |

En la Práctica 1 el agente creará `notas.txt` en esta carpeta, y en las
prácticas 3 a 5 dejará en `01-presupuestos/` el programa `analisis.R`, el
fichero `presupuestos_limpio.csv` y las tablas para Overleaf.

## Tres normas para todo el curso

1. **Trabaja sobre copias.** Un agente puede crear y cambiar ficheros de verdad.
2. **Lee antes de permitir.** Cuando el agente te pida permiso, lee qué va a hacer.
3. **Comprueba siempre.** Un resultado bien presentado no es lo mismo que un resultado correcto.
