# [`{}` enhanced Object Literals](https://github.com/lukehoban/es6features#enhanced-object-literals)

- sintaxis mejorada para propiedades
- sintaxis mejorada para métodos
- nombres de propiedad dinámicos
- [_getter_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/get) and [_setter_](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Functions/set)


👉 &nbsp; [ejemplos](https://gist.github.com/juanmaguitar/fa284ba904992a4ece44e6e42ec81498)

### shortcuts propiedades y nombres dinámicos

```javascript
var a = "foo",
    b = 42,
    c = {};

function myMethod() {
    console.log('ooOoh!');
}

// Shorthand property names
var o = { a, b, c };

// Shorthand method name and dynamic property name
var o2 = {
  myMethod,
  ['myPropertyNum'+b]: 'bar'
}
```

### `get` y `set`

```javascript
var messages = {
  get latest () {
    if (this.log.length == 0) return undefined;
    return this.log[this.log.length - 1]
  },
  set current (str) {
    this.log[this.log.length] = str;
  },
  log: []
}

messages.current = "hey!";
messages.latest // hey!
```

**⛏ &nbsp; ES6 Katas: Enhanced Object Literals**

Hacer las siguientes katas:
- [basics](http://tddbin.com/#?kata=es6/language/object-literal/basics)
- [computed properties](http://tddbin.com/#?kata=es6/language/object-literal/computed-properties)
- [getter](http://tddbin.com/#?kata=es6/language/object-literal/getter)
- [setter](http://tddbin.com/#?kata=es6/language/object-literal/setter)