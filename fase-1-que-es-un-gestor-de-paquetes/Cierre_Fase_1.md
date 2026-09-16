---
Tipo: cierre-de-fase
Fase: 01
Título: Cierre de la Fase 1 — Qué es un gestor de paquetes
---

## 🏁 Cierre de la Fase 1 — Qué es un gestor de paquetes

> [!info] Para qué es esta página
> No es un ejercicio nuevo y **no se graba**: es una parada para consolidar. La Fase 2 da por sabido todo lo que hay aquí, así que si algo no lo tienes claro, **para y repásalo** (o pregúntame) antes de seguir.

---

## 🎓 Lo que has aprendido en la Fase 1

- Qué es un **gestor de paquetes** y por qué existe: instalar software es una tarea de administración, no hacer clic en Siguiente.
- Que tu Windows **ya traía uno puesto de fábrica** y llevabas meses sin usarlo.
- A preguntarle a la herramienta con `--help` en vez de buscar un tutorial.
- Qué es una **fuente** y por qué es la pieza que de verdad te protege: un gestor de paquetes **no busca en Internet**, consulta un índice con dueño.
- A distinguir **quién mantiene el catálogo** (la fuente) de **quién fabrica el programa** (el editor).
- Que el **identificador** de un paquete se lee del catálogo con `winget search`, **nunca se escribe de memoria**.
- A mirar la ficha de un paquete con `winget show` **antes** de instalarlo.
- Qué significan `--id` y `-e`, y qué pasa si los quitas.
- Que la ventaja no es solo el tiempo: es **el número de decisiones en las que puedes equivocarte**.
- A **auditar** una instalación que hizo otro: comparar lo que hay contra lo que debería haber, y escribir un informe en vez de una opinión.

---

## ❓ Preguntas de repaso

> [!question] Responde en tus apuntes antes de seguir
> Con tus palabras. Si la respuesta es copiar una línea del ejercicio, no cuenta.
> 1. Explícale a alguien que no es informático qué hace un gestor de paquetes, **sin usar la palabra "paquete"**.
> 2. ¿Cuál es la diferencia real entre bajar un programa de Google y bajarlo de una fuente? Contesta pensando en **quién decide de dónde sale el fichero**.
> 3. ¿Por qué el identificador se lee de `winget search` y no se teclea de memoria? Di **qué puede pasar** si te equivocas en una letra.
> 4. ¿Para qué sirve `winget show` si de todas formas vas a instalar el programa?
> 5. Del ejercicio del cronómetro: ¿cuál de las dos columnas —tiempo o decisiones— te parece más importante, y **por qué**?
> 6. ¿Por qué "no lo sé" puede ser una conclusión válida en un informe de auditoría, y "me parece que" no?

---

## ✅ Tabla de verificación (¿sé hacerlo yo solo?)

> [!success] Marca solo lo que puedas hacer SIN mirar los apuntes
> | Sé… | ¿Sí? |
> | :--- | :---: |
> | Explicar qué es un gestor de paquetes y para qué sirve | ☐ |
> | Comprobar qué versión de winget tengo | ☐ |
> | Sacar la lista de comandos de winget y orientarme en ella | ☐ |
> | Enumerar las fuentes de mi equipo y decir quién es el dueño de cada una | ☐ |
> | Distinguir **fuente** de **editor** | ☐ |
> | Buscar un programa en el catálogo y localizar su identificador | ☐ |
> | Leer la ficha de un paquete antes de instalarlo | ☐ |
> | Leer entera una línea `winget install --id … -e` y explicar cada trozo | ☐ |
> | Auditar un programa instalado y escribir el informe de cinco apartados | ☐ |

---

## 🚑 Errores frecuentes de toda la Fase 1

> [!bug] Si algo falla, empieza por aquí
> | Síntoma | Causa habitual | Solución |
> | :--- | :--- | :--- |
> | `winget` no se reconoce | Estás en Git Bash, no en la Terminal de Windows | Abre la **Terminal de Windows / PowerShell**. Git Bash es solo para entregar. |
> | `winget -version` no funciona | Un solo guion | Son **dos**: `--version`. |
> | La búsqueda no encuentra el programa | El nombre comercial no es el del catálogo | Prueba **dos o tres formas** de escribirlo antes de concluir que no está. |
> | Instala algo parecido pero no lo que querías | Te faltó `--id` o te faltó `-e` | Identificador exacto **y** `-e`. Siempre. |
> | El identificador "no existe" | Lo has tecleado de memoria o sacado de un foro | **Léelo de la salida de `winget search`.** |
> | Mis apuntes dicen solo "ejecuté winget install" | No has pegado ni explicado las salidas | En este curso **el comando es el trabajo**: pega la salida y explica cada trozo. |

---

> [!warning] ⚠️ Recuerda dónde trabajas
> Este curso se hace en **tu Windows real**: no hay instantánea a la que volver. En la Fase 2 empiezas a instalar de verdad, así que las tres costumbres de la Fase 1 siguen vigentes: se instala **lo que dice el ejercicio**, se **comprueba antes** de quitar nada, y **se lee** lo que el sistema pregunta antes de aceptar.

---

> [!tip] Siguiente paso
> Cuando tengas la tabla de verificación completa, pasa a la **Fase 2 — Buscar e instalar con winget**: encontrar el paquete correcto y **saber que es el correcto** antes de instalarlo.

**Siguiente:** [Fase 2 — Buscar e instalar con winget](../fase-2-buscar-e-instalar/README.md) · [← Volver al índice del curso](../00_INDICE.md)
