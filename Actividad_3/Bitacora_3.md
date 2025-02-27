
# BITACORA DE CLASE/ Actividad 3


##  ¿Que es un diagrama de flujo?

Los diagramas de flujo son herramientas visuales que emplean una variedad de símbolos estandarizados para representar las diferentes operaciones y pasos en un algoritmo o proceso. A continuación, se detallan los símbolos más comunes y su significado:

- Inicio/Fin (Óvalo): Este símbolo indica el punto de inicio o finalización del diagrama de flujo. Generalmente contiene las palabras "Inicio" o "Fin".

- Proceso (Rectángulo): Representa una operación o acción específica dentro del proceso, como una tarea o actividad que se debe realizar.

- Decisión (Diamante): Utilizado para plantear una pregunta o condición que determinará el flujo del proceso, bifurcándose en diferentes caminos según la respuesta (por ejemplo, "Sí" o "No").

- Entrada/Salida (Paralelogramo): Indica la entrada de datos al sistema o la salida de información del mismo, como la recepción de una entrada del usuario o la presentación de un resultado.

- Conector (Círculo): Se emplea para conectar diferentes partes del diagrama, especialmente cuando el flujo se extiende a otra página o sección, facilitando la continuidad y evitando líneas cruzadas.

- Almacenamiento de Datos (Cilindro): Simboliza la etapa en la que los datos se almacenan en una base de datos o archivo.

- Documento (Rectángulo con una onda en la parte inferior): Representa un documento o informe generado durante el proceso.

- Preparación (Hexágono): Indica una etapa de configuración o inicialización necesaria antes de continuar con el siguiente paso del proceso.

- Entrada Manual (Trapecio): Señala un punto donde se requiere que un usuario introduzca información manualmente.

- Visualización (Pantalla): Muestra información que se presenta al usuario, como en una pantalla o panel de control.

Es importante utilizar estos símbolos de manera coherente y estandarizada para garantizar que el diagrama de flujo sea claro y comprensible para todos los que lo consulten. 


## Ejercicio 1
Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

### Pseudocódigo 

- INICIO
    - Leer cantidad de lapices 
        - Si cantidad de lapices >= 1000
            Total = 85 * cantidad de lapices 
        - sino 
            Total = 90 * cantidad de lapices 
    - Escribir valor total a pagar ($)
- FIN 

### Diagrama de Flujo 
 ![Imagen diagrama](../Imagenes/Diagrama_Flujo1.png)

## Ejercicio 2

Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

### Pseudocodigo 
- INICIO 
    - Leer compra 
        - Si compra > 250000 
            descuento = compra * 0.15
        - Si no
            descuento = compra * 0.08
        - FIN si 
        total = compra - descuento 
        Escribir total a pagar 
        escribir valor del descuento aplicado


## Ejercicio 3

El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

### Pseudocodigo 

- INICIO
    Escribir "Ingrese la cantidad de alumnos."
    -leer cantidad

     Si cantidad >= 100
        Precio = 65 
    Sino si cantidad > 50 
        precio = 70
    sino si cantidad >= 30
        precio= 95
    sino 
    precio = 4000/alumnos 


## Ejercicios propuestos 

1. Un profesor tiene un salario inicial de $1500, y recibe un incremento de 10% anual durante 6 años. ¿Qué salario ha recibido en cada uno de los 6 años?. Realice el algoritmo y represente la solucion mediante el diagrama de flujo, el pseudocodigo y el diagrama N/S, utilizando el ciclo apropiado. 

### Pseudocodigo 
INICIO
    salario inicial = $1500
    incremeto = 0.10
    salario con incremento + salario inicial 
- Para año = 1 hasta 6 hacer 
    Escribir "año" año, ": $", salario 
    salario = salario * 0.10 // Incremento del 10%
- fin 





4. Solicitar al usuario 2 números enteros, imprimir en pantalla los numeros pares comprendidos entre ellos:

**Pseudocodigo:**
INICIO
-	Ingresar “primer número entero”
	Leer num1
-	Ingresar “segundo número entero”
	Leer num2
- Asegurar que num1 sea menor que num2 
    Si num1 > num2
	    Mayor = num1
	    Menor = num2
    Si no 
	    Mayor = num2
	    Menor = num1 
- Fin si 
	Mientras menor < mayor 
		Si residuo (menor, 2) =0 // si menor es par 
			Escribir menor 
	Fin si 
		Menor = menor +1
	Fin mientras 
- Fin 


5. Serie de fibonacci. algoritmo, ¿Cuántos números de la serie desea imprimir?

INICIO 
- Leer n
    a = 0
    b = 1
- Escribir a, b 
 n= n - 2
- Mientras n > 0
    res = a + b
- Escribir 
    a = b
    b = res
    n = n - 1
    Fin mientras 
FN
