#### ESTRUCTURA NÚMERO 8  
# PROGRAMACIÓN FUNCIONAL Y EXCEPCIONES LAMBDA

---

**1. Descripción: Por qué y para qué se utilizan los bucles**

La programación funcional es un paradigma de programación que se basa en el uso de funciones como bloques de construcción fundamentales. En lugar de modificar el estado de las variables, se crean nuevas variables y se transforman los datos utilizando funciones puras (funciones que siempre devuelven el mismo resultado para las mismas entradas y no tienen efectos secundarios).

### ¿Por qué se utilizan?

Código más legible y mantenible: Las funciones puras son más fáciles de entender y probar, ya que no dependen de estados externos.
Menos errores: La inmutabilidad de los datos y la ausencia de efectos secundarios reducen la probabilidad de errores.
Concurrencia: La inmutabilidad facilita la escritura de código concurrente, ya que no hay problemas de sincronización.
Expresividad: La programación funcional permite escribir código más conciso y expresivo.

### ¿Para qué se utilizan?

Transformación de datos: Aplicar funciones a colecciones de datos para transformarlos.
Filtrado de datos: Seleccionar elementos de una colección que cumplan con una condición.
Reducción de datos: Combinar los elementos de una colección en un solo valor.

---
   
2. **Genere un ejemplo internamente en el recuadro.**  

   - Utilice un editor de código para lograrlo.

**EJEMPLO MAP**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun main() {
    val numeros = listOf(1, 2, 3, 4, 5)
    val cuadrados = numeros.map { it * it } // Utilizamos map para aplicar una función (elevar al cuadrado) a cada elemento de la lista.
    println("Cuadrados: $cuadrados") // Salida: [1, 4, 9, 16, 25]
}
```
**EJEMPLO FILTER**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun main() {
    val nombres = listOf("Salomé", "Edwin", "Marlon", "Yusef", "SofiaPlus")
    val nombresConM = nombres.filter { it.startsWith('M') } // Utilizamos filter para seleccionar solo los nombres que comienzan con 'M'.
    println("Nombres con M: $nombresConM") // Salida: [Marlon]
}
```
**EJEMPLO REDUCE**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun main() {
    val numeros = listOf(1, 2, 3, 4, 5)
    val suma = numeros.reduce { acc, numero -> acc + numero } // Utilizamos reduce para sumar todos los números de la lista en un solo valor.
    println("Suma: $suma") // Salida: 15
}
```
**EJEMPLO DE FUNCION DE ORDEN SUPERIOR CON EXPRESION LAMBA**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun main() {
    val nombres = listOf("Salomé", "Edwin", "Marlon", "Yusef")
    val saludos = nombres.map { "Hola, $it!" } // Utilizamos map para crear una nueva lista de saludos personalizados.
    println(saludos) // Salida: [Hola, Salomé!, Hola, Edwin!, Hola, Marlon!, Yusef!]
}
```

### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/edbe25d21d315732a7994f59e1bb5d1e38142023/tarjeta-8/FUNCIONA%20LAMBDA.ogg)**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/6e402ca82e6cb2aed514b8decb2e228a4e3db3d8/tarjeta-8/PROGRAMACI%C3%93N%20FUNCIONAL%20Y%20EXCEPCIONES%20LAMBDA.PNG)**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN
fun main() {
    // ¡Empezamos creando una lista de jugadores y cada jugador tiene su nombre y el número de goles que metió.
    val jugadores = listOf(
        "Marlon" to 5, // Marlon metió 5 goles
        "Edwin" to 8,  // Edwin metió 8 goles
        "Salome" to 3, // Salome metió 3 goles
        "Yusef" to 10  // Yusef metió 10 goles
    )

    // 1. Queremos saber los nombres de todos los jugadores. Usamos 'map' para transformar la lista.
    // 'it.first' nos da el nombre de cada jugador. Es como decirle "dame el primer dato de cada jugador."
    val nombres = jugadores.map { it.first } 
    println("Nombres de los jugadores: $nombres") // Aquí los imprimimos

    // 2. Ahora, vamos a ver quiénes son los goleadores, los que metieron más de 5 goles.
    // 'filter' nos ayuda a seleccionar solo los jugadores que cumplen la condición 'it.second > 5'.
    // 'it.second' es el número de goles de cada jugador.
    val goleadores = jugadores.filter { it.second > 5 }
    println("Goleadores (más de 5 goles): $goleadores") // Mostramos a los goleadores

    // 3. Queremos saber el total de goles que metió todo el equipo.
    // 'fold' nos permite acumular los goles de todos los jugadores.
    // Empezamos con 0 goles ('0') y vamos sumando los goles de cada jugador ('acumulador + jugador.second').
    val totalGoles = jugadores.fold(0) { acumulador, jugador -> acumulador + jugador.second }
    println("Total de goles anotados: $totalGoles") // Imprimimos el total

    // ¡Y ahora, algo importante, vamos a manejar el caso de que no haya jugadores en la lista.
    // Usamos 'try-catch' para atrapar posibles errores.
    try {
        // Buscamos el máximo número de goles. 'maxByOrNull' nos da el jugador con más goles, o 'null' si no hay jugadores.
        // Si no hay jugadores, lanzamos un error con 'throw Exception'.
        val maxGoles = jugadores.maxByOrNull { it.second }?.second ?: throw Exception("No hay jugadores en la lista")
        println("Máximo número de goles: $maxGoles") // Mostramos el máximo número de goles
    } catch (e: Exception) {
        // Si hubo un error, lo atrapamos aquí y imprimimos el mensaje.
        println("Error: ${e.message}")
    }
}
```
