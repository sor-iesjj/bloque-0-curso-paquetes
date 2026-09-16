# Curso de Gestores de Paquetes en Windows — 2.º SMR (práctica independiente)

> **Módulo:** SOR — Sistemas Operativos en Red · **Profesor:** Pedro Navarro Miralles · IES Jorge Juan (Alicante)
> **Autor y propietario:** © 2026 Pedro Navarro Miralles. **Licencia:** [CC BY-NC-SA 4.0](LICENSE) — atribución obligatoria, uso no comercial.

## Qué es este curso (y por qué existe)

Es un **curso de instalación de software desde el terminal de Windows**, en forma de simulación: sigues a **Marko**, un técnico junior ficticio, y aprendes a dejar un equipo con el software que tiene que tener **sin bajar un solo `.exe` de Google**.

Y existe por una razón que ya has vivido.

> [!danger] 🎯 El problema que este curso resuelve
> En la **Fase 0.2.1 de prerrequisitos**, para instalar Git y Obsidian, te mandé escribir esto:
>
> ```
> winget install --id Git.Git -e
> winget install --id Obsidian.Obsidian -e
> ```
>
> Y lo escribiste. Funcionó. **Y nadie te explicó qué era.**
>
> Ni qué es `winget`, ni de dónde sale ese `Git.Git`, ni qué pasaría si te lo inventas, ni qué hace el `-e`, ni cómo se busca el identificador de un programa que no viene en el enunciado. Copiaste un comando, que es exactamente lo que este módulo intenta que dejes de hacer.
>
> **Este curso es esa explicación que faltaba.** El objetivo es uno y se puede medir: que puedas instalar, actualizar y quitar **cualquier** programa desde el terminal, sin que nadie te dé el comando hecho.

> [!important] Este curso se hace en TU Windows, no en una máquina virtual
> Los cursos de Git y de Shell te mandaban a una VM. **Este no.** Un gestor de paquetes existe para administrar el equipo real de alguien, y aquí el software que instales se queda instalado y el que quites desaparece de verdad.
>
> No hay instantánea a la que volver. Se trabaja con cabeza, y el curso te dice cómo.

---

## El escenario y los personajes

Los mismos de los [cursos de Git](../02_Curso_Git/README.md) y [de Shell](../03_Curso_Shell/README.md):

- **Marko** — 19 años, recién titulado en SMR. Técnico junior en **Boochan Networks S.L.** Ya documenta con Git y ya se defiende en una terminal de Linux. Ahora le toca lo que hace un técnico el primer día en casa de un cliente: **dejar los equipos con lo que tienen que tener**.
- **Boochan Networks S.L.** — PYME ficticia de 12 empleados que da soporte de infraestructura.
- **Carlos** — técnico *senior*. Lo sabe todo y **nunca documenta nada**. Instala a mano, no apunta qué instaló, y cuando alguien pregunta ya se ha ido a comer.
- **Lucía** — **responsable de IT**. Encarga el trabajo, lo revisa, y no acepta un *"ya está puesto"* sin que le digas qué versión.

**Cada ejercicio arranca de un encargo real de la empresa.** No hay ni un solo *"instale el programa de prueba"*.

---

## Entorno: tu Windows 11 Pro y su terminal

Todo el curso se hace en el equipo que tienes delante. **No hace falta instalar nada para empezar:** `winget` ya viene con Windows 11.

Lo único que instalarás en el curso es **Chocolatey**, y eso es el ejercicio de la Fase 5, no un requisito previo.

> [!warning] Sin red de seguridad: se lee antes de aceptar
> Aquí no hay instantáneas. Por eso el curso impone tres costumbres desde el primer ejercicio:
>
> 1. **Se instala lo que dice el ejercicio.** Ni más por curiosidad, ni otra cosa parecida.
> 2. **Antes de desinstalar, se comprueba qué es eso.** Hay una fase entera sobre ello.
> 3. **Si el sistema pide confirmación, se lee.** Justo lo contrario de lo que hacías dándole a Siguiente.
>
> No es miedo: es la diferencia entre administrar un equipo y trastear en él.

---

## Cómo está montado el curso

**Seis fases**, cada una con una idea central. La numeración de los ejercicios es `EJ-0F-NN-MM` = **fase · nivel · número**, igual que en los cursos de Git y de Shell.

### Los cinco niveles

| Nivel | Nombre | Qué es |
| :--- | :--- | :--- |
| **N1** | Mínimo | Lo imprescindible. Sin esto no se puede seguir. |
| **N2** | Básico | El uso normal del día a día. |
| **N3** | Medio | Donde empieza el criterio técnico. |
| **N4** | Avanzado | Lo que separa administrar de ejecutar comandos. |
| **N5** | Reto | **Sin procedimiento.** Se da el objetivo y tú eliges el camino. |

Los **retos N5** son la parte que de verdad evalúa: no traen pasos numerados, traen un encargo de Lucía y unas pruebas que hay que superar.

---

## Los dos gestores

| | **winget** | **Chocolatey** |
| :--- | :--- | :--- |
| Quién lo hace | Microsoft | La comunidad |
| ¿Viene con Windows 11? | **Sí**, preinstalado | **No**: lo instalas tú, en la Fase 5 |
| Cuándo entra en el curso | Fases 2, 3 y 4 | Fase 5 |

> [!info] 🎓 Por qué dos y no uno
> Porque no hacen exactamente lo mismo, y un técnico no elige herramienta por costumbre sino por lo que necesita ese día.
>
> Y porque hay algo que se aprende solo en cuanto lo vives: **uno ya lo tienes puesto y el otro te lo tienes que montar**. Cuando instales Chocolatey a mano en la Fase 5, vas a entender de golpe por qué Microsoft acabó metiendo winget dentro de Windows.

Existe un tercero, **Scoop**, con otra filosofía. Lo verás nombrado en la comparativa de la Fase 5, pero no entra en los ejercicios.

---

## Índice de fases

> [!danger] 🛑 EMPIEZA POR AQUÍ: **[📦 Índice general del curso](00_INDICE.md)**
> Ahí tienes el mapa completo: las seis fases, cómo funciona cada ejercicio, qué se te evalúa y **los tres pasos previos que hay que dar antes de la Fase 1**.
>
> Y esos tres pasos, por orden:
> 1. **[🛠️ Antes de empezar](01_ANTES_DE_EMPEZAR.md)** — traer el curso a tu ordenador y dejar listo dónde guardas todo.
> 2. **[📦 Entregables](02_ENTREGABLES.md)** — qué se entrega, cómo se llama y cómo se sube.
> 3. Y ya sí, la Fase 1.
>
> Hay una razón para leer el paso 2 ahora y no luego: **cada ejercicio produce TRES entregables** —una entrada de apuntes, un vídeo y el `push` que la sube—, y **la entrada se abre al empezar el ejercicio, no al terminarlo**.
>
> Si dejas los apuntes para el final, o los escribes de memoria —y se nota— o los pierdes. Las dos cosas cuentan como **no entregado**.

| Fase | Idea central | Aterriza en |
| :--- | :--- | :--- |
| **1** | [Qué es un gestor de paquetes](fase-1-que-es-un-gestor-de-paquetes/README.md) y por qué el `.exe` de Google es la peor opción | Todo el módulo |
| **2** | [Buscar el paquete correcto](fase-2-buscar-e-instalar/README.md) y saber que es el correcto antes de instalarlo | La **Fase 0.2** de prerrequisitos |
| **3** | [Ver qué hay instalado](fase-3-el-parque-al-dia/README.md), actualizarlo y quitar lo que sobra | Mantenimiento de cualquier equipo |
| **4** | [Dejar un equipo montado sin quince clics](fase-4-instalacion-en-lote/README.md): se escribe una vez y se repite | `CE.01.f` |
| **5** | [Chocolatey](fase-5-chocolatey/README.md): instalarlo, usarlo y **compararlo** | El criterio de elección |
| **6** | [Reto de cierre](fase-6-reto-final/README.md), sin procedimiento | — |

---

## 📹 Grabación y entrega (LÉEME — aplica a TODOS los ejercicios)

Igual que en la Fase 0 y en los cursos de Git y de Shell, **cada ejercicio se graba entero con OBS**, de principio a fin. No es un repaso al final: se ve **cómo lo haces tú**. Cada ejercicio trae su caja **📹 Grabación** y un **Paso 0** para prepararte y arrancar.

> [!important] Las 5 reglas de grabación
> 1. **Grabación completa con OBS**, sin cortes, hablando lo que haces.
> 2. **Preséntate al empezar** y **muestra tu identidad** en pantalla (Teams, correo `@alu.edu.gva.es` o tu perfil de GitHub). Di qué vas a hacer.
> 3. **Timestamps SIEMPRE** en la descripción: `00:00 Presentación` y **uno por cada paso** (`mm:ss`).
> 4. **Nombre del vídeo:** `B0.P.f.n.e · <título>` — donde `f.n.e` = **fase . nivel . ejercicio**. El nombre exacto te lo da cada ejercicio.
> 5. **Súbelo a tu playlist del curso** como **"No listado"**.

> [!info] La `P` del principio
> El curso de Git usa `B0.G.1.1.1` y el de Shell `B0.S.1.1.1`. Este usa **`B0.P.1.1.1`** — **`P` de *paquetes*** — para que un vídeo suelto se sepa de qué curso sale sin abrirlo. Son cursos distintos del mismo Bloque 0 y sus vídeos conviven en el mismo canal.

> [!info] 🎬 UNA sola playlist para todo el curso
> Se llama **`B0_Curso_Paquetes`** — igual que tu carpeta de apuntes y que la carpeta del material. La creas una vez, al principio, y ahí van **todos** los vídeos del curso.
>
> **No hagas una playlist por fase.** El vídeo ya lleva la fase en su nombre (`B0.P.2.1.1`), así que dentro de la playlist salen ordenados solos.

> [!warning] Entrega ÚNICA (no se duplica casa/centro)
> Se graba y se sube el vídeo **una sola vez**. Los entregables escritos van a tu **repositorio de apuntes**, dentro de la entrada de cada ejercicio.

---

## Qué hay que entregar, además del vídeo

- **Apuntes:** **una entrada por ejercicio** en `00_Apuntes/Trimestre_1/B0_Curso_Paquetes/`, con el nombre que te da el propio ejercicio en su Paso 0 (`paq-2.1.1-....md`). **No son capturas de pantalla:** son salidas de comandos pegadas y explicadas con tus palabras. La estructura obligatoria está en **[📦 Entregables](02_ENTREGABLES.md)**.
- **Ficheros de trabajo:** a partir de la Fase 4 empiezas a generar ficheros de configuración e inventarios. Todo va al repositorio.

> [!question] Las preguntas no se responden copiando
> Todos los ejercicios acaban con preguntas del tipo *"con tus palabras"*, *"un ejemplo tuyo distinto"*, *"predice qué pasaría"*. Están escritas así a propósito: si la respuesta se puede copiar del enunciado, no demuestra nada.

---

## No todo pesa lo mismo

- El **núcleo** son las Fases 2 y 3: instalar y mantener. Sin eso, el curso no ha servido.
- La Fase **4** es la que se evalúa contra `CE.01.f`, y es la que de verdad se parece al trabajo real.
- La Fase **5** es criterio: no va de aprender otro programa, va de **saber elegir**.

El profesor indicará qué parte toca en cada momento.

---

> [!tip] Por dónde se empieza
> Por el **[📦 Índice general](00_INDICE.md)**, que te lleva a los tres pasos previos. **No abras la Fase 1 directamente:** sin el paso 1 no tienes dónde guardar el trabajo.
