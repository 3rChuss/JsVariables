# Diferentes maneras de declarar variables en JavaScript

**Tipos de declaraciones de variables**


**var**
```javascript
/* Declarando variables con var */
          var myVar; // inicializada sin declarar
          var myVar = 'hola mundo'; //Inicializada declarando el valor string 'hola mundo'
          console.log(myVar); 
          //Resultado:
          // 'hola mundo'
```

>Puede ser declarada tantas veces como quieras con el mismo nombre y no ocurrirá ningun problema.
>Su salida dependerá del último valor declarado, en nuestro caso 'hola mundo'.


**let**
```javascript
/* Declarando variables con let */
          let nombre = 'Jesus';
          let apellido = 'Abril';
          let nombre = 'Juan';
          console.log(nombre + ' ' + apellido);
          // Resultado:
          // Uncaught SyntaxError: Identifier 'nombre' has already been declared

          //tambien puedes declarar múltiples de la siguiente forma
          let  myNombre   = 'Jesus',  // como puedes observar se usa una coma.
               myApellido = 'Abril';
          console.log(myNombre + ' ' + myApellido);
          // Resultado:
          // Jesus Abril

          let otroNombre;
          console.log(otronombre);
          //Resultado
          //Uncaught ReferenceError: otronombre is not defined
          otroNombre = 'Juan Ramirez';
          console.log(otroNombre);
          // Resultado
          // Juan Ramirez

```

> No permite declaraciones de variables con el mismo nombre;
> Puede ser declarada sin inicializar.
> Debe ser inicializada antes de su uso.
> Deben llamarse diferente.

Utiliza let cuando su valor se cambien en un futuro.


**const**
```javascript
/* Declarando variables con const */
          const producto;
          console.log(producto);
          // Resultado
          // Uncaught SyntaxError: Missing initializer in const declaration

          const otroProducto = 'Jabón';
          console.log(otroProducto);
          // Resultado
          // Jabón

```

> Una constante *siempre* debe inicializarse
> No puede llamarse igual a otra variable

Úsala cuando sepas que su valor no cambiará en el futuro.


