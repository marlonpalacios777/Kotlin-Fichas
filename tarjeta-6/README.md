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

* **Ejemplo - Manejo de Datos (ejemplo simple):**
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
**Primer ejemplo - Formato JSON (Ejemplo práctico en la exposición):**

```json
{
  "descripcion": "Usos comunes del manejo de archivos en Kotlin",
  "usos": [
    {
      "nombre": "Almacenamiento de Configuración",
      "ejemplo": "Guardar preferencias del usuario en archivos .ini o JSON."
    },
    {
      "nombre": "Persistencia de Datos Simples",
      "ejemplo": "Almacenar tareas de una lista en un archivo de texto o JSON."
    },
    {
      "nombre": "Registro (Logging)",
      "ejemplo": "Escribir información de la aplicación y errores en archivos .log."
    },
    {
      "nombre": "Lectura de Datos Externos",
      "ejemplo": "Importar datos desde archivos CSV o leer instrucciones desde archivos de texto."
    },
    {
      "nombre": "Generación de Informes",
      "ejemplo": "Crear y guardar informes en formato texto, CSV, HTML o PDF."
    },
    {
      "nombre": "Procesamiento de Datos",
      "ejemplo": "Leer grandes conjuntos de datos desde archivos, transformarlos y guardar los resultados."
    },
    {
      "nombre": "Almacenamiento de Recursos",
      "ejemplo": "Leer plantillas de texto o pequeños archivos de datos desde el sistema de archivos."
    },
    {
      "nombre": "Operaciones de Entrada/Salida (I/O)",
      "ejemplo": "Leer o escribir información en archivos como parte del flujo de un programa."
    }
  ]
}
```

**EJEMPLO EN LA EXPOSICIÓN - KOTLIN:**
```kotlin
import kotlinx.serialization.*
import kotlinx.serialization.json.*

@Serializable
data class Producto(
    @SerialName("uuid") val uid: String,
    val name: String,
    val price: String // Se mantiene como String para que coincida con el JSON
)

fun main() {
    val jsonString = \"\"\" 
        [
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440000",
                "name": "producto aleatorio 1",
                "price": "10.99"
            },
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440001",
                "name": "producto aleatorio 2",
                "price": "20.50"
            },
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440002",
                "name": "producto aleatorio 3",
                "price": "15.75"
            },
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440003",
                "name": "producto aleatorio 4",
                "price": "8.99"
            },
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440004",
                "name": "producto aleatorio 5",
                "price": "12.30"
            },
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440005",
                "name": "producto aleatorio 6",
                "price": "5.99"
            },
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440006",
                "name": "producto aleatorio 7",
                "price": "18.20"
            },
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440007",
                "name": "producto aleatorio 8",
                "price": "22.45"
            },
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440008",
                "name": "producto aleatorio 9",
                "price": "30.99"
            },
            {
                "uuid": "550e8400-e29b-41d4-a716-446655440009",
                "name": "producto aleatorio 10",
                "price": "40.10"
            }
        ]
    \"\"\".trimIndent()

    val productos: List<Producto> = Json.decodeFromString(jsonString)

    productos.forEach {
        println("${'$'}{it.name} cuesta ${'$'}${'$'}{it.price}")
    }
}
```
    
### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO](https://marlonpalacios777.github.io/Kotlin-Fichas/tarjeta-6/Audio%20-%20Tarjeta%20n%C3%BAmero%206..mp4)**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/b2da4e8186f991cc449921345799388a5c69979e/tarjeta-6/Collections%2C%20json%20y%20manejo%20de%20datos.PNG)**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN
fun main() {
    // Imaginemos que tenemos una lista de aprendices del SENA.
    val aprendicesSENA = listOf("Salomé", "Edwin", "Marlon")

    // Y un mapa con sus fichas.
    val fichasAprendices = mapOf(
        "Salomé" to "2899621",
        "Edwin" to "2899622",
        "Marlon" to "2899623"
    )

    // Vamos a mostrar la información de cada aprendiz.
    aprendicesSENA.forEach { aprendiz ->
        // Obtenemos la ficha del aprendiz desde el mapa.
        val ficha = fichasAprendices[aprendiz]

        // Y la imprimimos.
        println("$aprendiz tiene la ficha $ficha")
    }
}
```
