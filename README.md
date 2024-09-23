# :pushpin: Introducción a Javascript.
Javascript es un lenguaje nacido para aumentar la capacidad de interacción y funcionalidades de las paginas web. Se escribe directamente en HTML y se ejcuta automaticamentea medida que la página va cargando las instrucciones.
- Es un lenguaje interpretado.
- Se puede ejecutar en cualquier tipo de dispositivo provisto de "motor" o interprete.


## :small_blue_diamond: Acerca de los motores de Javascript.
Los fundamentos de funcionamiento de un motor de Javascript son los siguientes.
1. El motor lee el script.
2. Luego convierte el script a lenguaje maquina.
3. Pro ultimo el codigo maquina se ejecuta muy rapido.

El motor aplica optimizaciones en cada paso del proceso. Incluso observa como el script
compilado se ejecuta, analiza los datos que fluyen a través de él y aplica optimizaciones al
código maquina basadas en ese conocimiento.

**Distintos navegadores usan distintos motores.**
<table>
    <tr>
        <th>Browser / Runtime</th>
        <th>JavaScript Engine</th>
    </tr>
    <tr>
        <td>Mozilla</td>
        <td>Spidermonkey</td>
    </tr>
    <tr>
        <td>Chrome</td>
        <td>V8</td>
    </tr>
    <tr>
        <td>Safari</td>
        <td>JavaScriptCore*</td>
    </tr>
    <tr>
        <td>IE</td>
        <td>Chakra</td>
    </tr>
    <tr>
        <td>Node.js</td>
        <td>V8</td>
    </tr>
    <tr>
        <td>Deno</td>
        <td>V8</td>
    </tr>
    <tr>
        <td>Bun</td>
        <td>JavaScriptCore</td>
    </tr>
    <tr>
        <td>Edge**</td>
        <td>Blink and V8</td>
    </tr>
</table>

## :small_blue_diamond: Limitaciones de Javascript.
El JavaScript moderno es un lenguaje "seguro" que no permite acceso directo a partes sensibles del equipo. Sus capacidades dependen del entorno:  
- En Node.js, puede manejar archivos y realizar solicitudes de red; 
- en el navegador, permite manipular páginas, reaccionar a interacciones, gestionar cookies y usar almacenamiento local para recordar datos del cliente.

**JavaScript en un navegador NO tiene acceso a:**
1. Memoria del sistema.
2. Sistema de archivos del ordenador (excepto mediante APIs específicas como File API, con consentimiento del usuario).
3. CPU.
4. Recursos del sistema operativo.
5. Datos de otros dominios (debido a la política de mismo origen).

**JavaScript en un navegador SI tiene acceso a:**

1. **DOM**: Manipulación de la estructura y el contenido de las páginas web.
2. **Eventos**: Responder a interacciones del usuario, como clics y movimientos del ratón.
3. **APIs del navegador**: Funciones como almacenamiento local, cookies, y AJAX para realizar solicitudes de red.
4. **Estilos CSS**: Modificar y aplicar estilos a los elementos de la página.

## :small_blue_diamond: Que diferencia a Javascript.
JavaScript es la única tecnología de los navegadores que presenta la combinación de estas tres características.
1. Completa integración con HTML y CSS.
2. Las cosas simples se hacen de manera simple.
3. Soportado por la mayoría de los navegadores y habilitado de forma predeterminada.

## :small_blue_diamond: Lenguajes basados en Javascript.
Al igual que ocurre con muchos lenguajes, Javascript ha sido adaptado a distintas ramas de desarrollo para satisfacer demandas para las que en su forma base no era optimo.

<table>
    <tr>
        <th>Lenguaje</th>
        <th>Descripción</th>
    </tr>
    <tr>
        <td>TypeScript</td>
        <td>Un superconjunto de JavaScript que añade tipos estáticos.</td>
    </tr>
    <tr>
        <td>CoffeeScript</td>
        <td>Compila a JavaScript, ofreciendo una sintaxis más limpia y concisa.</td>
    </tr>
    <tr>
        <td>Flow</td>
        <td>Herramienta para la verificación de tipos en JavaScript, desarrollada por Facebook.</td>
    </tr>
    <tr>
        <td>Dart</td>
        <td>Lenguaje independiente que puede compilarse a JavaScript para navegadores.</td>
    </tr>
    <tr>
        <td>Elm</td>
        <td>Lenguaje funcional que compila a JavaScript, centrado en aplicaciones web.</td>
    </tr>
    <tr>
        <td>ClojureScript</td>
        <td>Versión de Clojure que se compila a JavaScript, con enfoque funcional.</td>
    </tr>
    <tr>
        <td>PureScript</td>
        <td>Similar a Haskell, se compila a JavaScript y se utiliza para desarrollo web.</td>
    </tr>
</table>


## :small_blue_diamond: Costumbre arcaicas.
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