# :pushpin: Cargar instrucciones.

## :small_blue_diamond: Directamente desde documento HTML
```html
<script>
alert( '¡Hola, mundo!' );
</script>
```

## :small_blue_diamond: Desde fichero externo.
```html
<script src="/path/to/script.js"></script>
```

# :pushpin: Comentarios.

## :small_blue_diamond: Comentarios de linea.
```javascript
// Comentario de linea singular.
```
## :small_blue_diamond: Comentarios de bloque.
```javascript
/* 
Comentario
de bloque
*/
```

# :pushpin: Consola de Javascript.
```javascript
console.log("Punto de control.");

console.log(<instruccion a loguear>);
```

# :pushpin: Declaración de variables.
Los identificadores de las variables deben comenzar con una letra (`a-z`, `A-Z`), un guion bajo (`_`) o un símbolo de dólar (`$`). A partir del primer carácter, pueden contener números, pero no pueden comenzar con ellos.

>[!IMPORTANT]
> Javascript es **case-sensitive**.

## :small_blue_diamond: var
- Declara una **variable**.
- Variable de **ámbito de función**.
- Iniciaclización **opcional**.
- El valor inicializado es **mutable**.
- Uso tipico: Funciones y metodos.

## :small_blue_diamond: let
- Declara una **variable**.
- Variable de **ámbito de bloque**.
- Iniciaclización **opcional**.
- El valor inicializado es **mutable**.
- Uso tipico: bloques de código.


## :small_blue_diamond: const
- Declara una **constante**.
- Variable de **ámbito de bloque**.
- Iniciaclización **mandatoria**.
- El valor inicializado es **no mutable**.
- Uso tipico: bloques de código.

>[!NOTE]
> En este contexto, un bloque de código se refiere a una sección de código que está delimitada por llaves `{` `}`.

# :pushpin: Tipos de datos.
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
   
>[!CAUTION]
> Javascript es **case-sensitive**. Esto significa que "null", "Null" y "NULL" no hacen referencia al mismo elemento. El nombre correcto es `null`.

# :pushpin: Casteo y parsing.
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

# :pushpin: Operadores.
## :small_blue_diamond: Operadores de asignación.
<table>
    <thead>
        <tr>
            <th>Operador</th>
            <th>Descripción</th>
            <th>Ejemplo</th>
            <th>Equivalente</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>=</td>
            <td>Asigna el valor a la variable</td>
            <td><code>x = 5;</code></td>
            <td></td>
        </tr>
        <tr>
            <td>+=</td>
            <td>Suma y asigna</td>
            <td><code>x += 2;</code></td>
            <td><code>x = x + 2;</code></td>
        </tr>
        <tr>
            <td>-=</td>
            <td>Resta y asigna</td>
            <td><code>x -= 3;</code></td>
            <td><code>x = x - 3;</code></td>
        </tr>
        <tr>
            <td>*=</td>
            <td>Multiplica y asigna</td>
            <td><code>x *= 4;</code></td>
            <td><code>x = x * 4;</code></td>
        </tr>
        <tr>
            <td>/=</td>
            <td>Divide y asigna</td>
            <td><code>x /= 2;</code></td>
            <td><code>x = x / 2;</code></td>
        </tr>
        <tr>
            <td>%=</td>
            <td>Módulo y asigna</td>
            <td><code>x %= 3;</code></td>
            <td><code>x = x % 3;</code></td>
        </tr>
        <tr>
            <td>**=</td>
            <td>Potencia y asigna</td>
            <td><code>x **= 2;</code></td>
            <td><code>x = x ** 2;</code></td>
        </tr>
    </tbody>
</table>


## :small_blue_diamond: Operadores de comparación.
<table>
    <thead>
        <tr>
            <th>Operador</th>
            <th>Descripción</th>
            <th>Ejemplo</th>
            <th>Resultado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>==</td>
            <td>Igualdad (comparación no estricta)</td>
            <td><code>5 == '5'</code></td>
            <td>true</td>
        </tr>
        <tr>
            <td>===</td>
            <td>Igualdad estricta (mismo tipo y valor)</td>
            <td><code>5 === '5'</code></td>
            <td>false</td>
        </tr>
        <tr>
            <td>!=</td>
            <td>Desigualdad (comparación no estricta)</td>
            <td><code>5 != '6'</code></td>
            <td>true</td>
        </tr>
        <tr>
            <td>!==</td>
            <td>Desigualdad estricta (mismo tipo y valor)</td>
            <td><code>5 !== '5'</code></td>
            <td>true</td>
        </tr>
        <tr>
            <td>&lt;</td>
            <td>Menor que</td>
            <td><code>5 &lt; 10</code></td>
            <td>true</td>
        </tr>
        <tr>
            <td>&gt;</td>
            <td>Mayor que</td>
            <td><code>10 &gt; 5</code></td>
            <td>true</td>
        </tr>
        <tr>
            <td>&lt;=</td>
            <td>Menor o igual que</td>
            <td><code>5 &lt;= 5</code></td>
            <td>true</td>
        </tr>
        <tr>
            <td>&gt;=</td>
            <td>Mayor o igual que</td>
            <td><code>10 &gt;= 10</code></td>
            <td>true</td>
        </tr>
    </tbody>
</table>


## :small_blue_diamond: Operadores de aritméticos.
<table>
    <thead>
        <tr>
            <th>Operador</th>
            <th>Descripción</th>
            <th>Ejemplo</th>
            <th>Resultado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>+</td>
            <td>Adición</td>
            <td><code>5 + 3</code></td>
            <td>8</td>
        </tr>
        <tr>
            <td>-</td>
            <td>Resta</td>
            <td><code>5 - 3</code></td>
            <td>2</td>
        </tr>
        <tr>
            <td>*</td>
            <td>Multiplicación</td>
            <td><code>5 * 3</code></td>
            <td>15</td>
        </tr>
        <tr>
            <td>/</td>
            <td>División</td>
            <td><code>6 / 3</code></td>
            <td>2</td>
        </tr>
        <tr>
            <td>%</td>
            <td>Módulo (resto de la división)</td>
            <td><code>5 % 3</code></td>
            <td>2</td>
        </tr>
        <tr>
            <td>**</td>
            <td>Potencia</td>
            <td><code>2 ** 3</code></td>
            <td>8</td>
        </tr>
        <tr>
            <td>++</td>
            <td>Incremento</td>
            <td><code>let x = 5; x++;</code></td>
            <td>6 (después del incremento)</td>
        </tr>
        <tr>
            <td>--</td>
            <td>Decremento</td>
            <td><code>let x = 5; x--;</code></td>
            <td>4 (después del decremento)</td>
        </tr>
    </tbody>
</table>


## :small_blue_diamond: Operadores de asignación aritméticos (bit a bit).
<table>
    <thead>
        <tr>
            <th>Operador</th>
            <th>Descripción</th>
            <th>Ejemplo</th>
            <th>Equivalente</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>&=</td>
            <td>AND bit a bit y asigna</td>
            <td><code>x &= 1;</code></td>
            <td><code>x = x & 1;</code></td>
        </tr>
        <tr>
            <td>|=</td>
            <td>OR bit a bit y asigna</td>
            <td><code>x |= 1;</code></td>
            <td><code>x = x | 1;</code></td>
        </tr>
        <tr>
            <td>^=</td>
            <td>XOR bit a bit y asigna</td>
            <td><code>x ^= 1;</code></td>
            <td><code>x = x ^ 1;</code></td>
        </tr>
        <tr>
            <td><<=</td>
            <td>Desplazamiento a la izquierda y asigna</td>
            <td><code>x <<= 2;</code></td>
            <td><code>x = x << 2;</code></td>
        </tr>
        <tr>
            <td>>=</td>
            <td>Desplazamiento a la derecha y asigna</td>
            <td><code>x >>= 2;</code></td>
            <td><code>x = x >> 2;</code></td>
        </tr>
        <tr>
            <td>>> =</td>
            <td>Desplazamiento a la derecha sin signo y asigna</td>
            <td><code>x >>>= 2;</code></td>
            <td><code>x = x >>> 2;</code></td>
        </tr>
    </tbody>
</table>


## :small_blue_diamond: Operador de concatenación.
El operador de concatenación es el simbolo `+`.
Ejemplo:
```javascript
console.log("mi" + " " + "string"); // -> "mi string"
```

# :pushpin: Sentencias condicionales.

## :small_blue_diamond: Operador ternario.
Un operador ternario es como un "If" simplificado.

```javascript
condición ? valorSiTrue : valorSiFalse;
```

Se pueden anidar.

```javascript
condición ? valorSiTrue : (condición ? valorSiTrue : valorSiFalse);
```
**Ejemplo**
En este caso, primero se evalúa si x es mayor que 10. Si es verdadero, se evalúa la segunda condición para determinar si es mayor que 20. De lo contrario, devuelve "10 o menos".
```javascript
let x = 15;

let resultado = (x > 10) 
    ? (x > 20 ? "Mayor que 20" : "Entre 11 y 20") 
    : "10 o menos";

console.log(resultado); // "Entre 11 y 20"
```

## :small_blue_diamond: Sentencia IF.
Tomando el ejemplo, `condicion1` será la primera en evaluarse; si es cierta, se ejecutará su bloque de código. Si es falsa, se evaluarán las subsecuentes condiciones. Esto permite **encadenar tests** de condiciones a modo de filtro agregativo.

```javascript
if (condicion1){

} else if (condicion2) {

} else {

}
```