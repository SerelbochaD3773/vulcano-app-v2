# Operadores - Comparando y Conectando Ideas

> Este material utiliza la técnica de **Ondas Semánticas**: conectamos símbolos técnicos con lógica de la vida diaria para facilitar la comprensión.

## 1. El Glosario de Símbolos (Sintaxis y Métodos)

Para "hablar" Java, primero debemos conocer sus señales de tráfico. Estos símbolos no realizan cálculos matemáticos de suma, sino que nos dicen cómo se relacionan las cosas.

### A. Operadores Relacionales (Las Comparaciones)

Estos operadores siempre responden con un **SÍ** (`true`) o un **NO** (`false`):

- `==` (Igual a): ¡Cuidado! No es un solo `=`, son dos. ¿Es "A" igual a "B"?
- `!=` (Distinto de): ¿Es "A" diferente a "B"?
- `>` / `<` : Mayor que / Menor que.
- `>=` / `<=` : Mayor o igual / Menor o igual.

### B. Operadores Lógicos (Las Conexiones)

Sirven para unir dos o más comparaciones:

- `&&` (AND / Y): Ambas condiciones deben ser verdad. (Ej: Si tengo entrada **Y** tengo dinero, entro al cine).
- `||` (OR / O): Al menos una debe ser verdad. (Ej: Si es sábado **O** es domingo, descanso).
- `!` (NOT / NO): Invierte el valor. Lo que es `true` lo vuelve `false`.

### C. Operadores de Asignación (Los Atajos)

En lugar de escribir `x = x + 5`, Java te permite ser más rápido:

- `+=` : Suma y asigna.
- `*=` : Multiplica y asigna.

## 2. La Magia del "Cortocircuito"

Java es inteligente y ahorrador de energía.

- En un **`&&` (Y)**, si la primera parte es falsa, Java ni siquiera mira la segunda, porque ya sabe que todo el resultado será **falso**.
- En un **`||` (O)**, si la primera parte es verdadera, Java se detiene ahí; ya sabe que con una que sea verdad es suficiente.

Esto evita errores, como intentar dividir por cero si primero validamos que el divisor sea distinto de cero.

## 3. Práctica Avanzada: Método PRIMM

### A. Predecir

¿Cuál será el resultado final de `resultado`? Intenta resolverlo sin usar la computadora.

```java
int energia = 50;
int pociones = 2;
boolean puedePelear = (energia > 20) && (pociones > 0);
energia += 10; 
System.out.println("¿Puede pelear?: " + puedePelear);
System.out.println("Energía final: " + energia);

### B. Ejecutar e Investigar 

Copia el código en tu editor. ¿El resultado de `puedePelear` fue `true`? ¿Por qué la energía subió a `60`? Fíjate que el operador `+=` cambió el valor de la variable original.

### C. Modificar 

Cambia el valor de `pociones` a `0`. ¿Qué pasa con `puedePelear`? Ahora intenta cambiar el operador `&&` por un `||`. ¿Cómo cambia la lógica del juego? *Experimentar con estos cambios reduce tu carga cognitiva al aprender.*

### 4. Reto de Estructura: Problema de Parsons

Ordena estas piezas de código para crear un sistema que valide si un usuario puede entrar a una zona VIP (debe tener más de 18 años y una invitación válida).

```java
boolean tieneInvitacion = true;
if (esMayor && tieneInvitacion) {
boolean esMayor = edad >= 18;
int edad = 20;
System.out.println("¡Bienvenido al VIP!"); }

### Resolución

```java
int edad = 20;
boolean tieneInvitacion = true;
boolean esMayor = edad >= 18;
if (esMayor && tieneInvitacion) {
    System.out.println("¡Bienvenido al VIP!");
}