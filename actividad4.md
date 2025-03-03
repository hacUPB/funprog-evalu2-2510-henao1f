## 1. Introducción

¿Alguna vez te has preguntado cómo convertir un conjunto de pasos lógicos (pseudocódigo) en un programa funcional en C?

Este tutorial te guiará a través del proceso de:

1. Interpretar tu pseudocódigo.
2. Traducirlo a sintaxis C.
3. Añadir detalles específicos (tipos de datos, prototipos de funciones, etc.).

> Pregunta orientadora:
> 
> - ¿Por qué crees que el pseudocódigo es útil antes de escribir un programa en C?

R/= El pseudocódigo es útil antes de programar en C porque permite estructurar la lógica del algoritmo sin preocuparse por la sintaxis, facilitando la planificación, reduciendo errores tempranos y agilizando la implementación. Al ser un lenguaje independiente, mejora la colaboración y ayuda a dividir el problema en pasos claros, haciendo que la transición a C sea más eficiente y ordenada.

## 2. Estructura básica del pseudocódigo

Generalmente, el pseudocódigo se escribe en un lenguaje “amigable” que describe el **orden de las operaciones**. Por ejemplo:

```
INICIO
    Leer valor1
    Leer valor2
    suma = valor1 + valor2
    Mostrar suma
FIN
```

> Actividad
>
> - Toma un pseudocódigo de un ejercicio anterior o escribe tu propio pseudocódigo, similar al mostrado en el ejemplo de arriba.

**Retos**:

1. **Claridad**: Asegúrate de que cada paso esté claro y sea fácil de entender.
2. **Secuencia**: Verifica que tu pseudocódigo siga el orden lógico (entrada → procesamiento → salida).

R/= Algoritmo Resta

    Escribir "Ingrese el primer número: "

    Leer num1

    Escribir "Ingrese el segundo número: "

    Leer num2

    resultado <- num1 - num2

    Escribir "El resultado de la resta es: ", resultado

FinAlgoritmo


## 3. Traduciendo el pseudocódigo a C

Cuando traducimos un pseudocódigo a C, debemos prestar atención a:

- **Declaración de variables**: En C, es **obligatorio** especificar el tipo de cada variable (int, float, etc.).
- **Funciones de entrada/salida**: `scanf` para leer datos, `printf` para mostrar resultados.
- **Estructuras de control**: `if`, `while`, `for`, etc.

### Ejemplo de pseudocódigo a C

Pseudocódigo:

```
INICIO
    Leer valor1
    Leer valor2
    suma = valor1 + valor2
    Mostrar suma
FIN
```

Versión en C (programa completo):

> Pregunta orientadora
> 
> - ¿Por qué es importante declarar el tipo de variable (int, float, etc.) antes de usarla en C?

R/= Declarar el tipo de variable en C es clave porque le dice al programa cuánta memoria usar, qué valores puede almacenar y qué operaciones puede hacer. Esto evita errores raros, mejora el rendimiento y hace que el código sea más fácil de entender y mantener. Básicamente, ayuda a que el programa funcione bien y sin sorpresas.


## 4. Ejemplos adicionales de pseudocódigo y su traducción

**¡Importante!**

Estos ejemplos te ayudarán a ver la correspondencia entre el lenguaje natural del pseudocódigo y las instrucciones del lenguaje C. No te preocupes si no dominas todos los aspectos aún o si aún no conoces la sintaxis de C; lo importante es que veas cómo se transforman los pasos lógicos en sintaxis.

### Ejemplo 1: Encontrar el mayor de dos números

**Pseudocódigo**:

```
INICIO
    Leer num1
    Leer num2
    Si num1 > num2 Entonces
        Mostrar "El número 1 es mayor"
    Sino
        Mostrar "El número 2 es mayor"
FIN
```

**Lenguaje C**:

#include <stdio.h>

int main() {
    float num1, num2;

    printf("Ingresa el primer número: ");
    scanf("%f", &num1);
    printf("Ingresa el segundo número: ");
    scanf("%f", &num2);

    if (num1 > num2) {
        printf("El número 1 es mayor\n");
    } else {
        printf("El número 2 es mayor\n");
    }

    return 0;
}

Ejemplo 2: Calcular factorial de un número
Pseudocódigo:

```
INICIO
    Leer n
    factorial = 1
    Para i desde 1 hasta n
        factorial = factorial * i
    Mostrar factorial
FIN
```

**Lenguaje C**:

```c
#include <stdio.h>

int main() {
    int n;
    long factorial = 1;

    printf("Ingresa un número entero: ");
    scanf("%d", &n);

    for(int i = 1; i <= n; i++) {
        factorial *= i;
    }

    printf("El factorial es: %ld\n", factorial);

    return 0;
}
```
> Actividad
>
> - Escribe tu propio pseudocódigo para calcular el promedio de una lista de calificaciones y tradúcelo a C.

R/= Algoritmo Calificaciones

    Escribir "Ingrese la cantidad de calificaciones: "  

    Leer n  

    suma <- 0  

    Para i desde 1 hasta n hacer  

        Escribir "Ingrese la calificación ", i, ": "  

        Leer calificacion  

        suma <- suma + calificacion  

    Fin Para  

    promedio <- suma / n  

    Escribir "El promedio es: ", promedio 

FinAlgoritmo

LENGUAJE C: #include <stdio.h>

int main() {
    int n, i;
    float calificacion, suma = 0, promedio;

    printf("Ingrese la cantidad de calificaciones: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++) {
        printf("Ingrese la calificación %d: ", i);
        scanf("%f", &calificacion);
        suma += calificacion;
    }

    promedio = suma / n;
    printf("El promedio es: %.2f\n", promedio);

    return 0;
}


## 5. Buenas prácticas

1. **Comentarios**: Utiliza `/* comentario */` o `// comentario` para describir líneas clave.
2. **Funciones**: Divide tu código en funciones para mantenerlo ordenado.
3. **Convenciones de nombres**: Utiliza nombres descriptivos para variables y funciones.

> Pregunta orientadora
>
> - ¿Por qué es importante comentar el código, aunque sea breve y conciso?

R/= Comentar el código es importante porque ayuda a entender qué hace cada parte, facilita hacer cambios y encontrar errores rápido. También es útil cuando trabajas con otros programadores para que no se pierdan. Es una buena práctica porque hace que el código sea más claro y fácil de usar en el futuro.


## 6. Reto final

### Reto: toma el pseudocódigo de los 5 primeros ejercicios del Reto y realiza la traducción a C:

1. Revisa el pseudocódigo y verifica que no contenga errores.
2. **Traduce** ese pseudocódigo a C.
3. **Comenta** tu código para explicar los pasos principales.

1. 
R/= pseudocodigo:
inicio

   Escribir "Ingresa los datos deseados para X1

	definir X1 Como Entero

	Definir X2 Como Entero

	Definir Y1 Como Entero

	Definir Y2 Como Entero

	Leer X1

	Escribir "Ingresa el dato deseado para X2

	Leer X2

	Escribir "Ingresa el dato deseado para Y1

	Leer Y1

	Escribir "Ingresa el dato deseado para Y2

	Leer Y2
	
	diferencia_x = X2 - X1

    diferencia_y = Y2 - Y1
	
    D = sqrt(diferencia_x^2 + diferencia_y^2)
	
    Escribir "La distancia entre los dos puntos es:, D

Fin

Lenguaje en C: #include <stdio.h>
#include <math.h>  

int main() {
    int X1, X2, Y1, Y2;
    float D;

    printf("Ingresa el dato deseado para X1: ");
    scanf("%d", &X1);
    
    printf("Ingresa el dato deseado para X2: ");
    scanf("%d", &X2);
    
    printf("Ingresa el dato deseado para Y1: ");
    scanf("%d", &Y1);
    
    printf("Ingresa el dato deseado para Y2: ");
    scanf("%d", &Y2);

    D = sqrt(pow(X2 - X1, 2) + pow(Y2 - Y1, 2));

    printf("La distancia entre los dos puntos es: %.2f\n", D);

    return 0;
}



2. 
R/= Pseudocodigo: 

Algoritmo pulgadas

	Escribir "ingrese la cantidad de tela en metros"

	Leer metros

	pulgadas <- metros / 0.0254

	Escribir "debe pedir", pulgadas, "pulgadas de tela"

FinAlgoritmo

Lenguaje en C:  #include <stdio.h>

int main() {
    float metros, pulgadas;

    printf("Ingrese la cantidad de tela en metros: ");
    scanf("%f", &metros);

    pulgadas = metros / 0.0254;

    printf("Debe pedir %.2f pulgadas de tela.\n", pulgadas);

    return 0;
}

3. 
R/= Pseudocodigo:

Algoritmo TrianguloRectangulo

	Escribir "ingrese el valor del cateto A"

	Leer A

	Escribir "ingrese el valor del cateto B"

	leer B

	C <- Rc(A^2+B^2)

	Escribir "la hipotenusa es" C

FinAlgoritmo

Lenguaje en C: #include <stdio.h>
#include <math.h>  

int main() {
    float A, B, C;

    printf("Ingrese el valor del cateto A: ");
    scanf("%f", &A);

    printf("Ingrese el valor del cateto B: ");
    scanf("%f", &B);

    C = sqrt(pow(A, 2) + pow(B, 2));

    printf("La hipotenusa es: %.2f\n", C);

    return 0;
}

4. R/= Pseudocodigo:

Algoritmo EdadActual

		ESCRIBIR "Ingrese el día de nacimiento"

		LEER diaNac

		ESCRIBIR "Ingrese el mes de nacimiento"

		LEER mesNac

		ESCRIBIR "Ingrese el año de nacimiento"

		LEER añoNac

		ESCRIBIR "Ingrese el día actual"

		LEER diaAct

		ESCRIBIR "Ingrese el mes actual"

		LEER mesAct

		ESCRIBIR "Ingrese el año actual"

		LEER añoAct

		edad <- añoAct - añoNac

		SI (mesAct < mesNac) O (mesAct = mesNac Y diaAct < diaNac) ENTONCES

			edad <- edad - 1

			ESCRIBIR "Aún no ha cumplido años este año."

		SiNo

			ESCRIBIR "Ya cumplió años este año."

		FIN SI

		SI (mesAct = mesNac Y diaAct = diaNac) ENTONCES

			ESCRIBIR "Feliz Cumpleaños!"

		FinSi

		Imprimir "edad actual" edad

FinAlgoritmo

Lenguaje en C: #include <stdio.h>

int main() {
    int diaNac, mesNac, añoNac;
    int diaAct, mesAct, añoAct;
    int edad;

    printf("Ingrese el día de nacimiento: ");
    scanf("%d", &diaNac);

    printf("Ingrese el mes de nacimiento: ");
    scanf("%d", &mesNac);

    printf("Ingrese el año de nacimiento: ");
    scanf("%d", &añoNac);

    printf("Ingrese el día actual: ");
    scanf("%d", &diaAct);

    printf("Ingrese el mes actual: ");
    scanf("%d", &mesAct);

    printf("Ingrese el año actual: ");
    scanf("%d", &añoAct);

    edad = añoAct - añoNac;

    if (mesAct < mesNac || (mesAct == mesNac && diaAct < diaNac)) {
        edad--;
        printf("Aún no ha cumplido años este año.\n");
    } else {
        printf("Ya cumplió años este año.\n");
    }

    if (mesAct == mesNac && diaAct == diaNac) {
        printf("¡Feliz Cumpleaños!\n");
    }

    printf("Edad actual: %d años\n", edad);

    return 0;
}

5. R/= Pseudocodigo:

Algoritmo SueldoSemanal

	Escribir "Ingrese las horas trabajadas en la semana:"

    Leer horasTrabajadas

    Escribir "Ingrese el pago por hora:"

    Leer pagoPorHora

    Si horasTrabajadas > 50 Entonces

        Escribir "No está permitido trabajar más de 50 horas."

    Sino

        sueldo <- 0

	FinSi

        Si horasTrabajadas <= 40 Entonces

            sueldo <- horasTrabajadas * pagoPorHora

        Sino Si horasTrabajadas <= 45 Entonces

				sueldo <- (40 * pagoPorHora) + ((horasTrabajadas - 40) * (pagoPorHora * 2))

			Sino Si horasTrabajadas <= 50 Entonces

					sueldo <- (40 * pagoPorHora) + (5 * (pagoPorHora * 2)) + ((horasTrabajadas - 45) * (pagoPorHora * 3))

				FinSi

				Escribir "El sueldo semanal es: ", sueldo

			FinSi

	    FinSi

FinAlgoritmo

Lenguaje en C: #include <stdio.h>

int main() {
    int horasTrabajadas;
    float pagoPorHora, sueldo = 0;

    printf("Ingrese las horas trabajadas en la semana: ");
    scanf("%d", &horasTrabajadas);

    printf("Ingrese el pago por hora: ");
    scanf("%f", &pagoPorHora);

    if (horasTrabajadas > 50) {
        printf("No está permitido trabajar más de 50 horas.\n");
    } else {
        if (horasTrabajadas <= 40) {
            sueldo = horasTrabajadas * pagoPorHora;
        } else if (horasTrabajadas <= 45) {
            sueldo = (40 * pagoPorHora) + ((horasTrabajadas - 40) * (pagoPorHora * 2));
        } else if (horasTrabajadas <= 50) {
            sueldo = (40 * pagoPorHora) + (5 * (pagoPorHora * 2)) + ((horasTrabajadas - 45) * (pagoPorHora * 3));
        }

        printf("El sueldo semanal es: %.2f\n", sueldo);
    }

    return 0;
}

**Mensaje final**:
Traducir pseudocódigo a C implica **comprender la lógica** descrita en un lenguaje simple y llevarla a un **código C** con una estructura clara. Desarrollar esta habilidad te permitirá planificar proyectos, depurar problemas y comunicar ideas de programación de manera efectiva.

> Pregunta final
>
> - Después de este tutorial, ¿qué puntos crees que deberías reforzar para sentirte más seguro al traducir pseudocódigo a C?

R/= Los puntos que deberia reforzar es en donde hay que usar bien el printf y el scanf ya que hubo veces que no me funcionaba el codigo porque estas estaban mal puestas o porque no estaban, de resto me senti bastante comodo

