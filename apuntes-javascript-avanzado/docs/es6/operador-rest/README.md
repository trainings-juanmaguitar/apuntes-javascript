# [`...` operador Rest](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/rest_parameters)

- Asocia parámetros restantes a un array utilizando `...`
- Sustituye la necesidad de `arguments`

```javascript
function multiply(multiplier, ...numbers) {
  return numbers.map(n => multiplier * n);
}

var arr = multiply(2, 1, 2, 3);
console.log(arr); // [2, 4, 6]
```


**⛏ &nbsp; ES6 Katas: Operador REST**

Hacer las siguientes katas:
- [as parameter](http://tddbin.com/#?kata=es6/language/rest/as-parameter)
- [with destructuring](http://tddbin.com/#?kata=es6/language/rest/with-destructuring)