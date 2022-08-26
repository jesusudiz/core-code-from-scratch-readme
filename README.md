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

### Ejericicio : MULTIPLICAR 

Cree una función que logre multiplicar dos valores.



    const  multiply= (a, b)=> a * b;
    multiply(5,2)// 10
 

### Ejercicio:  TOTAL ASCII

Se le dará una cadena y tendrá que devolver la suma de todos los caracteres como un int. La función debería poder manejar todos los caracter

    function uniTotal (string) {
    let total = []
    if ( string.length === 0) return 0;
    for ( let i = 0; i < string.length; i++){
    total.push(string.charCodeAt(i))
    }
    return total.reduce((a,b)=>a + b,0)
    } 
    
    uniTotal("aaa") // 291
    
    
 ### Ejercicio : Obtener carácter de valor ASCII
 
 Escriba una función get_char()/ getChar()que tome un número y devuelva el carácter ASCII correspondiente a ese valor.
 Ejemplo:
 *  get_char(65) //debe regresar: "A"
      
 Respuesta:
 
     function getChar(c){
     return String.fromCharCode(c)
     }

### Ejercicio: Adición binaria
Implemente una función que sume dos números y devuelva su suma en binario. La conversión se puede hacer antes o después de la adición.

El número binario devuelto debe ser una cadena.

Ejemplos:(Entrada1, Entrada2 --> Salida (explicación)))

* 1, 1 --> "10" (1 + 1 = 2 in decimal or 10 in binary)
* 5, 9 --> "1110" (5 + 9 = 14 in decimal or 1110 in binary)

Respuesta:

    function addBinary(a,b) {
    return (a + b).toString(2)
    }
    
### Ejercicio: Calificación final del Estudiante

Cree una función notaFinal, que calcule la nota final de un estudiante en función de dos parámetros: una nota para el examen y una cantidad de proyectos completados.

Esta función debe tomar dos argumentos: examen - calificación del examen (de 0 a 100); proyectos - número de proyectos completados (de 0 en adelante);

Esta función debería devolver un número (calificación final). Hay cuatro tipos de calificaciones finales:

100, si la calificación del examen es superior a 90 o si el número de proyectos terminados es superior a 10.
90, si la calificación del examen es superior a 75 y si el número de proyectos completados es mínimo 5.
75, si la calificación del examen es superior a 50 y si el número de proyectos completados es mínimo 2.
0, en otros casos

Ejemplos ( Entradas --> Salida ):

* 100, 12 --> 100
* 99, 0 --> 100
* 10, 15 --> 100
* 85, 5 --> 90
* 55, 3 --> 75
* 55, 0 --> 0
* 20, 2 --> 0
*Utiliza Operadores Lógicos y de Comparación.

Respuesta:

    function finalGrade (exam, projects) {
     return  exam > 90 || projects > 10 ? 100 :
             exam > 75 && projects >= 5 ? 90 :
             exam > 50 && projects >= 2 ? 75 : 0
         }

### Ejercicio:Serie de signos de exclamación n.º 2: elimine todos los signos de exclamación del final de la oración

Elimina todos los signos de exclamación del final de la oración.
Ejemplos:

* remove("Hi!") === "Hi"
* remove("Hi!!!") === "Hi"
* remove("!Hi") === "!Hi"
* remove("!Hi!") === "!Hi"
* remove("Hi! Hi!") === "Hi! Hi"
* remove("Hi") === "Hi"

Respuesta: 

    function * remove (string) {  
     return string.replace(/!+$/, '');
    }

### Ejercicio: Eliminador de vocales
Cree una función llamada shortcutpara eliminar las vocales minúsculasa ( , e, i, o, u) en una cadena determinada.

Ejemplos:

* "hello"     -->  "hll"
* "codewars"  -->  "cdwrs"
* "goodbye"   -->  "gdby"
* "HELLO"     -->  "HELLO"

Respuesta:

  rfunction shortcut(string) {
  return string.replace(/[aeiou]/g, '');
}
### Ejercicio: Piedra Papel tijeras
¡Vamos a jugar! ¡Tienes que devolver qué jugador ganó! En caso de empate devolución Draw!.

Ejemplos (Entrada1, Entrada2 --> Salida):

* "scissors", "paper" --> "Player 1 won!"
* "scissors", "rock" --> "Player 2 won!"
* "paper", "paper" --> "Draw!"

Respuesta:

    const rps = (p1, p2) => {
  
     return( (p1 ==="scissors" && p2 ==="paper")? 'Player 1 won!':
        (p1 ==="paper" && p2 ==="rock")? 'Player 1 won!':
        (p1 ==="rock" && p2 ==="scissors")? 'Player 1 won!':
        (p1 ==="scissors" && p2 ==="rock")? "Player 2 won!":
        (p1 ==="rock" && p2 ==="paper")? "Player 2 won!": 
        (p1 ==="paper" && p2 ==="scissors")? "Player 2 won!":
        (p1 === p2 )? "Draw!":false)
    }
### Ejercicio: Bugger persistente.
Escribe una función, persistence, que tome un parámetro positivo numy devuelva su persistencia multiplicativa, que es el número de veces que debes multiplicar los dígitos num hasta llegar a un solo dígito.

Por ejemplo (Entrada --> Salida) :

* 39 --> 3 (because 3*9 = 27, 2*7 = 14, 1*4 = 4 and 4 has only one digit)
* 999 --> 4 (because 9*9*9 = 729, 7*2*9 = 126, 1*2*6 = 12, and finally 1*2 = 2)
* 4 --> 0 (because 4 is already a one-digit number)

Respuesta:

    function persistence(num) {
     let times = 0;
     num = num.toString();
         while (num.length > 1) {
          times++;
         num = num
        .split('')
        .map((a) => Number(a))
        .reduce((a, b) => a * b)
        .toString();
         }
    return times;
    }



### Ejercicio: Vacaciones VIII - Libre de impuestos

El propósito de este kata es calcular cuántas botellas de whisky libre de impuestos tendrías que comprar para que el ahorro sobre el precio normal de la calle cubra efectivamente el costo de tus vacaciones.

Se le dará el precio de venta al público (NormPrice), el descuento libre de impuestos (descuento) y el costo de las vacaciones.

Por ejemplo, si una botella cuesta normalmente 10€ y el descuento en el duty free es del 10%, ahorrarías 1€ por botella. Si sus vacaciones costaron £500, la respuesta que debe devolver sería 500.

Todas las entradas serán números enteros. Por favor, devuelva un número entero. Redondear a la baja.

Respuesta:

    function dutyFree(normPrice, discount, hol) {
  return Math.floor(hol / ((discount * normPrice) / 100));
}
### Ejercicio: El doble de viejo

Su función toma dos argumentos:

* edad del padre actual (años)
* edad actual de su hijo (años)

Calcula cuántos años hace que el padre tenía el doble de la edad de su hijo (o dentro de cuántos años tendrá el doble).


Respuesta:

   function twiceAsOld(dadYearsOld, sonYearsOld) {
   let calculo=(sonYearsOld*2)-dadYearsOld
   return Math.abs(calculo)
   }


### Ejercicio:  Espaciado válido    
Su tarea es escribir una función llamada valid_spacing()o validSpacing() que verifique si una cadena tiene un espacio válido. La función debe devolver trueo false(o el valor correspondiente en cada idioma).

Para este kata, la definición de espaciado válido es un espacio entre palabras, sin espacios iniciales ni finales. Las palabras pueden ser cualquier secuencia consecutiva de caracteres sin espacio. A continuación se muestran algunos ejemplos de lo que debe devolver la función:

Respuesta:

    function validSpacing(s) {
  if (s.length === 0) return true;
  if (s[0] === ' ' || s[s.length - 1] === ' ') return false;
  let aSpaces0 = s.split(' ');
  for (let i = 0, length = aSpaces0.length; i < length; i++) {
    if (aSpaces0[i] === '') return false;
  }
  return true;
}
### Ejercicio: Binario Falso

Dada una cadena de dígitos, debe reemplazar cualquier dígito debajo de 5 con '0' y cualquier dígito 5 y superior con '1'. Devuelve la cadena resultante.

Respuesta:
   
    function fakeBin(x) {
    return x.split('').map(n => n < 5 ? 0 : 1).join('');
    }



 ## SEMANA 3   
### Ejercicio: ¿A quién le gusta?

Probablemente conozcas el sistema de "me gusta" de Facebook y otras páginas. Las personas pueden "gustar" publicaciones de blog, imágenes u otros elementos. Queremos crear el texto que debe mostrarse junto a dicho elemento.

Implemente la función que toma una matriz que contiene los nombres de las personas a las que les gusta un artículo. Debe devolver el texto de la pantalla como se muestra en los ejemplos:

* []                                -->  "no one likes this"
* ["Peter"]                         -->  "Peter likes this"
* ["Jacob", "Alex"]                 -->  "Jacob and Alex like this"
* ["Max", "John", "Mark"]           -->  "Max, John and Mark like this"
* ["Alex", "Jacob", "Mark", "Max"]  -->  "Alex, Jacob and 2 others like this"

Respuesta:

    function likes(names) {
  
     if ( names.length === 0) return `no one likes this`;
     if ( names.length === 1) return `${names[0]} likes this`;
     if ( names.length === 2) return`${names[0]} and ${names[1]} like this`;
     if ( names.length ===3) return `${names[0]}, ${names[1]} and ${names[2]} like this`;
     if ( names.length >= 4) return `${names[0]}, ${names[1]} and ${names.length - 2} others like this`;

    }
### Ejercicio:
Respuesta:
### Ejercicio:
Respuesta:

### Ejercicio:
Respuesta:
### Ejercicio:
Respuesta:
### Ejercicio:
Respuesta: