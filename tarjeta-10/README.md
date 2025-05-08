## Programación Orientada a Objetos (POO)

---

### 1. Descripción: Fundamentos y Propósito

La Programación Orientada a Objetos (POO) es un **paradigma de programación** fundamental que se centra en la creación de **objetos**. Estos objetos encapsulan **atributos** (datos) y **comportamientos** (funciones o métodos), modelando entidades del mundo real dentro del software.

#### ¿Para qué sirve la POO?

La POO ofrece una estructura robusta para el desarrollo de software, mejorando significativamente:

* **Organización del código:** Facilita la comprensión y el manejo de proyectos complejos.
* **Reutilización:** Permite crear componentes de software que pueden ser utilizados en diferentes partes de la aplicación o en otros proyectos.
* **Mantenimiento:** Simplifica la identificación y corrección de errores, así como la adaptación a nuevos requerimientos.
* **Escalabilidad:** Facilita el crecimiento y la expansión de las aplicaciones de manera modular.

La POO es ampliamente utilizada en diversas áreas como aplicaciones de software de gran escala, videojuegos, sistemas de gestión e inteligencia artificial.

#### ¿Por qué se utiliza la POO?

La adopción de la POO se debe a sus numerosas ventajas:

* **Simplificación de la complejidad:** Divide problemas complejos en unidades más pequeñas y manejables (objetos).
* **Reutilización y eficiencia:** La herencia y la composición permiten reutilizar código existente, reduciendo el tiempo y el esfuerzo de desarrollo.
* **Seguridad:** El encapsulamiento protege los datos internos de los objetos, controlando su acceso y evitando modificaciones no deseadas.
* **Estándar en lenguajes modernos:** La mayoría de los lenguajes de programación populares (Kotlin, Java, Python, C#, Swift, C++) están diseñados para soportar la POO.
* **Modelado del mundo real:** Permite representar entidades y sus interacciones de forma intuitiva en el código (ej: un objeto `Coche` con atributos como `color` y comportamientos como `acelerar`).
* **Facilita el mantenimiento y la escalabilidad:** Los cambios en una parte del sistema (un objeto o una clase) tienen un impacto limitado en otras partes.
* **Mejora la legibilidad y la depuración:** La estructura modular del código facilita su comprensión y la localización de errores.
* **Trabajo en equipo eficiente:** Permite a diferentes desarrolladores trabajar en módulos independientes (clases) sin interferir entre sí.

En resumen, la POO es un pilar fundamental para desarrollar software organizado, reutilizable, mantenible y seguro, siendo esencial para cualquier programador.

---

### 2. Conceptos Clave de la POO en Kotlin

#### Clases y Objetos

* **Clase:** Una **plantilla** o **estructura** que define un **tipo de dato personalizado**. En Kotlin, agrupa:
    * **Propiedades:** Características o atributos del objeto.
    * **Funciones (métodos):** Comportamientos o acciones del objeto.
* **Características de las clases:**
    * Definen tipos de datos personalizados.
    * Pueden tener **constructores** (primario y/o secundarios).
    * Soportan **herencia**.
    * Permiten **control de visibilidad** (`private`, `public`, `protected`, `internal`).
    * Permiten **encapsular** datos y comportamientos.
* **Objeto:** Una **instancia concreta** de una clase. Cada objeto tiene su propio conjunto de datos y puede acceder a las funciones de su clase.

#### Constructores

* Un **constructor** es una función especial utilizada para **crear objetos** e **inicializar sus propiedades**.
* En Kotlin existen:
    * **Constructor primario:** Definido en la cabecera de la clase.
    * **Constructor secundario:** Declarado dentro del cuerpo de la clase usando la palabra clave `constructor`.

#### Encapsulación

* La **encapsulación** es el principio de **ocultar los detalles internos** de una clase y **proteger sus datos**, permitiendo el acceso solo a través de **métodos controlados**.
* **Modificadores de acceso en Kotlin:**
    * `public`: Accesible desde cualquier parte del programa.
    * `private`: Accesible solo dentro de la clase.
    * `protected`: Accesible dentro de la clase y sus subclases.
    * `internal`: Accesible solo dentro del mismo módulo.
* **Getters y Setters:** Métodos utilizados para **leer (`get`)** o **modificar (`set`)** propiedades privadas, permitiendo la implementación de lógica de validación.

#### Herencia

* La **herencia** permite que una clase (**subclase** o clase derivada) herede **propiedades** y **comportamientos** de otra clase (**superclase** o clase base).
* **Términos clave:**
    * `open`: Modificador que permite que una clase sea susceptible de ser heredada.
    * `override`: Palabra clave utilizada para **sobrescribir** un comportamiento heredado en la subclase.
    * `super`: Palabra clave utilizada para **acceder a miembros** (propiedades o métodos) de la clase padre desde la subclase.

#### Clases Abstractas

* Una **clase abstracta** define una **estructura común** para sus subclases, especificando qué métodos deben implementar, pero sin proporcionar una implementación completa para todos ellos.
* **No se puede instanciar directamente**.
* Puede contener:
    * **Métodos abstractos:** Declarados sin cuerpo (la implementación debe proporcionarse en las subclases concretas).
    * **Métodos normales:** Declarados con un cuerpo (implementación).

#### Polimorfismo

* El **polimorfismo** (que significa "muchas formas") permite utilizar la **misma función** o método para realizar **diferentes comportamientos** dependiendo del **objeto** que se esté utilizando.

#### Interfaces

* Una **interfaz** define un **contrato**: si una clase implementa una interfaz, **debe proporcionar una implementación** para todos los métodos declarados en esa interfaz.
* **Características:**
    * Se declara utilizando la palabra clave `interface`.
    * Puede contener **funciones abstractas** (sin cuerpo), **funciones con cuerpo** (con una implementación por defecto) y **propiedades abstractas** (sin inicialización).
    * Una clase puede **implementar múltiples interfaces**.

---
   
2. **Genere un ejemplo internamente en el recuadro.**
   - Utilice un editor de código para lograrlo.
## Ejemplos de Código Kotlin para POO

### Clases y Objetos

```kotlin
// Definiendo una clase
class Persona {
    var nombre: String = "Sin nombre"
    var edad: Int = 0

    fun mostrarInformacion() {
        println("Nombre: $nombre, Edad: $edad años")
    }
}

// Creando un objeto de la clase Persona
fun main() {
    val persona1 = Persona() // Instanciando la clase
    persona1.nombre = "Juan"
    persona1.edad = 25
    persona1.mostrarInformacion() // Mostrará: Nombre: Juan, Edad: 25 años
}
```

### Constructor Primario

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

### Constructor Secundario

```kotlin
class Persona {
    var nombre: String
    var edad: Int

    // Constructor Secundario
    constructor(nombre: String, edad: Int) {
        this.nombre = nombre
        this.edad = if (edad > 0) edad else 1 // Evitamos edades negativas
        println("Objeto Persona creado con nombre $nombre y edad $edad")
    }

    fun mostrarInformacion() {
        println("Nombre: $nombre, Edad: $edad años")
    }
}

fun main() {
    val persona1 = Persona("Juan", -5) // Edad negativa, se corrige a 1
    persona1.mostrarInformacion() // Muestra: Nombre: Juan, Edad: 1 años
}
```

### Encapsulación

```kotlin
class Empleado(private val nombre: String, private var salario: Double) {

    fun obtenerNombre(): String {
        return nombre
    }

    fun obtenerSalario(): Double {
        return salario
    }

    fun actualizarSalario(nuevoSalario: Double) {
        if (nuevoSalario > 0) {
            salario = nuevoSalario
        } else {
            println("❌ Error: El salario no puede ser negativo")
        }
    }

    fun mostrarInformacion() {
        println("Nombre: $nombre, Salario: $salario")
    }
}

fun main() {
    val empleado1 = Empleado("Juan", 2000.0)
    empleado1.mostrarInformacion()

    empleado1.actualizarSalario(2500.0)
    empleado1.mostrarInformacion()

    empleado1.actualizarSalario(-500.0)
    empleado1.mostrarInformacion()
}
```

### Herencia

```kotlin
// Superclase
open class Persona(val nombre: String, val edad: Int) {
    fun presentarse() {
        println("Hola, me llamo $nombre y tengo $edad años.")
    }
}

// Subclase que hereda de Persona
class Estudiante(nombre: String, edad: Int, val carrera: String) : Persona(nombre, edad) {
    fun estudiar() {
        println("$nombre está estudiando $carrera.")
    }
}

fun main() {
    val estudiante1 = Estudiante("Laura", 20, "Ingeniería")
    estudiante1.presentarse()
    estudiante1.estudiar()
}
```

```kotlin
open class Animal {
    open fun sonido() {
        println("Este animal hace un sonido")
    }
}

class Perro : Animal() {
    override fun sonido() {
        println("El perro dice: ¡Guau!")
    }
}

fun main() {
    val miPerro = Perro()
    miPerro.sonido()
}
```

### Clase Abstracta

```kotlin
abstract class Animal(val nombre: String) {
    abstract fun hacerSonido()

    fun presentarse() {
        println("Hola, soy $nombre")
    }
}

class Perro(nombre: String) : Animal(nombre) {
    override fun hacerSonido() {
        println("🐶 $nombre dice: ¡Guau guau!")
    }
}

class Gato(nombre: String) : Animal(nombre) {
    override fun hacerSonido() {
        println("🐱 $nombre dice: ¡Miau!")
    }
}

fun main() {
    val perro = Perro("Toby")
    val gato = Gato("Michi")

    perro.presentarse()
    perro.hacerSonido()

    gato.presentarse()
    gato.hacerSonido()
}
```

### Polimorfismo

```kotlin
abstract class Empleado(val nombre: String) {
    abstract fun trabajar()
}

class Programador(nombre: String): Empleado(nombre) {
    override fun trabajar() {
        println("👨‍💻 $nombre está programando en Kotlin.")
    }
}

class Diseñador(nombre: String): Empleado(nombre) {
    override fun trabajar() {
        println("🎨 $nombre está diseñando interfaces.")
    }
}

fun main() {
    val empleados: List<Empleado> = listOf(
        Programador("Ana"),
        Diseñador("Carlos"),
        Programador("Luis")
    )

    for (empleado in empleados) {
        empleado.trabajar()
    }
}
```

### Interfaz

```kotlin
interface Trabajador {
    fun trabajar()
}

interface Descansar {
    fun descansar()
}

class Diseñador(val nombre: String) : Trabajador, Descansar {
    override fun trabajar() {
        println("🎨 $nombre está diseñando.")
    }

    override fun descansar() {
        println("😴 $nombre está tomando una siesta creativa.")
    }
}

fun main() {
    val diseñador1 = Diseñador("Luisa")
    diseñador1.trabajar()
    diseñador1.descansar()
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
