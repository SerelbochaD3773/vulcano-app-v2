# Clase 2: Variables y Tipos de Datos en Java

¡Bienvenidos a esta segunda sesión! En esta clase aprenderemos los cimientos de cualquier programa en Java: cómo guardar información. Para esto, utilizaremos dos conceptos fundamentales: **Variables** y **Constantes**.

## 1. ¿Qué es una Variable y una Constante?

Antes de programar, debemos entender la diferencia entre estos dos contenedores de información:

- **Variable**: Es un espacio en la memoria de la computadora que almacena un valor que puede cambiar a lo largo del tiempo durante la ejecución del programa. Analogía: Imagina una caja donde guardas tu edad; cada año, el número dentro de la caja cambia.

- **Constante**: Es un valor que se mantiene fijo y no cambia en un periodo determinado. En Java, se definen usando la palabra clave `final`. Ejemplo: El valor del IVA (21%) o el número PI.

## 2. Tipos de Datos Primitivos

Java es un lenguaje fuertemente tipado, lo que significa que siempre debemos decirle al programa qué tipo de dato vamos a guardar en cada "caja". Los tipos más comunes son:

| Categoría | Tipo de Dato | Descripción |
|-----------|--------------|-------------|
| Enteros   | `int`        | Números enteros comunes (ej. 5, -10) |
| Enteros   | `long`       | Números enteros muy largos |
| Decimales | `double`     | Números con punto decimal de alta precisión |
| Decimales | `float`      | Números decimales de precisión sencilla (requiere una f al final) |
| Lógicos   | `boolean`    | Solo admite dos valores: true (verdadero) o false (falso) |
| Carácter  | `char`       | Almacena un solo carácter. Se escribe entre comillas simples (ej. 'A') |

## 3. Tipos de Datos de Referencia: El `String`

A diferencia de los anteriores, el `String` no es un tipo primitivo, sino una clase. Se utiliza para almacenar cadenas de texto (palabras o frases) y siempre debe ir entre comillas dobles.

Ejemplo: `"Hola Mundo"` o `"Luisina"`

## 4. Cómo declarar y asignar variables

La "fórmula" para crear una variable en Java consta de tres partes esenciales:

1. **Tipo de dato**: (¿Qué voy a guardar?)
2. **Nombre de la variable**: (¿Cómo se llama mi caja?)
3. **El punto y coma (`;`)**: (Indica el fin de la instrucción)

### Sintaxis:

```java
// Declaración y asignación en pasos separados
int numero;
numero = 5;

// Declaración y asignación en una misma línea
String nombre = "Ibra";