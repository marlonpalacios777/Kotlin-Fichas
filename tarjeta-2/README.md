### ESTRUCTURA NÚMERO 2  
# OPERADORES MATEMÁTICOS Y LÓGICOS 

---  

## 1. Por qué y para qué se utilizan

- **Operadores matemáticos:**  
  Se utilizan para realizar cálculos y operaciones numéricas básicas, como sumas, restas, multiplicaciones y divisiones.  

- **Operadores lógicos:**  
  Se emplean para combinar o negar condiciones booleanas (verdadero o falso), permitiendo la creación de expresiones lógicas complejas.  

- En Kotlin, los operadores nos permiten realizar cálculos y tomar decisiones en el código.  

## Operadores Matemáticos  
Para hacer cálculos en Kotlin:  

- **Suma (+):**  
  Ejemplo: `val suma = 5 + 3 // resultado: 8`  

- **Resta (-):**  
  Ejemplo: `val resta = 10 - 4 // resultado: 6`  

- **Multiplicación (*):**  
  Ejemplo: `val multiplicacion = 6 * 7 // resultado: 42`  

- **División (/):**  
  Ejemplo: `val division = 15 / 3 // resultado: 5`  

- **Módulo (%):**  
  Obtiene el resto de una división.  
  Ejemplo: `val modulo = 17 % 5 // resultado: 2`  

- **Incremento (++) y Decremento (--):**  
  Incrementa o decrementa el valor de una variable en 1.  
  Pueden ser prefijos (++x, --x) o sufijos (x++, x--).  
  Ejemplo:
  var x = 5  
  x++ // x ahora es 6  
  --x // x ahora es 5
   
2. **Genere un ejemplo internamente en el recuadro.**  
   - Utilice un editor de código para lograrlo.
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN OPERADORES MATEMÁTICOS
fun main() {
   val numero1 = 10
   val numero2 = 5


   // Suma
   val suma = numero1 + numero2
   println("La suma es: $suma")


   // Resta
   val resta = numero1 - numero2
   println("La resta es: $resta")


   // Multiplicación
   val multiplicacion = numero1 * numero2
   println("La multiplicación es: $multiplicacion")


   // División
   val division = numero1.toDouble() / numero2
   println("La división es: $division")


   // Módulo (resto de la división)
   val modulo = numero1 % numero2
   println("El módulo es: $modulo")
}
```
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN OPERADORES LÓGICOS
fun main() {
   val a = true
   val b = false


   // Operador AND (&&)
   val resultadoAnd = a && b
   println("a AND b: $resultadoAnd") // Imprime: a AND b: false


   // Operador OR (||)
   val resultadoOr = a || b
   println("a OR b: $resultadoOr") // Imprime: a OR b: true


   // Operador NOT (!)
   val resultadoNotA = !a
   println("NOT a: $resultadoNotA") // Imprime: NOT a: false
   val resultadoNotB = !b
   println("NOT b: $resultadoNotB")// Imprime: NOT b: true


   //Ejemplo combinado.
   val resultadoCombinado = (a || b) && !b
   println("(a OR b) AND (NOT b): $resultadoCombinado")//Imprime (a OR b) AND (NOT b):        true
}
```
```kotlin
// EJEMPLO EN CÓDIGO OPERADORES DE COMPARACIÓN
fun main() {
    val numero1 = 10
    val numero2 = 5

    println("numero1 es igual a numero2: ${numero1 == numero2}")
    println("numero1 no es igual a numero2: ${numero1 != numero2}")
    println("numero1 es mayor que numero2: ${numero1 > numero2}")
    println("numero1 es menor que numero2: ${numero1 < numero2}")
    println("numero1 es mayor o igual que numero2: ${numero1 >= numero2}")
    println("numero1 es menor o igual que numero2: ${numero1 <= numero2}")
}
```

### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO  
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/4d05f9612f44bb9941e0b1f4aa5f8e09bbda508b/tarjeta-2/Audio%20-%20Tarjeta%20n%C3%BAmero%202..mp4)**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/45ef0d0fe0430910e298521d3b0811d04be69143/tarjeta-2/OPERADORES%20MATEM%C3%81TICOS%20Y%20L%C3%93GICOS.PNG)**

```kotlin
// EJERCICIO CREADO EN KOTLIN
fun main() {
    // Edwin y Salome están haciendo cálculos, para saber quién gana y Marlon sera la consola
    val numEdwin = 17 // Edwin dice: "Yo tengo 17 años"
    val numSalome = 10 // Salome responde: "Pues yo tengo 10 años"

    // Vamos a sumar y restar para ver quién tiene más.
    val total = numEdwin + numSalome // Edwin: "Si sumamos, tenemos..."
    val diferencia = numEdwin - numSalome // Salome: "Y si restamos, la diferencia es..."

    // ¿Quién tiene más? Veremos si Edwin le gana a Salome.
    val edwinMayor = numEdwin > numSalome // Edwin: "¿Soy mayor que Salome?"

    // ¡Mostramos los resultados para que no haya trampa!
    println("Total: $total, Diferencia: $diferencia") // "El total es... y la diferencia es..."
    println("¿Edwin mayor que Salome? $edwinMayor") // "Y... ¿Edwin es mayor? Ya lo sabremos por parte de Marlon.."
}
```
