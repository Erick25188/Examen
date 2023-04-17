# JavaScript

### 1.- ¿Cómo se declaran propiedades privadas en JavaScript?
  - [ ] _ guión bajo
  - [ ] * asterisco
  - [x] # numeral
  - [ ] Las propiedades privadas no existen

💡 **Explicación:** 

🔗 **Recursos:** https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Classes/Private_class_fields

<br>

### 2.- ¿Cómo se declaran propiedades protegidas en JavaScript?
  - [x] _ guión bajo
  - [ ] * asterisco
  - [ ] # numeral
  - [ ] Las propiedades privadas no existen

💡 **Explicación:** 

🔗 **Recursos:** https://dev.to/bhagatparwinder/classes-in-js-public-private-and-protected-1lok

<br>

### 3.- ¿Cuál es el resultado?
```javascript
  const arr = [1,2,3,4,5];

  console.log(arr.at(-1));
```
- [ ] 0
- [x] 5
- [ ] 1
- [ ] undefined

💡 **Explicación:** arr.at(-1) devuelve el último elemento del array.

<br>

### 4.- Conbención binaria en las sumas
```javascript
  (0.1 + 0.2) === 0.3
```
- [ ] True 
- [x] False

💡 **Explicación:** (0.1 + 0.2) = 0.300000004 !== 0.3

<br>

### 5.- Arreglos
``` javascript
  const arr = [ , , , , ];
  
  console.log(arr.length);
```
- [ ] 0
- [ ] 1
- [x] 4
- [ ] 3

💡 **Explicación:**

<br>

### 6.- Promesas - promise.all
```javascript
  let promesa1 = new Promise(resolve => 
    setTimeout(() => resolve('promesa 1'), 2000)
  );

  let promesa2 = new Promise(resolve => 
    setTimeout(() => resolve('promesa 2'), 1000)
  );

  Promise.all([promesa1, promesa2]).then(res => console.log(res));
```

- [x] [ 'promesa1', 'promesa2' ];

- [ ] <code>
  promesa 2
  
  promesa 1
</code>

- [ ] [ promesa 2, promesa 1 ]

- [ ] <code>
  promesa 1
  
  promesa 2
</code>

💡 **Explicación:** 

<br>

### 7.- Promesas - promise.then
```javascript
  let promesa1 = new Promise(resolve => 
    setTimeout(() => resolve('promesa 1'), 2000)
  );

  let promesa2 = new Promise(resolve => 
    setTimeout(() => resolve('promesa 2'), 1000)
  );

  promesa1.then( res => console.log(res));
  promesa2.then( res => console.log(res));
```

- [ ] [promesa 1, promesa 2]

- [x] <code>
  promesa 2
  
  promesa 1
</code>

- [ ] [promesa 2, promesa 1]

- [ ] <code>
  promesa 1
  
  promesa 2
</code>

💡 **Explicación:** En este caso se ejecutan según el tiempo de setTimeout

<br>

### 8.- Método split
```javascript
  const array = ["Ana/Maria/Pedro/Juan"];
  
  console.log(array.split());
```
  - [x] TypeError
  - [ ] Ana Maria Pedro Juan
  - [ ] ["Ana/Maria/Pedro/Juan"]
  - [ ] Ana/Maria/Pedro/Juan

💡 **Explicación:** split es un método de strings no de arrays

<br>

### 9.- Método split
```javascript
  const array = "Ana/Maria/Pedro/Juan"

  console.log(array.split());
```
  - [ ] TypeError
  - [ ] Ana Maria Pedro Juan
  - [x] ["Ana/Maria/Pedro/Juan"]
  - [ ] Ana/Maria/Pedro/Juan

💡 **Explicación:** El método split es válido ya que la constante array es un string, split al no tener argumentos 'divide' todo el string como un solo elemento de un arreglo.

<br>

### 10.- padStart y padEnd
```javascript
  let face = "°-°"
  console.log(face.padStart(5,'-').padEnd(10,'-'));
```
- [x] --°-°-----
- [ ] -----°-°-------
- [ ] °-°
- [ ] -°-°-

💡 **Explicación:** padStart agregará - antes de la carita para que su longitud total sea de 5, padEnd agregará los - después de la carita para que su nueva longitud total sea de 10

<br>

### 11.- isNaN
```javascript
  console.log(isNaN('20'));
  console.log(isNaN(20));
```
- [ ] true - true
- [ ] false - true
- [x] false - false
- [ ] true - false

💡 **Explicación:** En ambos casos la evaluación SI es un número por lo que 'is not a number' retorna false

<br>

### 12.- typefo isNaN
```javascript
  console.log(typeof isNaN);
```
- [ ] Number
- [x] Function
- [ ] String
- [ ] Boolean

💡 **Explicación:** typeof isNaN == function; typeof NaN == number;

<br>

### 13.- notación numérica
```javascript
  let number = 114_00
  console.log(number);
```
- [ ] 114,00
- [ ] Error
- [ ] 114_00
- [x] 11400

💡 **Explicación:** los _ en los números solo tienen fines estéticos, para leerlos mejor, pero son ignorados al imprimir en consola

<br>

### 14.- spread operator
```javascript
  let persona = {
    nombre: 'Rick',
    pais: 'Estados Unidos'
  };

  let persona2 = {...person};

  persona.nombre = 'Morty';

  console.log(persona2);
```
- [x] Rick
- [ ] Estados Unidos
- [ ] Morty
- [ ] Undefined

💡 **Explicación:** 

<br>

### 15.- ¿Cómo agregar un valor a un arreglo de JavaScript?
- [x] arr[arr.length] = value
- [ ] arr[arr.length+1] = new Arrays() 
- [ ] arr[arr.length-1] = value
- [ ] arr[arr.length*1] = value

💡 **Explicación:** 

<br>

### 16.- Objeto persona
```javascript
  const persona = {
    nombre: 'Rick',
    direccion: {
      pais: 'Estados Unidos',
    }
  }

  console.log(persona.direccion.ciudad)
```
- [ ] error
- [ ] Estados Unidos
- [ ] TypeError
- [x] undefined 

💡 **Explicación:** 

<br>

### 17.- Desestructuración
```javascript
  const arr = ['uno', 'dos', 'tres', 'cuatro', 'cinco'];

  const { primero } = arr;

  console.log(primero);
```

- [ ] error
- [ ] uno
- [x] undefined 
- [ ] primero

💡 **Explicación:** la desestructuración correcta utilizaría [ primero ] = arr; y en ese caso si sería 'uno'.

<br>

### 18.- Objeto persona
```javascript
  const persona = {
    nombre: 'Rick',
    direccion: {
      pais: 'Estados Unidos',
    }
  }

  console.log(persona.direccion.pais.ciudad.colonia)
```
- [ ] error
- [ ] Estados Unidos
- [x] TypeError
- [ ] undefined 

💡 **Explicación:** Como ciudad no existe no se pueden leer las propiedades de lo indefinido, por lo tanto el mensaje será TypeError, si solo fuera ...pais.ciudad sería undefined

<br>

### 19.- Desestructuración de arreglos
```javascript
  const fruits = ['manzana', 'pera', 'uva', 'guayaba'];
  const { fruit1, fruit2 } = fruits;
  console.log(fruit, fruit2)
```
- [x] undefined
- [ ] 'manzana', 'pera' 
- [ ] error
- [ ] manzana, pera

💡 **Explicación:**

<br>

### 20.- funciones con parámetros predefinidos
```javascript
  function suma(param1 = 2, param2 = 3) {
    return param1 + param2;
  }
  console.log(suma(10));
```
- [ ] 3
- [ ] 10 
- [x] 13
- [ ] 2

💡 **Explicación:**

<br>

### 21.- ¿Cuál es la salida del siguiente código?
```javascript
  const obj = { 
    nombre: "Leeroy",
    apellido: "Jenkings",
  }
  console.log(obj.hasOwn(obj, 'edad'));
```
- [ ] undefined
- [ ] false
- [ ] Error
- [x] TypeError: obj.hasOwn is not a function

# Lit Element

### 1.- ¿Para qué sirve nothing?
- [x] Es un valor centinela para no renderizar nada
- [ ] Nothing no existe

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 2.- ¿Cuáles son maneras de no renderizar nada en Lit? 
- [x] return html\`<user-name>${this.userName ?? null}</user-name>\`;
- [x] return html\`<user-name>${this.userName ?? nothing}</user-name>\`;
- [ ] return html\`<user-name>${this.userName ?? empty}</user-name>\`;
- [x] return html\`<user-name>${this.userName ?? undefined}</user-name>\`;
- [x] return html\`<user-name>${this.userName ?? ''}</user-name>\`;

💡 **Explicación:** The empty string '', null, and undefined are specially treated and render nothing

🔗 **Recursos:** https://lit.dev/docs/templates/expressions/#removing-child

<br>

### 3.- ¿Cuál es el Binding correcto para un atributo?
- [ ] html\`\<div class=(${highlightClass})>\</div>\`
- [ ] html\`\<div .class=${highlightClass}>\</div>\`
- [x] html\`\<div class=${highlightClass}>\</div>\`
- [ ] html\`\<div .class=(highlightClass)>\</div>\`

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 4.- ¿Cuál es el Binding correcto para una propiedad?
- [x] html\`\<input .value=${value}>`
- [ ] html\`\<input value=${value}>` 
- [ ] html\`\<input .value=(value)>`
- [ ] html\`\<input value=(${value})>`

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 5.- ¿Cuál es el Binding correcto para atributos booleanos?
- [ ] html\`\<div ?hidden=$(!show)>\</div>\`
- [ ] html\`\<div .hidden=${!show}>\</div>\`
- [ ] html\`\<div hidden=$(!show)>\</div>\`
- [x] html\`\<div ?hidden=${!show}>\</div>\`

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 6.- ¿Cuál es el Binding correcto para un evento?
- [ ] html\`<button ?click=$(this._clickHandler)>Go</button>`
- [x] html\`<button @click=${this._clickHandler}>Go</button>`
- [ ] html\`<button ?click=${this._clickHandler}>Go</button>`
- [ ] html\`<button @click=$(this._clickHandler)>Go</button>`

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 7.- Binding que de error

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 8.-  correcto para static properties type String
```javascript
  import { LitElement, html } from 'lit';

  export class SimpleGreeting extends LitElement {
    static properties = {
      name: { type: String },
    };

    constructor() {
      super();
      this.name = 'Somebody';
    }

    render() {
      return html`<p>Hello, ${this.name}!</p>`;
    }
  }

  customElements.define('simple-greeting', SimpleGreeting);
```
- [x] \<simple-greeting name="World">\</simple-greeting>
- [ ] \<simple-greeting name=${World}>\</simple-greeting>
- [ ] \<simple-greeting .name="World">\</simple-greeting>
- [ ] \<simple-greeting name=("World")>\</simple-greeting>

💡 **Explicación:** PREGUNTAR A MAX

🔗 **Recursos:** 

<br>

### 9.-  para static properties type Array
```javascript
  import { LitElement, html } from 'lit';

  export class SimpleGreeting extends LitElement {
    static properties = {
      name: { type: Array },
    };

    constructor() {
      super();
      this.name = 'Somebody';
    }

    render() {
      return html`<p>Hello, ${this.name}!</p>`;
    }
  }

  customElements.define('simple-greeting', SimpleGreeting);
```
- [ ] \<simple-greeting name="Earth, Moon, Mars">\</simple-greeting>
- [ ] \<simple-greeting name=${"Earth","Moon","Mars"}>\</simple-greeting>
- [ ] \<simple-greeting .name=["Earth","Moon","Mars"]>\</simple-greeting>
- [x] \<simple-greeting name=["Earth","Moon","Mars"]>\</simple-greeting>

💡 **Explicación:** OMITIR - NO ESTOY SEGURO SI ESTÁ BIEN

🔗 **Recursos:** 

<br>

### 10.-  para static properties type objeto

💡 **Explicación:** PREGUNTAR A MAX

🔗 **Recursos:** 

<br>

### 11.- ¿Cuál es la manera correcta de renderizar condicionalmente?
- [x] <code>
  ```javascript
  render() {
    return this.userName
      ? html`Welcome ${this.userName}`
      : html`Please log in <button>Login</button>`;
  }
  ```
</code>

- [ ] <code>
  ```javascript
  render (
    return this.userName
      ? html`Welcome ${this.userName}`
      : html`Please log in <button>Login</button>`;
  )
  ```
</code>

- [ ] <code>
  ```javascript
  render() {
    return this.userName
      && html`Welcome ${this.userName}`
      ? html`Please log in <button>Login</button>`;
  }
  ```
</code>

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 12.- ¿Para qué sirve la opción de propiedad reflect? 
- [ ] Refleja las propiedades hacia el padre
- [ ] Refleja las propiedades como atributos y viceversa.
- [ ] Reflect no existe
- [x] Refleja la propiedad al atributo asociado

💡 **Explicación:** -PENDIENTE REVISAR-

🔗 **Recursos:** 

<br>

### 13.- ciclo de vida update

### 14.- Name=${this.name}
.name="nombre"
Fullname= {this.name}
.fullname="nombre"

💡 **Explicación:** ALGUIEN LO ESCRIBIÓ EN WHATS PERO NO RECUERDO LA PREGUNTA

🔗 **Recursos:** 

<br>

### 15.- De lit también, un contador con intervalos de un segundo, lo declara en el constructor el setInterval y la pregunta dice, que mostrará después de 5 segundos.

💡 **Explicación:** ALGUIEN LO ESCRIBIO EN WHATS PERO NO RECUERDO LA PREGUNTA

🔗 **Recursos:** 

<br>

### 16.- que hace la funcion firstupdated

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 17.- ¿Cuál es el resultado del Array color?
```javascript
  import { LitElement, html } from 'lit';

  class MyElement extends LitElement {
    static properties = {
      colors: { type: Array },
    };

    constructor() {
      super();
      this.colors = ['Rojo', 'Verde', 'Negro', 'Azul'];
    }

    render() {
      return html`
        <ul>
          ${this.colors.map(color => html`
            <li style="color:${color}">${color}</li>
          `)}
        </ul>
      `;
    }
  }
  customElements.define('my-element', MyElement);
```
- [ ] Rojo, Verde Negro, Azul (con sus respectivos colores)
- [x] Rojo, Verde Negro, Azul (todo negro)
- [ ] Rojo, Verde Negro, Azul (colores invertidos)
- [ ] error

💡 **Explicación:** Los colores tendrían que estar en inglés para funcionar

🔗 **Recursos:** 

<br>

### 18.- De las siguientes palabras ¿Cuál es una palabra reservada de Lit?
- [ ] do
- [ ] map
- [x] ifdefined
- [ ] null

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 19.- Este método es llamado cada vez que se asigna un valor a una propiedad reactiva
- [ ] 
- [ ] 
- [ ] 
- [x] hasChanged

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 20.- ¿Cuál de las opciones de la propiedad name obtendrá el valor "Some Name"?
```javascript
  import { LitElement, html } from 'lit';

  export class MyWebComponent extends LitElement {
    static get properties() {
      return {
        name: {
          type: String,
          attribute: 'fullname'
        }
      }
    };

    render() {
      return html`
        <p>${this.name}</p>
      `
    };
  }

  customElements.define('my-web-component', MyWebComponent);
```
- [ ] \<my-webcomponent .fullname="Some Name"></my-webcomponent>
- [ ] \<my-webcomponent name="Some Name"></my-webcomponent>
- [x] \<my-webcomponent fullname="Some Name"></my-webcomponent>
- [ ] \<my-webcomponent .name="Some Name"></my-webcomponent>

💡 **Explicación:** el nuevo nombre es fullname, es posible asignarlo como atributo ya que los atributos solo reciben strings, además si el componente se está llamando desde el HTML no reconocerá la sintaxis de propiedad (el punto .)

🔗 **Recursos:** 

<br>


### 21.- ¿Cuál es la manera correcta de renderizar la siguiente lista?
```javascript
  const list = ['Peas', 'Carrots', 'Tomatoes'];
  // 0:Peas
  // 1:Carrots
  // 2:Tomatoes
```
- [x] ```${this.list.map((item, index) => html`<li>${index}:${item}</li>`)}```
- [ ] ```${this.list.map((index, item) => html`<li>${index}:${item}</li>`)}```
- [ ] ```${this.list.map(item, index => html`<li>${index}:${item}</li>`)}```
- [ ] ```${this.list.map((item, index) => html`<li>${index}:${item}</li>`)}```

# Conceptos Generales

### 1.- Una petición a una API devuelve un código exitoso pero la espuesta está vacía, ¿Cuál es el código?
 - [ ] 201
 - [ ] 200
 - [ ] 203
 - [x] 204

💡 **Explicación:** La petición se ha completado con éxito pero su respuesta no tiene ningún contenido

🔗 **Recursos:** https://developer.mozilla.org/es/docs/Web/HTTP/Status

<br>

### 2- ¿Cuál es el método HTTP para actualizar parcialmente un recurso?
- [ ] PUT
- [x] PATCH
- [ ] POST 
- [ ] DELETE

💡 **Explicación:** El método PATCH es utilizado para aplicar modificaciones parciales a un recurso.

🔗 **Recursos:** https://developer.mozilla.org/es/docs/Web/HTTP/Methods

<br>

### 2- ¿Cuál es el método HTTP para actualizar completamente un recurso?
- [x] PUT
- [ ] PATCH
- [ ] POST 
- [ ] DELETE

💡 **Explicación:** El método PUT reemplaza todas las representaciones actuales del recurso.

🔗 **Recursos:** https://developer.mozilla.org/es/docs/Web/HTTP/Methods

<br>

### 3.- Elige la definición que se adapte a cada concepto.
- [x] **sobrecarga:** 2 o más metodos con el mismo nombre y diferente funcionalidad. **sobreescritura:** extender la funcionalidad que tiene un método en una clase específica.
- [ ] **sobrecarga:** extender la funcionalidad que tiene un método en una clase específica. **sobreescritura:** 2 o más metodos con el mismo nombre y diferente funcionalidad.

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 4.- ¿Qué indica el código HTTP 401?
- [x] Es necesario autenticar para obtener la respuesta solicitada.
- [ ] No posee los permisos necesarios, por lo que el servidor rechaza otorgar una respuesta.
- [ ] El servidor no pudo encontrar el contenido solicitado.
- [ ] El servidor no pudo interpretar la solicitud dada una sintaxis inválida.

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 5.- ¿Cuál es el código HTTP que describe: el método solicitado no está soportado por el servidor y no puede ser manejado?
- [ ] 500
- [ ] 502
- [x] 501
- [ ] 503

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 6.- Esta cabecera indica el tipo que el cliente envía en la solicitud al servidor (para saber el tipo de contenido)
- [ ] Cache-Control
- [ ] Content-Encoding
- [x] Content-Type
- [ ] No existe


💡 **Explicación:** Content-Type indica el tipo del medio del recurso.

🔗 **Recursos:** https://developer.mozilla.org/es/docs/Web/HTTP/Headers#mensajes_sobre_la_informaci%C3%B3n_del_cuerpo_body

<br>

### 7.- ¿Cuál de los siguientes es un objeto de javascript del lado del servidor?
- [ ] función
- [x] archivo
- [ ] carga de un archivo
- [ ] fecha

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 8.- ¿JavaScript se puede usar para almacenar el contenido del formulario en un archivo de la base de datos en el servidor?
- [x] false
- [] true

💡 **Explicación:** Me parece un poco engañosa, creo que si se podría con NodeJS

🔗 **Recursos:** 

<br>

### 9.- ¿Cuál de los siguientes se usa en JavaScript para insertar caracteres especiales?
- [ ] &
- [x] \
- [ ] -
- [ ] %

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 10.- ¿Cómo almacena JavaScript las fechas en objetos de tipo Fecha?
- [ ] El número de días desde el 1 de enero de 1900.
- [ ] El número de segundos desde el 1 de enero de 1970.
- [x] El número de milisegundos desde el 1 de enero de 1970.
- [ ] El número de picosegundos desde el 1 de enero de 1970.

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 11.- ¿El nivel de bloque de estilo C no es soportado en JavaScript?
- [ ] False
- [x] True

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 12.- JavaScript ignora los espacios extra
- [ ] False
- [ ] True

💡 **Explicación:** -IMPORTANTE- PENDIENTE

🔗 **Recursos:** 

<br>

### 13.- ¿Cuál de las siguientes es correcta para escribir “â€œHello Worldâ€ en la página web?
- [ ] System.out.println(â€œHello Worldâ€)
- [ ] print(â€œHello Worldâ€)
- [x] document.write(â€œHello Worldâ€)
- [ ] response.write(â€œHello Worldâ€) 

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 14.- ¿Cuál de las siguientes es la propiedad contaminada de un objeto de ventana en JavaScript?
- [ ] Pathname
- [ ] Protocol
- [x] Defaultstatus
- [ ] Host

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 15.- ¿Qué atributo debe cambiarse para que los elementos sean invisibles?
- [x] visibilty
- [ ] visible
- [ ] invisibility
- [ ] invisible

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 16.- ¿Cuál de los siguientes se usa para capturar todos los eventos de clic en una ventana?
- [x] window.captureEvents(Event.CLICK); 
- [ ] window.routeEvents(Event.CLICK );
- [ ] window.handleEvents(Event.CLICK); 
- [ ] window.raiseEvents(Event.CLICK );

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 17.- ¿Cuál de las siguientes formas es incorrecta para instanciar una fecha?
- [ ] new Date(dateString) 
- [ ] new Date() 
- [x] new Date(seconds) 
- [ ] new Date(year, month, day, hours, minutes, seconds, milliseconds)

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 18.- ¿Cuál de los siguientes es un objeto JavaScript del lado del cliente?
- [ ] archivo
- [ ] función
- [x] carga de archivo
- [ ] tiempo 

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 19.- ¿Es posible declarar una variable en Java Script junto con su tipo?
- [x] Si
- [ ] No

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 20.- _____ JavaScript también se llama JavaScript del lado del cliente.
- [ ] Microsoft
- [x] Navigator
- [ ] LiveWire
- [ ] Native

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 21.- Las entidades de JavaScript comienzan con ____________ y ​​terminan con ______________ 
- [ ] ; semicolon : dos puntos
- [ ] ; Semicolon & Ampersand
- [ ] & Ampersand : dos puntos
- [x] & Ampersand ; semicolon

💡 **Explicación:** 

🔗 **Recursos:** 

<br>

### 22.- De acuerdo con la definición de encapsulamiento, ¿Cuál de las siguientes atributos debe ser encapsulado?
```javascript
  persona: {
    nombre: String,
    edad: Number,
    fecha_nacimiento: Date,
    nacionalidad: String
  }
```
- [ ] nacionalidad
- [ ] nombre
- [ ] edad
- [x] fecha_nacimiento

💡 **Explicación:** IMPORTANTE- PENDIENTE PREGUNTAR A DYLAN

🔗 **Recursos:** 

<br>

### 23.- ¿Qué indican los códigos HTTP 300?
- [ ] Error del servidor
- [x] Redirecciones 
- [ ] Error del cliente
- [ ] Respuesta informativa

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 24.- Es el método HTTP que se utiliza para solicitar un recurso a una API.
- [x] GET 
- [ ] PUT 
- [ ] POST
- [ ] SEND

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 25.- Código HTTP que regresa si un cliente tiene prohibido el acceso
- [ ] 404
- [ ] 400
- [ ] 401
- [x] 403 

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 26.- Son tipos de polimorfismo
- [x] sobrecarga
- [x] parametrico
- [x] redefinición
- [ ] encapsulamiento

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 27.- Cabecera que indica el tipo que el cliente puede entender como respuesta
- [ ] 
- [ ] 
- [ ] 
- [x] accept

💡 **Explicación:**

🔗 **Recursos:** 

<br>

# Estructuras de Datos

### 1.- Esta estructura trabaja con un mecanismo First in - First out
- [ ] 
- [ ] pila
- [x] cola
- [ ] 

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 2.- Esta estructura trabaja con un mecanismo Last in - First out
- [ ] 
- [x] pila
- [ ] cola
- [ ] 

💡 **Explicación:**

🔗 **Recursos:** 

<br>

# Patrones de Diseño

### 1.- Es una solución general reutilizable y que aplica a diferentes problemas cuando se desarrolla software
- [ ] POO
- [x] Patrones de Diseño
- [ ] Clases
- [ ] Objetos

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 2- El siguiente patrón de diseño define un mecanismo para modificar a uno o varios objetos sobre cualquier evento que ocurra con el objeto que se monitorea.
- [ ] 
- [ ] 
- [ ] 
- [x] Observer

💡 **Explicación:**

🔗 **Recursos:** 

<br>

### 3.- Es un patrón de diseño creacional que proporciona una interfaz para crear objetos en una superclase, mientras permite a las subclases alterar el tipo de objetos que se crearán.
- [ ] 
- [ ] 
- [x] Factory Method
- [ ] 

💡 **Explicación:**

🔗 **Recursos:** 

<br>