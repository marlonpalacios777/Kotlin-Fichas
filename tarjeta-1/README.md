#### ESTRUCTURA NÚMERO 1
# VARIABLES Y TIPOS DE DATOS

---

## 1. Por qué y para qué se utilizan

En Kotlin, una variable actúa como un contenedor para almacenar un valor. Este valor puede ser modificable (variable mutable) o inmutable (constante) durante la ejecución del programa. Las variables son fundamentales para la manipulación y almacenamiento de datos.

### ¿Por qué se utilizan las variables?

* **Almacenamiento de datos:** Permiten guardar información temporal o permanente durante la ejecución del programa.
* **Manipulación de datos:** Facilitan la realización de operaciones como cálculos, comparaciones y transformaciones.
* **Control del flujo del programa:** Se utilizan en estructuras de control (condicionales, bucles) para tomar decisiones.
* **Reutilización de datos:** Permiten usar la misma información en múltiples partes del programa.

### ¿Para qué se utilizan las variables?

* **Información del usuario:** Almacenar datos proporcionados por el usuario (nombre, edad, etc.).
* **Cálculos matemáticos:** Guardar números y realizar operaciones aritméticas.
* **Estado del programa:** Utilizar valores booleanos para controlar el flujo lógico.
* **Colecciones de datos:** Almacenar listas, conjuntos o mapas de datos.

## 2. Tipos de datos en Kotlin:

Kotlin es un lenguaje de tipado estático, donde el tipo de una variable se define en tiempo de compilación. Ofrece una variedad de tipos de datos:

### Tipos de datos numéricos:

* `Int`: Números enteros (ej: 10, -5, 0).
* `Long`: Números enteros de mayor rango (ej: 10000000000L).
* `Double`: Números de punto flotante de doble precisión (ej: 3.14, 2.71828).
* `Float`: Números de punto flotante de precisión simple (ej: 3.14f, 2.71828f).

### Tipo de dato booleano:

* `Boolean`: Valores lógicos (verdadero/falso: `true`, `false`).

### Tipo de dato carácter:

* `Char`: Caracteres individuales (ej: 'a', 'b', 'c').

### Tipo de dato cadena:

* `String`: Secuencias de caracteres (ej: "Hola, mundo!", "Somos un equipo muy unido", "Conformado por Salome,Marlon y Edwin").

---
   
2. **Genere un ejemplo internamente en el recuadro.**  

   - Utilice un editor de código para lograrlo.
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN


```

### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO]()**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/f8aa10d9293a7a1c464674d5f2bda1a400a98b3b/tarjeta-1/Variables%20Tipos%20de%20Datos.PNG)**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN
fun main() {
    // Aquí definimos el nombre del cliente. "val" significa que este nombre no va a cambiar.
    val nombreCliente: String = "Edwin"

    // Ahora, el estilo del corte, que sí puede variar, por eso usamos "var".
    var estiloCorte: String = "Fade"

    // Y el precio del corte, que también podría cambiar, así que "var" otra vez.
    var precioCorte: Double = 20.50

    // Por último, si el cliente es frecuente o no, que tampoco cambia, usamos "val".
    val esClienteFrecuente: Boolean = true

    // Aquí hacemos como si el cliente se hubiera cambiado de opinión.
    estiloCorte = "Corte clasico"

    // Ahora, vamos a imprimir toda la info del cliente.
    println("Cliente: $nombreCliente") // Aquí mostramos el nombre.
    println("Corte elegido: $estiloCorte") // Y aquí, el estilo del corte.
    println("Precio: $$precioCorte") // ¡Y el precio!
    println("¿Cliente frecuente?: $esClienteFrecuente") // Y si es cliente frecuente o no.
}

```
