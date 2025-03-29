#### ESTRUCTURA NÚMERO 5  
# ESTRUCTURAS DE DESICIÓN, CONTROL Y MANEJO DE ERRORES

---

## 1. Por qué y para qué se utilizan

Las estructuras de decisión y control son herramientas fundamentales en la programación que permiten que un programa tome decisiones y controle el flujo de ejecución. Esto significa que el programa puede elegir diferentes caminos o repetir acciones según ciertas condiciones.

### ¿Por qué se utilizan las variables?

Flexibilidad: Permiten que los programas se adapten a diferentes situaciones y entradas.
Lógica compleja: Facilitan la implementación de algoritmos y lógica compleja.
Eficiencia: Permiten evitar la repetición innecesaria de código.

### ¿Para qué se utilizan las variables?

Tomar decisiones: Ejecutar diferentes bloques de código según si se cumplen ciertas condiciones.
Repetir acciones: Ejecutar un bloque de código varias veces hasta que se cumpla una condición.
Controlar el flujo: Determinar el orden en que se ejecutan las instrucciones.

---

2. **Genere un ejemplo internamente en el recuadro.**  

   - Utilice un editor de código para lograrlo.

**Ejemplo - Condicionales (if-else):**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun verificarEdad(edad: Int) {
    if (edad >= 18) {
        println("Puede votar")
    } else {
        println("No puede votar")
    }
}
fun main() {
    verificarEdad(20) // Imprime "Puede votar"
    verificarEdad(15) // Imprime "No puede votar"
}
```
**Ejemplo - Condicionales (if-else):**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun verificarEdad(edad: Int) {
    if (edad >= 18) {
        println("Puede votar")
    } else {
        println("No puede votar")
    }
}
fun main() {
    verificarEdad(20) // Imprime "Puede votar"
    verificarEdad(15) // Imprime "No puede votar"
}
```
**Ejemplo - Bucles (for, while):**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun imprimirNumeros() {
    // Bucle for
    for (i in 1..10) {
        println(i)
    }

    // Bucle while con entrada simulada.
    val respuestas = listOf("no", "no", "si") // Simulamos la entrada del usuario.
    var i = 0;
    var respuesta = "";
    while (respuesta != "si") {
        println("¿Desea continuar? (si/no)")
        respuesta = respuestas[i];
        println(respuesta);
        i++;
    }
}

fun main() {
    imprimirNumeros()
}
```
**Sentencias when:**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun diaDeLaSemana(dia: Int) {
    when (dia) {
        1 -> println("Lunes")
        2 -> println("Martes")
        3 -> println("Miércoles")
        4 -> println("Jueves")
        5 -> println("Viernes")
        6 -> println("Sábado")
        7 -> println("Domingo")
        else -> println("Día inválido")
    }
}

fun main() {
    diaDeLaSemana(3) // Imprime "Miércoles"
    diaDeLaSemana(8) // Imprime "Día inválido"
}
```
**Ejemplo - Códigos de error:**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun encontrarElemento(lista: List<Int>, elemento: Int): Int {
    for (i in lista.indices) {
        if (lista[i] == elemento) {
            return i // Devuelve el índice si se encuentra el elemento
        }
    }
    return -1 // Devuelve -1 si el elemento no se encuentra
}

fun main() {
    val lista = listOf(1, 2, 3, 4, 5)
    val indice = encontrarElemento(lista, 3)
    if (indice != -1) {
        println("Elemento encontrado en el índice $indice")
    } else {
        println("Elemento no encontrado")
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
fun main() {
    // Definimos los días en que cada estudiante asistió a clase, usando números (1=Lunes, 2=Martes, etc.)
    val diasMarlon = 1 // Marlon asistió el Lunes
    val diasSalome = 3 // Salome asistió el Miércoles
    val diasEdwin = 5 // Edwin asistió el Viernes

    // Usamos 'when' para determinar el nombre del día para cada estudiante
    val diaMarlonNombre = when (diasMarlon) {
        1 -> "Lunes"
        2 -> "Martes"
        3 -> "Miércoles"
        4 -> "Jueves"
        5 -> "Viernes"
        6 -> "Sábado"
        7 -> "Domingo"
        else -> "Día inválido" // Manejamos el caso de un número de día incorrecto
    }
    val diaSalomeNombre = when (diasSalome) {
        1 -> "Lunes"
        2 -> "Martes"
        3 -> "Miércoles"
        4 -> "Jueves"
        5 -> "Viernes"
        6 -> "Sábado"
        7 -> "Domingo"
        else -> "Día inválido" // Manejamos el caso de un número de día incorrecto
    }
    val diaEdwinNombre = when (diasEdwin) {
        1 -> "Lunes"
        2 -> "Martes"
        3 -> "Miércoles"
        4 -> "Jueves"
        5 -> "Viernes"
        6 -> "Sábado"
        7 -> "Domingo"
        else -> "Día inválido" // Manejamos el caso de un número de día incorrecto
    }
    // Imprimimos los resultados
    println("Marlon asistió el $diaMarlonNombre.")
    println("Salome asistió el $diaSalomeNombre.")
    println("Edwin asistió el $diaEdwinNombre.")
}
```
