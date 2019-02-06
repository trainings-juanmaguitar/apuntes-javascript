# [`...` operador Spread](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_operator)

Permite expandir una expresión en sitios donde se esperan multiples argumentos:
- En **llamadas a funciones**
- En **arrays**

```javascript
function f(x, y, z) {
  return x + y + z;
}

var arr = [1, 2, 3];
f(...arr) === 6; // true

[0, ...arr, 4, 5, 6, 7]; // [0, 1, 2, 3, 4, 5, 6, 7]
```


**⛏ &nbsp; ES6 Katas: Operador Spread**

Hacer las siguientes katas:
- [with arays](http://tddbin.com/#?kata=es6/language/spread/with-arrays)
- [with strings](http://tddbin.com/#?kata=es6/language/spread/with-strings)
