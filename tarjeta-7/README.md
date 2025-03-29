#### ESTRUCTURA NÚMERO 6
# BUCLES (LOOPS) EN KOTLIN

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

## 2. Ejemplos de bucles en Kotlin

### Bucle `for`

Se utiliza para iterar sobre una secuencia de valores (rangos, colecciones, arrays).

```kotlin
fun main() {
    val nombres = listOf("Ficha 2899621", "Profesor Yusef", "Salomé", "Edwin", "Marlon")
    for (nombre in nombres) {
        println("Hola, $nombre!") // Imprime un saludo para cada nombre en la lista.
    }
}
```
```kotlin
WHILE:
fun main() {
    var contador = 0
    while (contador < 5) {
        println("Contador: $contador") // Imprime el valor del contador en cada iteración.
        contador++ // Incrementa el contador en 1.
    }
}
```
```kotlin
DO-WHILE:
fun main() {
    var intentos = 0
    do {
        println("Intento número ${intentos + 1}") // Imprime el número de intento.
        intentos++ // Incrementa el número de intentos.
    } while (intentos < 3) // Continúa hasta que se realicen 3 intentos.
}
```
```kotlin
FOR:
fun main() {
    for (i in 1..5) {
        println("Número: $i") // Imprime los números del 1 al 5.
    }
}
```
```kotlin
FOREACH:
fun main() {
    val salidas = listOf("el centro comercial", "el parque", "el SENA")

    salidas.forEach { salida ->
        println("Me gusta $salida") // Imprime una frase para cada elemento de la lista.
    }
}
```

### EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO  
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO]()**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB]()**
