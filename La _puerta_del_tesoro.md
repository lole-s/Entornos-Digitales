# Actividad ED: La puerta del tesoro

**1.º año — Operadores de comparación y lógicos — 80 minutos**

## Objetivos
Reconocer variables y condiciones; comparar valores con `>`, `<`, `>=`, `<=`, `==`; combinar expresiones con **Y**, **O** y **NO**; interpretar y modificar las reglas de un videojuego.

## 1. Repaso (15 minutos)
Una **variable** guarda un dato que puede cambiar. En el juego: `monedas` (número) y `tieneLlave` (verdadero/falso).

Una **comparación** devuelve verdadero o falso:

| Operador | Significado | Ejemplo |
|---|---|---|
| `>` | Mayor que | `monedas > 3` |
| `<` | Menor que | `monedas < 5` |
| `>=` | Mayor o igual | `monedas >= 3` |
| `<=` | Menor o igual | `monedas <= 4` |
| `==` | Igual | `monedas == 2` |

**Y**: deben cumplirse ambas condiciones. **O**: basta una. **NO**: invierte verdadero/falso.

**Para el pizarrón:** con `monedas = 3` y `tieneLlave = verdadero`, determinar:
1. `monedas >= 3 Y tieneLlave`
2. `monedas == 5 O tieneLlave`
3. `NO tieneLlave Y monedas < 4`

## 2. ¡A jugar! (30 minutos)
**Juego:** [LA PUERTA DEL TESORO](https://makecode.com/_5MhEHpTDdChF)]

Abrí el enlace, leé la regla del nivel y conseguí que la puerta se abra.

**Controles:**
- Flechas: mover al personaje.
- **Espacio** (botón A de MakeCode): intentar salir estando sobre la puerta.
- **Botón virtual B**: tomar la llave si estás cerca, o soltarla si ya la tenés.
- **Flecha abajo + botón B**: reiniciar el nivel.
- **Botón Menú del simulador**: volver a consultar la regla.

**Atención:** A y B son botones del simulador, no necesariamente las letras del teclado. La puerta cerrada no indica qué condición falló: tenés que razonarlo.

## 3. Antes de probar, pensá (15 minutos)
Completá si la puerta se abre y justificá.

| Regla | Situación | ¿Se abre? ¿Por qué? |
|---|---|---|
| `LLAVE Y MONEDAS >= 2` | Con llave y 1 moneda | |
| `LLAVE O MONEDAS >= 4` | Sin llave y 4 monedas | |
| `NO LLAVE Y MONEDAS >= 3` | Con llave y 5 monedas | |
| `MONEDAS == 2` | Con 3 monedas | |

**Pregunta:** ¿Por qué a veces conviene **soltar** la llave?

## 4. Modificar el juego (15 minutos)
Con ayuda del docente, abrí el proyecto en el editor MakeCode Arcade y buscá la función `cumpleRegla`.

1. Cambiá `monedas >= 2` por `monedas >= 4`. ¿Qué cambia?
2. Reemplazá **Y** por **O** en una regla. Inventá una situación que ahora permita salir.
3. **Bonus:** inventá una regla con **NO**, **Y** y **O**. Describí dos situaciones que permitan salir y una que no.

En JavaScript, `&&` es Y, `||` es O y `!` es NO.

## 5. Cierre (5 minutos)
- ¿Qué diferencia hay entre `==` y `>=`?
- ¿En qué se diferencian Y y O?
- ¿Por qué conviene probar distintos casos?

---

## Guía docente
**Repaso:** verdadero, verdadero, falso.

**Tabla:** no, sí, no, no.

**Organización:** proyectar los primeros niveles; dejar el resto como trabajo individual o en parejas. Quienes avancen rápido pueden modificar una regla y probar casos límite.

**Antes de la clase:** importar el código del juego en MakeCode Arcade, comprobar controles y sonido, publicar el proyecto y reemplazar el marcador del enlace.

**Estado del código:** la versión con llave que se toma/suelta y reinicio con abajo+B está preparada, pero pendiente de compilación y prueba en el simulador.
