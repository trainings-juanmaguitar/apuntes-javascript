# [`Map`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map)

- Nueva **estructura de datos** para manejar colecciones
- Sencillo mapa clave/valor
- Cualquier valor (tanto objetos como primitivas) pueden ser usadas clave o valor
- Limpio y eficiente

```javascript
var m = new Map();
m.set("hello", 42);
m.get("hello") === 42;

var s = { n:4 };
m.set(s, 34);
m.get(s) === 34;
```

```javascript
var myMap = new Map();

var keyString = "a string",
    keyObj = {},
    keyFunc = function () {};

// setting the values
myMap.set(keyString, "value associated with 'a string'");
myMap.set(keyObj, "value associated with keyObj");
myMap.set(keyFunc, "value associated with keyFunc");

myMap.size; // 3

// getting the values
myMap.get(keyString);    // "value associated with 'a string'"
myMap.get(keyObj);       // "value associated with keyObj"
myMap.get(keyFunc);      // "value associated with keyFunc"

myMap.get("a string");   // "value associated with 'a string'"
                         // because keyString === 'a string'
myMap.get({});           // undefined, because keyObj !== {}
myMap.get(function() {}) // undefined, because keyFunc !== function () {}
```

**⛏ &nbsp; ES6 Katas: Map**

Hacer las siguientes katas:
- [basics](http://tddbin.com/#?kata=es6/language/map/basics)
- [`map.get()`](http://tddbin.com/#?kata=es6/language/map/get)
- [`map.set()`](http://tddbin.com/#?kata=es6/language/map/set)
- [initalize](http://tddbin.com/#?kata=es6/language/map/initialize)
- [`map.has()`](http://tddbin.com/#?kata=es6/language/map/has)