#### ESTRUCTURA NÚMERO 6
# BUCLES (LOOPS)

---

## 1. Descripción: Por qué y para qué se utilizan los bucles

Los bucles son estructuras de control esenciales en programación que permiten repetir un bloque de código múltiples veces. En Kotlin, se utilizan para automatizar tareas repetitivas, procesar colecciones de datos y controlar el flujo del programa.

### ¿Por qué se utilizan los bucles?

* **Automatización**: Ejecutar tareas repetitivas sin escribir el mismo código varias veces.
* **Procesamiento de datos**: Iterar sobre colecciones (listas, arrays, mapas) para analizar o modificar datos.
* **Control de flujo**: Repetir un bloque de código hasta que se cumpla una condición específica.

### ¿Para qué se utilizan los bucles?

* **Iterar sobre listas**: Procesar cada elemento de una lista de nombres, productos, etc.
* **Realizar cálculos repetitivos**: Sumar elementos de un array, calcular promedios, etc.
* **Generar secuencias**: Crear patrones numéricos, tablas de multiplicar, etc.
* **Validar entradas de usuario**: Solicitar datos hasta que se cumpla una condición.

**Genere un ejemplo internamente en el recuadro.**

## Tipos de bucles en Kotlin:

### Bucle `for`

Se utiliza para iterar sobre una secuencia de valores (rangos, colecciones, arrays).

* **Iterar sobre un rango**:

    ```kotlin
    for (i in 1..5) {
        println(i) // Imprime 1, 2, 3, 4, 5
    }
    ```

* **Iterar sobre una colección**:

    ```kotlin
    val frutas = listOf("manzana", "banana", "cereza")
    for (fruta in frutas) {
        println(fruta)
    }
    ```

* **Iterar sobre un array**:

    ```kotlin
    val numeros = intArrayOf(1, 2, 3)
    for (numero in numeros) {
        println(numero)
    }
    ```

* **Iterar con saltos**:

    ```kotlin
    for (i in 1..10 step 2) {
        println(i) // Imprime 1, 3, 5, 7, 9
    }
    ```

* **Iterar en orden descendente**:

    ```kotlin
    for (i in 5 downTo 1) {
        println(i) // Imprime 5, 4, 3, 2, 1
    }
    ```

### Bucle `while`

Ejecuta un bloque de código mientras una condición sea verdadera.

```kotlin
var contador = 0
while (contador < 5) {
    println("Contador: $contador")
    contador++
}
 ``` 
### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO]()**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB]()**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN
fun main() {
    // Lista de aprendices del SENA
    val aprendices = listOf("Marlon", "Salomé", "Edwin")

    // Imprimir nombres usando un bucle for
    for (aprendiz in aprendices) {
        println("Aprendiz: $aprendiz")
    }

    // Mapa de aprendices y sus roles
    val rolesAprendices = mapOf("Marlon" to "Desarrollador", "Salomé" to "Diseñadora", "Edwin" to "Analista")

    // Imprimir roles usando un bucle for
    for ((aprendiz, rol) in rolesAprendices) {
        println("$aprendiz es $rol")
    }

    // Contar hasta 3 con un bucle while
    var contador = 1
    while (contador <= 3) {
        println("Contador: $contador")
        contador++
    }

    // Validar nombre del profesor Yusef con do-while
    var nombre: String
    var intentos = 0
    do {
        print("Ingresa el nombre del profesor: ")
        nombre = readLine() ?: ""
        intentos++
        if (intentos >= 5) {
            println("Demasiados intentos. Saliendo.")
            return // Salir de la función main
        }
    } while (nombre.lowercase() != "yusef")

    println("¡Bienvenido, profesor $nombre!")
}
```


