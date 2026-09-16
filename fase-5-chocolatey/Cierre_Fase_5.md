---
Tipo: cierre-de-fase
Fase: 05
Título: Cierre de la Fase 5 — Chocolatey
---

## 🏁 Cierre de la Fase 5 — Chocolatey

> [!info] Para qué es esta página
> No es un ejercicio nuevo y **no se graba**: es una parada para consolidar. La Fase 6 es el reto final del curso y da por sabido todo lo anterior, así que si algo no lo tienes claro, **para y repásalo** (o pregúntame) antes de seguir.

---

## 🎓 Lo que has aprendido en la Fase 5

- Que **hay más de un gestor de paquetes**, y por qué uno viene con Windows y el otro no.
- A **leer un script antes de ejecutarlo**, aunque no lo entiendas entero — el hábito, no la auditoría.
- Qué hace cada trozo de una orden de instalación: la que permite ejecutar scripts, la que descarga y la que ejecuta.
- Que **un gestor de paquetes puede instalar otro gestor de paquetes**, y cuándo eso te conviene.
- Que los conceptos se repiten entre herramientas: **buscar, ver, instalar, actualizar, quitar**.
- Que los **nombres de los paquetes no se traducen** de un catálogo a otro: se buscan.
- Que las herramientas **cambian** —`choco list` ya no busca en remoto— y que por eso manda la ayuda de la que tienes instalada, no un tutorial de hace años.
- A comparar dos herramientas con **criterios medibles**, y a declarar **el tamaño de la muestra**.
- Que un informe serio incluye **lo que no ha podido medir**.
- Que una recomendación tiene **por defecto, excepción y límite**, y que *"depende"* solo vale si dices de qué.
- A **buscarte tú el mejor argumento en contra** de tu propia decisión.

---

## ❓ Preguntas de repaso

> [!question] Responde en tus apuntes antes de seguir
> Con tus palabras. Si la respuesta es copiar una línea del ejercicio, no cuenta.
> 1. ¿Por qué winget viene instalado y Chocolatey no? Contesta por **quién hace cada uno**.
> 2. Una orden que descarga un script y lo ejecuta en el mismo gesto: **¿qué riesgo tiene ese patrón**, más allá de Chocolatey?
> 3. Nombra las **cinco casillas** que tiene todo gestor de paquetes, y di cómo se llaman en los dos que conoces.
> 4. ¿Por qué el identificador de un paquete no se puede traducir de memoria de un gestor a otro?
> 5. Comparaste cuatro programas. ¿Qué **puedes** afirmar con esa muestra y qué **no**?
> 6. ¿En qué caso no usarías ningún gestor de paquetes?

---

## ✅ Tabla de verificación (¿sé hacerlo yo solo?)

> [!success] Marca solo lo que puedas hacer SIN mirar los apuntes
> | Sé… | ¿Sí? |
> | :--- | :---: |
> | Instalar Chocolatey y comprobar que ha quedado bien | ☐ |
> | Explicar qué hace cada parte de su orden de instalación | ☐ |
> | Decir por qué se mira un script antes de ejecutarlo | ☐ |
> | Instalar Chocolatey usando winget, y decir cuándo me interesa esa vía | ☐ |
> | Buscar en el catálogo de Chocolatey | ☐ |
> | Ver lo que tengo instalado por Chocolatey, y saber qué NO me enseña | ☐ |
> | Instalar un paquete con `choco` sin que se pare a preguntar | ☐ |
> | Poner al lado las cinco casillas de los dos gestores | ☐ |
> | Comparar dos herramientas declarando la muestra y la fecha | ☐ |
> | Escribir lo que mi comparativa **no** demuestra | ☐ |
> | Dar una recomendación con su por defecto, su excepción y su límite | ☐ |

---

## 🚑 Errores frecuentes de toda la Fase 5

> [!bug] Si algo falla, empieza por aquí
> | Síntoma | Causa habitual | Solución |
> | :--- | :--- | :--- |
> | `choco` no se reconoce tras instalarlo | La terminal vieja no conoce el comando nuevo | Cierra y abre una terminal nueva. |
> | La instalación de Chocolatey falla a mitad | Terminal sin elevar | Ejecutar como administrador. |
> | `choco install` da error de permisos | Lo mismo | Como administrador. |
> | Busco con `choco list` y no encuentro nada | Desde la v2, `list` es solo local | `choco search` para el catálogo. |
> | El identificador de winget no funciona en choco | Los catálogos usan nombres distintos | Búscalo en el catálogo que estés usando. |
> | La instalación se para preguntando | Falta la confirmación automática | `-y`, sabiendo lo que aceptas. |
> | Mi comparativa no convence a nadie | Sin muestra declarada ni datos | Muestra, fecha y un dato por conclusión. |

---

> [!warning] ⚠️ Lo que te llevas de esta fase, más allá de los comandos
> Que aprender una herramienta nueva **no es empezar de cero**: es buscar dónde están las casillas que ya conoces. Y que elegir entre dos herramientas es un trabajo con método —medir, declarar límites, decidir, buscarse las objeciones— y no una cuestión de gustos.

---

> [!tip] Siguiente paso
> Cuando tengas la tabla de verificación completa, pasa a la **Fase 6 — el reto final**: un encargo completo, sin decirte con qué herramienta ni con qué comandos. Solo el problema y las pruebas que hay que superar.

**Siguiente:** [Fase 6 — El reto final](../fase-6-reto-final/README.md) · [← Volver al índice del curso](../00_INDICE.md)
