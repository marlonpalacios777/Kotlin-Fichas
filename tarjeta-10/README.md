#### ESTRUCTURA NÚMERO 10  
# Programación Orientada a Objetos (POO)

---

## 1. Descripción: Por qué y para qué se utiliza

La Programación Orientada a Objetos (POO) es un paradigma de programación que organiza el código en objetos, los cuales agrupan tanto datos (atributos) como funciones (métodos) dentro de una estructura llamada clase.

### ¿Para qué sirve la POO?

La POO sirve para organizar y estructurar mejor el código, lo que facilita la reutilización, el mantenimiento y la escalabilidad de los programas. Se usa en aplicaciones de software grandes, videojuegos, sistemas de gestión, inteligencia artificial y más.

### ¿Por qué se utiliza la POO?

* La POO se utiliza porque permite desarrollar software de manera más organizada, reutilizable y escalable, facilitando el mantenimiento y la colaboración en proyectos grandes.
* **Simplifica la complejidad de los programas**: En lugar de manejar miles de líneas de código, organizas todo en objetos con responsabilidades específicas.
* **Permite reutilizar código y reducir esfuerzo**: Puedes crear una clase "base" y reutilizarla en varios lugares sin tener que escribir el mismo código otra vez.
* **Hace que los programas sean más seguros**: Gracias al encapsulamiento, los datos pueden protegerse y solo permitir acceso a ciertas partes del código.
* **Es el estándar en la mayoría de lenguajes modernos**: Lenguajes como Kotlin, Java, Python, C#, Swift y C++ están diseñados para trabajar con POO.

### ¿Para qué se utiliza la POO?

* **Para modelar el mundo real en software**: Representa objetos reales con atributos y comportamientos (Ej: un "Coche" tiene un "color" y puede "acelerar").
* **Para reutilizar código y reducir errores**: Gracias a la herencia, puedes crear clases basadas en otras, evitando escribir el mismo código varias veces.
* **Para facilitar el mantenimiento y escalabilidad**: Si necesitas modificar un programa, solo actualizas las clases, sin afectar otras partes del código.
* **Para estructurar mejor el código y hacerlo más legible**: Divide el programa en módulos independientes llamados objetos, facilitando la lectura y depuración.
* **Para trabajar en equipo de manera eficiente**: En proyectos grandes, cada desarrollador puede encargarse de diferentes clases sin afectar el trabajo de otros.

La POO se utiliza porque permite hacer código más organizado, reutilizable, mantenible y seguro. Se aplica en múltiples industrias y facilita el desarrollo de software a gran escala. Si queremos ser buenos programadores, la POO es un pilar fundamental que debes dominar.

---
   
2. **Genere un ejemplo internamente en el recuadro.**
   - Utilice un editor de código para lograrlo.

### Ejemplo sin POO (código desordenado y difícil de mantener):
     
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun main() {
    val empleadoNombre = "Marlon"
    val empleadoEdad = 21
    val empleadoSalario = 2500.0

    println("$empleadoNombre tiene $empleadoEdad años y gana $$empleadoSalario al mes.")
}
```
### Ejemplo Con POO (Código reutilizable y organizado):

```kotlin
// EJEMPLO EN CÓDIGO KOTLIN - Con POO (Código reutilizable y organizado)
fun main() {
    val empleado1 = Empleado("Marlon", 21, 2500.0)
    empleado1.mostrarInfo()
}

class Empleado(val nombre: String, val edad: Int, val salario: Double) {
    fun mostrarInfo() {
        println("$nombre tiene $edad años y gana $$salario al mes.")
    }
}
```

### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO]()**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB]()**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN


```
