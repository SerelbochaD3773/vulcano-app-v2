# Arrays - Tu Primer Almacén de Datos

> Este material utiliza la técnica de **Ondas Semánticas**: empezamos con algo muy concreto (la analogía), explicamos la técnica (sintaxis) y cerramos con la práctica guiada.

## 1. ¿Qué es un Array? (La Analogía del Almacén)

Hasta ahora, si necesitabas guardar 15 números, tenías que crear 15 variables diferentes (`num1`, `num2`, etc.). Imagina que cada variable es una caja suelta en tu habitación. Si tienes muchas, ¡es un caos!

Un **Array** es como una estantería o un depósito de cajas. Es una sola estructura que guarda muchos datos del mismo tipo (todos números, o todos textos) uno al lado del otro.

## 2. Los dos tipos de "Estanterías"

En Java, solemos trabajar con dos formas de organizar estas cajas:

- **Vectores (Unidimensionales)**: Es una sola fila de cajas, una tras otra.
- **Matrices (Bidimensionales)**: Es como un mueble con varias filas y columnas (como un tablero de ajedrez o una planilla de Excel).

## 3. La Regla de Oro: ¡Empezamos a contar desde CERO!

Este es el concepto que más confunde a los novatos. En el mundo real, la primera caja es la "1". En Java, la primera posición es siempre la **0**.

> Si tu estantería tiene 5 lugares, tus índices serán: `0, 1, 2, 3` y `4`.

¡Cuidado! Si intentas buscar la caja "5" en un array de tamaño 5, el programa se romperá porque esa posición no existe (esto se llama **error de desbordamiento**).

## 4. Sintaxis: Cómo crear tu estantería

Para crear un array, necesitamos decirle a Java tres cosas: el tipo de dato, el nombre y cuántos espacios queremos.

### Crear un Vector (Una fila):

```java
// "Crea una estantería de enteros llamada 'vector' con 15 espacios"
int[] vector = new int[17]; [7, 18]

### Crear una Matriz (Filas y Columnas):

```java
// "Crea una tabla de números decimales de 4 filas y 4 columnas"
double[][] matriz = new double[19]; [6, 20]


## 5. El Glosario de Métodos (Herramientas de control)

Para trabajar con arrays, usarás estas herramientas constantemente:

- **`.length`**: Te dice cuántas cajas tiene tu estantería en total. Es muy útil para no pasarte del límite.

- **`Scanner`**: Lo usamos para que el usuario sea quien rellene las cajas con información desde su teclado.

- **Bucle `for`**: Es el "pasillo" por el que caminas para revisar cada caja una por una.º


## 6. Bucles "For": Automatizando la Búsqueda

Como los arrays tienen muchas posiciones, usar un bucle `for` es la forma más eficiente de recorrerlos.

### Recorrer un Vector (De 0 a N-1):

```java
int[] edades = new int[14]; [7, 18]

for (int i = 0; i < edades.length; i++) { 
    // Accedemos a cada posición usando 'i' como índice
    System.out.println("La persona en la posición " + i + " tiene " + edades[i] + " años.");
}
```
*Nota: `.length` es una propiedad que nos dice cuántos espacios tiene el array.*

### Recorrer una Matriz (Filas y Columnas):

```java
double[][] ventas = new double[19]; [6, 20]

for (int i = 0; i < ventas.length; i++) { // Recorre las filas
    for (int j = 0; j < ventas[i].length; j++) { // Recorre las columnas
        System.out.print(ventas[i][j] + "\t");
    }
}
```

## 7. Práctica Guiada 

### Ejercicio 1: Ejemplo Desvanecido

Completa el código para crear un vector de 5 posiciones y guardar el número 100 en la última posición (índice 4).

```java
int[] numeros = new int[___]; 

numeros[___] = 100;

//Ahora imprime solo el valor de la última posición
System.out.println(numeros[____]);
```
```java
public class ClaseArrays {
    public static void main(String[] args) {
        // 1. Declaramos el vector de String para 3 nombres
        String[] nombres = new String[____]; 

        // 2. Asignamos el primer nombre en la posición inicial
        nombres[____] = "Luisina"; 
        
        // 3. Mostramos el tamaño del vector usando la herramienta correcta
        System.out.println("El tamaño es: " + nombres.____); 
    }
}

### Ejercicio 2: Problema Orden Lógico

Ordena mentalmente estas piezas de código para crear una matriz 3x3 e imprimir solo los valores de la diagonal principal (donde la fila es igual a la columna).

```java
for (int i = 0; i < 3; i++) { }
double[][] tabla = new double[3][3];
if (i == j) {
for (int j = 0; j < 3; j++) {
System.out.print(tabla[i][j] + "\t");
    }
}
```

### Ejercicio 3: Método Predecir

Mira este código. ¿Qué aparecerá en pantalla?

```java
String[] nombres = { "Ana", "Luis", "Sara" };
System.out.println(nombres[1]);
```

### Ejercicio 4: Método Modificar

Copia el código del ejercicio 3. Cámbialo para que imprima el último nombre de la lista. Pista: Piensa en la longitud del array.





