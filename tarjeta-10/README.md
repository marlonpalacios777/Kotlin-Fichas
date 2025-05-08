## Programación Orientada a Objetos (POO)

---

### 1. Descripción: Fundamentos y Propósito

La Programación Orientada a Objetos (POO) es un **paradigma de programación** fundamental que se centra en la creación de **objetos**. Estos objetos encapsulan **atributos** (datos) y **comportamientos** (funciones o métodos), modelando entidades del mundo real dentro del software.

#### ¿Para qué sirve la POO?

La POO ofrece una estructura robusta para el desarrollo de software, mejorando significativamente:

* **Organización del código:** Facilita la comprensión y el manejo de proyectos complejos.
* **Reutilización:** Permite crear componentes de software que pueden ser utilizados en diferentes partes de la aplicación o en otros proyectos.
* **Mantenimiento:** Simplifica la identificación y corrección de errores, así como la adaptación a nuevos requerimientos.
* **Escalabilidad:** Facilita el crecimiento y la expansión de las aplicaciones de manera modular.

La POO es ampliamente utilizada en diversas áreas como aplicaciones de software de gran escala, videojuegos, sistemas de gestión e inteligencia artificial.

#### ¿Por qué se utiliza la POO?

La adopción de la POO se debe a sus numerosas ventajas:

* **Simplificación de la complejidad:** Divide problemas complejos en unidades más pequeñas y manejables (objetos).
* **Reutilización y eficiencia:** La herencia y la composición permiten reutilizar código existente, reduciendo el tiempo y el esfuerzo de desarrollo.
* **Seguridad:** El encapsulamiento protege los datos internos de los objetos, controlando su acceso y evitando modificaciones no deseadas.
* **Estándar en lenguajes modernos:** La mayoría de los lenguajes de programación populares (Kotlin, Java, Python, C#, Swift, C++) están diseñados para soportar la POO.
* **Modelado del mundo real:** Permite representar entidades y sus interacciones de forma intuitiva en el código (ej: un objeto `Coche` con atributos como `color` y comportamientos como `acelerar`).
* **Facilita el mantenimiento y la escalabilidad:** Los cambios en una parte del sistema (un objeto o una clase) tienen un impacto limitado en otras partes.
* **Mejora la legibilidad y la depuración:** La estructura modular del código facilita su comprensión y la localización de errores.
* **Trabajo en equipo eficiente:** Permite a diferentes desarrolladores trabajar en módulos independientes (clases) sin interferir entre sí.

En resumen, la POO es un pilar fundamental para desarrollar software organizado, reutilizable, mantenible y seguro, siendo esencial para cualquier programador.

---

### 2. Conceptos Clave de la POO en Kotlin

#### Clases y Objetos

* **Clase:** Una **plantilla** o **estructura** que define un **tipo de dato personalizado**. En Kotlin, agrupa:
    * **Propiedades:** Características o atributos del objeto.
    * **Funciones (métodos):** Comportamientos o acciones del objeto.
* **Características de las clases:**
    * Definen tipos de datos personalizados.
    * Pueden tener **constructores** (primario y/o secundarios).
    * Soportan **herencia**.
    * Permiten **control de visibilidad** (`private`, `public`, `protected`, `internal`).
    * Permiten **encapsular** datos y comportamientos.
* **Objeto:** Una **instancia concreta** de una clase. Cada objeto tiene su propio conjunto de datos y puede acceder a las funciones de su clase.

#### Constructores

* Un **constructor** es una función especial utilizada para **crear objetos** e **inicializar sus propiedades**.
* En Kotlin existen:
    * **Constructor primario:** Definido en la cabecera de la clase.
    * **Constructor secundario:** Declarado dentro del cuerpo de la clase usando la palabra clave `constructor`.

#### Encapsulación

* La **encapsulación** es el principio de **ocultar los detalles internos** de una clase y **proteger sus datos**, permitiendo el acceso solo a través de **métodos controlados**.
* **Modificadores de acceso en Kotlin:**
    * `public`: Accesible desde cualquier parte del programa.
    * `private`: Accesible solo dentro de la clase.
    * `protected`: Accesible dentro de la clase y sus subclases.
    * `internal`: Accesible solo dentro del mismo módulo.
* **Getters y Setters:** Métodos utilizados para **leer (`get`)** o **modificar (`set`)** propiedades privadas, permitiendo la implementación de lógica de validación.

#### Herencia

* La **herencia** permite que una clase (**subclase** o clase derivada) herede **propiedades** y **comportamientos** de otra clase (**superclase** o clase base).
* **Términos clave:**
    * `open`: Modificador que permite que una clase sea susceptible de ser heredada.
    * `override`: Palabra clave utilizada para **sobrescribir** un comportamiento heredado en la subclase.
    * `super`: Palabra clave utilizada para **acceder a miembros** (propiedades o métodos) de la clase padre desde la subclase.

#### Clases Abstractas

* Una **clase abstracta** define una **estructura común** para sus subclases, especificando qué métodos deben implementar, pero sin proporcionar una implementación completa para todos ellos.
* **No se puede instanciar directamente**.
* Puede contener:
    * **Métodos abstractos:** Declarados sin cuerpo (la implementación debe proporcionarse en las subclases concretas).
    * **Métodos normales:** Declarados con un cuerpo (implementación).

#### Polimorfismo

* El **polimorfismo** (que significa "muchas formas") permite utilizar la **misma función** o método para realizar **diferentes comportamientos** dependiendo del **objeto** que se esté utilizando.

#### Interfaces

* Una **interfaz** define un **contrato**: si una clase implementa una interfaz, **debe proporcionar una implementación** para todos los métodos declarados en esa interfaz.
* **Características:**
    * Se declara utilizando la palabra clave `interface`.
    * Puede contener **funciones abstractas** (sin cuerpo), **funciones con cuerpo** (con una implementación por defecto) y **propiedades abstractas** (sin inicialización).
    * Una clase puede **implementar múltiples interfaces**.

---
   
2. **Genere un ejemplo internamente en el recuadro.**
   - Utilice un editor de código para lograrlo.


### CREAR ALGORITMO PROPIO Y EXPLIQUELO PASO A PASO 
- Genere el link del audio y el link de GitHub.  

🔗 **[LINK DEL AUDIO]()**  
🔗 **[LINK CÓDIGO PROBADO POR US Y GUARDADO EN GITHUB]()**.

**ALGORITMO CREADO Y EXPLICACION DE COMO FUNCIONA LA ESTRUCTURA**
```kotlin
// EJERCICIO CREADO EN KOTLIN

```
