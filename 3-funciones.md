# 📌 Funciones.
Podemos crear funciones de varios modos.
Ambos modos de creación asignan la función a una variable.
```javascript
// Declaración de funcion.
function sayHi() {
alert( "Hola" );
}

// Expresión de funcion.
let sayHi = function() {  // De este modo se puede omitir el nombrar la función.
alert( "Hola" );
};

// Expresión lambda.
(parametros) => código retorno ;
```

## Diferencias entre Declaración de funcion y Expresión de funcion.
La diferencia más sutil es cuándo la función es creada por el motor de JavaScript.
- Una Expresión de Función es creada cuando la ejecución la alcance y es utilizable desde
ahí en adelante.
- Una Declaración de Función puede ser llamada antes de ser definida.

**Declaración de función**
```javascript
// Declaración de Función
function sum(a, b) {
return a + b;
}
```
**Expresión de funcion**
```javascript
// Expresión de Función
let sum = function(a, b) {
return a + b;
};
```

## Llamadas de funciones.
Para llamar a una función debemos invocarla mediante su nombre seguido de parentesis que contengan los posibles valores parametro.
```javascript
minimum(10,12);
```
Existen lenguajes de programación en los que cualquier mención del nombre de una función causa su ejecución, pero JavaScript no funciona así.

**Las funciones son valores**
En JavaScript, una función es un valor, por lo tanto podemos tratarlo como tal. 
```javascript
console.log( minimum );
```
El código de arriba muestra su representación de cadena, que es el código fuente.


# 📌 Funciones Callback.

