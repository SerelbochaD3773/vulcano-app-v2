# Módulo 3: Operadores Aritméticos - Manipulando la Información

> Este módulo utiliza la técnica de **Ondas Semánticas**: empezamos con algo sencillo (lo concreto), pasamos al código (lo técnico) y volvemos a la práctica (reempaquetado).

## 1. ¿Qué es un Operador? (La Analogía)

Imagina que Java es un chef. Las variables son los ingredientes guardados en cajas, y los **operadores** son las instrucciones del chef: *"mezcla esto"*, *"divide aquello"* o *"añade 1 más"*. Sin operadores, los datos solo estarían guardados sin hacer nada útil.

## 2. Los 5 Operadores Fundamentales

En Java, usamos estos símbolos para transformar tus números:

| Operación | Símbolo | Ejemplo en Código       |
|-----------|---------|-------------------------|
| Suma      | `+`     | `resultado = 10 + 5;`   |
| Resta     | `-`     | `resultado = 10 - 5;`   |
| Multiplicación | `*` | `resultado = 10 * 5;`   |
| División  | `/`     | `resultado = 10 / 5;`   |
| Resto (Módulo) | `%` | `sobrante = 10 % 3;` (El resultado es 1) |

> **Truco de aprendizaje:** El operador **Módulo (`%`)** no te da el resultado de la división, sino lo que *"sobra"*. Es como repartir 10 caramelos entre 3 niños: cada uno recibe 3 y te sobra **1**.

## 3. Atajos Inteligentes: Incrementos y Decrementos

A veces solo queremos sumar o restar **1** a una variable (muy común en contadores). En lugar de escribir `x = x + 1`, Java te permite usar estos *"atajos"*:

- `++` **(Incremento)**: Suma 1 a la variable.
- `--` **(Decremento)**: Resta 1 a la variable.

## 4. Método de Estudio

Para aprender sin frustrarte, no intentes escribir código desde cero. Sigue estos pasos con el ejemplo de abajo:

### Paso 1: Predecir

Mira este código. ¿Qué número crees que aparecerá en pantalla? (No lo ejecutes todavía).

```java
int manzanas = 10;
int amigos = 3;
int sobra = manzanas % amigos;
System.out.println("Sobran: " + sobra);
```

### Paso 2: Ejecutar y Investigar

Copia el código en tu editor y ejecútalo.

¿Fue igual a tu predicción?

Si el resultado fue `1`, investiga por qué:

## Paso 3: Modificar

Cambia el valor de `manzanas` a `12`. ¿Qué pasa con el resultado?

```java
int manzanas = 12;  // Modificado de 10 a 12
int amigos = 3;
int sobra = manzanas % amigos;
System.out.println("Sobran: " + sobra);

## 5. Ejercicios Desvanecidos (Faded Examples)

Completa los espacios en blanco (`____`) para que el programa funcione correctamente:

```java
public class Practica {
    public static void main(String[] args) {
        int base = 10;
        int altura = 5;
        
        // Queremos calcular el área de un rectángulo (base por altura)
        int area = base ____ altura; 
        
        System.out.println("El área es: " + ____);
    }
}