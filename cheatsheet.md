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