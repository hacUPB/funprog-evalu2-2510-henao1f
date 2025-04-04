1-¿Qué es un computador?
Un computador es una máquina electrónica que está diseñada para realizar tareas específicas. En muchos países se le conoce como computadora u ordenador, pero todas estas palabras se refieren a lo mismo.

Con esta máquina se pueden desarrollar tareas que ahora hacen parte de nuestra vida cotidiana, como elaborar cartas o una hoja de vida, hablar con personas de otros países, hacer presupuestos, jugar y hasta navegar en internet.

Nuestro computador hace esto, procesando datos para convertirlos en información útil para nosotros.

https://edu.gcfglobal.org/es/informatica-basica/que-es-un-computador/1/

![compa](./imágenes/computador.jpg)

2-Lo que sucede en CISC es que se reduce la cantidad de instrucciones de un software y se ignora el número de ciclos por instrucción. Se especializa en crear instrucciones complejas en el hardware, ya que el hardware siempre será mucho más rápido que el software.

Este tipo de diseño es la base de los procesadores de Intel y de AMD, sin importar la gama o la estructura interna. Cualquiera de los procesadores producidos por ambas compañías se basan en la arquitectura CISC.

Características de los procesadores CISC

El tamaño del código es pequeño, lo que implica una baja necesidad de memoria RAM
Las instrucciones complejas suelen necesitar más de un ciclo de reloj para ejecutar el código
Se requieren menos instrucciones para escribir un software
Ofrece programación más sencilla en lenguaje ensamblador
Soporte para una estructura de datos compleja y fácil de compilar en lenguajes de alto nivel
Compuesto por menos registros y más nodos de direccionamiento, habitualmente entre 5 y 20
Instrucciones pueden ser más grandes que una sola palabra
Se enfatiza la construcción de instrucciones en el hardware, ya que es más rápido que crear el software

Ventajas de los procesadores CISC

Para el compilador se requiere de poco esfuerzo para traducir programas de alto nivel o lenguajes de instrucciones a lenguaje ensamblador o máquina
El tamaño del código es corto, reduciendo los requisitos de memoria
Almacenar las instrucciones CISC requieren de menos cantidad de memoria RAM
Genera procesos de administración de uso de energía que permiten ajustar la velocidad y el voltaje del reloj
Requiere de menos instrucciones configuradas para realizar la misma instrucción que la arquitectura RISC
Desventajas de los procesadores CISC
Pueden requerir de varios ciclos de reloj para completar una instrucción de un software
El rendimiento del equipo sufre un descenso debido a la velocidad del reloj
La ejecución mediante canalización en procesadores CISC puede ser realmente complicado
Este diseño de procesadores requiere muchos más transistores que la arquitectura RISC
Utilizan sobre el 20% de las instrucciones existentes en un evento de programación
Tienen un diseño mucho mayor que la arquitectura RISC, lo cual conlleva más generación de temperatura, mayor consumo y mayor requisito de espacio físico

-La arquitectura RISC tiene la capacidad de por cada ciclo de instrucción se da solo un ciclo de reloj. Cada ciclo debe contener estos tres parámetros: buscar, decodificar y ejecutar. RISC también tiene la propiedad de ejecutar varias instrucciones complejas cuando se combinan con otras más simples. Este diseño de procesadores requiere menor cantidad de transistores, reduciendo costes y tiempos de fabricación.

Todos los procesadores basados en los diseños de ARM, como por ejemplo los Qualcomm Snapdragon y los Samsung Exynos se basan en la arquitectura RISC. Incluso los procesadores integrados en las Raspberry Pi son de arquitectura RISC, al basarse en procesadores Broadcom que hace uso de licencias ARM.

Características de RISC

Para ejecutar una instrucción en estos procesadores, en un procesador de este tipo se requiere un ciclo de reloj. Cada ciclo de reloj incluye un método de obtención, decodificación y ejecución de la instrucción
La técnica de canalización se usa en esta arquitectura para ejecutar múltiples partes o etapas de instrucciones para obtener un funcionamiento más eficiente
Estos procesadores están optimizados basándose en múltiples registros que se pueden usar para el almacenamiento de instrucciones y la respuesta rápida del procesador y se minimicen las interacciones con la memoria del sistema
Soporta un modo de direccionamiento simple y que tiene una longitud de instrucción fija para la ejecución de la canalización
Usan instrucciones LOAD y STORE para acceder a la memoria
Las instrucciones simples y limitadas permiten reducir los tiempos de ejecución de un proceso

Ventajas de los procesadores RISC

Tienen la capacidad de ofrecer un mejor rendimiento gracias al menor número de instrucciones y la simplicidad de las mismas
Requieren de menos transistores, lo cual los hace más económicos de diseñar y producir
Permiten crear procesadores con «espacio» libre para añadir otros circuitos o reducir sencillamente el encapsulado
Este diseño requiere de menos consumo de energía y generan menos calor que los procesadores RISC
Desventajas de los procesadores RISC
El rendimiento del procesador puede variar dependiendo del código que se ejecuta, ya que las instrucciones posteriores que se ejecuten pueden depender de una instrucción anterior
Actualmente la mayoría de software y compiladores hacen uso de instrucciones complejas
Necesitan de memorias muy rápidas para almacenar diferentes cantidades de instrucciones, que requieren de una gran cantidad de memoria caché para responder a la instrucción en el menor tiempo posible

https://www.profesionalreview.com/2021/07/18/risc-vs-cisc/#Que_es_CISC

![imagen2](./imágenes/RISC.jpg)

3-¿Qué es el hardware? 

El hardware son los componentes físicos de un ordenador, como la placa base, el procesador, la memoria, las unidades de almacenamiento y otros dispositivos. Es el hardware que aloja y soporta el software o los programas que proporcionan instrucciones para que el ordenador complete sus tareas. El hardware también puede incluir dispositivos externos de entrada/salida como teclados, ratones, monitores, impresoras y altavoces.

El hardware existe desde la invención de los ordenadores. Los primeros componentes de hardware estaban hechos de piezas mecánicas básicas e interruptores, como la Máquina Diferencial de Charles Babbage en 1822. A mediados del siglo XX, el hardware se basaba principalmente en la tecnología de tubos de vacío, que acabó dando paso a los transistores a finales de los años 50 y principios de los 60. Hoy en día, el hardware se utiliza ampliamente en todo tipo de sistemas y dispositivos informáticos, desde ordenadores de sobremesa y portátiles hasta smartphones y smartwatches.

Placa base: Es la placa de circuito principal que aloja y conecta todos los componentes de un ordenador, tales como el procesador, la memoria, las unidades de almacenamiento y otros dispositivos.

Procesador: El componente de hardware que procesa los datos y ejecuta las instrucciones. Puede incluir múltiples núcleos, que son componentes de hardware específicamente diseñados para ejecutar varios programas de software simultáneamente.

Memoria: Hardware que almacena datos temporalmente para su uso por el procesador. Puede incluir tanto memoria de acceso aleatorio (RAM), que se utiliza para tareas a corto plazo, como memoria de sólo lectura (ROM).

Unidades de almacenamiento: Dispositivos de hardware que almacenan datos de forma permanente, como discos duros, unidades de estado sólido (SSD) y discos ópticos. Cada componente de hardware desempeña un papel vital en los sistemas de hardware de los ordenadores modernos, permitiéndoles realizar sus diversas tareas de forma eficiente y eficaz.

Impresoras: dispositivos de hardware que permiten a los usuarios producir copias físicas de documentos, fotografías y otros tipos de soportes.

https://www.arimetrics.com/glosario-digital/hardware

![hard](./imágenes/hardware.jpg)

4.¿Qué es un software?

El término software es un vocablo inglés que fue tomado por otros idiomas y designa a todo componente intangible (y no físico) que forma parte de dispositivos como computadoras, teléfonos móviles o tabletas y que permite su funcionamiento.

El software está compuesto por un conjunto de aplicaciones y programas diseñados para cumplir diversas funciones dentro de un sistema. Además, está formado por la información del usuario y los datos procesados.

Los programas que forman parte del software le indican al hardware (parte física de un dispositivo), por medio de instrucciones, los pasos a seguir.

Softwares de sistema: Programas que dan al usuario la capacidad de relacionarse con el sistema, para ejercer control sobre el hardware. El software de sistema también se ofrece como soporte para otros programas. Por ejemplo: sistemas operativos o servidores.

Softwares de programación: Programas diseñados como herramientas que le permiten a un programador desarrollar programas informáticos. Se valen de técnicas y un lenguaje de programación específico. Por ejemplo: compiladores o editores multimedia.

Softwares de aplicación: Programas diseñados para realizar una o más tareas específicas a la vez, pueden ser automáticos o asistidos. Por ejemplo: videojuegos o reproductores multimedia.

https://concepto.de/software/
![software](./imágenes/software.jpg)

5-funcionamiento del computador

Pasos para arrancar un PC

Inicialización de la fuente de alimentación. En el momento en que apretamos el botón de arranque de la caja, se cierra un contacto. Este contacto se recibe como señal de arranque por parte de la placa base, la cual manda orden a la fuente de alimentación para que se active.

Inicialización del procesador. Con la fuente en marcha y suministrando energía eléctrica a todos los componentes, el primero de ellos que comienza a funcionar es el procesador. Como sabréis, los procesadores tienen su propio sistema de diagnóstico interno. Este software (el Management Engine de Intel, o el AGESA de AMD) es el que se encarga de comprobar que los parámetros de funcionamiento son los indicados para el componente. En caso de detectar algún parámetro no correcto, inmediatamente detiene todo el proceso de arranque del equipo.

Arranque de la placa base. Dado que todo el hardware del PC está conectado a la placa base, es imprescindible que esta esté inicializada para que el procesador pueda comunicarse con el resto de las componentes.

Comprobación de la memoria RAM. Si el test del procesador ha sido satisfactorio, el siguiente componente en comprobarse es la RAM del sistema. Lo primero que va a comprobar es si hay RAM en el equipo. Luego, si está correctamente insertada en sus ranuras. En caso de no estar correctamente insertada, el arranque se detendrá.

Arranque de todos los buses primarios y secundarios: aunque puede considerarse un apartado de la propia placa base, lo cierto es que merece especial mención porque actualmente la cantidad de buses es abrumadora. Hasta tal punto que muchos de ellos cuando se detecta fallo impiden el avance del POST. Lo normal es que esto no ocurra, pero…

Arranque de la tarjeta gráfica. Exactamente al igual de lo sucedido con el procesador, se procede a la comprobación de la tarjeta gráfica. Independientemente de si esta es dedicada o integrada. Hace bastantes años solía salir unas letras que indicaban el modelo de tarjeta gráfica que teníamos en nuestro sistema. Pero ya hace años que ya no se usan.

Monitorización de las unidades de almacenamiento. Tras la comprobación de la gráfica se testan los discos duros y SSD conectados directamente a la placa base. Si uno de ellos tiene problemas al inicializarse, el proceso de arranque se ralentizará muchísimo. Dado que la BIOS de la placa base va a intentar seguir arrancándolo siempre. Y no va a poder pasar a los pasos siguientes.

Comprobación de las tarjetas de expansión. Una vez que se han comprobado las unidades de almacenamiento, es cuando se comprueban el resto de tarjetas de expansión que tenemos conectadas a la placa base. Es por ello que es, entonces, cuando salen las letras relacionadas con las tarjetas para RAID de discos duros/SSD (en caso de tener uno configurado en la placa).
Finaliza el P.O.S.T. Es decir, ya se ha iniciado y completado la fase de arrancar el ordenador.

Se inicia la GUI de la BIOS/UEFI de la placa base. Aunque la placa base ha estado inicializada desde casi el comienzo del arranque, es solo en este punto cuando nos saldrá el logo del fabricante de la placa (si no lo tenemos desactivado, claro). Esto nos indicará que ya se habrá cargado la interfaz gráfica de usuario (GUI, Graphical User Interface) con la que podremos interactuar con los parámetros internos de ella.

Carga del sistema operativo. Una vez todos los componentes se han inicializado, la BIOS de la placa da luz verde al disco de arranque donde se encuentra almacenado el sistema operativo, en el caso de tenerlo instalado. En el caso de usar Microsoft Windows como sistema, la tarea queda en manos del Bootloader, que ya se encargará de ir cargando todos los componentes de ese sistema, hasta llegar al escritorio de Windows.
https://hardzone.es/tutoriales/montaje/arrancar-ordenador/

Entrada de datos (teclado):

Cuando presionas una tecla, esta genera una señal eléctrica que es convertida en un código que representa esa tecla. El teclado está conectado a una controladora de teclado, que envía estos códigos al procesador de la computadora.
Procesamiento de la información (CPU):

La señal (código) del teclado es enviada al procesador central (CPU) de la computadora, que interpreta los datos. El procesador es el "cerebro" de la computadora, donde ocurre la ejecución de las instrucciones. El procesador, a través de una unidad de control, interpreta los datos y los convierte en instrucciones que se ejecutan.
Si, por ejemplo, es una operación matemática o un comando, el procesador llevará a cabo esas operaciones usando su unidad aritmético-lógica (ALU), que realiza los cálculos.
Comunicación con la memoria:

Para realizar las operaciones o almacenar datos temporales, el procesador usa la memoria RAM (memoria de acceso aleatorio), que es donde se guardan los datos en ejecución. La CPU puede acceder a la RAM para leer o escribir los valores necesarios.
Generación de la salida (pantalla):

Una vez que el procesador termina de ejecutar las operaciones, el resultado se prepara para ser mostrado en la pantalla.
El procesador envía este resultado a la tarjeta gráfica (GPU) si se requiere mostrar gráficos complejos o a un controlador de pantalla para simplemente mostrar texto.
La tarjeta gráfica toma los datos y los traduce a señales eléctricas específicas para controlar los píxeles en la pantalla. Si es una operación sencilla, el controlador de pantalla se encarga directamente de gestionar la visualización del texto o número.
Visualización del resultado (pantalla):

Finalmente, la pantalla recibe las señales de la tarjeta gráfica o del controlador, que iluminan los píxeles correspondientes para mostrar el resultado de la operación. Esto se logra mediante el control preciso de los colores y la disposición de los píxeles en la pantalla, creando la imagen que ves.
https://support.kaspersky.com/kis/2017/es-MX/70895.htm

Los datos por lo general son una mezcla de
tipos.

Se utiliza una representación Uniforme de todos
los tipos de datos.

Los datos de entrada a una computadora se
transforman en la representación uniforme al ser
utilizados y almacenados por la PC.

A esta representación uniforme o formato
universal se le llama PATRÓN DE BITS.
https://www.uv.mx/personal/llopez/files/2011/09/Herencia-de-Ciencias.pdf
![bit](./imágenes/bit.jpg)

¿Cuáles son las unidades de medida de datos en un computador?

Las unidades de medida más usadas son el Bit, Byte, Kilobyte, Megabyte, Gigabyte y Terabyte.

Para que entiendas cómo se relacionan estas unidades de medida entre sí, imagina esto:
Tienes un libro muy grande, y una sola letra de ese libro representa un Byte. Esta letra está compuesta por (8) ocho partes y cada una de esas partes se llama Bit.

Si juntas varias letras (bytes) formarías palabras, y con las palabras un párrafo, que aquí contaría como un Kilobyte.

Con varios párrafos (Kilobytes) podrías conformar algunas páginas del libro, lo que podría ser un Megabyte.

Y uniendo todas las páginas (megabytes), tendrías el libro completo, que puedes imaginar que es Gigabyte.

Si unes ese libro a muchos otros libros (Gygabytes), tendrías una gran biblioteca que, en este caso, equivaldría a un Terabyte.

Bit:
Es la unidad mínima de información empleada en informática.

Byte (B):
Equivale a 8 bits. Con dos bytes guardas o procesas una letra.

Kilobyte (kB):
1024 bytes forman un Kilobyte.

Megabyte (MB):
Equivale a 1024 Kilobytes.

Gigabyte (GB):
Es igual a 1024 Megabytes. Es la unidad de medida que se suele usar para determinar la capacidad de almacenamiento de las USB.

Terabyte (TB):
Lo componen 1024 Gigabytes. Muchas veces esta medida determina la capacidad de almacenamiento de los discos duros. ¡Imagina la cantidad de archivos que podrías guardar!
https://edu.gcfglobal.org/es/cultura-tecnologica/medidas-de-almacenamiento-de-informacion/1/
![bits](./imágenes/bits.jpg)

.
