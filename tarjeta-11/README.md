#### ESTRUCTURA NÚMERO 11
# Manejo de archivos

## ¿Qué es el Manejo de archivos?

Es la capacidad de interactuar con archivos y directorios del sistema para leer, escribir, modificar o almacenar datos de forma persistente.

## ¿Para qué sirve?

En Kotlin te permite interactuar con los archivos que se encuentran en el sistema de archivos de tu computadora o dispositivo.

## Conceptos Fundamentales

* **File:** Puedes crear una instancia de `File` proporcionando la ruta del archivo o directorio.
* **Rutas (Paths):** Una ruta es una cadena de caracteres que especifica la ubicación de un archivo o directorio.
* **Streams:** Para leer o escribir datos en un archivo, se utilizan streams. Un stream es un flujo de datos que se mueve desde o hacia el archivo. Kotlin proporciona varias formas de trabajar con streams para diferentes tipos de datos (texto, bytes, etc.).

## ¿Por qué se utiliza el manejo de archivos?

El manejo de archivos se utiliza porque permite guardar y usar información de forma permanente, incluso después de cerrar el programa. Aquí están las razones principales:

* **Persistencia de datos:** Los archivos permiten que la información se conserve, como documentos, configuraciones o resultados. Sin ellos, todo se perdería al cerrar la app.
* **Entrada de datos:** Permite leer información ya existente desde archivos, como registros, estadísticas, textos, etc.
* **Salida de resultados:** Los programas pueden guardar sus resultados en archivos, como reportes, imágenes o datos generados.
* **Configuración:** Se usan archivos para guardar preferencias del usuario, como idioma, tema, rutas, etc.
* **Intercambio de información:** Facilita compartir datos entre programas o plataformas, usando formatos como CSV, JSON, TXT.
* **Organización:** Se pueden guardar archivos dentro de carpetas, lo que facilita tener todo ordenado.
* **Registros (Logs):** Muchas apps crean archivos para registrar errores, eventos o funcionamiento interno.

## ¿Para qué se utiliza el manejo de archivos?

El manejo de archivos se utiliza principalmente para:

* Guardar información de forma permanente para que no se pierda cuando el programa se cierra.
* Leer datos existentes que el programa necesita para funcionar o procesar.
* Guardar los resultados o la información generada por el programa.
* Almacenar la configuración de las aplicaciones para recordar las preferencias del usuario.
* Compartir datos entre diferentes programas o sistemas.
* Organizar la información en directorios para una mejor gestión.
* Registrar eventos importantes para el seguimiento y diagnóstico de problemas.

**Formato JSON (Ejemplo práctico en la exposición):**

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

---
   
2. **Genere un ejemplo creado internamente en el recuadro.**
   - Utilice un editor de código para lograrlo.
     
```kotlin
// EJEMPLO EN CÓDIGO KOTLIN

```

### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO]()**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB]()**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN

```
