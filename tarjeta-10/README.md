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

### Clases y Objetos:
* **"Una clase es una plantilla o estructura que define un tipo de datos personalizado. En
Kotlin, una clase agrupa:
Propiedades: características o atributos del objeto.
Funciones (también llamadas métodos): comportamientos o acciones que
puede realizar el objeto.
Las clases son la base de la programación orientada a objetos (POO)..
     
```kotlin
// Definiendo una clase
class Persona {
    var nombre: String = "Sin nombre"
    var edad: Int = 0

    fun mostrarInformacion() {
        println("Nombre: $nombre, Edad: $edad años")
    }
}

```
```kotlin
// Creando un objeto de la clase Persona
fun main() {
    val persona1 = Persona() // Instanciando la clase
    persona1.nombre = "Juan"
    persona1.edad = 25
    persona1.mostrarInformacion() // Mostrará: Nombre: Juan, Edad: 25 años
}

```
### Constructor primario:
```kotlin
class Persona(val nombre: String, val edad: Int) {
    fun mostrarInformacion() {
        println("Nombre: $nombre, Edad: $edad años")
    }
}

fun main() {
    val persona1 = Persona("Ana", 25)
    persona1.mostrarInformacion() // Muestra: Nombre: Ana, Edad: 25 años
}

```
### Constructor Se:
```kotlin
class Persona(val nombre: String, val edad: Int) {
    fun mostrarInformacion() {
        println("Nombre: $nombre, Edad: $edad años")
    }
}

fun main() {
    val persona1 = Persona("Ana", 25)
    persona1.mostrarInformacion() // Muestra: Nombre: Ana, Edad: 25 años
}

```
### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/776d13c463722d49205333887d15b41524249562/tarjeta-10/Audio%20-%20Tarjeta%20n%C3%BAmero%2010.ogg)**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/2d566f077edac58599b08bf15da2f22b1b10b6d7/tarjeta-10/Programaci%C3%B3n%20Orientada%20a%20Objetos%20(POO).PNG)**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN
fun main() {
    // Aquí empezamos a crear objetos, imaginemos que estamos configurando los datos de los empleados.
    // Aqui nosotros creamos un Gerente llamado Marlon, con 25 años y un salario de 5000.0, que trabaja en el departamento de Tecnología.
    val marlon = Gerente("Marlon", 25, 5000.0, "Tecnología")

    // Ahora, creamos un Desarrollador llamado Edwin, con 22 años y un salario de 3500.0, que programa en Kotlin.
    val edwin = Desarrollador("Edwin", 22, 3500.0, "Kotlin")

    // Y finalmente, creamos otra Desarrolladora llamada Salomé, con 27 años y un salario de 3600.0, que programa en Python.
    val salome = Desarrollador("Salomé", 27, 3600.0, "Python")

    // ¡Ahora vamos a mostrar la información de cada empleado!
    // Primero, mostramos la información de Marlon, que es Gerente.
    marlon.mostrarInfo() // Esto muestra su nombre, edad y salario.
    marlon.gestionarEquipo() // Esto muestra que Marlon gestiona su equipo.

    // Luego, mostramos la información de Edwin, que es Desarrollador.
    edwin.mostrarInfo() // Esto muestra su nombre, edad y salario.
    edwin.programar() // Esto muestra que Edwin está programando en Kotlin.

    // Y finalmente, mostramos la información de Salomé, que también es Desarrolladora.
    salome.mostrarInfo() // Esto muestra su nombre, edad y salario.
    salome.programar() // Esto muestra que Salomé está programando en Python.
}

// Aquí definimos una clase base llamada "Empleado". imaginemos que esta clase tiene la información básica de cualquier empleado.
open class Empleado(val nombre: String, val edad: Int, var salario: Double) {

    // Este es un método (función dentro de una clase) para mostrar la información básica del empleado.
    // Usamos 'open' porque queremos que las subclases puedan modificar este método.
    open fun mostrarInfo() {
        println("Empleado: $nombre | Edad: $edad | Salario: $$salario")
    }
}

// Aquí definimos una subclase llamada "Gerente", que hereda de "Empleado".
// Esto significa que un Gerente es un tipo de Empleado, pero con información adicional.
class Gerente(nombre: String, edad: Int, salario: Double, val departamento: String)
    : Empleado(nombre, edad, salario) {

    // Este es un método exclusivo para Gerentes. Solo los Gerentes pueden gestionar un equipo.
    fun gestionarEquipo() {
        println("$nombre es el gerente del departamento de $departamento y gestiona su equipo.")
    }
}

// Aquí definimos otra subclase llamada "Desarrollador", que también hereda de "Empleado".
// Un Desarrollador es un tipo de Empleado, pero con información específica de su trabajo.
class Desarrollador(nombre: String, edad: Int, salario: Double, val lenguaje: String)
    : Empleado(nombre, edad, salario) {

    // Este es un método exclusivo para Desarrolladores. Solo ellos pueden programar.
    fun programar() {
        println("$nombre está programando en $lenguaje.")
    }
}
```
