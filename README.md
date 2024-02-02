![Logo](https://blog.logrocket.com/wp-content/uploads/2023/12/nesting-web-components-vanilla-javascript.png)

# JavaScript Fundamentals

Let's learn the basics of building code.

####

#### 1. [Hello, world!](#hello-world)

#### 2. [Code structure](#code-structure)

#### 3. [The modern "use strict" mode](#the-modern-use-strict-mode)

#### 4. [Variables](#variables)

#### 5. [Types of data](#types-of-data)

#### 6. [Interaction: alert, prompt, confirm](#interaction-alert-prompt-confirm)

#### 7. [Type Conversions](#type-conversions)

#### 8. [Basic operators, mathematics](#basic-operators-mathematics)

#### 9. [Comparisons](#comparisons)

#### 10. Conditional execution if (#conditional-execution-if)

#### 11. [Logical Operators](#logical-operators)

#### 12. [Operador Nullish Coalescing '??'](#operador-nullish-coalescing)

#### 13. [Bucles: while y for](#bucles-while-y-for)

#### 14. [The "switch" statement](#the-switch-statement)

#### 16. [Functions](#functions)

#### 16. [Function expressions](#function-expressions)

#### 17. [Arrow functions, the basics](#arrow-functions-the-basics)

#### 18. [Especiales JavaScript](#especiales-javascript)

## Documentation

#### Hello, world!
Le etiqueta `<script></script>` se puede colocar en casi cualquier parte del documento HTML. <br>
La etiqueta `<script></script>` tiene algunos atributos, que ya no se utilizan en la actualidad. <br>
Otro punto a tener en cuenta es que si tenemos una parte de código en Javascript, que es extensa, mejor la ponemos en un archivo a parte, así tenemos el código mas organizado y podemos trabajar mejor con él. <br>
Además, el navegador lo guardará en **caché**. Por lo que el código solo se descargará una vez, reduciendo el **tiempo de carga**.

#### Code structure
Ahora vamos a ver que son *sentencias*. <br>
Son la sintaxis y comandos que realizan acciones, como por ejemplo el alert del módulo anterior, que muestra un mensaje. <br>
Las podemos separar con `;` para que quede mas organizado, y se ejecutarán una detrás de otra. <br> 
Siempre es recomendable ponerlo entre sentencias para que no haya errores de código.

#### The modern "use strict" mode
El `use strict` se utiliza para solucionar problemas de compatibilidad. <br>
Se puede combinar sintaxis antigua de Javascript y nueva.<br>
A lo largo el tiempo, Javascript ha evolucionado sin problemas de compatibilidad, pero en 2009, se añadieron nuevas características al lenguaje y se modificaron otras.<br>
Para mantener el código antiguo funcionando correctamente, las modificaciones están desactivadas por defecto, y aquí es cuándo entra en juego `use strict`. <br>
Al colocarse al principio de un script o de una función, este funciona de la **manera moderna**.<br>
Un apunte interesante, es que Javascript moderno, funciona con **clases** y **módulos**, que automáticamente habilitan el `use strict`. Por lo que no es necesario activarlo.

#### Variables
Podemos decir que las variables son **contenedores** de información, dónde guardamos **datos** importantes. <br>
Lo podemos hacer uno por uno, o en línea. En línea no es tan recomendable, por la legibilidad <br>
    • let message = 'Hola!'; <br>
    • let user = 'John', age = 25, message = 'Hola'; <br>
Las variables tienen dos **limitaciones**: <br>
    • Solo puede incluir letras, dígitos, o los símbolos $ y _. <br>
    • El primer carácter no puede ser un dígito. <br>

#### Types of data
    • Number, representa tanto números enteros como de punto flotante.
      Además de los comunes, existen otros valores especiales, como Infinity y NaN.
      
    • BigInt, el tipo number no puede representar número a partir de una cifra muy alta, por lo que utilizamos  BigInt para número a partir de 9007199254740992 o 2^53.
      Para indicar que es un BigInt, añadimos una n al final del número. 123….21312n.
      
    • String, cadena de caracteres y debe colocarse entre comillas.
      
    • Boolean, solo tiene dos valores posibles, false o true.
      
    • Null, no es ninguno de los tipos anteriores. Representa a nada, vacío o valor desconocido.
      
    • Undefined, quiere decir que no se le ha asignado un valor.
      
    • Object y Symbol, los objetos pueden almacenar un conjunto de datos y entidades complejas.
      Symbol se utiliza para crear identificadores únicos para estos objetos.
      
    • El operador typeof, devuelve el tipo de dato del operando. Es importante decir que es un operador y no una función.
      Se utiliza (), por agrupación matemática, no por ser parte del operador.


#### 6. Interaction: alert, prompt, confirm (#interaction-alert-prompt-confirm)
Este es el contenido de la sección "Interaction: alert, prompt, confirm".

#### 7. Type Conversions (#type-conversions)
Este es el contenido de la sección "Type Conversions".

#### 8. Basic operators, mathematics (#basic-operators-mathematics)
Este es el contenido de la sección "Basic operators, mathematics".

#### 9. Comparisons (#comparisons)
Este es el contenido de la sección "Comparisons".

#### 10. Conditional execution: if, '?' (#conditional-execution-if)
Este es el contenido de la sección "Conditional execution: if, '?'".

#### 11. Logical Operators (#logical-operators)
Este es el contenido de la sección "Logical Operators".

#### 12. Operador Nullish Coalescing '??' (#operador-nullish-coalescing)
Este es el contenido de la sección "Operador Nullish Coalescing '??'".

#### 13. Loops: while and for
Los bucles son una forma de repetir elementos de una lista o ejecutar un código tantas veces como se indique.<br>
En este documento voy a exponer los **básicos**:<br>

    • While, este bucle se ejecuta mientras la condición sea verdadera. Con while, primero se hace una comprobación, y si se cumple, comienza la ejecución. <br> 
      A cada ejecución le llamamos iteración. <br>
      Punto a tener en cuenta, cualquier número diferente a 0, se evalúa como verdadero. Por lo tanto, lo que se indica en la condición, es el número de iteraciones. Cuándo se llega a 0, el bucle se cierra. <br> 
      Además, i++, es muy importante, puesto que si no se pone, el bucle será infinito.<br>
          
          let i = 0
          while( i < 3 ) { <br>
            alert(“Bucle while” + 1) <br>
            i++<br>
            	} <br>

	      let i = 3; <br>
	      while (i) { <br>
	      alert(i)<br>
	      i--;<br>
                  }	<br>

    • Do...while, primero se ejecuta el cuerpo y después se comprueba la condición, esto se usa, cuándo mínimo se quiere ejecutar una vez, independientemente si se cumple o no la condición.<br> 
	
	let i = 0; <br>
	do { <br>
	 alert(i);<br>
	 i++; <br>
	}while (1 < 3);<br>

    • For, el bucle empieza, y si la condición es true, se ejecuta el código.<br>
      Podemos utilizar break para detener en cualquier momento el bucle, por ejemplo, si una condición no se cumple. <br>
      Podemos utilizar continue, para detener el bucle solo si se cumple la condición, y seguir con el resto.
      
      for(let i = 0;  i < 3; i++ ) { <br>
          alert(i) <br>
          }<br>

#### 14. The "switch" statement (#the-switch-statement)
Este es el contenido de la sección "The 'switch' statement".

#### 16. Functions (#functions)
Este es el contenido de la sección "Functions".

#### 16. Function expressions (#function-expressions)
Este es el contenido de la sección "Function expressions".dam

#### 17. Arrow functions, the basics (#arrow-functions-the-basics)
Este es el contenido de la sección "Arrow functions, the basics".

#### 18. Especiales JavaScript (#especiales-javascript)
Este es el contenido de la sección "Especiales JavaScript".
