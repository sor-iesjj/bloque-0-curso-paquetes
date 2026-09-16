# 📦 Qué tienes que entregar — LÉEME ANTES DEL PRIMER EJERCICIO

> **Módulo:** SOR — Sistemas Operativos en Red · **Bloque 0 · Curso de Gestores de Paquetes**
> **Profesor:** Pedro Navarro Miralles · IES Jorge Juan (Alicante)
>
> **📍 Cuándo se lee:** **AHORA.** Antes de abrir la Fase 1, antes de instalar nada.

---

> [!danger] 🛑 No empieces ningún ejercicio sin haber leído esta página
> Aquí está **todo lo que se te va a pedir**: dónde van tus apuntes, cómo se llaman, qué tienen que contener y cómo se entregan.
>
> Si empiezas a hacer ejercicios y dejas los apuntes "para luego", te va a pasar una de estas dos: o los escribes de memoria al final —y se nota—, o los pierdes. **Las dos cuentan como no entregado.**

---

## **1 · LOS TRES ENTREGABLES DE CADA EJERCICIO**

| # | Entregable | Dónde vive |
| :--- | :--- | :--- |
| 1 | **Una entrada de apuntes** | Tu repositorio de apuntes, en GitHub |
| 2 | **Un vídeo** | Tu playlist de YouTube, **No listado** |
| 3 | **El `push`** que sube la entrada | Tu repositorio |

**No hay entrega parcial.** Un vídeo sin entrada no cuenta, y una entrada sin el enlace del vídeo tampoco.

---

## **2 · DÓNDE VAN TUS APUNTES**

Dentro de **tu bóveda**, en esta ruta exacta:

```
00_Apuntes/Trimestre_1/B0_Curso_Paquetes/
```

> [!warning] ⚠️ Esa carpeta la creaste en [🛠️ Antes de empezar](01_ANTES_DE_EMPEZAR.md)
> Si te saltaste ese paso, vuelve ahora. Lo que no cambia nunca es el nombre: **`B0_Curso_Paquetes`**.

---

## **3 · CÓMO SE LLAMA CADA ENTRADA**

**Una entrada por ejercicio.** El nombre se construye siempre igual:

```
paq-<fase>.<nivel>.<numero>-<titulo-en-minusculas-con-guiones>.md
```

| Ejercicio | Fichero de apuntes |
| :--- | :--- |
| `EJ-02-01-01` — Marko busca antes de instalar | `paq-2.1.1-busca-antes-de-instalar.md` |
| `EJ-03-02-01` — Marko ve qué hay puesto en el equipo | `paq-3.2.1-ve-que-hay-puesto.md` |
| `EJ-05-01-01` — Marko se monta Chocolatey | `paq-5.1.1-se-monta-chocolatey.md` |

> [!info] 🎓 El `paq-` del principio
> Cada material del Bloque 0 tiene su prefijo: `b0-` los prerrequisitos, `git-` el curso de Git, `shell-` el de Shell y **`paq-` este**. Así, dentro de tu repositorio de apuntes, se ve de un vistazo de dónde sale cada entrada.

> [!important] 📌 El nombre exacto te lo da cada ejercicio
> **No tienes que inventártelo.** Al principio de cada ejercicio, en el `Paso 0`, aparece el nombre que le toca. Cópialo tal cual.

> [!danger] ⚠️ Los nombres NO son orientativos
> Con un grupo entero entregando, si cada uno pone el nombre que le apetece **corregir se vuelve imposible y tu entrega se pierde**. Sin dramas y sin excepciones: el nombre es el que pone el ejercicio.

---

## **4 · 🔴 QUÉ LLEVA DENTRO CADA ENTRADA**

**Esta estructura es obligatoria.** Es la misma de todo el módulo, la que fijaste en la **Bloque 0 · Fase 0.1**. Cópiala y rellénala:

```markdown
# paq-2.1.1 · Marko busca antes de instalar

- **Alumno:** Nombre Apellido
- **Fecha de inicio:** 2026-09-15
- **Fecha de entrega:** 2026-09-17
- **Fase:** 2 — Buscar e instalar con winget
- **Nivel:** N1 — Mínimo
- **Ejercicio:** EJ-02-01-01

---

## 🎯 Qué se pedía

*(Dos o tres líneas con tus palabras: qué te encargaba Lucía y qué había que resolver.)*

---

## ⌨️ Comandos y pasos importantes

*(Los comandos de este ejercicio, con una línea diciendo QUÉ HACE cada uno.
No pegues la terminal entera: quédate con los que importan.)*

- `comando` — para qué sirve.

---

## 🛠️ Qué he hecho

*(Los pasos que has seguido. No copies el enunciado: cuenta lo que hiciste tú.)*

---

## 🚩 Qué me ha fallado y cómo lo he resuelto

*(Los errores que te han salido, con el mensaje literal, y qué hiciste.
Si no te falló nada, escribe "nada" — pero piénsalo dos veces antes.)*

---

## 🤔 Respuestas a las preguntas

*(Las preguntas del apartado "Comprueba que lo has entendido", con tus palabras.
Copiar del enunciado NO cuenta como respuesta.)*

**1.**
**2.**
**3.**

---

## 🔗 Enlaces

- **Vídeo de esta práctica:**
- **Playlist:** `B0_Curso_Paquetes`

---

## 💭 Dudas / a repasar

*(Lo que no te ha quedado claro.)*
```

> [!success] 🎯 En este curso, el apartado de comandos pesa más que en ningún otro
> Porque aquí **el comando ES el trabajo**. Instalar un programa es una línea; lo que se evalúa es que sepas **de dónde sale cada trozo de esa línea** y qué pasaría si cambias uno.
>
> Un apuntes que diga *"ejecuté winget install"* y nada más, no vale. Uno que diga *"`winget install --id Git.Git -e`: el `--id` es para buscar por identificador exacto y no por nombre, y el `-e` para que no me instale otra cosa parecida"*, sí.

> [!warning] ⚠️ El apartado que más se deja vacío es el de los fallos
> Y es el que más dice de ti. **Un ejercicio donde todo salió a la primera es casi siempre un ejercicio que no se ha entendido**, o uno donde se copió y pegó sin mirar.
>
> Anota el mensaje de error **literal**. Te servirá a ti dentro de tres semanas y a un compañero la semana que viene.

---

## **5 · LOS VÍDEOS**

| | |
| :--- | :--- |
| **Playlist** | `B0_Curso_Paquetes` — **una sola para todo el curso**, No listado |
| **Nombre del vídeo** | `B0.P.f.n.e · título`. Te lo da cada ejercicio. Cópialo **exacto** |
| **Al empezar** | Preséntate y **muestra tu identidad** (tu perfil de GitHub, tu Teams o tu correo `@alu.edu.gva.es`) |
| **Timestamps** | `00:00 Presentación` y uno por paso. **Sin timestamps no se corrige** |
| **Duración** | La que ponga el ejercicio. Si se te va de largo, pártelo en dos y pon los dos enlaces |

> [!important] 📹 En este curso, la pantalla que se graba es la terminal
> No hace falta que enseñes el escritorio ni el navegador todo el rato. **Lo que tiene que verse es lo que escribes y lo que responde el sistema**, legible.
>
> Si la letra de tu terminal es diminuta, súbela antes de grabar. Un vídeo donde no se lee la salida del comando no demuestra nada.

> [!info] 🎓 Por qué te obligo a identificarte en cada vídeo
> Porque un vídeo sin cara y sin nombre **no demuestra que lo hayas hecho tú**.

---

## **6 · CÓMO SE ENTREGA**

**Al terminar cada ejercicio, en este orden:**

1. **Guarda tu entrada** con el nombre correcto en `00_Apuntes/Trimestre_1/B0_Curso_Paquetes/`.
2. **Sube el vídeo** a tu playlist del curso y **pega su enlace dentro de la entrada**.
3. **Sube la entrada a tu repositorio**, desde **Git Bash**:
   ```bash
   cd ~/Boveda_SOR/00_Apuntes/Trimestre_1
   git add B0_Curso_Paquetes/
   git commit -m "Curso Paquetes: EJ-02-01-01 terminado"
   git push
   ```
4. **Entrega el enlace** a tu repositorio por la tarea de Teams.

> [!warning] ⚠️ Un `commit` sin `push` no ha salido de tu ordenador
> Es el fallo más habitual de todo el curso: das el trabajo por entregado, y sigue solo en tu disco. **Si el portátil se rompe esta noche, no existe.**

> [!question] 🤔 ¿Y si hago tres ejercicios el mismo día?
> **Tres entradas y tres `commit`.** Uno por ejercicio, con su mensaje.
>
> No juntes tres ejercicios en un `commit` que diga *"apuntes"*: el historial de tu repositorio es parte de lo que se mira.

---

## **7 · CRITERIO DE ÉXITO**

> [!success] 🎯 Qué miro cuando corrijo
> Abro tu repositorio, busco la entrada del ejercicio, y dentro tiene que estar:
>
> - **Qué se pedía**, con tus palabras.
> - **Los comandos**, con qué hace cada trozo — no solo pegados.
> - **Qué hiciste** tú, no lo que decía el enunciado.
> - **Qué te falló** y cómo saliste.
> - **Las respuestas** a las preguntas, contestadas y no copiadas.
> - **El enlace al vídeo** donde se te ve haciéndolo.
>
> **Si falta el enlace o faltan las respuestas, el ejercicio no cuenta como entregado.**

---

## **8 · RESUMEN PARA TENER A MANO**

```
CARPETA   00_Apuntes/Trimestre_1/B0_Curso_Paquetes/
FICHERO   paq-<fase>.<nivel>.<num>-<titulo>.md   (lo dice cada ejercicio)
DENTRO    cabecera · qué se pedía · comandos · qué hice · qué falló ·
          respuestas · enlaces (vídeo + playlist) · dudas
VÍDEO     playlist "B0_Curso_Paquetes", No listado, con timestamps
ENTREGA   git add → commit → push → enlace del repo por Teams
```

---

> [!summary] 🎓 Lo que tienes que llevarte de esta página
> Que **los apuntes no son un trámite del final: son parte del trabajo**, y se abren **antes** de empezar.
>
> Y que en este curso tus apuntes se van a convertir, sin que te des cuenta, en **tu propio manual de instalación**: la lista de los programas que sabes poner en un equipo y cómo. Eso es exactamente lo que un técnico se lleva de un trabajo al siguiente.
>
> **Siguiente:** [empieza por la Fase 1](fase-1-que-es-un-gestor-de-paquetes/README.md).
