# Solución de la Actividad 4

## 1. Introducción

### Pregunta orientadora:
**¿Por qué crees que el pseudocódigo es útil antes de escribir un programa en Python?**

El pseudocódigo es útil porque permite estructurar la lógica de un programa haciendo que sea mas facil la compresión de la sintaxis de progración tambien hace que la planificación del algoritmo y que la traducción al código sea más sencilla y organizada.


## 2. Estructura básica del pseudocódigo

### Actividad:

Pseudocódigo para calcular el promedio de tres calificaciones:

```plaintext
INICIO
    Leer calificacion1
    Leer calificacion2
    Leer calificacion3
    suma = calificacion1 + calificacion2 + calificacion3
    promedio = suma / 3
    Mostrar promedio
FIN
```

---

## 3. Traducción del pseudocódigo a Python

```python
# Solicitar tres calificaciones al usuario
calificacion1 = float(input("Ingresa la primera calificación: "))
calificacion2 = float(input("Ingresa la segunda calificación: "))
calificacion3 = float(input("Ingresa la tercera calificación: "))

# Calcular el promedio
suma = calificacion1 + calificacion2 + calificacion3
promedio = suma / 3

# Mostrar el resultado
print("El promedio es:", promedio)
```

### Pregunta orientadora:
**¿Cuál es la diferencia entre usar `int(input())` y `float(input())` en Python?**

La diferencia es que `int(input())` convierte la entrada en un número entero, descartando los decimales, mientras que `float(input())` permite valores con decimales, lo que es útil cuando se trabaja con datos como calificaciones o promedios.


## 4. Ejemplos adicionales de pseudocódigo y su traducción

**Ejemplo:** Encontrar el menor de dos números

**Pseudocódigo:**

```plaintext
INICIO
    Leer num1
    Leer num2
    Si num1 < num2 Entonces
        Mostrar "El número 1 es menor"
    Sino
        Mostrar "El número 2 es menor"
FIN
```

**Python:**

```python
num1 = float(input("Ingresa el primer número: "))
num2 = float(input("Ingresa el segundo número: "))

if num1 < num2:
    print("El número 1 es menor")
else:
    print("El número 2 es menor")
```

### Actividad:
**Escribe un pseudocódigo y tradúcelo a Python para calcular el promedio de una lista de calificaciones.**

**Pseudocódigo:**

```plaintext
INICIO
    Leer cantidad de calificaciones
    Inicializar suma en 0
    Para i desde 1 hasta cantidad
        Leer calificacion
        suma = suma + calificacion
    promedio = suma / cantidad
    Mostrar promedio
FIN
```

**Python:**

```python
cantidad = int(input("Ingrese la cantidad de calificaciones: "))
suma = 0

for i in range(cantidad):
    calificacion = float(input(f"Ingrese la calificación {i+1}: "))
    suma += calificacion

promedio = suma / cantidad
print("El promedio es:", promedio)
```



## 5. Buenas prácticas

### Pregunta orientadora:
**¿Por qué es importante comentar el código, aunque sea breve y conciso?**

Comentar el código es importante porque facilita la comprensión del programa tanto para el programador como para otras personas que puedan leer el código en el futuro, tambien ayuda a identificar la funcionalidad de diferentes secciones del programa. 



## 6. Reto final

### Traducción de pseudocódigo a Python

**Ejercicio 1:** Determinar si un número es par o impar

**Pseudocódigo:**

```plaintext
INICIO
    Leer numero
    Si numero mod 2 == 0 Entonces
        Mostrar "El número es par"
    Sino
        Mostrar "El número es impar"
FIN
```

**Python:**

```python
numero = int(input("Ingrese un número: "))

if numero % 2 == 0:
    print("El número es par")
else:
    print("El número es impar")
```

### Pregunta final:
**Después de este tutorial, ¿qué puntos crees que deberías reforzar para sentirte más seguro al traducir pseudocódigo a Python?**

Desde mi punto de vista y desde mi experiencia me parece muy importante reforzar la comprensión de estructuras de control como `if`, `for` y `while`, tambien conocer un poco mas las funciones de ciertos comandos que facilitan el trabajo de traducir el pseudocodigo a un leguaje de programación, en este caso python. 