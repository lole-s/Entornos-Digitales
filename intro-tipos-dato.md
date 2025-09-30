# Introducción a los tipos de datos, variables y operadores

## 1. ¿Qué son los **tipos de datos**?

En Scratch o PilasBloques cuando usabas un bloque de **texto**, de **número** o de **verdadero/falso**, ya estabas usando distintos **tipos de datos**.
En programación, los tipos de datos nos dicen **qué clase de información guardamos o usamos**.
Los más comunes son:

* **Números** → sirven para contar o calcular. Ej: `5`, `12`, `3.14`.
* **Texto (cadenas de caracteres)** → palabras o frases. Ej: `"Hola"`, `"Mi nombre es Ana"`.
* **Verdadero o Falso (booleanos)** → solo tienen dos valores: `True` (sí) o `False` (no).
* (Más adelante veremos otros, como listas o conjuntos de datos).

---

## 2. ¿Qué son las **variables**?

Una **variable** es como una **cajita con nombre** donde podemos guardar información.

* En Scratch seguramente usaste, o sino vamos a usar, el bloque **“crear variable”** para guardar un número de vidas o puntos.
* En Python funciona igual, pero en lugar de bloques usamos texto.

Ejemplo en Scratch:

* Variable → `puntos`
* Le damos valor → `puntos = 10`

En Python se vería así:

```python
puntos = 10
nombre = "Ana"
ganador = True
```

Cada variable puede guardar un **tipo de dato distinto**: número, texto o booleano.

---

## 3. ¿Qué son los **operadores**?

Los operadores son símbolos que nos permiten **hacer operaciones** con los datos.

Los más usados son:

* **Aritméticos** (con números):

  * `+` → sumar
  * `-` → restar
  * `*` → multiplicar
  * `/` → dividir

  Ejemplo: `5 + 3` da `8`.

* **De comparación o relacionales** (devuelven Verdadero o Falso):

  * `==` → ¿son iguales?
  * `!=` → ¿son distintos?
  * `<` → menor que
  * `>` → mayor que

  Ejemplo: `5 > 3` es `True`.

* **Lógicos o booleanos** (combinan condiciones):

  * `and` → se cumple si **las dos** condiciones son verdaderas.
  * `or` → se cumple si **al menos una** es verdadera.
  * `not` → niega el resultado (cambia de verdadero a falso y al revés).

---

## 4. Conexión con lo que ya conocés

* En Scratch cuando usas un bloque verde de suma (`3 + 2`) estas usando **operadores aritméticos**.
* Cuando preguntas `¿x es mayor que 10?`, estaas usando un **operador de comparación**.
* Cuando guardas el puntaje o el nombre de un personaje, estas usando una **variable**.

---

## 5. Ejemplo simple en Python

```python
# Guardamos datos
nombre = "Sofía"
edad = 11
es_estudiante = True

# Usamos operadores
suma = edad + 5        # suma da 16
mayor = edad > 10      # mayor da True
```

