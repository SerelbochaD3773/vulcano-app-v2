# Módulo 5: Estructuras de Control - El Cerebro del Código

En este módulo aprenderás a darle "lógica" a tus programas. Java no solo lee líneas; puede decidir qué camino tomar o repetir una acción hasta que se cumpla una meta.

## 1. El Alfabeto de este Módulo (Glosario de Métodos)

Antes de ver la lógica, entendamos estas "palabras" que verás en los ejercicios:

- `System.out.println("...")`: Es un método que sirve para imprimir (mostrar) texto en la consola.
- `main(String[] args)`: Es el "punto de entrada". Java siempre busca esta palabra para saber dónde empezar a correr tu código.
- `Scanner` o `read()`: Métodos que se usan para que el programa "escuche" lo que el usuario escribe en el teclado.

## 2. Bloques de Código: Las Llaves `{ }`

Para agrupar varias instrucciones y que Java sepa que pertenecen a una misma decisión o bucle, usamos llaves.

> **Regla de oro:** Cada `{` que abras debe tener su `}` que la cierre. Las instrucciones dentro de las llaves suelen terminar en punto y coma `;`.

## 3. Estructuras de Selección (Tomar Decisiones)

### A. La instrucción `if-else`

Se usa para evaluar si algo es verdadero o falso. Sintaxis:

```java
if (condicion) {
    // Código si la condición es VERDADERA
} else {
    // Código si la condición es FALSA
}
Reorganiza estas líneas (mentalmente o en papel) para crear un programa que pida una contraseña hasta que sea correcta (`"1234"`).

```java
}
while (!password.equals("1234"));
String password;
do {
password = leerTeclado();


### B. La instrucción `switch`

Útil cuando tienes muchas opciones fijas (como un menú). Usa la palabra `case` para cada opción y `break` para detenerse.

## 4. Estructuras de Iteración (Bucles)

### A. El bucle `for`

Se usa cuando sabes exactamente cuántas veces quieres repetir algo. Sintaxis:


for (inicializacion; condicion; incremento) {
    // Código que se repite
}
> **Ejemplo:** `for(int i=0; i<5; i++)` repetirá el código 5 veces.

### B. Bucles `while` y `do-while`

- **`while`**: Repite mientras la condición sea verdadera. Si la condición es falsa desde el inicio, el código nunca corre.
- **`do-while`**: Asegura que el código corra al menos una vez, porque la condición se revisa al final.

## 5. Práctica Guiada (Sin "Pantallas en Blanco")

### Ejercicio 1: Ejemplo Desvanecido 

Completa el código para que el programa diga si una persona es mayor de edad (18 años).


int edad = 20;

if (edad ____ 18) { // Usa el operador "mayor o igual" (>=)
    System.out.println("Eres adulto");
} ____ { 
    System.out.println("Eres menor de edad");
}

### Ejercicio 2: Problema Orden Lógico

Ordena mentalmente estas líneas para crear un bucle que cuente del 1 al 3.


System.out.println(i);
for (int i = 1; i <= 3; i++) {
}

### Ejercicio 3: Método Predecir

Mira este código y responde: ¿Qué aparecerá en pantalla?


int x = 1;
while (x < 3) {
    System.out.print(x + " ");
    x++;
}

### Ejercicio 4: Método Modificar

Ahora modifica el código del ejercicio 3. Cambia `while` por `do-while`. ¿El resultado cambia? ¿Por qué?