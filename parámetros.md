### **¿Qué es un parámetro?**
Imagina que tienes una **máquina mágica** que hace galletas. Esta máquina tiene un **botón de sabor**: tú le das el sabor (por ejemplo, "chocolate" o "vainilla"), y la máquina hace una galleta con ese sabor exacto.  
👉 **El parámetro es como ese "botón de sabor"**: le dice a la máquina **cómo debe hacer su trabajo**.

---

### **En la vida real:**
- Si le dices a un amigo: "¡Saluda a María!", el nombre "María" es como un parámetro.  
- Si le dices: "Dibuja un círculo de tamaño gigante", "gigante" es el parámetro.

---

### **En programación:**
Un parámetro es un **dato que le pasas a una función** para que se comporte de manera diferente cada vez.  
Es como un "comodín" que la función usa para personalizar lo que hace.

---

### **Ejemplo en Scratch:**
1. Creamos un bloque llamado `Saludar` con un parámetro de texto llamado `nombre`.  
2. Dentro del bloque, ponemos:  
   `decir "¡Hola, [nombre]!"`  
3. Cuando usemos el bloque y escribamos `Saludar [Ana]`, el gato dirá: "¡Hola, Ana!".  
   Si usamos `Saludar [Luis]`, dirá "¡Hola, Luis!".

📌 **El parámetro `nombre` hace que el saludo cambie.**

---

### **Ejemplo en Python:**
```python
def saludar(nombre):  # "nombre" es el parámetro
    print("¡Hola,", nombre, "!")

saludar("Ana")   # Imprime: ¡Hola, Ana!
saludar("Luis")  # Imprime: ¡Hola, Luis!
```

---

### **¿Por qué usamos parámetros?**
- **Evitan repetir código**: En vez de hacer 100 funciones para saludar a 100 personas, hacemos **una sola función** que acepte un parámetro.  
- **Hacen los programas más flexibles**: La misma función puede hacer muchas cosas distintas dependiendo del parámetro.

---

### **Analogía final:**
Un parámetro es como **el ingrediente secreto** que le das a una receta.  
La receta (función) es la misma, pero el ingrediente (parámetro) cambia el resultado final. 🍪🎨

---

