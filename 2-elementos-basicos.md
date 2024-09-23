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
> En este contexto, un bloque de código se refiere a una sección de código que está delimitada por llaves {}.