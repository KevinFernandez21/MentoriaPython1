# Ejercicios de Programación - Estructuras de Control

## Ejercicio 1: Sistema de Registro y Login

**Objetivo:** Crear un sistema básico de registro e inicio de sesión usando variables y estructuras de control.

**Descripción:**
Desarrolla un programa que permita a un usuario registrarse con un nombre de usuario y contraseña, y luego iniciar sesión con esas credenciales.

**Requisitos:**
- El programa debe mostrar un menú con dos opciones: "Registrarse" e "Iniciar sesión"
- Para registrarse, el usuario debe ingresar un nombre de usuario y una contraseña
- Guardar las credenciales en variables
- Para iniciar sesión, el usuario debe ingresar sus credenciales
- Validar si las credenciales coinciden con las registradas
- Mostrar mensajes de éxito o error según corresponda
- El programa debe permitir al usuario intentar iniciar sesión mientras las credenciales no sean correctas

**Pistas:**
- Usa variables para almacenar el usuario y contraseña registrados
- Utiliza `if/else` para validar las opciones del menú
- Usa un bucle `while` para permitir múltiples intentos de inicio de sesión
- Compara las credenciales ingresadas con las almacenadas usando operadores de comparación

---

## Ejercicio 2: Calculadora de Promedio de Calificaciones

**Objetivo:** Calcular el promedio de calificaciones de un estudiante y determinar si aprobó o reprobó.

**Descripción:**
Crea un programa que solicite al usuario ingresar un número determinado de calificaciones y calcule el promedio. Luego debe indicar si el estudiante aprobó (promedio >= 6) o reprobó.

**Requisitos:**
- Preguntar cuántas calificaciones se van a ingresar
- Usar un bucle `for` para solicitar cada calificación
- Sumar todas las calificaciones
- Calcular el promedio dividiendo la suma entre el número de calificaciones
- Mostrar el promedio
- Usar `if/else` para determinar si aprobó o reprobó
- Si el promedio es mayor o igual a 9, mostrar "Excelente"
- Si está entre 7 y 8.9, mostrar "Bien"
- Si está entre 6 y 6.9, mostrar "Suficiente"
- Si es menor a 6, mostrar "Reprobado"

**Ejemplo de salida:**
¿Cuántas calificaciones vas a ingresar? 4
Ingresa la calificación 1: 8
Ingresa la calificación 2: 7
Ingresa la calificación 3: 9
Ingresa la calificación 4: 6
Tu promedio es: 7.5 - Bien - APROBADO

## Ejercicio 3: Juego de Adivinar el Número

**Objetivo:** Crear un juego donde el usuario debe adivinar un número secreto.

**Descripción:**
El programa genera un número secreto entre 1 y 50, y el usuario tiene intentos limitados para adivinarlo. Después de cada intento, el programa debe dar pistas si el número es mayor o menor.

**Requisitos:**
- Define un número secreto fijo (por ejemplo, 27)
- El usuario tiene máximo 7 intentos para adivinar
- Usar un bucle `while` o `for` para controlar los intentos
- Después de cada intento incorrecto, indicar si el número secreto es mayor o menor que el número ingresado
- Si adivina el número, mostrar un mensaje de felicitación y terminar el juego
- Si agota los intentos sin adivinar, revelar el número secreto
- Mostrar cuántos intentos le quedan después de cada intento fallido

**Ejemplo de salida:**
¡Adivina el número entre 1 y 50!
Tienes 7 intentos.
Intento 1: 25
El número secreto es MAYOR. Te quedan 6 intentos.
Intento 2: 35
El número secreto es MENOR. Te quedan 5 intentos.
Intento 3: 27
¡CORRECTO! Adivinaste en 3 intentos.

---

## Ejercicio 4: Validador de Contraseña

**Objetivo:** Crear un programa que valide si una contraseña cumple con ciertos requisitos de seguridad.

**Descripción:**
El usuario debe ingresar una contraseña y el programa verificará si cumple con todos los requisitos de seguridad establecidos.

**Requisitos:**
- Solicitar al usuario que ingrese una contraseña
- La contraseña debe cumplir con los siguientes requisitos:
  - Tener al menos 8 caracteres de longitud
  - Contener al menos una letra mayúscula
  - Contener al menos un número
  - No contener espacios
- Usar un bucle `for` para recorrer cada carácter de la contraseña y verificar los requisitos
- Usar variables booleanas o contadores para verificar cada requisito
- Mostrar qué requisitos cumple y cuáles no
- Si no cumple todos los requisitos, permitir al usuario intentar de nuevo con un bucle `while`
- Cuando la contraseña sea válida, mostrar mensaje de éxito

**Pistas:**
- Para verificar mayúsculas puedes comparar si el carácter es diferente cuando usas `.toLowerCase()`
- Para verificar números puedes usar comparaciones con caracteres '0' a '9'
- Cuenta cuántos requisitos se cumplen

**Ejemplo de salida:**
Ingresa una contraseña: hola123
x Debe tener al menos 8 caracteres
x Debe contener al menos una mayúscula
✓ Contiene números
✓ No tiene espacios
Ingresa una contraseña: Hola1234
✓ Tiene al menos 8 caracteres
✓ Contiene mayúsculas
✓ Contiene números
✓ No tiene espacios
¡Contraseña válida!
---

# Ejercicios de Programación - Estructuras de Datos

## Ejercicio 5: Sistema de Gestión de Biblioteca

**Objetivo:** Crear un sistema para gestionar libros usando listas y diccionarios.

**Descripción:**
Desarrolla un programa que permita administrar una pequeña biblioteca. Podrás agregar libros, buscar libros por título, mostrar todos los libros disponibles y prestar libros.

**Requisitos:**
- Crear una lista vacía para almacenar los libros
- Cada libro debe ser un diccionario con las siguientes claves:
  - `titulo`: nombre del libro
  - `autor`: autor del libro
  - `año`: año de publicación
  - `disponible`: True si está disponible, False si está prestado
- Implementar un menú con las siguientes opciones:
  1. Agregar un nuevo libro
  2. Mostrar todos los libros
  3. Buscar libro por título
  4. Prestar un libro
  5. Devolver un libro
  6. Salir
- Usar bucles `while` y `for` para navegar por el menú y las listas
- Validar que el libro exista antes de prestarlo o devolverlo

**Ejemplo de estructura de datos:**
```python
biblioteca = [
    {
        "titulo": "Cien años de soledad",
        "autor": "Gabriel García Márquez",
        "año": 1967,
        "disponible": True
    },
    {
        "titulo": "Don Quijote",
        "autor": "Miguel de Cervantes",
        "año": 1605,
        "disponible": False
    }
]
=== BIBLIOTECA ===
1. Agregar libro
2. Mostrar todos los libros
3. Buscar libro por título
4. Prestar libro
5. Devolver libro
6. Salir
Elige una opción: 2

--- Libros en la biblioteca ---
1. Cien años de soledad - Gabriel García Márquez (1967) - DISPONIBLE
2. Don Quijote - Miguel de Cervantes (1605) - PRESTADO

Elige una opción: 4
Ingresa el título del libro a prestar: Cien años de soledad
El libro "Cien años de soledad" ha sido prestado exitosamente.