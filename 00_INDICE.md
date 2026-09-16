# 📦 Curso de Gestores de Paquetes en Windows — Índice general

> **Módulo:** SOR — Sistemas Operativos en Red · **Bloque 0** · **Profesor:** Pedro Navarro Miralles · IES Jorge Juan (Alicante)

---

## **1 · QUÉ ES ESTE CURSO Y PARA QUÉ SIRVE**

Piensa en cómo instalas un programa ahora: buscas el nombre en Google, entras en una web que parece la oficial, bajas un `.exe`, le das a Siguiente cuatro veces y aceptas sin leer. Y si mañana hay que hacerlo en quince equipos, lo repites quince veces.

**Eso no es instalar software: es ir a ciegas.** Es lento, no se puede repetir igual dos veces, no deja rastro de qué instalaste, y es la vía de entrada número uno del software basura en un equipo.

En Linux nadie trabaja así desde hace treinta años: se escribe una línea y el sistema baja el paquete de un sitio de confianza, lo instala y lo apunta. **Windows también tiene eso.** Se llama **winget**, lo llevas ya instalado y probablemente no lo has abierto nunca.

Este curso va de eso: **instalar, actualizar, buscar y desinstalar software desde el terminal**, con criterio y dejando rastro.

> [!info] 🎓 Sigues a Marko, igual que en los cursos de Git y de Shell
> **Marko** es técnico junior en **Boochan Networks S.L.** Ya versiona con Git y ya se defiende en una terminal de Linux. Ahora le toca lo que hace de verdad un técnico el primer día de un cliente: **dejar un Windows con el software que tiene que tener**.
>
> Cada ejercicio arranca de un encargo real: algo que le pide **Lucía**, su responsable, o un marrón que le ha dejado **Carlos**, el senior que nunca documenta nada.

---

## **2 · DÓNDE SE HACE ESTE CURSO**

> [!important] 🖥️ Aquí **no hay máquina virtual**
> Los cursos de Git y de Shell te mandaban a una VM. Este no: **este curso se hace en el Windows 11 Pro que tienes delante**, con su terminal.
>
> Y es a propósito. Un gestor de paquetes existe para administrar **el equipo real de alguien**. Practicarlo en una máquina de usar y tirar le quitaría la mitad de la gracia: aquí el software que instales se queda instalado, y el que desinstales desaparece de verdad.

**Lo que necesitas:** un Windows 11 Pro, el terminal y conexión a Internet. Nada más.

> [!warning] ⚠️ Con el equipo real se trabaja con cabeza
> No hay instantánea a la que volver. Por eso, en este curso:
>
> - **Se instala lo que dice el ejercicio**, no lo que te apetezca probar.
> - **Antes de desinstalar algo, se comprueba qué es.** Hay una fase entera dedicada a eso.
> - Si un comando te pide confirmación, **se lee antes de aceptar**. Justo lo contrario de lo que hacías con los `.exe`.

---

## **3 · LAS SEIS FASES**

Cada fase tiene **su propio índice** con sus ejercicios ordenados por dificultad. Entra en la que toque:

| # | Fase | La idea central | Dónde te va a servir |
| :--- | :--- | :--- | :--- |
| **1** | **[Qué es un gestor de paquetes](fase-1-que-es-un-gestor-de-paquetes/README.md)** | Por qué bajar un `.exe` de Google es la peor forma de instalar software | Todo el módulo, y tu vida profesional |
| **2** | **[Buscar e instalar con winget](fase-2-buscar-e-instalar/README.md)** | Encontrar el paquete correcto y **saber que es el correcto** antes de instalarlo | La Fase 0.2 de prerrequisitos, que ya instala Git y Obsidian así |
| **3** | **[El parque al día](fase-3-el-parque-al-dia/README.md)** | Ver qué hay instalado, actualizarlo y quitar lo que sobra | Mantenimiento de cualquier equipo |
| **4** | **[Instalación en lote](fase-4-instalacion-en-lote/README.md)** | Dejar un equipo entero montado sin quince clics: se escribe una vez y se repite | `CE.01.f` — automatización de instalaciones |
| **5** | **[Chocolatey](fase-5-chocolatey/README.md)** | El otro gestor: **instalarlo tú**, usarlo y compararlo con winget | El criterio para elegir herramienta |
| **6** | **[Reto de cierre](fase-6-reto-final/README.md)** | Sin procedimiento: te dan el encargo y te lo montas | — |

> [!tip] 💡 Cómo se recorre
> **En orden.** La 4 no se entiende sin la 2, y la 5 no sirve de nada si no sabes contra qué estás comparando.
>
> Dentro de cada fase, los ejercicios van **de menos a más**:
>
> | Nivel | Qué es |
> | :--- | :--- |
> | 🟢 **N1 · Mínimo** | Lo que no se puede no saber |
> | 🔵 **N2 · Básico** | El uso normal del día a día |
> | 🟡 **N3 · Medio** | Donde empieza a hacer falta criterio |
> | 🟠 **N4 · Avanzado** | Lo que separa a quien administra de quien copia |
> | 🔴 **N5 · Reto** | Sin procedimiento: te lo montas tú |

**La numeración de los ejercicios es `EJ-0F-NN-MM`** = fase · nivel · número, igual que en los cursos de Git y de Shell.

---

## **4 · LOS DOS GESTORES, Y POR QUÉ DOS**

| | **winget** | **Chocolatey** |
| :--- | :--- | :--- |
| Quién lo hace | Microsoft | La comunidad |
| ¿Viene con Windows 11? | **Sí**, preinstalado | **No**: lo instalas tú, en la Fase 5 |
| Cuándo entra en el curso | Fases 2, 3 y 4 | Fase 5 |

> [!info] 🎓 Por qué te hago aprender dos cosas que hacen lo mismo
> Porque **no hacen exactamente lo mismo**, y un técnico no elige herramienta por costumbre: la elige por lo que necesita ese día.
>
> Y porque hay una diferencia que se aprende sola en cuanto la vives: **uno ya lo tienes y el otro te lo tienes que montar**. Cuando en la Fase 5 instales Chocolatey a mano, vas a entender de golpe por qué Microsoft acabó metiendo winget dentro de Windows.

Existe un tercero, **Scoop**, con otra filosofía. Lo verás nombrado en la comparativa de la Fase 5. No entra en los ejercicios.

---

## **5 · 📋 QUÉ SE TE EVALÚA EN ESTE CURSO**

> [!abstract] 📋 Resultados de aprendizaje y criterios de evaluación
> **RA.01** — Instala sistemas operativos en red describiendo sus características e interpretando la documentación técnica.
> **RA.05** — Realiza tareas de monitorización y uso del sistema operativo en red, describiendo las herramientas utilizadas.
>
> | Código | Criterio de evaluación | Dónde lo demuestras |
> | :--- | :--- | :--- |
> | `CE.05.d` | Se han realizado tareas de mantenimiento del software instalado en el sistema. | Todas las fases (1 a 6) |
> | `CE.01.f` | Se han aplicado procedimientos para la automatización de instalaciones. | Fases 4 y 6 |
> | `CE.01.e` | Se han seleccionado los componentes a instalar. | Fases 1, 2, 4, 5 y 6 — **cuando justificas la elección**, no cuando copias el comando |
> | `CE.05.e` | Se han ejecutado operaciones para la automatización de tareas del sistema. | Fases 3, 4 y 6 |
>
> Los criterios están tomados **literalmente del RD 1691/2007** y de la programación del módulo.

---

## **6 · CÓMO ES CADA EJERCICIO**

Todos siguen la misma estructura que ya conoces de Git y de Shell:

```
📌 Ficha            código, fase, nivel, playlist y nombre del vídeo
💼 Situación        el encargo de Lucía o el marrón de Carlos
📚 Fundamento       la idea, el error nº1, el vocabulario
🔗 Dónde lo usarás  dónde te aparece esto más adelante
📹 Grabación        las obligaciones del vídeo
🛠️ Procedimiento    Paso 0 (abre tus apuntes) y los pasos del ejercicio
🚩 Errores          tabla: error · qué pasa · cómo evitarlo
🤔 Comprueba        las preguntas, que van en tus apuntes
✅ Entregables      qué subes y cómo se llama
🎓 Qué has aprendido + Siguiente
```

---

## **7 · LO QUE ENTREGAS**

**Cada ejercicio son tres cosas**, y las tres van juntas:

| | |
| :--- | :--- |
| 📝 **Una entrada de apuntes** | En tu repositorio `apuntes-sor-t1`, carpeta `B0_Curso_Paquetes` |
| 📹 **Un vídeo** | En tu playlist `B0_Curso_Paquetes`, No listado |
| ⬆️ **El `push`** | Que sube la entrada a GitHub |

El nombre de cada entrada te lo da el propio ejercicio, y sigue el patrón `paq-<fase>.<nivel>.<num>-<titulo>.md`. El nombre del vídeo es **`B0.P.f.n.e · título`** — la **`P`** es de *paquetes*, igual que la `G` es de Git y la `S` de Shell.

El detalle completo —ruta, plantilla copiable y cómo se entrega— está en **[📦 Entregables](02_ENTREGABLES.md)**.

---

## **8 · 🛑 LOS TRES PASOS PREVIOS — NO TE LOS SALTES**

**Antes de abrir la Fase 1**, en este orden:

| # | Qué | Dónde está explicado |
| :--- | :--- | :--- |
| **1** | **Prepara tu sitio de trabajo:** descarga este curso y deja listo dónde vas a guardar todo | **[🛠️ Antes de empezar](01_ANTES_DE_EMPEZAR.md)** |
| **2** | **Entérate de qué tienes que entregar** y cómo se llaman tus ficheros | **[📦 Entregables](02_ENTREGABLES.md)** |
| **3** | **Empieza la Fase 1** | [Fase 1](fase-1-que-es-un-gestor-de-paquetes/README.md) |

> [!danger] 🛑 Si te saltas el paso 1, no tendrás dónde guardar el trabajo
> Y si te saltas el 2, escribirás los apuntes al final de memoria — que **cuenta como no entregado**.

---

> [!summary] 🎓 Lo que te llevas de este curso
> Que instalar software **no es hacer clic en Siguiente**: es una tarea de administración que se puede escribir, repetir y auditar.
>
> Y que el día que te toque dejar veinte equipos iguales, la diferencia entre tardar dos días y tardar una hora **es exactamente lo que se enseña aquí**.
>
> **Empieza por:** [🛠️ Antes de empezar](01_ANTES_DE_EMPEZAR.md).
