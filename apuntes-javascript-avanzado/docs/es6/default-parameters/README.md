# [Parámetros por defecto](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Default_parameters)

```javascript
function f(x, y=12) {
  // y is 12 if not passed (or passed as undefined)
  return x + y;
}

f(3) === 15;
f(3, undefined) === 15;
```

**⛏ &nbsp; ES6 Katas: Default parameters**

Hacer las siguientes katas:
- [basic](http://tddbin.com/#?kata=es6/language/default-parameters/basics)
