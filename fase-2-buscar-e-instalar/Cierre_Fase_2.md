---
Tipo: cierre-de-fase
Fase: 02
Título: Cierre de la Fase 2 — Buscar e instalar con winget
---

## 🏁 Cierre de la Fase 2 — Buscar e instalar con winget

> [!info] Para qué es esta página
> No es un ejercicio nuevo y **no se graba**: es una parada para consolidar. La Fase 3 da por sabido todo lo que hay aquí, así que si algo no lo tienes claro, **para y repásalo** (o pregúntame) antes de seguir.

---

## 🎓 Lo que has aprendido en la Fase 2

- A leer la tabla de `winget search` columna a columna, y a saber que **la que importa es `Id`**.
- Que el **nombre es para humanos** y el **identificador para pedir el paquete sin ambigüedad**.
- A estrechar una búsqueda con comillas y con `--id`.
- A instalar con `--id` y `-e`, y a comprobar después con `winget list`.
- Qué hace winget cuando la petición es **ambigua** — visto en tu máquina, no contado.
- Por qué **lo repetible vale más que lo corto**: un comando que pregunta rompe cualquier instalación desatendida.
- A leer entera la **ficha** de un paquete: versión, editor, licencia y origen del instalador.
- A **preguntarle al comando** con `--help` en vez de fiarte de tu memoria o de un tutorial de hace tres años.
- Que se puede **fijar una versión**, y que hacerlo exige un motivo escrito.
- Que **seleccionar software se evalúa** (`CE.01.e`): los criterios se escriben **antes** de ver los candidatos.
- A dejar una decisión documentada para que se sostenga seis meses después.

---

## ❓ Preguntas de repaso

> [!question] Responde en tus apuntes antes de seguir
> Con tus palabras. Si la respuesta es copiar una línea del ejercicio, no cuenta.
> 1. Explica la diferencia entre `winget install vlc` y `winget install --id <Id> -e` **en términos de qué puede salir mal**, no de qué es más largo.
> 2. ¿Por qué un comando que hace una pregunta es un problema en una instalación desatendida?
> 3. Alguien te dice que una opción de winget "no existe". ¿Cómo lo compruebas en treinta segundos?
> 4. ¿Cuándo está justificado instalar una versión que no es la última? Y una vez justificado, ¿qué tienes que dejar escrito?
> 5. ¿Por qué los criterios de elección se escriben **antes** de mirar los candidatos?
> 6. Un compañero eligió otro paquete que tú para la misma necesidad. ¿Puede estar bien? Explica cuándo.

---

## ✅ Tabla de verificación (¿sé hacerlo yo solo?)

> [!success] Marca solo lo que puedas hacer SIN mirar los apuntes
> | Sé… | ¿Sí? |
> | :--- | :---: |
> | Buscar un programa y localizar su `Id` entre varios resultados | ☐ |
> | Buscar algo cuyo nombre lleva espacios | ☐ |
> | Sacar la ficha de un paquete y leer versión, editor, licencia y origen | ☐ |
> | Instalar un paquete de forma exacta y repetible | ☐ |
> | Comprobar después que está instalado, y con qué versión | ☐ |
> | Explicar cada trozo de `winget install --id X -e` | ☐ |
> | Consultar la ayuda del propio comando y encontrar una opción en ella | ☐ |
> | Comparar dos candidatos con criterios escritos antes | ☐ |
> | Justificar una elección con un dato, no con una impresión | ☐ |
> | Documentar una entrega para que otro la reproduzca sin mí | ☐ |

---

## 🚑 Errores frecuentes de toda la Fase 2

> [!bug] Si algo falla, empieza por aquí
> | Síntoma | Causa habitual | Solución |
> | :--- | :--- | :--- |
> | La búsqueda no encuentra el programa | El nombre comercial no es el del catálogo | Prueba otras palabras y busca también con `--id`. |
> | Salen demasiados resultados | Buscaste por un concepto genérico | Acota: comillas, nombre más concreto o `--id`. |
> | Varias palabras devuelven cualquier cosa | Te faltaron las comillas | `winget search "visual studio code"`. |
> | Me pregunta entre varios candidatos | Petición ambigua: faltó `--id` o `-e` | Identificador exacto **y** `-e`. |
> | Instala algo parecido pero no lo que querías | Coincidencia parcial | `-e`. Es un carácter. |
> | El identificador "no existe" | Tecleado de memoria o sacado de un foro | **Léelo de la salida de `winget search`.** |
> | Una opción del tutorial no me funciona | Tu versión de winget puede ser otra | `winget install --help` en **tu** equipo. |
> | Mis apuntes no me sirven meses después | No pegaste salidas ni escribiste motivos | Salidas pegadas y motivos con su dato. |

---

> [!warning] ⚠️ Recuerda dónde trabajas
> Seguimos en **tu Windows real**. En esta fase ya has instalado programas de verdad, y en la Fase 3 vas a empezar a **quitar** cosas. Las tres reglas no cambian: se instala lo que dice el ejercicio, se comprueba antes de quitar nada, y se lee lo que el sistema pregunta.

---

> [!tip] Siguiente paso
> Cuando tengas la tabla de verificación completa, pasa a la **Fase 3 — El parque al día**: ver qué hay instalado en un equipo, actualizarlo y quitar lo que sobra. Ahí es donde esto deja de ser instalar programas sueltos y empieza a ser **mantener un equipo**.

**Siguiente:** [Fase 3 — El parque al día](../fase-3-el-parque-al-dia/README.md) · [← Volver al índice del curso](../00_INDICE.md)
