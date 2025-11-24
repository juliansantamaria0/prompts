# 30 Prompts correccion - JavaScript Junior

## Prompt 1

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comentaré anteriormente y cómo me responderás.

### contexto

Enséñame a validar un formulario simple en JavaScript (nombre y correo). Dame el código paso a paso.apa inicial de aprendizaje, he tenido dificultades para entender los conceptos del `hoisting` en JavaScript, pese a que yo los implemente dentro de mi código, pero lo hago sin entender su concepto.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

```js
// El hoisting en JavaScript se puede entender con variables de la siguiente manera:
console.log(x); // undefined
var x = 5;
console.log(x); // 5
````

En donde:

1. JavaScript "eleva" la declaración de `x` al inicio del scope
2. La asignación del valor permanece en su lugar original
3. Por eso la primera línea muestra `undefined` en lugar de error

### Pregunta #1

Explícame, paso a paso, cómo funciona el `hoisting` en JavaScript usando ejemplos sencillos. Quiero que el resultado sea una explicación en lenguaje fácil.

---

## Prompt 2

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comentaré anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, he tenido dificultades para entender las diferencias entre `var`, `let` y `const`, pese a que los uso en mi código, pero no comprendo cuándo es apropiado usar cada uno.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

La diferencia entre las declaraciones se puede ver así:

```js
// var - Scope de función
function ejemploVar() {
  var x = 1;
  if (true) {
    var x = 2; // Misma variable
    console.log(x); // 2
  }
  console.log(x); // 2
}

// let - Scope de bloque
function ejemploLet() {
  let y = 1;
  if (true) {
    let y = 2; // Variable diferente
    console.log(y); // 2
  }
  console.log(y); // 1
}

// const - No puede reasignarse
const z = 3;
z = 4; // Error: Assignment to constant variable
```

### Pregunta #2

Ayúdame a entender la diferencia entre `var`, `let` y `const`. Dame ejemplos y dime cuándo debería usar cada uno.

---

## Prompt 3

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comentaré anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, me encuentro con errores en mi código que no comprendo, específicamente cuando intento usar variables antes de declararlas con `let`.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### código:

```js
// ❌ ERROR
console.log(x); 
let x = 5;
```

### Pregunta #3

¿Por qué el siguiente código en JavaScript da error y cómo podría corregirse? Explícame de forma clara y sencilla.

---

## Prompt 4

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comentaré anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, he tenido dificultades para entender el concepto de 'scope' o alcance de las variables, especialmente cuando trabajo con funciones y bloques de código.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

El scope determina dónde podemos acceder a las variables:

```js
// Scope global
let global = "Accesible en todo el código";

function miFuncion() {
  // Scope de función
  let local = "Solo accesible aquí";
  console.log(global); // ✅ Funciona
  console.log(local);  // ✅ Funciona

  if (true) {
    // Scope de bloque
    let bloque = "Solo en este bloque";
    console.log(local); // ✅ Funciona
  }
  console.log(bloque); // ❌ Error: bloque is not defined
}

console.log(local); // ❌ Error: local is not defined
```

### Pregunta #4

Quiero entender qué es el 'scope' en JavaScript. Explícalo usando ejemplos de funciones y bloques.

---

## Prompt 5

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comentaré anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, he visto código con funciones flecha (=>) pero no comprendo bien sus diferencias con las funciones tradicionales ni cuándo debería usar cada una.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Las funciones flecha tienen una sintaxis más concisa:

```js
// Función tradicional
function sumar(a, b) {
  return a + b;
}

// Función flecha equivalente
const sumar = (a, b) => a + b;

// Con más líneas
const procesarDatos = (datos) => {
  const resultado = datos * 2;
  return resultado;
};

// Diferencia importante con 'this'
const objeto = {
  nombre: "Juan",
  saludar: function() {
    console.log("Hola, soy " + this.nombre);
  },
  despedir: () => {
    console.log("Adiós, soy " + this.nombre); // undefined
  }
};
```

### Pregunta #5

Explícame qué es exactamente una función flecha en JavaScript y compárala con una función tradicional. Dame casos de uso.

---

## Prompt 6

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comentaré anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender los métodos de arrays, específicamente `.map()`, ya que veo que se usa mucho en código moderno pero no comprendo su funcionamiento.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

El método `.map()` transforma cada elemento de un array:

```js
const numeros = [1, 2, 3, 4, 5];

const duplicados = numeros.map(num => num * 2);
console.log(duplicados); // [2, 4, 6, 8, 10]

const cuadrados = numeros.map(num => num ** 2);
console.log(cuadrados); // [1, 4, 9, 16, 25]

console.log(numeros); // [1, 2, 3, 4, 5]
```

En donde:

1. `.map()` recorre cada elemento del array
2. Aplica una función a cada elemento
3. Retorna un nuevo array con los resultados
4. El array original permanece sin cambios

### Pregunta #6

¿Qué hace el método `.map()` en JavaScript? Dame un ejemplo práctico con un arreglo de números.

---

## Prompt 7

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, escucho mucho sobre los "callbacks" pero no comprendo qué son exactamente ni cómo funcionan en JavaScript.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Un callback es una función que se pasa como argumento:

```js
function procesarUsuario(nombre, callback) {
  console.log("Procesando usuario: " + nombre);
  callback(nombre);
}

function saludar(nombre) {
  console.log("¡Hola, " + nombre + "!");
}

procesarUsuario("Juan", saludar);
// Salida:
// "Procesando usuario: Juan"
// "¡Hola, Juan!"

// Callback inline
procesarUsuario("María", function(nombre) {
  console.log("Bienvenida, " + nombre);
});

// Callback con función flecha
procesarUsuario("Pedro", (nombre) => {
  console.log("Hola " + nombre + ", ¿cómo estás?");
});
```

### Pregunta #7

Dame una explicación clara de qué son los callbacks en JavaScript y muéstrame cómo crear uno desde cero.

---

## Prompt 8

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito comprender el asincronismo y las promesas, ya que es un concepto que me resulta confuso cuando trabajo con operaciones que toman tiempo.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Las promesas manejan operaciones asíncronas:

```js
const miPromesa = new Promise((resolve, reject) => {
  setTimeout(() => {
    const exito = true;
    if (exito) {
      resolve("¡Operación exitosa!");
    } else {
      reject("Error en la operación");
    }
  }, 2000);
});

miPromesa
  .then(resultado => {
    console.log(resultado);
  })
  .catch(error => {
    console.log(error);
  });

function obtenerUsuario(id) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      if (id > 0) {
        resolve({ id: id, nombre: "Juan" });
      } else {
        reject("ID inválido");
      }
    }, 1000);
  });
}
```

### Pregunta #8

Explícame paso a paso cómo funciona el asincronismo en JavaScript usando promesas.

---

## Prompt 9

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, tengo una función que no devuelve el valor esperado y no comprendo por qué está fallando.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Código:

```js
// ❌ INCORRECTO
function saludar(nombre) {
  return;
  "Hola " + nombre;
}
```

### Pregunta #9

Tengo una función en JavaScript que no está devolviendo el valor esperado, ¿puedes explicarme por qué y cómo puedo corregirla? Explícame de forma sencilla.

---

## Prompt 10

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender qué es el DOM y cómo puedo manipular elementos HTML desde JavaScript.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

```html
<!DOCTYPE html>
<html>
<body>
  <h1 id="titulo">Texto Original</h1>
  <button onclick="cambiarTexto()">Cambiar</button>

  <script>
    function cambiarTexto() {
      const elemento = document.getElementById("titulo");
      elemento.textContent = "¡Texto Cambiado!";
      elemento.style.color = "blue";
    }
  </script>
</body>
</html>
```

En donde:

1. `document` representa toda la página HTML
2. `getElementById()` busca un elemento por su atributo `id`
3. `textContent` cambia el texto del elemento
4. `style` permite modificar estilos CSS

### Pregunta #10

Enséñame qué es el DOM en JavaScript y dame un ejemplo básico para cambiar el texto de un elemento HTML.

---

## Prompt 11

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, me confundo con los operadores de comparación `==` y `===`, no entiendo cuándo usar cada uno.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

La diferencia está en la conversión de tipos:

```js
// == (igualdad débil)
console.log(5 == "5");    // true
console.log(true == 1);   // true
console.log(null == undefined); // true

// === (igualdad estricta)
console.log(5 === "5");   // false
console.log(true === 1);  // false
console.log(null === undefined); // false

const edad = "18";

if (edad == 18) {
  console.log("Igual con =="); // ✅ Se ejecuta
}

if (edad === 18) {
  console.log("Igual con ==="); // ❌ No se ejecuta
}

// Recomendación: SIEMPRE usa ===
if (edad === "18") {
  console.log("Correcto"); // ✅ Se ejecuta
}
```

### Pregunta #11

Dime cuál es la diferencia entre `==` y `===` en JavaScript y dame ejemplos simples.

---

## Prompt 12

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito comprender mejor cómo funcionan los objetos y cómo puedo manipular sus propiedades dinámicamente.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Los objetos son colecciones de propiedades:

```js
const persona = {
  nombre: "Juan",
  edad: 25,
  ciudad: "Madrid"
};

console.log(persona.nombre);    // "Juan"
console.log(persona["edad"]);   // 25

persona.profesion = "Desarrollador";
persona["hobby"] = "Programar";

console.log(persona);

delete persona.ciudad;
delete persona["hobby"];

console.log(persona);

persona.edad = 26;
persona["nombre"] = "Juan Carlos";
```

### Pregunta #12

Explícame qué es un objeto en JavaScript y cómo puedo añadir y eliminar propiedades.

---

## Prompt 13

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, veo que hay varios métodos para trabajar con arrays (`.filter()`, `.map()`, `.reduce()`) pero no comprendo sus diferencias ni cuándo usar cada uno.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Cada método tiene un propósito específico:

```js
const numeros = [1, 2, 3, 4, 5, 6];

// .filter() - Filtra elementos
const pares = numeros.filter(num => num % 2 === 0);
console.log(pares); // [2, 4, 6]

// .map() - Transforma elementos
const duplicados = numeros.map(num => num * 2);
console.log(duplicados); // [2, 4, 6, 8, 10, 12]

// .reduce() - Reduce a un valor
const suma = numeros.reduce((acumulador, num) => acumulador + num, 0);
console.log(suma); // 21

const productos = [
  { nombre: "Laptop", precio: 1000, stock: 5 },
  { nombre: "Mouse", precio: 20, stock: 15 },
  { nombre: "Teclado", precio: 50, stock: 0 }
];

const disponibles = productos.filter(p => p.stock > 0);
const nombres = productos.map(p => p.nombre);
const valorTotal = productos.reduce((total, p) => {
  return total + (p.precio * p.stock);
}, 0);
```

### Pregunta #13

Quiero entender qué son los métodos `.filter()`, `.map()` y `.reduce()`. Compáralos y dame ejemplos aplicados.

---

## Prompt 14

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender cómo manejar errores en mi código para que no se detenga cuando algo falla.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

El bloque try-catch captura errores:

```js
function dividirSeguro(a, b) {
  try {
    if (b === 0) {
      throw new Error("No se puede dividir por cero");
    }
    return a / b;
  } catch (error) {
    console.log("Error capturado: " + error.message);
    return null;
  } finally {
    console.log("Operación finalizada");
  }
}

try {
  const datos = JSON.parse('{"nombre": "Juan"}');
  console.log(datos.nombre);

  const datosMalos = JSON.parse('texto inválido');
  console.log(datosMalos);
} catch (error) {
  console.log("Error al parsear JSON: " + error.message);
}

console.log("El programa continúa ejecutándose");
```

### Pregunta #14

Explícame cómo funciona `try...catch` en JavaScript con un ejemplo donde haya un error real.

---

## Prompt 15

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, escucho mucho sobre las APIs pero no entiendo qué son ni cómo puedo consumirlas desde mi código.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Una API es como un menú de restaurante:

```js
fetch('https://jsonplaceholder.typicode.com/users/1')
  .then(response => response.json())
  .then(usuario => {
    console.log("Nombre: " + usuario.name);
    console.log("Email: " + usuario.email);
  })
  .catch(error => {
    console.log("Error: " + error);
  });

async function obtenerDatos() {
  try {
    const respuesta = await fetch('https://api.ejemplo.com/datos');

    if (!respuesta.ok) {
      throw new Error('Error en la petición');
    }

    const datos = await respuesta.json();
    console.log(datos);
  } catch (error) {
    console.log("Error al obtener datos: " + error.message);
  }
}
```

En donde:

1. La API es un "servidor" que nos da información
2. `fetch()` es como hacer un "pedido" a ese servidor
3. La respuesta viene en formato JSON (datos estructurados)
4. Usamos `.then()` o `async/await` para esperar la respuesta

### Pregunta #15

Dame una analogía sencilla para entender qué es una API y cómo se consume desde JavaScript con `fetch()`.

---

## Prompt 16

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender qué es JSON y cómo puedo convertir datos entre objetos JavaScript y formato JSON.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

JSON es un formato de texto para intercambiar datos:

```js
// Objeto JavaScript
const persona = {
  nombre: "Juan",
  edad: 25,
  activo: true,
  hobbies: ["programar", "leer"]
};

// Convertir objeto a JSON (stringify)
const personaJSON = JSON.stringify(persona);
console.log(personaJSON);
// '{"nombre":"Juan","edad":25,"activo":true,"hobbies":["programar","leer"]}'

console.log(typeof personaJSON); // "string"

// Convertir JSON a objeto (parse)
const personaObjeto = JSON.parse(personaJSON);
console.log(personaObjeto);
// { nombre: 'Juan', edad: 25, activo: true, hobbies: ['programar', 'leer'] }

console.log(typeof personaObjeto); // "object"
console.log(personaObjeto.nombre); // "Juan"

// Uso práctico: guardar en localStorage
localStorage.setItem('usuario', JSON.stringify(persona));
const usuarioGuardado = JSON.parse(localStorage.getItem('usuario'));
```

### Pregunta #16

Explícame qué es JSON y muéstrame cómo convertir un objeto a JSON y viceversa.

---

## Prompt 17

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, escucho términos técnicos sobre JavaScript como "lenguaje interpretado" y "single-threaded" pero no comprendo qué significan.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

JavaScript funciona de manera especial:

```js
// INTERPRETADO: El código se ejecuta línea por línea
console.log("Línea 1");
console.log("Línea 2");
console.log("Línea 3");
// No necesita compilarse antes de ejecutarse

// SINGLE-THREADED: Una sola tarea a la vez
console.log("Inicio");

// Operación síncrona (bloquea)
for (let i = 0; i < 1000000000; i++) {
  // Esto bloquea todo hasta terminar
}

console.log("Fin del bucle");

// Por eso usamos asincronismo
console.log("Inicio async");

setTimeout(() => {
  console.log("Esto se ejecuta después");
}, 0);

console.log("Fin async");

// Salida:
// "Inicio async"
// "Fin async"
// "Esto se ejecuta después"
```

En donde:

1. **Interpretado**: No se compila, se ejecuta directamente
2. **Single-threaded**: Ejecuta una operación a la vez
3. El Event Loop permite manejar tareas asíncronas
4. Por eso es importante entender async/await

### Pregunta #17

¿Qué significa que JavaScript sea un lenguaje interpretado y de un solo hilo? Dame una explicación para principiantes.

---

## Prompt 18

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender qué son las clases en JavaScript y cómo puedo crear instancias de ellas.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Las clases son plantillas para crear objetos:

```js
// Definir una clase
class Persona {
  constructor(nombre, edad) {
    this.nombre = nombre;
    this.edad = edad;
  }

  saludar() {
    console.log(`Hola, soy ${this.nombre} y tengo ${this.edad} años`);
  }

  cumplirAnios() {
    this.edad++;
    console.log(`Ahora tengo ${this.edad} años`);
  }
}

// Crear instancias (objetos) de la clase
const persona1 = new Persona("Juan", 25);
const persona2 = new Persona("María", 30);

persona1.saludar(); // "Hola, soy Juan y tengo 25 años"
persona2.saludar(); // "Hola, soy María y tengo 30 años"

persona1.cumplirAnios(); // "Ahora tengo 26 años"

// Cada instancia es independiente
console.log(persona1.edad); // 26
console.log(persona2.edad); // 30
```

En donde:

1. `class` define la plantilla
2. `constructor()` inicializa los valores
3. Los métodos son funciones de la clase
4. `new` crea una nueva instancia

### Pregunta #18

Enséñame cómo crear una clase en JavaScript y cómo instanciarla con `new`. Usa un ejemplo simple.

---

## Prompt 19

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, me confunde el comportamiento de `this` porque parece cambiar su valor dependiendo del contexto.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

`this` cambia según el contexto:

```js
// 1. En un objeto - this es el objeto
const persona = {
  nombre: "Juan",
  saludar: function() {
    console.log("Hola, soy " + this.nombre);
  }
};
persona.saludar(); // "Hola, soy Juan"

// 2. En una función normal - this es window (en navegador)
function mostrar() {
  console.log(this);
}
mostrar(); // Window {...}

// 3. En una función flecha - this del contexto padre
const objeto = {
  nombre: "María",
  metodo1: function() {
    console.log(this.nombre); // "María"

    const funcionFlecha = () => {
      console.log(this.nombre); // "María" (hereda this)
    };
    funcionFlecha();
  },
  metodo2: function() {
    console.log(this.nombre); // "María"

    function funcionNormal() {
      console.log(this.nombre); // undefined
    }
    funcionNormal();
  }
};

// 4. En un event listener - this es el elemento
const boton = document.querySelector('button');
boton.addEventListener('click', function() {
  console.log(this); // <button>...</button>
});
```

### Pregunta #19

Explícame qué es `this` en JavaScript con ejemplos donde cambie su valor según el contexto.

---

## Prompt 20

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender cómo usar `localStorage` para guardar información en el navegador del usuario.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

localStorage guarda datos en el navegador:

```js
// Guardar datos
localStorage.setItem('nombre', 'Juan');
localStorage.setItem('edad', '25');

// Guardar objetos (convertir a JSON)
const usuario = {
  nombre: 'María',
  email: 'maria@ejemplo.com'
};
localStorage.setItem('usuario', JSON.stringify(usuario));

// Obtener datos
const nombre = localStorage.getItem('nombre');
console.log(nombre); // "Juan"

const edad = localStorage.getItem('edad');
console.log(edad); // "25"

// Obtener objetos (convertir de JSON)
const usuarioGuardado = localStorage.getItem('usuario');
const usuarioObjeto = JSON.parse(usuarioGuardado);
console.log(usuarioObjeto.nombre); // "María"

// Borrar un dato específico
localStorage.removeItem('edad');

// Borrar todo
localStorage.clear();

// Verificar si existe
if (localStorage.getItem('nombre')) {
  console.log('El nombre existe');
} else {
  console.log('No hay nombre guardado');
}
```

En donde:

1. Los datos persisten aunque cierres el navegador
2. Solo guarda strings (usa JSON para objetos)
3. Los datos son por dominio (cada sitio web tiene su propio localStorage)

### Pregunta #20

Quiero aprender a usar `localStorage`. Explícame cómo guardar, obtener y borrar datos.

---

## Prompt 21

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, tengo un bucle con `setTimeout` que no funciona como espero y no entiendo por qué.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### código:

```js
// ❌ 
console.log("Con var:");
for (var i = 0; i < 5; i++) {
  setTimeout(() => console.log(i), 1000);
}
```

### Pregunta #21

¿Por qué este código da el mismo resultado en todas las funciones? Explícame cómo puedo evitar esto usando `let` en lugar de `var`.

---

## Prompt 22

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender cómo usar `async` y `await` para hacer peticiones a APIs de forma más legible.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

async/await simplifica las promesas:

```js
// Con .then() - más difícil de leer
function obtenerUsuarioThen() {
  fetch('https://jsonplaceholder.typicode.com/users/1')
    .then(response => response.json())
    .then(usuario => {
      console.log("Usuario:", usuario.name);
      return fetch(`https://jsonplaceholder.typicode.com/posts?userId=${usuario.id}`);
    })
    .then(response => response.json())
    .then(posts => {
      console.log("Posts:", posts.length);
    })
    .catch(error => console.log("Error:", error));
}

// Con async/await - más claro
async function obtenerUsuarioAsync() {
  try {
    // await espera a que termine
    const response = await fetch('https://jsonplaceholder.typicode.com/users/1');
    const usuario = await response.json();
    console.log("Usuario:", usuario.name);

    const postsResponse = await fetch(`https://jsonplaceholder.typicode.com/posts?userId=${usuario.id}`);
    const posts = await postsResponse.json();
    console.log("Posts:", posts.length);
  } catch (error) {
    console.log("Error:", error);
  }
}

// Llamar la función
obtenerUsuarioAsync();

// async siempre retorna una promesa
async function sumar(a, b) {
  return a + b;
}

sumar(2, 3).then(resultado => console.log(resultado)); // 5
```

### Pregunta #22

Enséñame cómo usar `async` y `await` con un ejemplo sencillo que haga un `fetch` a una API pública.

---

## Prompt 23

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender qué son los módulos y cómo puedo organizar mi código en diferentes archivos.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Los módulos organizan el código en archivos:

```js
// ===== archivo: matematicas.js =====
// Exportar funciones individuales
export function sumar(a, b) {
  return a + b;
}

export function restar(a, b) {
  return a - b;
}

// Exportar por defecto
export default function multiplicar(a, b) {
  return a * b;
}

// Exportar constantes
export const PI = 3.1416;

// ===== archivo: utilidades.js =====
// Exportar todo junto
function formatearNombre(nombre) {
  return nombre.toUpperCase();
}

function validarEmail(email) {
  return email.includes('@');
}

export { formatearNombre, validarEmail };

// ===== archivo: app.js (principal) =====
// Importar funciones específicas
import { sumar, restar, PI } from './matematicas.js';

// Importar el export default
import multiplicar from './matematicas.js';

// Importar todo con alias
import * as utils from './utilidades.js';

console.log(sumar(5, 3));        // 8
console.log(restar(10, 4));      // 6
console.log(multiplicar(3, 4));  // 12
console.log(PI);                 // 3.1416

console.log(utils.formatearNombre('juan')); // "JUAN"
```

En HTML:

```html
<script type="module" src="app.js"></script>
```

### Pregunta #23

Explícame qué son los módulos en JavaScript y cómo funcionan `import` y `export` con ejemplos.

---

## Prompt 24

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, escucho mucho sobre el "event loop" pero no comprendo cómo JavaScript maneja las tareas asíncronas.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

El Event Loop gestiona la ejecución del código:

```js
console.log("1. Inicio");

setTimeout(() => {
  console.log("2. setTimeout");
}, 0);

Promise.resolve().then(() => {
  console.log("3. Promise");
});

console.log("4. Fin");

// Orden de ejecución:
// "1. Inicio"
// "4. Fin"
// "3. Promise"
// "2. setTimeout"

// Explicación:
// 1. Código síncrono se ejecuta primero
// 2. Microtareas (Promises) tienen prioridad
// 3. Macrotareas (setTimeout) se ejecutan al final
```

Diagrama simple:

```txt
[Call Stack] → Ejecuta código síncrono
     ↓
[Microtask Queue] → Promises (.then, async/await)
     ↓
[Macrotask Queue] → setTimeout, setInterval, eventos
```

Ejemplo práctico:

```js
function tarea1() {
  console.log("Tarea 1 - Síncrona");
}

function tarea2() {
  setTimeout(() => {
    console.log("Tarea 2 - Asíncrona");
  }, 1000);
}

function tarea3() {
  console.log("Tarea 3 - Síncrona");
}

tarea1();
tarea2();
tarea3();

// Salida:
// "Tarea 1 - Síncrona"
// "Tarea 3 - Síncrona"
// (espera 1 segundo)
// "Tarea 2 - Asíncrona"
```

### Pregunta #24

No entiendo qué es un 'event loop'. Explícamelo con palabras simples y un diagrama pequeño.

---

## Prompt 25

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender cómo ordenar un array de objetos por un campo numérico usando `.sort()`.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

El método `.sort()` ordena arrays:

```js
const productos = [
  { nombre: 'Laptop', precio: 1000 },
  { nombre: 'Mouse', precio: 20 },
  { nombre: 'Teclado', precio: 50 },
  { nombre: 'Monitor', precio: 300 }
];

// Ordenar por precio (menor a mayor)
productos.sort((a, b) => a.precio - b.precio);
console.log(productos);
// [
//   { nombre: 'Mouse', precio: 20 },
//   { nombre: 'Teclado', precio: 50 },
//   { nombre: 'Monitor', precio: 300 },
//   { nombre: 'Laptop', precio: 1000 }
// ]

// Ordenar por precio (mayor a menor)
productos.sort((a, b) => b.precio - a.precio);

// Ordenar por nombre (alfabéticamente)
productos.sort((a, b) => {
  if (a.nombre < b.nombre) return -1;
  if (a.nombre > b.nombre) return 1;
  return 0;
});

// Ordenar números simples
const numeros = [5, 2, 8, 1, 9];
numeros.sort((a, b) => a - b);
console.log(numeros); // [1, 2, 5, 8, 9]
```

En donde:

1. `sort()` recibe una función de comparación
2. Si retorna negativo, `a` va antes que `b`
3. Si retorna positivo, `b` va antes que `a`
4. Si retorna 0, mantiene el orden

### Pregunta #25

Tengo un arreglo de objetos y quiero ordenarlo por un valor numérico. Enséñame cómo usar `.sort()`.

---

## Prompt 26

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender cómo conectar eventos de HTML con funciones de JavaScript.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Hay varias formas de conectar eventos:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Eventos en JavaScript</title>
</head>
<body>
  <!-- Método 1: onclick en HTML (no recomendado) -->
  <button onclick="saludar()">Saludar (Método 1)</button>

  <!-- Método 2: Con addEventListener (recomendado) -->
  <button id="miBoton">Saludar (Método 2)</button>

  <!-- Método 3: Con propiedad onclick -->
  <button id="otroBoton">Saludar (Método 3)</button>

  <script>
    // Método 1: Función en HTML
    function saludar() {
      alert("¡Hola desde el método 1!");
    }

    // Método 2: addEventListener (RECOMENDADO)
    const miBoton = document.getElementById('miBoton');
    miBoton.addEventListener('click', function() {
      alert("¡Hola desde el método 2!");
    });

    // O con función flecha
    miBoton.addEventListener('click', () => {
      console.log("Click en el botón");
    });

    // Método 3: Propiedad onclick
    const otroBoton = document.getElementById('otroBoton');
    otroBoton.onclick = function() {
      alert("¡Hola desde el método 3!");
    };

    // Pasar parámetros
    function mostrarMensaje(mensaje) {
      alert(mensaje);
    }

    miBoton.addEventListener('click', () => {
      mostrarMensaje("Mensaje personalizado");
    });
  </script>
</body>
</html>
```

### Pregunta #26

Muéstrame cómo crear un botón en HTML que ejecute una función de JavaScript al hacer clic.

---

## Prompt 27

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender cómo detectar diferentes tipos de eventos del usuario como teclado, mouse y cambios en formularios.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

```js
// ========== EVENTOS DE MOUSE ==========
const caja = document.getElementById('miCaja');

// Click
caja.addEventListener('click', (e) => {
  console.log('Click en:', e.target);
});

// Doble click
caja.addEventListener('dblclick', () => {
  console.log('Doble click');
});

// Mouse entra y sale
caja.addEventListener('mouseenter', () => {
  console.log('Mouse entró');
});
caja.addEventListener('mouseleave', () => {
  console.log('Mouse salió');
});

// ========== EVENTOS DE TECLADO ==========
const input = document.getElementById('miInput');

// Tecla presionada
input.addEventListener('keydown', (e) => {
  console.log('Tecla presionada:', e.key);
  if (e.key === 'Enter') {
    console.log('Presionaste Enter');
  }
});

// Tecla liberada
input.addEventListener('keyup', (e) => {
  console.log('Tecla liberada:', e.key);
});

// ========== EVENTOS DE FORMULARIO ==========
const select = document.getElementById('miSelect');

// Cambio de valor
select.addEventListener('change', (e) => {
  console.log('Nuevo valor:', e.target.value);
});

// Input en tiempo real
input.addEventListener('input', (e) => {
  console.log('Escribiendo:', e.target.value);
});

// Focus y blur
input.addEventListener('focus', () => {
  console.log('Input tiene el foco');
});
input.addEventListener('blur', () => {
  console.log('Input perdió el foco');
});
```

En donde:

1. `addEventListener` permite escuchar cualquier tipo de evento
2. El objeto `e` (evento) contiene información útil como `target`, `key`, `value`
3. Puedes agregar múltiples listeners al mismo elemento

### Pregunta #27

Enséñame a detectar eventos de teclado, mouse y cambios en formularios usando JavaScript.

---

## Prompt 28

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito entender cómo usar temporizadores para ejecutar código después de un tiempo o de forma repetitiva.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Los temporizadores controlan la ejecución del código:

```js
// setTimeout - Ejecuta UNA VEZ después de un tiempo
console.log("Inicio");
setTimeout(() => {
  console.log("Esto se ejecuta después de 2 segundos");
}, 2000); // 2000 milisegundos = 2 segundos
console.log("Fin");

// Salida:
// "Inicio"
// "Fin"
// (espera 2 segundos)
// "Esto se ejecuta después de 2 segundos"

// setTimeout con parámetros
function saludar(nombre, edad) {
  console.log(`Hola ${nombre}, tienes ${edad} años`);
}
setTimeout(saludar, 1000, "Juan", 25);

// Cancelar un setTimeout
const temporizador = setTimeout(() => {
  console.log("Esto no se ejecutará");
}, 3000);
clearTimeout(temporizador); // Cancela el temporizador

// ========================================
// setInterval - Ejecuta REPETIDAMENTE cada X tiempo
let contador = 0;
const intervalo = setInterval(() => {
  contador++;
  console.log(`Contador: ${contador}`);
  if (contador === 5) {
    clearInterval(intervalo); // Detener después de 5 veces
    console.log("Intervalo detenido");
  }
}, 1000); // Cada 1 segundo

// Ejemplo práctico: Reloj
function mostrarHora() {
  const ahora = new Date();
  const hora = ahora.toLocaleTimeString();
  console.log(hora);
}

// Actualizar cada segundo
const reloj = setInterval(mostrarHora, 1000);

// Detener el reloj después de 10 segundos
setTimeout(() => {
  clearInterval(reloj);
  console.log("Reloj detenido");
}, 10000);
```

En donde:

1. `setTimeout` ejecuta código una sola vez después de un tiempo
2. `setInterval` ejecuta código repetidamente cada cierto intervalo
3. `clearTimeout` y `clearInterval` cancelan los temporizadores
4. El tiempo se especifica en milisegundos (1000ms = 1 segundo)

### Pregunta #28

Quiero aprender a usar `setTimeout` y `setInterval`. Dame ejemplos prácticos con explicaciones.

---

## Documento 29

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, veo código con sintaxis de desestructuración pero no comprendo cómo funciona ni para qué sirve.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

La desestructuración extrae valores de forma rápida:

```js
// ========== OBJETOS ==========

// Sin desestructuración
const persona = {
  nombre: "Juan",
  edad: 25,
  ciudad: "Madrid"
};

const nombre = persona.nombre;
const edad = persona.edad;

// Con desestructuración
const { nombre: nombre2, edad: edad2, ciudad } = persona;
console.log(nombre2); // "Juan"
console.log(edad2);   // 25
console.log(ciudad);  // "Madrid"

// Renombrar variables
const { nombre: nombrePersona, edad: años } = persona;
console.log(nombrePersona); // "Juan"
console.log(años);          // 25

// Valores por defecto
const { nombre: nombre3, profesion = "Desconocida" } = persona;
console.log(profesion); // "Desconocida"

// Desestructuración anidada
const usuario = {
  id: 1,
  datos: {
    nombre: "María",
    email: "maria@ejemplo.com"
  }
};

const { datos: { nombre: nombreUsuario, email } } = usuario;
console.log(nombreUsuario); // "María"
console.log(email);         // "maria@ejemplo.com"

// ========== ARRAYS ==========

// Sin desestructuración
const colores = ["rojo", "verde", "azul"];
const color1 = colores[0];
const color2 = colores[1];

// Con desestructuración
const [primero, segundo, tercero] = colores;
console.log(primero);  // "rojo"
console.log(segundo);  // "verde"
console.log(tercero);  // "azul"

// Saltar elementos
const [, , ultimo] = colores;
console.log(ultimo); // "azul"

// Rest operator
const numeros = [1, 2, 3, 4, 5];
const [uno, dos, ...resto] = numeros;
console.log(uno);   // 1
console.log(dos);   // 2
console.log(resto); // [3, 4, 5]

// Intercambiar variables
let a = 1;
let b = 2;
[a, b] = [b, a];
console.log(a); // 2
console.log(b); // 1

// ========== EN FUNCIONES ==========

function mostrarUsuario({ nombre, edad }) {
  console.log(`${nombre} tiene ${edad} años`);
}

mostrarUsuario({ nombre: "Pedro", edad: 30 });
```

### Pregunta #29

Explícame cómo funciona la desestructuración de objetos y arreglos en JavaScript con ejemplos claros.

---

## Documento 30

### Instrucción:

Vas a actuar como un docente de programación para estudiantes de 17-24 años con enfoque en JavaScript, donde mi manera de pregunta y respuesta será explicando varios conceptos que no entiendo. Más adelante te daré un contexto de mi persona y la situación, cómo será la entrada de lo que te comenté anteriormente y cómo me responderás.

### Contexto:

Soy un estudiante de programación, donde actualmente me estoy enfocando en el lenguaje de JavaScript, especialmente Vanilla. En mi etapa inicial de aprendizaje, necesito aprender a validar formularios HTML usando JavaScript para asegurarme de que los datos ingresados sean correctos.

### Entrada:

Voy a pasarte la pregunta puntual, con el fin de que me expliques a nivel de caso de estudio cómo funciona dicho concepto. Esta pregunta será de manera directa como mensaje del prompt.

### Salida:

Me responderás con una explicación pedagógica a nivel de caso de estudio, donde mezcles la explicación teórica, con ejemplos codificables y texto argumentativo, haciendo lineal el código que se genera.

### Ejemplo:

Validación paso a paso de un formulario:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Validación de Formulario</title>
  <style>
    .error {
      color: red;
      font-size: 14px;
    }
    .success {
      color: green;
    }
  </style>
</head>
<body>
  <form id="miFormulario">
    <div>
      <label>Nombre:</label>
      <input type="text" id="nombre" placeholder="Ingresa tu nombre">
      <span id="errorNombre" class="error"></span>
    </div>

    <div>
      <label>Correo:</label>
      <input type="email" id="correo" placeholder="ejemplo@correo.com">
      <span id="errorCorreo" class="error"></span>
    </div>

    <button type="submit">Enviar</button>
    <div id="mensaje"></div>
  </form>

  <script>
    // Obtener elementos
    const formulario = document.getElementById('miFormulario');
    const inputNombre = document.getElementById('nombre');
    const inputCorreo = document.getElementById('correo');
    const errorNombre = document.getElementById('errorNombre');
    const errorCorreo = document.getElementById('errorCorreo');
    const mensaje = document.getElementById('mensaje');

    // Función para validar nombre
    function validarNombre(nombre) {
      if (nombre.trim() === '') {
        return 'El nombre es obligatorio';
      }
      if (nombre.length < 3) {
        return 'El nombre debe tener al menos 3 caracteres';
      }
      if (!/^[a-zA-ZáéíóúÁÉÍÓÚñÑ\s]+$/.test(nombre)) {
        return 'El nombre solo puede contener letras';
      }
      return '';
    }

    // Función para validar correo
    function validarCorreo(correo) {
      if (correo.trim() === '') {
        return 'El correo es obligatorio';
      }
      const regex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      if (!regex.test(correo)) {
        return 'Ingresa un correo válido';
      }
      return '';
    }

    // Validar en tiempo real
    inputNombre.addEventListener('blur', () => {
      const error = validarNombre(inputNombre.value);
      errorNombre.textContent = error;
    });

    inputCorreo.addEventListener('blur', () => {
      const error = validarCorreo(inputCorreo.value);
      errorCorreo.textContent = error;
    });

    // Validar al enviar
    formulario.addEventListener('submit', (e) => {
      e.preventDefault(); // Prevenir envío por defecto

      // Limpiar mensajes previos
      errorNombre.textContent = '';
      errorCorreo.textContent = '';
      mensaje.textContent = '';

      // Validar todos los campos
      const errorNom = validarNombre(inputNombre.value);
      const errorCor = validarCorreo(inputCorreo.value);

      // Mostrar errores
      errorNombre.textContent = errorNom;
      errorCorreo.textContent = errorCor;

      // Si no hay errores, enviar
      if (!errorNom && !errorCor) {
        mensaje.textContent = '✓ Formulario válido. Enviando...';
        mensaje.className = 'success';

        // Aquí iría el código para enviar al servidor
        console.log('Datos:', {
          nombre: inputNombre.value,
          correo: inputCorreo.value
        });

        // Limpiar formulario
        formulario.reset();
      }
    });
  </script>
</body>
</html>
```

### Pregunta #30

Enséñame a validar un formulario simple en JavaScript (nombre y correo). Dame el código paso a paso.

```

