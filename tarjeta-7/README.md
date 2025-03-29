#### ESTRUCTURA NÚMERO 7
# Loopers, Bucles

---

## 1. Descripción: Por qué y para qué se utilizan los bucles

Los bucles, también conocidos como "loopers", son estructuras de control fundamentales en programación que permiten ejecutar un bloque de código de forma repetida hasta que se cumple una condición específica. Son esenciales para automatizar tareas repetitivas y procesar colecciones de datos de manera eficiente.

### ¿Por qué se utilizan?

* **Automatización**: Permiten ejecutar código repetitivo sin necesidad de escribirlo múltiples veces, lo que ahorra tiempo y reduce la posibilidad de errores.
* **Manejo de datos**: Facilitan el recorrido y procesamiento de listas, matrices, diccionarios y otras estructuras de datos, lo que es crucial para analizar y manipular información.
* **Generación de secuencias**: Permiten crear patrones numéricos, series y otras secuencias de forma automática, lo que es útil en diversas aplicaciones matemáticas y científicas.
* **Control de flujo**: Permiten repetir un bloque de código hasta que se alcanza un objetivo específico, lo que es esencial para implementar algoritmos y resolver problemas complejos.

### ¿Para qué se utilizan?

* **Iterar sobre listas de elementos**: Mostrar cada elemento de una lista de nombres, productos o cualquier otro tipo de datos.
* **Realizar cálculos repetitivos**: Calcular promedios, sumatorias, factoriales y otras operaciones matemáticas sobre conjuntos de datos.
* **Buscar elementos específicos**: Encontrar un elemento que cumpla con ciertas condiciones dentro de una lista o matriz.
* **Generar tablas y patrones**: Crear tablas de multiplicar, gráficos y otros tipos de representaciones visuales de datos.
* **Procesar archivos de datos**: Leer y analizar grandes cantidades de información almacenadas en archivos de texto o binarios.
* **Validación de entradas de usuario**: Solicitar al usuario que ingrese datos válidos y repetir la solicitud hasta que se cumpla una condición específica.
* **Implementación de algoritmos**: Ejecutar pasos repetitivos en algoritmos de búsqueda, ordenamiento y otros tipos de procesos computacionales.

## Ejemplos de bucles

### Bucle `FOR`

Se utiliza para iterar sobre una secuencia de valores (rangos, colecciones, arrays).

```kotlin
fun main() {
    val nombres = listOf("Ficha 2899621", "Profesor Yusef", "Salomé", "Edwin", "Marlon")
    for (nombre in nombres) {
        println("Hola, $nombre!") // Imprime un saludo para cada nombre en la lista.
    }
}
```
### Bucle `WHILE`
```kotlin
fun main() {
    var contador = 0
    while (contador < 5) {
        println("Contador: $contador") // Imprime el valor del contador en cada iteración.
        contador++ // Incrementa el contador en 1.
    }
}
```
### Bucle `DO-WHILE`
```kotlin
fun main() {
    var intentos = 0
    do {
        println("Intento número ${intentos + 1}") // Imprime el número de intento.
        intentos++ // Incrementa el número de intentos.
    } while (intentos < 3) // Continúa hasta que se realicen 3 intentos.
}
```
### Bucle `FOR`
```kotlin
fun main() {
    for (i in 1..5) {
        println("Número: $i") // Imprime los números del 1 al 5.
    }
}
```
### Bucle `FOREACH`
```kotlin
fun main() {
    val salidas = listOf("el centro comercial", "el parque", "el SENA")

    salidas.forEach { salida ->
        println("Me gusta $salida") // Imprime una frase para cada elemento de la lista.
    }
}
```
### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO]()**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/3d904ffd13dd2435450720eeb709c1d2f69239ae/tarjeta-7/BUCLES%20(LOOPS).PNG)**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN
fun main() {
    // Lista de aprendices del SENA
    val aprendices = listOf("Marlon", "Salomé", "Edwin", "Yusef")

    // Imprimir nombres con un bucle for-each
    aprendices.forEach { aprendiz ->
        println("Aprendiz: $aprendiz")
    }

    // Mapa de aprendices y sus edades
    val edadesAprendices = mapOf("Marlon" to 25, "Salomé" to 22, "Edwin" to 28, "Yusef" to 30)

    // Imprimir aprendices y edades con for-each y desestructuración
    edadesAprendices.forEach { (aprendiz, edad) ->
        println("$aprendiz tiene $edad años.")
    }

    // Contar hasta 5 con un bucle while
    var contador = 1
    while (contador <= 5) {
        println("Contador: $contador")
        contador++
    }

    // Simular una suma de números con un bucle do-while
    var suma = 0
    var numeros = listOf(2, 3, 4, 5) // Lista de números de ejemplo
    var indice = 0
    do {
        suma += numeros[indice]
        println("Suma actual: $suma")
        indice++
    } while (suma <= 10 && indice < numeros.size)

    println("La suma es $suma.")
}

```
