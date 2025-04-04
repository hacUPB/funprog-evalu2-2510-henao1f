RETOS

# Instrucciones

🔍 Para cada ejercicio, realice un análisis detallado y registre sus conclusiones en una tabla donde clasifique las variables de entrada, salida y las constantes. Enuncie las ecuaciones involucradas y explique el enfoque analítico que utilizará para plantear la solución.

1. Se requiere obtener la distancia entre dos puntos en el plano cartesiano,
tal y como se muestra en la figura 1. Realice un diagrama de flujo y pseudocódigo
que representen el algoritmo para obtener la distancia entre
esos puntos.

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

2. Una modista, para realizar sus prendas de vestir, encarga las telas al extranjero.
Para cada pedido, tiene que proporcionar las medidas de la tela
en pulgadas, pero ella generalmente las tiene en metros. Realice un algoritmo
para ayudar a resolver el problema, determinando cuántas pulgadas
debe pedir con base en los metros que requiere. Represéntelo mediante un
diagrama de flujo y pseudocódigo (1 pulgada = 0.0254 m).

R/= Pseudocodigo: 
```
Algoritmo pulgadas
	Escribir "ingrese la cantidad de tela en metros"
	Leer metros
	pulgadas <- metros / 0.0254
	Escribir "debe pedir", pulgadas, "pulgadas de tela"
FinAlgoritmo
```
     
3. Se requiere determinar la hipotenusa de un triángulo rectángulo. ¿Cómo sería el diagrama de flujo y el pseudocódigo que representen el algoritmo para obtenerla? 
Recuerde que por Pitágoras se tiene que: C^2 = A^2 + B^2.

R/= Pseudocodigo:
```
Algoritmo TrianguloRectangulo
	Escribir "ingrese el valor del cateto A"
	Leer A
	Escribir "ingrese el valor del cateto B"
	leer B
	C <- Rc(A^2+B^2)
	Escribir "la hipotenusa es" C
FinAlgoritmo
```

4. Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año.

R/= Pseudocodigo:
```
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
```

5. Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar
más de 50 horas no está permitido. Represente el algoritmo mediante pseudocódigo.

R/= Pseudocodigo:
```
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
```

6. Se requiere un algoritmo para determinar, de N cantidades, cuántas son cero, cuántas son menores a cero, y cuántas son mayores a cero.
Realice el pseudocódigo para representarlo, utilizando el ciclo apropiado.

R/= Pseudocodigo:
```
Algoritmo Cantidades
    Escribir "Ingrese la cantidad de números a evaluar (N):"
    Leer N
    ContadorCeros <- 0
	ContadorPositivos <- 0
	ContadorNegativos <- 0
	Para i <- 1 Hasta N Hacer
        Escribir "Ingrese un número:"
        Leer numero
        Si numero = 0 Entonces
            ContadorCeros <- ContadorCeros + 1
        Sino Si numero > 0 Entonces
				ContadorCerosPositivos <- ContadorCerosPositivos + 1
			Sino
				ContadorCerosNegativos <- ContadorCerosNegativos + 1
				FIN SI
		FinSi
	FinPara
		Escribir "Cantidad de ceros: ", ContadorCeros
		Escribir "Cantidad de números positivos: ", ContadorCerosPositivos
		Escribir "Cantidad de números negativos: ", ContadorCerosNegativos
FinAlgoritmo
```

7. Se requiere un algoritmo para determinar cuánto ahorrará en pesos una persona diariamente, y en un año, si ahorra 3¢ el primero de enero, 9¢ el dos de enero, 27¢ el 3 de enero y así sucesivamente todo el año. Represente la solución mediante pseudocódigo.

R/= Peudocodigo:
```
Algoritmo AHORRO
	Definir AhorroDiario como real
    Definir AhorroTotal como real
    Definir dia como entero
    AhorroDiario <- 0.03
    AhorroTotal <- 0
    dia <- 1
    Mientras dia <= 365 Hacer
        Mostrar "Día ", dia, ": ", AhorroDiario, " pesos"
        AhorroTotal <- AhorroTotal + AhorroDiario
        AhorroDiario <- AhorroDiario * 3
        dia <- dia + 1
    Fin Mientras
    Mostrar "El total ahorrado en un año es: ", AhorroTotal, " pesos"
FinAlgoritmo
```

8. Realice el algoritmo para determinar cuánto pagará una persona que adquiere N artículos, los cuales están de promoción. Considere que si su precio es mayor o igual a $200 se le aplica un descuento de 15%, y si su precio es mayor a $100, pero menor a $200, el descuento es de
12%; de lo contrario, solo se le aplica 10%. Se debe saber cuál es el costo y el descuento que tendrá cada uno de los artículos y finalmente cuánto se pagará por todos los artículos obtenidos. Represente la solución mediante pseudocódigo.

R/= Pseudocodigo:
```
Algoritmo Compras
    ESCRIBIR "Ingrese la cantidad de artículos a comprar: "
    LEER N
    TotalaPagar <- 0
    PARA i <- 1 HASTA N HACER
        ESCRIBIR "Ingrese el precio del artículo ", i, ": "
        LEER Precio
        SI Precio >= 200 ENTONCES
            Descuento <- Precio * 0.15
        SINO SI Precio >= 100 Y Precio < 200 ENTONCES
	        Descuento <- Precio * 0.12
	     SINO
		Descuento <- Precio * 0.10
       	     FIN SI
	fin si
	PrecioFinal <- Precio - DESCUENTO
		TotalaPagar <- TotalaPagar + PrecioFinal
		ESCRIBIR "Artículo ", i, ": Precio = ", Precio, ", Descuento = ", Descuento, ", Precio final = ", PrecioFinal
		FIN PARA
		ESCRIBIR "Total a pagar por todos los artículos: ", TotalaPagar
FinAlgoritmo
```

9. Realice un algoritmo y represéntelo mediante pseudocódigo para obtener una función exponencial, la cual está dada por:  
    $𝑒^𝑥 = 1+\frac x {1!} + \frac {x^2}{2!}+ \frac {x^3}{3!}+ …$

R/= Pseudocodigo
```
Algoritmo Exponencial
    ESCRIBIR "Ingrese el valor de x: "
    LEER x
    ESCRIBIR "Ingrese la cantidad de términos a considerar en la serie: "
    LEER n
    EX <- 1
    Termino <- 1
    PARA i <- 1 HASTA n - 1 HACER
        Termino <- (Termino * x) / i
        EX <- EX + Termino
    FIN PARA
    ESCRIBIR "La aproximación de e^", x, " usando ", n, " términos es: ", EX
FinAlgoritmo
```

10. Realice un algoritmo para obtener el seno de un ángulo y represéntelo mediante pseudocódigo. Utilice la siguiente ecuación:
    Sen x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + ...$

R/= Pseudocodigo
```
Algoritmo Trigonometrica
    ESCRIBIR "Ingrese el valor del ángulo en radianes: "
    LEER x
    ESCRIBIR "Ingrese la cantidad de términos a considerar en la serie: "
    LEER n
    SenX <- x  
    Termino <- x  
    Signo <- -1  
    PARA i <- 1 HASTA n - 1 HACER
        Exponente <- 2 * i + 1  
        Termino <- (Termino * x * x) / ((Exponente - 1) * Exponente)  
        SenX <- SenX + (Signo * Termino)  
        Signo <- -Signo  
    FIN PARA
    ESCRIBIR "La aproximación de Sen(", x, ") usando ", n, " términos es: ", SENX
FinAlgoritmo
```
