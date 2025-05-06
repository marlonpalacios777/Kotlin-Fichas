#### ESTRUCTURA NÚMERO 9 
# Pruebas, test y depuración 

---

## 1. Descripción: Pruebas y Depuración

### Pruebas (Tests):

Las pruebas son un proceso fundamental en el desarrollo de software que consiste en verificar que el código funcione correctamente y cumpla con los requisitos especificados. Se escriben casos de prueba para diferentes escenarios y se ejecutan para detectar posibles errores o fallos en el código.

#### ¿Por qué se utilizan?

* **Asegurar la calidad del código**: Las pruebas ayudan a garantizar que el código funcione correctamente y sea confiable.
* **Detectar errores tempranamente**: Las pruebas permiten identificar errores en las primeras etapas del desarrollo, lo que facilita su corrección.
* **Facilitar la refactorización**: Las pruebas proporcionan una red de seguridad al modificar el código, asegurando que no se introduzcan nuevos errores.
* **Documentar el comportamiento del código**: Las pruebas pueden servir como documentación del comportamiento esperado del código.

#### ¿Para qué se utilizan?

* **Pruebas unitarias**: Verificar el funcionamiento de unidades individuales de código, como funciones o clases.
* **Pruebas de integración**: Verificar la interacción entre diferentes módulos o componentes del sistema.
* **Pruebas de aceptación**: Verificar que el sistema cumpla con los requisitos del usuario o cliente.
* **Pruebas de regresión**: Verificar que las modificaciones recientes no hayan introducido nuevos errores en el código existente.

### Depuración (Debugging):

La depuración es el proceso de identificar y corregir errores en el código. Se utilizan herramientas y técnicas para analizar el comportamiento del programa, localizar la causa de los errores y corregirlos.

#### ¿Por qué se utilizan?

* **Encontrar y corregir errores**: La depuración es esencial para encontrar y corregir errores en el código.
* **Entender el comportamiento del programa**: La depuración ayuda a comprender cómo se ejecuta el programa y cómo interactúan sus diferentes partes.
* **Mejorar el rendimiento**: La depuración puede ayudar a identificar cuellos de botella y optimizar el rendimiento del programa.

#### ¿Para qué se utilizan?

* **Puntos de interrupción (Breakpoints)**: Pausar la ejecución del programa en puntos específicos para inspeccionar el estado de las variables.
* **Paso a paso (Step-by-step)**: Ejecutar el programa línea por línea para seguir el flujo de ejecución.
* **Inspección de variables (Variable inspection)**: Examinar los valores de las variables en diferentes puntos del programa.
* **Registro de mensajes (Logging)**: Imprimir mensajes en la consola para rastrear el flujo de ejecución y el estado de las variables.

---

2. **Genere un ejemplo internamente en el recuadro.**  

   - Utilice un editor de código para lograrlo.

**EJEMPLO PRUEBA FUNCIÓN SIMPLE**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun sumar(a: Int, b: Int): Int {
    return a + b // Esta función simplemente suma dos números enteros.
}

fun main() {
    val resultado = sumar(6, 3) // Llamamos a la función sumar con los valores 5 y 3.
    if (resultado == 8) { // Verificamos si el resultado es igual a 8.
        println("Prueba de suma: ¡Pasó!") // Si el resultado es 8, la prueba pasa.
    } else {
        println("Prueba de suma: ¡Falló! Se esperaba 8, pero se obtuvo $resultado") // Si el resultado no es 8, la prueba falla.
    }
}
```
**EJEMPLO PRINTLN**
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun main() {
    var suma = 0 // Inicializamos la variable suma en 0.
    for (i in 1..5) { // Iteramos sobre los números del 1 al 5.
        suma += i // Sumamos el valor de i a la variable suma.
        println("i = $i, suma = $suma") // Imprimimos el valor de i y suma en cada iteración para ver cómo cambian.
    }
    println("Suma total: $suma") // Imprimimos la suma total después de completar el bucle.
}
```

### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO](https://marlonpalacios777.github.io/Kotlin-Fichas/tarjeta-9/Audio%20-%20Tarjeta%20n%C3%BAmero%209..mp4)**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB](https://github.com/marlonpalacios777/Kotlin-Fichas/blob/93d11db4531678d7618ab8f5f08a4b9b65a7f1b5/tarjeta-9/Pruebas%2C%20test%20y%20depuraci%C3%B3n.PNG)**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN
fun main() {
    fun dividir(a: Int, b: Int): Int {
        // Posible error: división por cero
        return a / b
    }

    // Pruebas
    println("Prueba: dividir 10 / 2 = ${dividir(10, 2)}")
    //println("Prueba error: dividir 10 / 0 = ${dividir(10, 0)}") // Esto causa un error

    // Depuración:
    // Puedes usar un punto de interrupción en la función "dividir"
    // para revisar los valores de "a" y "b".
}
```
