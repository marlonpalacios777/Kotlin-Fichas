#### ESTRUCTURA NÚMERO 4 
# CONTROL DE FLUJO  

---

1. **Describa el por qué y para qué se utiliza.**

  Los condicionales en programación son estructuras de control que permiten ejecutar diferentes bloques de código según si una condición es verdadera o falsa. Pueden ser simples (if), compuestos (if-else), múltiples (if-elseif-else o switch-case)
Son esenciales para la toma de decisiones y el control del flujo de un programa:


-If:
  Se utiliza para ejecutar un bloque de código si una condición especifica es verdadera.

-Else:
  Utilizado en conjunto con if.

-Else if:
  Se utiliza para verificar múltiples condiciones en secuencia permitiendo manejar múltiples casos sin anidar múltiples   sentencias if.

-When:
  La expresión when es una estructura de control de flujo que permite ejecutar diferentes bloques de código basados en el valor de una variable o expresión.

---
   
2. **Genere un ejemplo internamente en el recuadro.**  
  - Utilice un editor de código para lograrlo.
```kotlin
// EJEMPLO #1 EN CÓDIGO KOTLIN - IF
fun main() {
    val edad = 20
    if(edad>=18){
        println("Eres mayor de edad")
    }
}
```
// EJEMPLO #2 EN CÓDIGO KOTLIN - ELSE
fun main(){
   val edad = 16
   if (edad >= 18){
       println("Eres mayor de edad")
   } else {
       println("Eres menor de edad")
   }
}
```
// EJEMPLO #3 EN CÓDIGO KOTLIN - ELSE IF
fun main(){
   val puntuacion = 90
   if (puntuacion >= 90) {
       println("Excelente")
   } else if (puntuacion >= 80){
       println("Muy bien")
   } else if (puntuacion >= 70) {
       println("Bien")
       } else {
           println("A mejorar")
   }
}
```
// EJEMPLO #4 EN CÓDIGO KOTLIN - WHEN
fun main() {
    val numero = 3

    when (numero) {
        1 -> println("El número es uno.")
        2 -> println("El número es dos.")
        3 -> println("El número es tres.")
        in 4..10 -> println("El número está entre 4 y 10.")
        else -> println("El número no está en la lista.")
    }
}
```

### EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO  
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO]()**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB]()**

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**

// EJERCICIO CREADO EN KOTLIN
fun main() {
    // Ejemplo de if, else if y else:

    // Declaramos una variable llamada 'puntuacion' con el valor 85.
    // Esta variable la usaremos para evaluar el rendimiento de alguien.
    val puntuacion = 85

    // Declaramos 'diaDeLaSemana' con el valor 3. Esto representa un día de la semana (1=Lunes, 2=Martes, etc.)
    val diaDeLaSemana = 3

    // Aquí vamos a evaluar la 'puntuacion' para dar una calificación basada en rangos.
    if (puntuacion >= 90) {
        // Si la puntuación es 90 o más, vamos a imprimir "Excelente".
        println("Excelente")
    } else if (puntuacion >= 80) {
        // Si no es 90 o más, pero es 80 o más, vamos a imprimir "Muy bien".
        println("Muy bien")
    } else if (puntuacion >= 70) {
        // Si no es 80 o más, pero es 70 o más, vamos a imprimir "Bien".
        println("Bien")
    } else {
        // Si no cumple ninguna de las condiciones anteriores, vamos a imprimir "A mejorar".
        println("A mejorar")
    }

    // Ejemplo de when:
    // Ahora vamos a usar 'when' para obtener el nombre del día de la semana basado en 'diaDeLaSemana'.
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
    // Ahora vamos a imprimir el mensaje "Hoy es" seguido del nombre del día obtenido con 'when'.
    println("Hoy es $nombreDia")

    // Ejemplo de when con rangos
    // Aquí usamos 'when' nuevamente, pero esta vez con rangos para asignar una calificación de letra a la 'puntuacion'.
    val calificacion = when (puntuacion) {
        in 90..100 -> "A"
        in 80..89 -> "B"
        in 70..79 -> "C"
        in 60..69 -> "D"
        else -> "F"
    }
    // Aqui vamos a imprimir el mensaje "Tu calificación es" seguido de la calificación de letra obtenida.
    println("Tu calificación es $calificacion")
}
```
