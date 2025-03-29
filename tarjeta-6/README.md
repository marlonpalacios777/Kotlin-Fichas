#### ESTRUCTURA NÚMERO 6
# Collections, json y manejo de datos

---

## 1. Descripción: Por qué y para qué se utilizan las colecciones

Las colecciones son estructuras de datos que permiten almacenar y organizar múltiples elementos de manera eficiente. Proporcionan métodos para agregar, eliminar, buscar y manipular datos.

### ¿Por qué se utilizan?

* **Organización**: Permiten estructurar los datos de manera lógica, facilitando su acceso y manipulación.
* **Eficiencia**: Ofrecen métodos optimizados para realizar operaciones comunes, mejorando el rendimiento del código.
* **Flexibilidad**: Pueden almacenar diferentes tipos de datos, adaptándose a diversas necesidades.

### ¿Para qué se utilizan?

* **Almacenar listas de elementos**: Permiten mantener conjuntos de datos ordenados o no ordenados.
* **Implementar estructuras de datos**: Facilitan la creación de pilas, colas y mapas, entre otros.
* **Realizar operaciones de búsqueda y filtrado**: Permiten encontrar y seleccionar datos específicos de manera eficiente.
* **Manejo de datos JSON**: Las colecciones son muy utiles para manejar datos que vienen de un archivo JSON, ya que estos datos se pueden organizar en listas, diccionarios, etc.
* **Transformacion de datos**: Se puede transformar la información que existe en las colecciones, para que se adapte a nuestras necesidades.

## 2. Tipos de colecciones comunes en Kotlin

* **Listas (Lists)**: Colecciones ordenadas de elementos, que pueden contener duplicados.
* **Conjuntos (Sets)**: Colecciones no ordenadas de elementos únicos.
* **Mapas (Maps)**: Colecciones de pares clave-valor, donde cada clave es única.

## 3. Manejo de JSON en Kotlin

JSON (JavaScript Object Notation) es un formato de intercambio de datos ligero y fácil de leer. Kotlin ofrece bibliotecas como `kotlinx.serialization` y `Gson` para trabajar con JSON.

### ¿Por qué se utiliza JSON?

* **Intercambio de datos**: Es un formato estándar para enviar y recibir datos entre aplicaciones.
* **Almacenamiento de datos**: Permite guardar datos estructurados en archivos de texto.
* **Comunicación con APIs**: Es ampliamente utilizado en APIs web para enviar y recibir respuestas.

### ¿Cómo se maneja JSON en Kotlin?

* **Serialización**: Convertir objetos Kotlin a formato JSON.
* **Deserialización**: Convertir datos JSON a objetos Kotlin.
* **Manipulación de datos JSON**: Buscar, modificar y eliminar datos dentro de un objeto JSON.

**Genere un ejemplo internamente en el recuadro.**

* **Ejemplo - Colecciones:**:
 ```kotlin
  fun main() {
    // Listas (Lists)
    val nombres = listOf("Marlon", "Edwin", "Salome")
    println("Nombres: $nombres") // Imprime la lista completa

    // Conjuntos (Sets)
    val numeros = setOf(1, 2, 3, 4, 5, 5) // El 5 se repite, pero solo se almacena una vez
    println("Números: $numeros") // Imprime el conjunto sin duplicados

    // Mapas (Maps)
    val edades = mapOf("Marlon" to 25, "Edwin" to 30, "Salome" to 28)
    println("Edad de Marlon: ${edades["Marlon"]}") // Imprime la edad de Marlon
}
```

* **Ejemplo - JSON**:
    ```kotlin
//Para poder trabajar con JSON en Kotlin Playground, necesitamos agregar una librería externa como kotlinx.serialization.
import kotlinx.serialization.*
import kotlinx.serialization.json.*

@Serializable
data class Jugador(val nombre: String, val goles: Int)

fun main() {
    val jugadoresJson = """
        [
            { "nombre": "Marlon", "goles": 10 },
            { "nombre": "Edwin", "goles": 8 }
        ]
    """

    val listaJugadores = Json.decodeFromString<List<Jugador>>(jugadoresJson)
    println("Jugadores: $listaJugadores")

    val jugador = Jugador("Salome", 5)
    val jugadorJson = Json.encodeToString(jugador)
    println("Jugador JSON: $jugadorJson")
}
```

* **Ejemplo - Manejo de Datos (ejemplo simple):**:
    ```kotlin
  fun main() {
    // Almacenar datos en una lista
    val datos = mutableListOf<Int>()
    datos.add(10)
    datos.add(20)
    datos.add(30)

    // Procesar datos
    val suma = datos.sum()
    val promedio = datos.average()

    // Imprimir resultados
    println("Suma: $suma")
    println("Promedio: $promedio")
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


