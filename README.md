# DESARROLLO DE SOFTWARE DESDE CERO

Este readme contiene parte de las actividades realizadas en el BOOTCAMP DE CORE-CODE DE DESARROLLO DE SOFTWARE.

## SEMANA I 

#### Lenguaje de programación compilado vs lenguaje de programación interpretado. 

> Un lenguaje compilado es un lenguaje de programación cuyas implementaciones son normalmente compiladores (traductores que generan código de máquina a partir del código fuente) y no intérpretes (ejecutores paso a paso del código fuente, donde no se lleva a cabo una traducción en la preejecución).

> Un lenguaje interpretado es un lenguaje de programación para el que la mayoría de sus implementaciones ejecuta las instrucciones directamente, sin una previa compilación del programa a instrucciones en lenguaje máquina.

#### ¿Java está compilado o interpretado, o ambos?

> El lenguaje Java es a la vez compilado e interpretado. Con el compilador se convierte el código fuente que reside en archivos cuya extensión es . java, a un conjunto de instrucciones que recibe el nombre de bytecodes que se guardan en un archivo cuya extensión es . class.

### Conversor de divisas en pseudocódigo

#### Descripción

Has sido seleccionado para desarrollar el algoritmo que se utilizará para convertir dólares (USD) a bitcoin (BTC), para ello lo primero que debes hacer es entregar un pseudocódigo con el algoritmo a desarrollar, de esta forma podrás explicarlo en una mejor manera para el equipo lo que será la operación requerida. La idea principal es tener un sitio web donde se le pedirá al usuario que ingrese la cantidad a convertir.

1. INICIO.
2. INGRESE MONTO.
3. VALOR DEL BTC.
4. OPERACION (MONTO * VALOR BTC)
5. MOSTRAR RESULTADO DE LA OPERACION
6. FIN

### Lenguaje de alto y bajo nivel.

> Un lenguaje de bajo nivel es trasladado fácilmente a lenguaje de máquina (la palabra bajo se refiere a la abstracción reducida entre el lenguaje y el hardware). Y los lenguajes de programación de **alto nivel se caracterizan por expresar los programas de una manera sencilla.**

#### Lenguajes de alto nivel

Son aquellos que se encuentran mas cercanos al lenguaje natural que al lenguaje maquina. Están dirigidos a solucionar problemas mediante el uso de Estructuras Dinámicas de Datos.

Se tratan de lenguajes independientes de la arquitectura del ordenador. Por lo que, en principio, un programa escrito en un lenguaje de alto nivel, lo puedes migrar de una maquina a otra sin ningún tipo de problema.

Estos lenguajes permiten al programador olvidarse por completo del funcionamiento interno de la maquina/s para la que están diseñando el programa. Tan solo necesitan un traductor que entiendan el código fuente como las características de la maquina.

Suelen usar tipos de datos para la programación y hay lenguajes de propósito general (cualquier tipo de aplicación) y de propósito especifico (como FORTRAN para trabajos científicos).

> Los típicos lenguajes mas usados son : Java, C#, Python, JavaScript.

#### Lenguajes de medio nivel

Lenguaje de medio nivel es un lenguaje de programación como el lenguaje C, que se encuentran entre los lenguajes de alto nivel y los lenguajes de bajo nivel.

Suelen ser clasificados muchas veces de bajo nivel, pero permiten ciertos manejos de alto nivel. Son precisos para ciertas aplicaciones como la creación de sistemas operativos, ya que permiten un manejo abstracto (independiente de la maquina, a diferencia del ensamblador), pero sin perder mucho del poder y eficiencia que tienen los lenguajes de bajo nivel.

Una característica distintiva, por ejemplo, que convierte a C en un lenguaje de medio nivel y al Pascal en un lenguaje de alto nivel es que en el primero es posible manejar las letras como si fueran números (en Pascal no), y por el contrario en Pascal es posible concatenar las cadenas de caracteres con el operador suma y copiarlas con la asignación (en C es el usuario el responsable de llamar a las funciones correspondientes).

Una de las características mas peculiares del lenguaje de programación C; es el uso de “apuntadores”, los cuales son muy útiles en la implementación de algoritmos como Listas ligadas, Tablas Hash y algoritmos de búsqueda y ordenamiento que para otros lenguajes de programación (como Java por ejemplo) les suele ser un poco mas complicado implementar.

> Los típicos lenguajes mas usados son : C, C++.

#### Lenguajes de bajo nivel

Son lenguajes totalmente dependientes de la maquina, es decir que el programa que se realiza con este tipo de lenguajes no se pueden migrar o utilizar en otras maquinas.

Al estar prácticamente diseñados a medida del hardware, aprovechan al máximo las características del mismo.

Dentro de este grupo se encuentran:

> El lenguaje maquina: este lenguaje ordena a la maquina las operaciones fundamentales para su funcionamiento. Consiste en la combinación de 0’s y 1’s para formar las ordenes entendibles por el hardware de la maquina. Este lenguaje es mucho mas rápido que los lenguajes de alto nivel.
>
> El lenguaje ensamblador es un derivado del lenguaje maquina y esta formado por abreviaturas de letras y números llamadas. Con la aparición de este lenguaje se crearon los programas traductores para poder pasar los programas escritos en lenguaje ensamblador a lenguaje maquina. Como ventaja con respecto al código maquina es que los códigos fuentes eran mas cortos y los programas creados ocupaban menos memoria.
>> Generaciones
>>- **Primera generación:** lenguaje maquina.
>>- **Segunda generación:** se crearon los primeros lenguajes ensambladores.
>>- **Tercera generación:** se crean los primeros lenguajes de alto nivel. Ej. C#, Pascal, Cobol
>>- **Cuarta generación:** son los lenguajes capaces de generar código por si solos, son los llamados RAD.
>>- **Quinta generación:** aquí se encuentran los lenguajes orientados a la inteligencia artificial.
>>> Aclaraciones
>>> En la actualidad, se suele omitir los lenguajes de medio nivel, quedando asi los grupos:
>>>
>>> Alto Nivel -> Java, C#, Python, JavaScript
>>>
>>> Bajo Nivel -> C, C++


## SEMANA II 

### Ejericicio I - MULTIPLICAR 

Cree una función que logre multiplicar dos valores.



    const  multiply= (a, b)=> a * b;
    multiply(5,2)// 10
 

### Ejercicio II - TOTAL ASCII

Se le dará una cadena y tendrá que devolver la suma de todos los caracteres como un int. La función debería poder manejar todos los caracter

    function uniTotal (string) {
    let total = []
    if ( string.length === 0) return 0;
    for ( let i = 0; i < string.length; i++){
    total.push(string.charCodeAt(i))
    }
    return total.reduce((a,b)=>a + b,0)
    } 
    
    uniTotal()