---
Tipo: cierre-de-fase
Fase: 04
Título: Cierre de la Fase 4 — Instalación en lote
---

## 🏁 Cierre de la Fase 4 — Instalación en lote

> [!info] Para qué es esta página
> No es un ejercicio nuevo y **no se graba**: es una parada para consolidar. La Fase 5 da por sabido todo lo que hay aquí, así que si algo no lo tienes claro, **para y repásalo** (o pregúntame) antes de seguir.

---

## 🎓 Lo que has aprendido en la Fase 4

- Que **un equipo cabe en un fichero de texto**, y que ese fichero es la receta para reconstruirlo.
- Que el fichero exportado solo lleva **lo que el catálogo reconoce**, y que la diferencia **se declara siempre**.
- A decidir entre un equipo **idéntico** (con versiones) y uno **al día** (sin ellas), y a justificar cuál quieres.
- Que un **perfil de puesto** no es una foto: es una decisión que se escribe, se revisa y se reutiliza.
- A construir un fichero de importación partiendo de uno válido, sin romper su estructura.
- Qué hace una importación con lo que **ya está instalado**, y cómo cambiar ese comportamiento.
- Las tres formas en que una importación se tuerce en un equipo ajeno: **paquete no disponible**, **versión que ya no existe** y **algo que pregunta**.
- Que **ignorar un error no es resolverlo**: obliga a una revisión posterior, y esa revisión se documenta.
- Que aceptar acuerdos automáticamente es **una decisión**, no un tecnicismo para quitar un mensaje.
- Que *"en mi equipo funciona"* no es una entrega.
- A escribir documentación para **dos lectores distintos**: quien ejecuta y quien mantiene.

---

## ❓ Preguntas de repaso

> [!question] Responde en tus apuntes antes de seguir
> Con tus palabras. Si la respuesta es copiar una línea del ejercicio, no cuenta.
> 1. ¿Por qué el fichero exportado **no** es el equipo entero? Explica qué se queda fuera y por qué.
> 2. Diferencia entre el fichero del `EJ-04-01-01` y el del `EJ-04-02-01`: **qué representa cada uno**.
> 3. Toda la fase se apoya en algo que aprendiste en la Fase 2: los identificadores exactos. **¿Por qué es aquí donde de verdad importa?**
> 4. Explica la diferencia entre **resolver** un error y **ignorarlo**, con el caso del paquete no disponible.
> 5. ¿Qué hay que revisar **después** de una instalación desatendida, y por qué no basta con que no diera error?
> 6. ¿Por qué una automatización se diseña pensando en un equipo recién formateado y no en el tuyo?

---

## ✅ Tabla de verificación (¿sé hacerlo yo solo?)

> [!success] Marca solo lo que puedas hacer SIN mirar los apuntes
> | Sé… | ¿Sí? |
> | :--- | :---: |
> | Exportar el software de un equipo a un fichero | ☐ |
> | Abrir ese fichero y explicar qué guarda de cada paquete | ☐ |
> | Decir qué parte del equipo **no** ha entrado en el fichero, y por qué | ☐ |
> | Elegir entre exportar con versiones o sin ellas, y justificarlo | ☐ |
> | Escribir el fichero de un puesto que no existe todavía | ☐ |
> | Lanzar una instalación en lote y comprobar el resultado | ☐ |
> | Hacer que la importación no se pare si falta un paquete | ☐ |
> | Hacer que no se detenga a preguntar | ☐ |
> | Decir qué acepto automáticamente y por qué | ☐ |
> | Explicar qué hay que revisar después de ejecutarla | ☐ |
> | Documentar el puesto para quien lo ejecuta **y** para quien lo mantiene | ☐ |

---

## 🚑 Errores frecuentes de toda la Fase 4

> [!bug] Si algo falla, empieza por aquí
> | Síntoma | Causa habitual | Solución |
> | :--- | :--- | :--- |
> | La importación no arranca | El JSON está roto: falta una llave o una coma | Vuelve a copiar un fichero exportado y edítalo con cuidado. |
> | Se para a la mitad | Un paquete no disponible, o algo que pregunta | Mira las opciones de `winget import --help`, una cada vez. |
> | No instala lo que esperaba | Identificador mal escrito o de otra fuente | De `winget search`, y comprueba la columna de fuente. |
> | Dice que todo fue bien pero faltan programas | Usaste una opción que ignora errores | Revisa con `winget list` **cada** paquete de la lista. |
> | Funciona en mi equipo y en otro no | Tu equipo ya tenía cosas puestas y acuerdos aceptados | Piensa siempre en la máquina recién formateada. |
> | Exporté y faltan programas en el fichero | winget no los reconoce en el catálogo | Es normal: **decláralo**, no lo escondas. |
> | Nadie entiende mis instrucciones | Escritas para un técnico | Reescríbelas para quien va a ejecutarlas. |

---

> [!warning] ⚠️ Lo que te llevas de esta fase, más allá de los comandos
> Que automatizar **no es escribir un comando más largo**: es describir en un documento cómo tiene que quedar algo, y que ese documento sobreviva a salir de tu escritorio.
>
> El comando es una línea. El trabajo es el fichero, las decisiones que hay detrás y la documentación que permite a otro repetirlo.

---

> [!tip] Siguiente paso
> Cuando tengas la tabla de verificación completa, pasa a la **Fase 5 — Chocolatey**: el otro gestor. Lo vas a **instalar tú**, usarlo, y compararlo con winget con criterios propios.
>
> Y ahí verás por qué el curso ha insistido tanto en entender **qué es una fuente** y **qué es un identificador**: cuando llegas a la segunda herramienta, todo eso se repite con otros nombres.

**Siguiente:** [Fase 5 — Chocolatey](../fase-5-chocolatey/README.md) · [← Volver al índice del curso](../00_INDICE.md)
