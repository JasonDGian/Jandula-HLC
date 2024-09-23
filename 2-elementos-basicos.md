## :small_blue_diamond: La consola de Javascript.
Proporciona información sobre la página web que se está ejecutando y ofrece una línea de comandos donde puedes ejecutar expresiones de JavaScript directamente en la página actual. La función console.log permite mostrar en la consola cualquier información que desees. Por ejemplo, al usar console.log('holamundo'), se imprimirá el mensaje "holamundo" en la consola de JavaScript.

**Ejemplo de uso de consola**
```javascript
console.log("Punto de control.");

console.log(<instruccion a loguear>);
```

## :small_blue_diamond: Comentarios.
Javascript tiene dos sintaxis de comentarios.
```javascript
// Comentario de linea singular.

alert("Hola mundo");

/* 
Comentario
de bloque
*/
```

## :small_blue_diamond: Declaración de variables.
Los identificadores de las variables deben comenzar con una letra (`a-z`, `A-Z`), un guion bajo (`_`) o un símbolo de dólar (`$`). A partir del primer carácter, pueden contener números, pero no pueden comenzar con ellos.

>[!IMPORTANT]
> Javascript es **case-sensitive**.

### :white_small_square: var
- Declara una **variable**.
- Variable de **ámbito de función**.
- Iniciaclización **opcional**.
- El valor inicializado es **mutable**.
- Uso tipico: Funciones y metodos.

### :white_small_square: let
- Declara una **variable**.
- Variable de **ámbito de bloque**.
- Iniciaclización **opcional**.
- El valor inicializado es **mutable**.
- Uso tipico: bloques de código.


### :white_small_square: const
- Declara una **constante**.
- Variable de **ámbito de bloque**.
- Iniciaclización **mandatoria**.
- El valor inicializado es **no mutable**.
- Uso tipico: bloques de código.

>[!NOTE]
> En este contexto, un bloque de código se refiere a una sección de código que está delimitada por llaves `{` `}`.

## :small_blue_diamond: Hoistin de variables.
En JavaScript, el hoisting se refiere al comportamiento interno del lenguaje mediante el cual las declaraciones de funciones, variables y clases se mueven al **inicio de su ámbito**, todo antes de la ejecución del código. Esto nos permite utilizar funciones, variables y clases antes de haberlas declarado.

Sin embargo, solo las declaraciones se "hoistean"; **las inicializaciones no se hoistean.**

Por ejemplo:
```javascript
console.log(x); // undefined
var x = 5;
console.log(x); // 5
```
En este caso, la declaración de `x` es hoisteada, pero su inicialización no.

## :small_blue_diamond: Tipos de datos.
Como en todos los lenguajes, en Javascript existen distintos tipos de datos. He aqui una tabla.

<table>
    <thead>
        <tr>
            <th>Tipo de Dato</th>
            <th>Descripción</th>
            <th>Ejemplo de Declaración</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Number</td>
            <td>Representa números (enteros y decimales).</td>
            <td><code>let num = 42;</code></td>
        </tr>
        <tr>
            <td>String</td>
            <td>Representa cadenas de texto.</td>
            <td><code>let str = "Hola";</code></td>
        </tr>
        <tr>
            <td>Boolean</td>
            <td>Representa valores de verdad: <code>true</code> o <code>false</code>.</td>
            <td><code>let isTrue = true;</code></td>
        </tr>
        <tr>
            <td>Object</td>
            <td>Colecciones de pares clave-valor.</td>
            <td><code>let obj = { clave: "valor" };</code></td>
        </tr>
        <tr>
            <td>Array</td>
            <td>Colección ordenada de elementos.</td>
            <td><code>let arr = [1, 2, 3];</code></td>
        </tr>
        <tr>
            <td>Function</td>
            <td>Bloque de código reutilizable.</td>
            <td><code>function myFunc() { }</code></td>
        </tr>
        <tr>
            <td>Null</td>
            <td>Representa la ausencia intencional de valor.</td>
            <td><code>let value = null;</code></td>
        </tr>
        <tr>
            <td>Undefined</td>
            <td>Indica que una variable no ha sido inicializada.</td>
            <td><code>let value;</code></td>
        </tr>
        <tr>
            <td>Symbol</td>
            <td>Representa un valor único e inmutable.</td>
            <td><code>let sym = Symbol("desc");</code></td>
        </tr>
        <tr>
            <td>BigInt</td>
            <td>Permite representar números enteros grandes.</td>
            <td><code>let bigInt = 1234567890123456789012345678901234567890n;</code></td>
        </tr>
    </tbody>
</table>

## :small_blue_diamond: function typeof.
Este funcion se usa para obtener el tipo de dato al que pertenece una variable.

```javascript
let num = 42;
let str = "Hola";
let isTrue = true;
let obj = { clave: "valor" };
let arr = [1, 2, 3];
let fn = function() {};
let value = null;
let undefinedVar;
let sym = Symbol("desc");
let bigInt = 1234567890123456789012345678901234567890n;

console.log(typeof num);         // "number"
console.log(typeof str);         // "string"
console.log(typeof isTrue);      // "boolean"
console.log(typeof obj);         // "object"
console.log(typeof arr);         // "object" (los arrays son objetos)
console.log(typeof fn);          // "function"
console.log(typeof value);       // "object" (null es un caso especial)
console.log(typeof undefinedVar); // "undefined"
console.log(typeof sym);         // "symbol"
console.log(typeof bigInt);      // "bigint"
```
## :small_blue_diamond: Lenguaje poco-tipado.
En javascript no es obligatorio especificar el tipo de dato al declarar una variable. Podemos definir una variable de la siguiente manera.
```javascript
var ejemplo = 55;
```
y luego reasignarle un valor de literal distinto.
```javascript
var ejemplo = "Hola mundo";
```
**Al ser un lenguaje de tipo dinámico (poco tipado) esta nueva asignación a distinto tipo no provoca un mensaje de error.**

## :small_blue_diamond:Parseo.
```javascript
let numStr = "42";
let num = parseInt(numStr); // num es 42 (tipo Number)

let floatStr = "3.14";
let floatNum = parseFloat(floatStr); // floatNum es 3.14 (tipo Number)
```

## :small_blue_diamond: Casteo.
```javascript
let num = 42;
let str = String(num); // str es "42" (tipo String)

let floatNum = 3.14;
let floatStr = floatNum.toString(); // floatStr es "3.14" (tipo String)
```