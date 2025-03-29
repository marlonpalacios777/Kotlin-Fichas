#### ESTRUCTURA NÚMERO 5  
# COLLECTIONS Y ARRAYS

---

# COLLECTIONS 
---

1. **Describa el por qué y para qué se utiliza.**

  Las colecciones son estructuras de datos que permiten almacenar y manejar múltiples elementos:

- Listas (Lists):
  Las listas son colecciones ordenadas de elementos que Pueden contener elementos duplicados.
  List: Interfaz inmutable (no se pueden modificar los elementos después de la creación).
  MutableList: Interfaz mutable (se pueden agregar, eliminar o modificar elementos).

- Conjuntos (Sets):
  Colecciones de elementos únicos (no pueden contener duplicados).
  Set: Interfaz inmutable.
  MutableSet: Interfaz mutable.

- Mapas (Maps):
  Colecciones de pares clave:valor el cual la clave es inmutables y el valor es mutable 
  Map: Interfaz inmutable.
  MutableMap: Interfaz mutable.

# ARRAYS
---
- Son colecciones de tamaño fijo de elementos del mismo tipo accediendo a ellos mediante los índices.
  En Kotlin, los arrays se representan mediante la clase Array. También proporciona clases especializadas para arrays de tipos primitivos, como IntArray, DoubleArray.
  Se declaran con val para variables inmutables o var para variables mutables.

---
2. **Genere un ejemplo internamente en el recuadro.**  

   - Utilice un editor de código para lograrlo.
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN - LIST
fun main() {
   val frutas = listOf("banana", "pera", "kiwi", "mango", "piña")


   println("Usando get(): ${frutas.get(2)}")
   println("Usando elemnetAt(): ${(frutas.elementAt(3))}")


   println("Primer Elemento: ${(frutas.first())}")
   println("Ultimo Elemento: ${(frutas.last())}")
}
```
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN - SETS
fun main() {
   val mapInmutable: Map<String, Int> = mapOf(
       "manzana" to 1,
       "banana" to 2,
       "naranja" to 3
   )
   println("Map inmutable: $mapInmutable")
  
   val mapMutable: MutableMap<String, Int> = mutableMapOf(
       "manzana" to 1,
       "banana" to 2,
       "naranja" to 3
   )
   mapMutable["manzana"] = 4
   println("MutableMap después de modificar un valor: $mapMutable")
  
   mapMutable["uva"] = 5
   println("MutableMap después de añadir una nueva clave y valor: $mapMutable")
  
   mapMutable.remove("banana")
   println("MutableMap después de eliminar una clave: $mapMutable")
}
```
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN - MAPS
val mapa: Map<String, String> = mapOf("Edwin" to "Giraldo",
                                        "Angela" to "Agilar",
                                        "Emmanuel" to "Cano",
                                        "Emma" to "Lopez",
                                        "Salomon" to "Tovar")
   for ((name, lastName) in mapa){
       if(name.startsWith("E")){
           println(lastName)
       }
   }
}
```
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN - ARRAYS
val numeros: Array<Int> = arrayOf(60, 2, 3, 4, 5, 6, 7, 8, 9)
for (elem in numeros){
   println(elem)
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
    // Variables de ejemplo
    val puntuacion = 85
    val diaDeLaSemana = 3

    // Calificación basada en la puntuación
    val calificacion = when (puntuacion) {
        in 90..100 -> "A"
        in 80..89 -> "B"
        in 70..79 -> "C"
        in 60..69 -> "D"
        else -> "F"
    }
    println("Tu calificación es $calificacion")

    // Nombre del día de la semana
    val nombreDia = when (diaDeLaSemana) {
        1 -> "Lunes"
        2 -> "Martes"
        3 -> "Miércoles"
        4 -> "Jueves"
        5 -> "Viernes"
        6 -> "Sábado"
        7 -> "Domingo"
        else -> "Día inválido"
    }
    println("Hoy es $nombreDia")
}
```
