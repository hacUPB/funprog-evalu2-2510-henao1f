## 📤 Ejercicio 1.

Investiga cuáles son los símbolos que se utilizan para representar cada operación de un algorimo con un diagrama de flujo. Asegúrate de que la fuente es confiable, discute lo que encontraste con tus compañeros y con el profe. Cuando estés seguro/a de tener los símbolos correctos, consigna la información en la bitácora.


![imagen]

[def]: ./imagenes/diag_flujo_-_Algoritmo.jpg

## 📔 Reglas para el uso de diagramas de flujo

1. Todo diagrama de flujo debe tener un **inicio y** un **fin.** 
2. Las líneas utilizadas para indicar la dirección del flujo del  diagrama deben ser rectas: verticales u horizontales. 
3. Todas las líneas utilizadas para indicar la dirección del flujo  del diagrama deben estar conectadas. La conexión puede  ser a un símbolo que exprese lectura, proceso, decisión,  impresión, conexión o fin del diagrama. 
4. El diagrama de flujo debe construirse de arriba hacia abajo  (*top-down*) y de izquierda a derecha (*right to left*).
5. La notación utilizada en el diagrama de flujo debe ser  independiente del lenguaje de programación. 
6. Al realizar una tarea compleja, es conveniente poner  comentarios que expresen o ayuden a entender lo que  hayamos hecho. 
7. Si la construcción del diagrama de flujo requiriera más de  una hoja, debemos utilizar los conectores adecuados y  enumerar las páginas correspondientes. 
8. No puede llegar más de una línea a un símbolo  determinado


1. # lápices
Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; 
de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

´´´
inicio
escribir "ingrese el número de lápices que va a comprar"
si lapices >= 1000
   costo = 85 * lapices
si no
   costo = 90 * lapices
fin si
escribir "el valor total es: ", costo
fin
```
![llll](./imagenes/lapices.png)

2. # ropa
Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, 
sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto
 es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

 ```
 inicio
 escribir "la ropa que va a comprar"
 si ropa >= 250000$
    costo = ropa * 15%
si no 
    costo = ropa * 8%
fin si
escribir "el valor total es: ", costo
fin
```

1. muestre en pantalla los números del 10 al -10
inicio
 a= 10
hacer
   escribir a
   a = a - 1
   mientras a > -11
fin


2.serie de fibonacci
0 1 1 2 3 5 8 13 21 34 55....
imprimir N números de la serie
N->lo pedimos al usuario

inicio
leer N
   a = 0
   b = 1
imprimir a, b
hacer
   c = a + b
imprimir c
 a = b
 b = c
 N = N - 1
mientras N > 0
fin


### Parte 1: Identificar Algoritmos

Responde si los siguientes enunciados representan un algoritmo. Justifica la respuesta:

1. Una página web.
2. Una receta para hacer un pastel, donde se indican ingredientes y pasos a seguir.
3. "Piensa en un número y multiplícalo por otro".
4. Un manual de instrucciones para armar un mueble, con pasos detallados y un orden claro.
5. Una lista de compras organizada en orden alfabético

RESPUESTA

1. no, porque esta es como mas libre, no tiene como un orden de pasos para ir de una parte a otra

2. si, ya que este tiene un orden y unos pasos que seguir

3. no, No es un conjunto de pasos claros, ya que no indica qué hacer con el resultado ni qué números usar. Además, falta una condición de término.

4. si, Contiene pasos bien definidos y organizados que llevan a un objetivo específico (armar el mueble). Siguiendo las instrucciones correctamente, se obtiene el resultado esperado.

5. no, Es solo una recopilación de elementos sin una serie de pasos a seguir. No hay un proceso ni instrucciones para resolver un problema, solo una lista ordenada.

### Parte 2: Variables y Constantes

Indica si las siguientes afirmaciones describen una variable o una constante:

1. El valor de la gravedad en la Tierra, 9.8 m/s².
2. La edad de una persona calculada en base al año actual y su año de nacimiento.
3. La cantidad de dinero en una cuenta bancaria.
4. La velocidad de la luz en el vacío, 299,792,458 m/s.
5. El radio de un círculo.

RESPUESTA

1. constante, El valor de la gravedad en la Tierra es fijo y no cambia en condiciones normales. 

2. variable, La edad cambia cada año, por lo que no tiene un valor fijo.

3. variable, Puede aumentar o disminuir dependiendo de depósitos y retiros.

4. constante, Es un valor universalmente aceptado y no cambia.

5. variable, Puede tomar diferentes valores dependiendo del tamaño del círculo.

### Parte 3: Características de los Algoritmos

Responde si los siguientes enunciados cumplen con las características de un algoritmo. Justifica la respuesta:

1. Para elegir la ruta más corta entre varias ciudades, el algoritmo examina rutas candidatas, deteniéndose cuando los cambios en la distancia parecen lo suficientemente pequeños.
2. Suma los números ingresados y muestra el resultado.
3. Un conjunto de pasos para calcular el área de un rectángulo dado su base y altura.
4. El algoritmo cuenta el número de votos obtenidos por cada uno de los candidatos de una elección para presidente. Empieza solicitando el nombre del candidato y finaliza cuando se ingresa el valor -1.

RESPUESTA

1. no, Un algoritmo debe ser preciso y tener un criterio de parada bien definido. En este caso, la detención basada en "cambios lo suficientemente pequeños" es ambigua, lo que puede generar incertidumbre en la ejecución.

2. si, Especifica un conjunto de pasos claros: recibir números, sumarlos y mostrar el resultado. Es finito, definido y produce un resultado.

3. si, Describe un procedimiento claro y preciso

4. si, Cumple con las características de un algoritmo: tiene una secuencia clara de pasos, maneja entrada y salida de datos, es finito y tiene un criterio de terminación bien definido (cuando se ingresa -1).

### Parte 4: Comprensión de Herramientas

Indica si las siguientes afirmaciones son ciertas o falsas respecto al pseudocódigo y diagramas de flujo:

1. El pseudocódigo utiliza símbolos estándar para representar las operaciones lógicas.
2. Los diagramas de flujo son una representación gráfica de un algoritmo.
3. El pseudocódigo debe estar escrito en un lenguaje de programación específico.
4. Un diagrama de flujo siempre debe tener un inicio y un fin claramente definidos.

RESPUESTA

1. F, El pseudocódigo usa descripciones en lenguaje natural o semiestructurado, sin símbolos gráficos estandarizados como los de los diagramas de flujo.

2. V, Representan visualmente un algoritmo usando símbolos estándar como óvalos (inicio/fin), rombos (decisiones) y rectángulos (procesos).

3. F, El pseudocódigo no sigue la sintaxis de ningún lenguaje de programación, sino que es una herramienta descriptiva para representar algoritmos de manera comprensible.

4. V, Todo diagrama de flujo debe tener un punto de inicio y de finalización para asegurar que el algoritmo sea finito y comprensible.

### Parte 5: Estructuras de Control

Describe para qué sirven las estructuras de control. Redacta dos ejemplos, uno de tu vida diaria, es decir cuando tienes que tomar decisiones en tus actividades diarias y oto ejemplo en el que se tengan que utilizar cálculos matemáticos para tomar una u otra decisión.

RESPUESTA

Las estructuras de control permiten gestionar el flujo de un programa. Se dividen en: Condicionales (if-else, switch): Toman decisiones según condiciones. - Bucles (for, while, do-while): Repiten instrucciones varias veces. - Saltos (break, continue, goto): Alteran la ejecución del código.  Estas son esenciales para hacer programas más eficientes, dinámicos y organizados.

EJEMPLO1

Vida diaria: ¿Llevar sombrilla o no?
Cuando sales de casa, decides si llevar una sombrilla dependiendo del clima:

Si está nublado o hay pronóstico de lluvia, entonces te llevas una sombrilla.
Si no, sales sin él.
Yo digo que esto es equivalente a una estructura if-else en programación.


Calculos matematicos: Aprobar o reprobar una materia
Para determinar si un estudiante aprueba un curso, se usa el promedio de sus calificaciones:
Si el promedio es mayor o igual a 60, entonces aprueba.
Si es menor a 60, reprueba.

