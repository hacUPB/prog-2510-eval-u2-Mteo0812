# Problemas

1. Se requiere obtener la distancia entre dos puntos en el plano cartesiano,
tal y como se muestra en la figura 1. Realice un diagrama de flujo y pseudocódigo
que representen el algoritmo para obtener la distancia entre
esos puntos.

## Tabla de Variables  

| Tipo     | Nombre | Descripción |
|----------|--------|-------------|
| Entrada  | x1, y1 | Coordenadas del primer punto |
| Entrada  | x2, y2 | Coordenadas del segundo punto |
| Salida   | d     | Distancia entre los dos puntos |
| Constante | Ninguna | No hay valores fijos |

## Ecuación Involucrada  

La distancia entre dos puntos en el plano cartesiano se calcula con la fórmula:  
\[
d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}
\]


## Estrategia de Solución  

1. Solicitar las coordenadas (x₁, y₁, x₂, y₂).
2. Aplicar la fórmula de distancia entre dos puntos.
3. Mostrar el resultado.

- Pseudocodigo:

        Inicio
        Escribir "Ingrese x1:"
            Leer x1
        Escribir "Ingrese y1:"
            Leer y1
        Escribir "Ingrese x2:"
            Leer x2
        Escribir "Ingrese y2:"
            Leer y2
        d = RaízCuadrada((x2 - x1)^2 + (y2 - y1)^2)
            Escribir "La distancia entre los dos puntos es:", d
        Fin

2. Una modista, para realizar sus prendas de vestir, encarga las telas al extranjero.
Para cada pedido, tiene que proporcionar las medidas de la tela
en pulgadas, pero ella generalmente las tiene en metros. Realice un algoritmo
para ayudar a resolver el problema, determinando cuántas pulgadas
debe pedir con base en los metros que requiere. Represéntelo mediante un
diagrama de flujo y pseudocódigo (1 pulgada = 0.0254 m).

## Tabla de Variables  

| Tipo     | Nombre | Descripción |
|----------|--------|-------------|
| Entrada  | metros | Cantidad de tela en metros |
| Salida   | pulgadas | Cantidad de tela convertida a pulgadas |
| Constante | factor_conversion | Valor fijo: 1 pulgada = 0.0254 metros |

## Ecuación Involucrada  


\[
pulgadas = \frac{metros}{0.0254}
\]

## Estrategia de Solución  

1. Solicitar la cantidad de metros de tela.
2. Aplicar la conversión usando la ecuación.
3. Mostrar la cantidad equivalente en pulgadas.

- Pseudocodigo:

        Inicio
        Escribir "Ingrese la cantidad de metros de tela:"
            Leer metros
        pulgadas = metros / 0.0254
            Escribir "La cantidad en pulgadas es:", pulgadas
        Fin

3. Se requiere determinar la hipotenusa de un triángulo rectángulo. ¿Cómo sería el diagrama de flujo y el pseudocódigo que representen el algoritmo para obtenerla? 
Recuerde que por Pitágoras se tiene que: $C^2 = A^2 + B^2$.

## Tabla de Variables  

| Tipo     | Nombre | Descripción |
|----------|--------|-------------|
| Entrada  | A | Cateto 1 del triángulo |
| Entrada  | B | Cateto 2 del triángulo |
| Salida   | C | Hipotenusa del triángulo |
| Constante | Ninguna | No hay valores fijos |

## Ecuación Involucrada  

La hipotenusa se obtiene con el Teorema de Pitágoras:

\[
C = \sqrt{A^2 + B^2}
\]

## Estrategia de Solución  

1. Solicitar los valores de los catetos A y B.
2. Aplicar la fórmula de Pitágoras.
3. Mostrar la hipotenusa C.

- Pseudocodigo:

        Inicio
        Escribir "Ingrese el valor del cateto A:"
            Leer A
        Escribir "Ingrese el valor del cateto B:"
            Leer B
        C = RaízCuadrada(A^2 + B^2)
            Escribir "La hipotenusa del triángulo es:", C
        Fin

4. Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año.

## Tabla de Variables  

| Tipo     | Nombre | Descripción |
|----------|--------|-------------|
| Entrada  | díaN, mesN, añoN | Fecha de nacimiento (día, mes, año) |
| Entrada  | díaA, mesA, añoA | Fecha actual (día, mes, año) |
| Salida   | edad | Edad de la persona |
| Salida   | mensaje | Indica si ya cumplió años, si aún no lo ha hecho o si es su cumpleaños |
| Constante | Ninguna | No hay valores fijos |

## Estrategia de Solución  

1. Restar el año de nacimiento del año actual para calcular la edad.
2. Comparar mes y día para verificar si la persona ya cumplió años o aún no.
3. Si la fecha actual coincide con la fecha de nacimiento, mostrar "Feliz Cumpleaños".


- Pseudocodigo:

        Inicio
        Escribir "Ingrese su fecha de nacimiento (día, mes, año):"
            Leer dia, mes, año
        Escribir "Ingrese la fecha actual (día, mes, año):"
            Leer dia, mes, año
                edad = año - año

        Si (mesA < mesN) o (mesA = mesN y diaA < diaN) 
            edad = edad - 1
         Escribir "Aún no ha cumplido años este año."
        Sino Si (mesA = mes y dia = dia) 
         Escribir "Feliz Cumpleaños!"
        Sino
            Escribir "Ya ha cumplido años este año."
        FinSi

         Escribir "Su edad actual es:", edad
        Fin

5. Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar
más de 50 horas no está permitido. Represente el algoritmo mediante pseudocódigo.

## Tabla de Variables  

| Tipo     | Nombre | Descripción |
|----------|--------|-------------|
| Entrada  | horas | Horas trabajadas en la semana |
| Entrada  | pagoHora | Pago por hora normal |
| Salida   | sueldo | Sueldo total semanal |
| Constante | Ninguna | No hay valores fijos |

## Estrategia de Solución  

1. Calcular el sueldo de las primeras 40 horas con tarifa normal.
2. Las horas 41 a 45 se pagan doble.
3. Las horas 46 a 50 se pagan triple.
4. Si las horas son mayores a 50, mostrar un error.

- Pseudocodigo:

        Inicio
        Escribir "Ingrese las horas trabajadas en la semana:"
            Leer horas
        Escribir "Ingrese el pago por hora:"
            Leer pagoHora
        sueldo = 0

        Si horas > 50 Entonces
            Escribir "No es permitido trabajar más de 50 horas."
        Sino Si horas > 45 Entonces
            sueldo = (40 * pagoHora) + (5 * pagoHora * 2) + ((horas - 45) * pagoHora * 3)
        Sino Si horas > 40 Entonces
            sueldo = (40 * pagoHora) + ((horas - 40) * pagoHora * 2)
        Sino
            sueldo = horas * pagoHora
        FinSi

            Escribir "El sueldo semanal es:", sueldo
        Fin

6. Se requiere un algoritmo para determinar, de N cantidades, cuántas son cero, cuántas son menores a cero, y cuántas son mayores a cero. Realice el pseudocódigo para representarlo, utilizando el ciclo apropiado.

## Tabla de Variables  

| Tipo     | Nombre | Descripción |
|----------|--------|-------------|
| Entrada  | N | Cantidad de números a evaluar |
| Entrada  | num | Número ingresado por el usuario |
| Salida   | ceros, positivos, negativos | Cantidad de ceros, positivos y negativos |
| Constante | Ninguna | No hay valores fijos |

## Estrategia de Solución  

1. Pedir la cantidad N de números a evaluar.
2. Recorrer cada número y clasificarlo como positivo, negativo o cero.

- Pseudocodigo:

        Inicio
        Escribir "Ingrese la cantidad de números a evaluar:"
            Leer N
            ceros = 0
            positivos = 0
            negativos = 0

        Para i = 1 Hasta N Hacer
                Escribir "Ingrese un número:"
            Leer num
        Si num = 0 Entonces
            ceros = ceros + 1
        Sino Si num > 0 Entonces
            positivos = positivos + 1
        Sino
            negativos = negativos + 1
        FinSi
        FinPara

            Escribir "Cantidad de ceros:", ceros
            Escribir "Cantidad de números positivos:", positivos
            Escribir "Cantidad de números negativos:", negativos
        Fin

7. Se requiere un algoritmo para determinar cuánto ahorrará en pesos una persona diariamente, y en un año, si ahorra 3$ el primero de enero, 9¢ el dos de enero, 27$ el 3 de enero y así sucesivamente todo el año. Represente la solución mediante pseudocódigo.

## Tabla de Variables  

| Tipo     | Nombre | Descripción |
|----------|--------|-------------|
| Entrada  | Ninguna | El proceso se basa en días del año |
| Salida   | ahorroTotal | Cantidad ahorrada en un año |
| Constante| 3 | Cantidad inicial de ahorro |

## Estrategia de Solución  

1. Cada día, multiplicar el ahorro del día anterior por 3.
2. Sumar cada ahorro al total del año.
- Pseudocodigo:

        Inicio
            ahorro = 3
            ahorroTotal = 0

        Para dia = 1 Hasta 365 Hacer
            ahorroTotal = ahorroTotal + ahorro
            ahorro = ahorro * 3
        FinPara

            Escribir "El ahorro total en un año es:", ahorroTotal
        Fin

8. Realice el algoritmo para determinar cuánto pagará una persona que adquiere N artículos, los cuales están de promoción. Considere que si su precio es mayor o igual a $200 se le aplica un descuento de 15%, y si su precio es mayor a $100, pero menor a $200, el descuento es de
12%; de lo contrario, solo se le aplica 10%. Se debe saber cuál es el costo y el descuento que tendrá cada uno de los artículos y finalmente cuánto se pagará por todos los artículos obtenidos. Represente la solución mediante pseudocódigo.
- Pseudocodigo:

        Inicio
         Escribir "Ingrese la cantidad de artículos:"
            Leer N
        total = 0

            Para i = 1 Hasta N Hacer
             Escribir "Ingrese el precio del artículo ", i, ":"
                    Leer precio

        Si precio >= 200 Entonces
            descuento = precio * 0.15
        Sino Si precio >= 100 Entonces
            descuento = precio * 0.12
        Sino
            descuento = precio * 0.10
        FinSi

            precioFinal = precio - descuento
            total = total + precioFinal

            Escribir "Descuento aplicado:", descuento
            Escribir "Precio final del artículo:", precioFinal
        FinPara

         Escribir "Total a pagar por todos los artículos:", total
        Fin
9. Realice un algoritmo y represéntelo mediante pseudocódigo para obtener una función exponencial, la cual está dada por:
    
    $𝑒^𝑥 = 1+\frac x {1!} + \frac {x^2}{2!}+ \frac {x^3}{3!}+ …$
- Pseudocodigo:

        Inicio
            Escribir "Ingrese el valor de x:"
             Leer x
            exp = 1
            termino = 1

            Para i = 1 Hasta 10 Hacer
             termino = (termino * x) / i
              exp = exp + termino
        FinPara

            Escribir "El valor aproximado de e^x es:", exp
        Fin
10. Realice un algoritmo para obtener el seno de un ángulo y represéntelo mediante pseudocódigo. Utilice la siguiente ecuación:
$Sen x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + ...$
- Pseudocodigo:

        Inicio
            Escribir "Ingrese el valor de x (en radianes):"
            Leer x
            seno = 0
            signo = 1
            termino = x

        Para i = 1 Hasta 10 Hacer
            seno = seno + signo * termino
            termino = (termino * x * x) / ((2*i) * (2*i+1))
            signo = signo * -1
        FinPara

           Escribir "El valor aproximado de sen(x) es:", seno
        Fin





