#### ESTRUCTURA NÚMERO 3
# FUNCIONES DE STRINGS Y PRINTING

---

1. **Describa el por qué y para qué se utiliza.**

## Funciones de Cadenas (Strings):

Permiten manipular y transformar texto, desde unir cadenas hasta extraer partes específicas o cambiar su formato.

### Concatenación:

Se utiliza el operador + para unir dos o más cadenas.

Ejemplo: val nombreCompleto = "Juan" + " " + "Pérez"

### Interpolación de Cadenas:

Permite insertar variables o expresiones dentro de una cadena usando $.

Ejemplo: val edad = 30; println("Mi edad es $edad")

### Longitud de una Cadena:

La propiedad length devuelve el número de caracteres en una cadena.

Ejemplo: val longitud = "Hola".length // resultado: 4

### Subcadenas:

La función substring() extrae una parte de una cadena.

Ejemplo: val subcadena = "Kotlin".substring(0, 3) // resultado: "Kot"

### Funciones de transformación:

* toUpperCase(): convierte todos los caracteres a mayúsculas.
* toLowerCase(): convierte todos los caracteres a minúsculas.
* trim(): elimina los espacios en blanco al principio y al final de la cadena.

### Funciones de comparación:

* equals(): Permite comparar si dos String son iguales.
* contains(): Permite verificar si un String contiene una secuencia de caracteres determinada.

## Funciones de Impresión (Printing):

**Propósito:** Muestran texto en la consola, lo que es útil para depurar código, mostrar resultados o interactuar con el usuario.

### print():

Imprime el texto sin agregar una nueva línea al final.

Ejemplo: print("Hola, ")

### println():

Imprime el texto y agrega una nueva línea al final.

Ejemplo: println("Mundo!")

---
   
2. **Genere un ejemplo internamente en el recuadro.**  
   - Utilice un editor de código para lograrlo.
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN
fun main() {  
    val nombre = "Salome"  

    // Imprimir el nombre en mayúsculas  
    println("Nombre en mayúsculas: ${nombre.uppercase()}")  

    // Imprimir el nombre en minúsculas  
    println("Nombre en minúsculas: ${nombre.lowercase()}")  

    // Contar cuántas letras tiene el nombre  
    println("El nombre tiene ${nombre.length} letras.")  

    // Verificar si el nombre contiene la letra 'a'  
    println("¿El nombre contiene la letra 'a'? ${nombre.contains("a")}")  
}  
```

### EN EL LISTADO COMPARTIDO BUSQUE EL ALGORITMO QUE CORRESPONDA Y EXPLÍQUELO PASO A PASO  
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO]()**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB]()**

```kotlin
// EJERCICIO CREADO EN KOTLIN
fun main() {
   val mensaje = "¡Hola, mundo!"


   // Imprime la cadena original
   println(mensaje)


   // Imprime la longitud de la cadena
   println("La longitud del mensaje es ${mensaje.length}")


   // Imprime la cadena en mayúsculas
   println("Mensaje en mayúsculas: ${mensaje.uppercase()}")


   // Imprime una subcadena
   println("Subcadena (primeros 5 caracteres): ${mensaje.substring(0, 5)}")
}
```
