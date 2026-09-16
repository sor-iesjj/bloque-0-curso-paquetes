# 🛠️ Antes de empezar — prepara tu sitio de trabajo

> **Módulo:** SOR — Sistemas Operativos en Red · **Bloque 0 · Curso de Gestores de Paquetes**
>
> **📍 Cuándo se lee:** **AHORA.** Antes de la Fase 1 y antes de instalar nada.

---

> [!danger] 🛑 No abras la Fase 1 sin haber hecho esto
> Aquí dejas listas **las tres cosas** que vas a necesitar durante todo el curso: **el material**, **tu cuaderno** y **dónde se guarda todo**.
>
> Si empiezas sin esto, en el primer ejercicio te van a pedir que guardes una entrada y que hagas un `push`… **y no vas a tener ni dónde ni a dónde.**

---

## **1 · DE DÓNDE VIENES**

Este curso **no empieza de cero**. Das por hecho que ya tienes:

| Ya deberías tener | De dónde sale |
| :--- | :--- |
| Una **cuenta de GitHub** con Git configurado y SSH | **Bloque 0 · Fase 0.2** |
| Tu **bóveda** `Boveda_SOR` en Obsidian | **Bloque 0 · Fase 0.1** |
| Tu **repositorio de apuntes** `apuntes-sor-t1` | **Bloque 0 · Fase 0.3** |
| Saber hacer `clone`, `add`, `commit` y `push` | El **curso de Git** |

> [!warning] ⚠️ Si te falta alguna de las cuatro, para aquí
> Vuelve a los prerrequisitos y termínalos. **Este curso los usa desde el primer ejercicio** y no los vuelve a explicar.

---

## **2 · 🔴 LAS DOS TERMINALES — no las confundas**

Esto es nuevo y conviene tenerlo claro desde hoy, porque en este curso vas a usar **dos terminales distintas para dos cosas distintas**:

| Para qué | Dónde se escribe |
| :--- | :--- |
| Los comandos del curso: `winget`, y más adelante Chocolatey | **Terminal de Windows / PowerShell** |
| Los comandos de Git para entregar: `add`, `commit`, `push` | **Git Bash**, igual que vienes haciendo desde la Fase 0.2 |

> [!info] 🎓 Por qué dos
> Porque son dos mundos: **Git Bash** es un intérprete de estilo Unix que te instalaste con Git para trabajar como en Linux, y **PowerShell** es el intérprete propio de Windows, que es donde vive `winget`.
>
> No te compliques: **el ejercicio te dice siempre en cuál estás**. Cuando veas comandos de instalación, PowerShell. Cuando veas `git`, Git Bash, como siempre.

**Abre la Terminal de Windows ahora** y escribe:

```
winget --version
```

- **✅ Bien:** te responde con un número de versión. Ya tienes winget. **No hay nada que instalar.**
- **❌ Mal:** *"no se reconoce como el nombre de un cmdlet"* → avísame en clase. No sigas por tu cuenta.

> [!success] 🎯 Acabas de hacer algo importante
> Has comprobado que la herramienta existe **antes** de necesitarla, en vez de descubrirlo a mitad del primer ejercicio con la grabación en marcha. Esa costumbre vale para todo lo que viene después.

---

## **3 · CÓMO ESTÁ ORGANIZADA TU BÓVEDA** *(recuerdo rápido)*

```
Boveda_SOR/
├── 00_Apuntes/
│   └── Trimestre_1/               ← 📝 ESTO es tu repositorio 'apuntes-sor-t1'
│       ├── B0_Prerrequisitos/
│       ├── B0_Curso_Shell/
│       └── B0_Curso_Paquetes/     ← 🆕 la creas hoy: aquí van tus entradas
│
└── 01_Practicas/
    └── B0_Curso_Paquetes/         ← 🆕 la creas hoy: aquí va ESTE material
```

> [!info] 🎓 Por qué van separados tus apuntes y el material
> Porque **son de dueños distintos**: los apuntes los escribes tú y te los corrijo; el material te lo doy yo.
>
> Y porque **son dos repositorios distintos**: cuando hagas `push` de tus apuntes, no quieres estar subiendo también los ficheros del curso.

---

## **4 · 🔴 PASO 1 — TRAE ESTE CURSO A TU ORDENADOR**

El material vive en un **repositorio plantilla** mío. Tú **sacas tu propia copia** y la clonas.

### **4A · Saca tu copia en GitHub**

1. Abre el repositorio del curso: **`github.com/sor-iesjj/bloque-0-curso-paquetes`**
2. Pulsa el botón verde **`Use this template`** → **`Create a new repository`**
3. **Repository name:** `bloque-0-curso-paquetes` *(déjalo igual)*
4. Ponlo **público** o **privado**, como prefieras
5. **`Create repository`**

> [!info] 🎓 Qué acaba de pasar
> Ese repositorio **ya no es mío: es tuyo.** Tiene su propio historial y puedes escribir, romper y subir sin pedirle permiso a nadie.
>
> Es exactamente lo que hiciste en la **Bloque 0 · Fase 0.4.a**. Todos los repos del curso son plantilla.

### **4B · Clónalo en tu bóveda**

Abre **Git Bash** y ve a tu carpeta de prácticas:

```bash
cd ~/Boveda_SOR/01_Practicas
git clone git@github.com:TU-USUARIO/bloque-0-curso-paquetes.git B0_Curso_Paquetes
cd B0_Curso_Paquetes
ls
```

> [!warning] ⚠️ Cambia `TU-USUARIO` por tu usuario de GitHub
> El resto de la línea, **tal cual**. Incluido el `B0_Curso_Paquetes` del final.

> [!important] 📌 El `B0_Curso_Paquetes` del final no está de adorno
> Es el **segundo argumento** de `git clone`, y es el que decide **cómo se va a llamar la carpeta** en tu ordenador:
>
> ```
> git clone  <dirección del repositorio>  <nombre de la carpeta>
> ```
>
> **Si lo omites**, Git le pone el nombre del repositorio — te quedaría `bloque-0-curso-paquetes/` — y tendrías **la misma cosa con dos nombres distintos** según dónde la mires.
>
> Ya lo usaste en la **Bloque 0 · Fase 0.3**, cuando clonaste `apuntes-sor-t1` y le dijiste que se llamara `Trimestre_1`.

> [!info] 🎓 Entonces, ¿por qué el repositorio se llama de otra manera?
> Porque **GitHub obliga**: los nombres de repositorio van en minúsculas y con guiones, no admite `B0_Curso_Paquetes`.
>
> | Dónde vive | Cómo se llama |
> | :--- | :--- |
> | **En GitHub**, el repositorio | `bloque-0-curso-paquetes` *(me lo impone GitHub)* |
> | **En tu ordenador**, la carpeta | `B0_Curso_Paquetes` *(lo decides tú, con el segundo argumento)* |
>
> **Dentro de tu bóveda, una cosa tiene un nombre y solo uno.** Tus apuntes están en `B0_Curso_Paquetes`, el material está en `B0_Curso_Paquetes`, y tu playlist se llama `B0_Curso_Paquetes`.

- **✅ Bien:** el `ls` te muestra `00_INDICE.md`, `01_ANTES_DE_EMPEZAR.md`, `02_ENTREGABLES.md` y las carpetas de las fases.
- **❌ Mal:** *"Permission denied (publickey)"* → tu SSH no está configurado. Vuelve a la **Bloque 0 · Fase 0.2.2**.

---

## **5 · 🔴 PASO 2 — PREPARA TU CUADERNO**

Tus apuntes **NO van en la carpeta del curso**. Van en tu repositorio de apuntes. Sigue en **Git Bash**:

```bash
cd ~/Boveda_SOR/00_Apuntes/Trimestre_1
mkdir -p B0_Curso_Paquetes
ls
```

- **✅ Bien:** ves `B0_Curso_Paquetes` junto a `B0_Prerrequisitos`.

> [!danger] 🛑 Comprueba que estás dentro de tu repositorio
> ```bash
> git status
> ```
> - **✅ Bien:** te responde algo sobre la rama y los cambios.
> - **❌ Mal:** *"not a git repository"* → **te has equivocado de carpeta**. `Trimestre_1` es tu repositorio `apuntes-sor-t1`; si `git` no lo reconoce, estás fuera.
>
> **No sigas hasta que `git status` responda.** Si no, escribirás apuntes que no se van a subir a ninguna parte.

---

## **6 · 🔴 PASO 3 — HAZ LA PRUEBA COMPLETA AHORA, CON UN FICHERO TONTO**

**No esperes al primer ejercicio para descubrir que algo no funciona.** Recorrido entero con un fichero de prueba, en **Git Bash**:

```bash
cd ~/Boveda_SOR/00_Apuntes/Trimestre_1
echo "# Prueba del curso de Paquetes" > B0_Curso_Paquetes/prueba.md

git add B0_Curso_Paquetes/
git commit -m "Curso Paquetes: prueba de que puedo subir apuntes"
git push
```

**Ahora abre `github.com/TU-USUARIO/apuntes-sor-t1` en el navegador.**

- **✅ Bien:** ves la carpeta `B0_Curso_Paquetes` con `prueba.md` dentro.
- **❌ Mal:** si el `push` da error, **arréglalo hoy**. Es el mismo problema que tendrás en todos los ejercicios.

**Y ahora borra el fichero de prueba**, que ya ha cumplido:

```bash
rm B0_Curso_Paquetes/prueba.md
git add B0_Curso_Paquetes/
git commit -m "Curso Paquetes: quito el fichero de prueba"
git push
```

> [!success] 🎯 Por qué te hago esto antes de empezar
> Porque **acabas de comprobar el circuito entero** —escribir, añadir, confirmar, subir y verlo en GitHub— **con algo que no importa**.
>
> El día que falle, fallará con un fichero de prueba y no con el trabajo de tres horas.

---

## **7 · 🔴 PASO 4 — CREA TU PLAYLIST**

En tu cuenta de YouTube, crea **una playlist llamada `B0_Curso_Paquetes`** y ponla como **No listada**.

**Una sola para todo el curso.** No hagas una por fase: el nombre del vídeo ya lleva la fase dentro (`B0.P.2.1.1`), así que se ordenan solos.

---

## **8 · CÓMO VA A SER TU DÍA A DÍA**

A partir de ahora, en cada ejercicio:

```
1. Abres el ejercicio en   01_Practicas/B0_Curso_Paquetes/fase-N-…/EJ-….md
2. Abres tu entrada en     00_Apuntes/Trimestre_1/B0_Curso_Paquetes/paq-….md
   (el nombre te lo da el propio ejercicio, en su Paso 0)
3. Grabas con OBS y haces el ejercicio en la Terminal de Windows
4. Escribes tus apuntes MIENTRAS trabajas, no al final
5. Subes el vídeo y pegas su enlace en la entrada
6. En Git Bash: git add → git commit → git push
```

> [!important] 📌 Los seis pasos, siempre iguales
> **No te los vas a aprender leyéndolos**: te los vas a aprender repitiéndolos. En los tres primeros ejercicios te los recuerdo enteros. A partir del cuarto, ya son tuyos.

---

## ✅ **CHECKLIST — no pases a la Fase 1 sin esto**

- [ ] `winget --version` me responde con un número de versión.
- [ ] Tengo mi copia del curso en GitHub *(botón `Use this template`)*.
- [ ] La he clonado en `01_Practicas/B0_Curso_Paquetes/` y el `ls` muestra las fases.
- [ ] He creado `00_Apuntes/Trimestre_1/B0_Curso_Paquetes/`.
- [ ] `git status` me responde desde `Trimestre_1` *(estoy dentro del repo)*.
- [ ] **He hecho la prueba completa**: fichero → `add` → `commit` → `push` → **lo he visto en GitHub**.
- [ ] He borrado el fichero de prueba y he subido el borrado.
- [ ] He creado la playlist `B0_Curso_Paquetes` como **No listada**.
- [ ] He leído **[📦 Entregables](02_ENTREGABLES.md)** y sé cómo se llama cada entrada.

---

> [!summary] 🎓 Qué has dejado listo
> **El material** en `01_Practicas/`, **tu cuaderno** en `00_Apuntes/`, **la playlist** y **comprobado que puedes subir a GitHub**.
>
> Y sabes algo que hace cinco minutos no sabías: **que tu Windows ya traía un gestor de paquetes puesto de fábrica**, y que llevas meses sin usarlo.
>
> **Siguiente:** [📦 Qué tienes que entregar](02_ENTREGABLES.md).
