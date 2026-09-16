---
Tipo: cierre-de-fase
Fase: 03
Título: Cierre de la Fase 3 — El parque al día
---

## 🏁 Cierre de la Fase 3 — El parque al día

> [!info] Para qué es esta página
> No es un ejercicio nuevo y **no se graba**: es una parada para consolidar. La Fase 4 da por sabido todo lo que hay aquí, así que si algo no lo tienes claro, **para y repásalo** (o pregúntame) antes de seguir.

---

## 🎓 Lo que has aprendido en la Fase 3

- Que `winget list` enseña **el equipo entero**, no solo lo que instaló winget.
- A distinguir un paquete **reconocido** —que se puede mantener— de uno que no lo es.
- Que **un inventario lleva fecha**, o no sirve.
- Que `winget upgrade` a secas **lista y no toca nada**, y a comparar versión instalada contra disponible.
- Que **"no sale en la lista" no es "está al día"**: existe el montón de los que no se pueden comprobar, y se declara.
- El orden profesional para actualizar: mirar, **uno primero**, comprobar, el resto, volver a mirar.
- Que la comprobación de verdad es **abrir el programa**, no leer un número de versión.
- Que `uninstall` **exige puntería** y te para si hay ambigüedad — y que eso te protege.
- Que winget puede **desinstalar** lo que él no instaló, pero no **actualizarlo**.
- La regla que más equipos salva: **si no sabes qué es, no lo tocas y lo apuntas.**
- A **fijar** un paquete para que el mantenimiento lo respete, en sus dos intensidades, y a deshacerlo.
- Que una decisión de administración **sin documentar se pierde**, y con ella el motivo.

---

## ❓ Preguntas de repaso

> [!question] Responde en tus apuntes antes de seguir
> Con tus palabras. Si la respuesta es copiar una línea del ejercicio, no cuenta.
> 1. Un compañero dice: *"he mirado el equipo y está todo al día"*. Dile **las dos preguntas** que le harías antes de creerle.
> 2. ¿Por qué se actualiza uno primero y luego el resto? Explícalo en términos de **qué pasa cuando algo falla**.
> 3. ¿Por qué `uninstall` no adivina cuando la consulta es ambigua, y `install` en cambio a veces sí resolvía solo?
> 4. winget puede quitar un programa que no instaló, pero no actualizarlo. **¿Por qué esa asimetría?**
> 5. ¿Qué tres cosas tiene que llevar por escrito un paquete fijado, además del propio fijado?
> 6. De todo lo de esta fase, ¿qué harías **antes** de tocar el equipo de un cliente? Ordena los pasos.

---

## ✅ Tabla de verificación (¿sé hacerlo yo solo?)

> [!success] Marca solo lo que puedas hacer SIN mirar los apuntes
> | Sé… | ¿Sí? |
> | :--- | :---: |
> | Sacar el inventario de un equipo y filtrarlo | ☐ |
> | Distinguir un paquete reconocido de uno que no lo es | ☐ |
> | Sacar la lista de lo que tiene actualización disponible | ☐ |
> | Hacer aparecer los que no se pueden comprobar, y explicar qué son | ☐ |
> | Actualizar un paquete concreto y comprobarlo de verdad | ☐ |
> | Actualizar todo el equipo sabiendo qué va a tocar | ☐ |
> | Desinstalar un paquete sin ambigüedad y comprobar que se ha ido | ☐ |
> | Decidir que algo **no** se toca, y justificarlo | ☐ |
> | Fijar un paquete, comprobar que el mantenimiento lo respeta y quitarlo | ☐ |
> | Explicar la diferencia entre fijado normal y bloqueante | ☐ |
> | Escribir la ficha de decisión de un fijado | ☐ |

---

## 🚑 Errores frecuentes de toda la Fase 3

> [!bug] Si algo falla, empieza por aquí
> | Síntoma | Causa habitual | Solución |
> | :--- | :--- | :--- |
> | `winget upgrade` no lista nada | Puede que esté todo al día, o que no pueda comprobarlo | Prueba `--include-unknown` antes de concluir. |
> | Actualicé y el programa no abre | Cambio de versión con efectos | Por eso se actualiza **uno primero** y se abre. |
> | `uninstall` me pide afinar | Consulta ambigua | `--id` con el identificador exacto y `-e`. |
> | Quité algo y otro programa dejó de funcionar | Era una dependencia | Si no sabes qué es, **no se toca**. |
> | Un paquete no se actualiza nunca y no sé por qué | Puede estar fijado | `winget pin list`. |
> | Puse un fijado y ya no me deja actualizar ni a la fuerza | Es **bloqueante** | `pin remove`, o `--force` sabiendo lo que haces. |
> | Mi inventario de hace meses no me sirve | No tenía fecha | Cabecera con fecha, siempre. |

---

> [!warning] ⚠️ Lo que te llevas de esta fase, más allá de los comandos
> Que mantener un equipo es **decidir**, no ejecutar. Qué se actualiza, qué se quita, qué se deja quieto y **por qué** — y que todo eso se escribe, porque el siguiente que abra ese equipo no vas a ser tú.

---

> [!tip] Siguiente paso
> Cuando tengas la tabla de verificación completa, pasa a la **Fase 4 — Instalación en lote**: dejar un equipo entero montado sin quince clics, escribiendo una vez lo que se repite muchas. Es donde todo lo de las Fases 2 y 3 se convierte en algo que se lanza solo.

**Siguiente:** [Fase 4 — Instalación en lote](../fase-4-instalacion-en-lote/README.md) · [← Volver al índice del curso](../00_INDICE.md)
