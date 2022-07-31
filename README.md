# DESARROLLO DE SOFTWARE DESDE CERO

Este readme contiene parte de las actividades realizadas en el BOOTCAMP DE CORE-CODE DE DESARROLLO DE SOFTWARE.

## SEMANA I 

#### Lenguaje de programación compilado vs lenguaje de programación interpretado. 

> Un lenguaje compilado es un lenguaje de programación cuyas implementaciones son normalmente compiladores (traductores que generan código de máquina a partir del código fuente) y no intérpretes (ejecutores paso a paso del código fuente, donde no se lleva a cabo una traducción en la preejecución).

> Un lenguaje interpretado es un lenguaje de programación para el que la mayoría de sus implementaciones ejecuta las instrucciones directamente, sin una previa compilación del programa a instrucciones en lenguaje máquina.

![tipos de programación](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQqJzHvV0u1RY1X0xjY2fJndsCBEL14-eWapw&usqp=CAU) 

![imagen explicativa](https://www.google.com/imgres?imgurl=https%3A%2F%2Fwww.cursosgis.com%2Fwp-content%2Fuploads%2F4-97.jpg&imgrefurl=https%3A%2F%2Fwww.cursosgis.com%2Fque-preguntas-hacer-para-saber-que-estan-contratando-a-un-verdadero-desarrollador-python%2F&tbnid=TU2rkHqVtVsoEM&vet=12ahUKEwjX_oPG9qH5AhVoM7kGHb6rDwEQMygTegUIARDmAQ..i&docid=HBkTJMg8jeFL4M&w=712&h=402&q=lenguaje%20de%20programaci%C3%B3n%20compilado&ved=2ahUKEwjX_oPG9qH5AhVoM7kGHb6rDwEQMygTegUIARDmAQ)


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