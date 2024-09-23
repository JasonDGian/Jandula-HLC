# :pushpin: Primeros pasos

## Carga de scripts.
Para cargar un script en una web podemos hacerlo mediante la etiqueta `<script> ... </script>`, ya sea introduciendo en ella las instrucciones que deseamos ejecutar o cargando un fichero externo.

Para indicar un fichero de javascript adjunto deberemos emplear el atributo de origen `src` indicando donde encontrar dicho fichero. Podemos emplear tanto rutas absolutas como relativas.

**Ejemplo de script integrado**:
```html
<script>
alert( '¡Hola, mundo!' );
</script>
```

**Ejemplo de carga de fichero**
```html
<script src="/path/to/script.js"></script>
```

### Script intergado vs fichero externo.
La ventaja de tener un script almacenado en un fichero dedicado es la posibilidad de reutilizarlo una vez almacenado en el caché del navegador, facilitando asi su reutilización y el funcionamiento para scripts de complejitud más amplia. 
  
TL:DR; Cuando las instrucciones son pocas y sencillas podemos almacenarlas directamente en la etiqueta `<script>` mientras que cuando se trata de instrucciones más complejas y extensas conviene hacer uso de un fichero dedicado. 

>[!IMPORTANT]
> Una etiqueta `<script>` **NO PUEDE** especificar una ruta, y a la vez, contener instrucciones. 


## Costumbre arcaicas.
Con versiones anteriores de HTML se debia especificar ciertos atributos para la etiqueta Script como lo son el atributo `language=...` y el atributo `type=...`. Hoy en dia esto está en desuso y es bandera de código arcaico. De misma naturaleza son los 'comentarios' de ocultación de instrucciones.

**Ejemplos de codigo anticuado:**
```html
<script type=...></script>

<script language=...></script>

<script type="text/javascript"><!--
...
instrucciones
...
//--></script>
```

