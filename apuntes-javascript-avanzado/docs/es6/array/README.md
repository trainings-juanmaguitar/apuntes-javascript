# [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

Array object extended with:

- New static methods: [`from()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from), [`of()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/of)
- New instance methods: [`copyWithin()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/copyWithin), [`entries()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/entries) , [`fill()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/fill), [`find()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/find), [`findIndex()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex), [`keys()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/keys), [`values()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/values)


```javascript
Array.from(arguments) // [].slice.call(arguments);
Array.from({0: 'hello', 1: world, length: 2}); // ['hello', 'world']
Array.of(1, 2, 3) // [1, 2, 3]

[1, 2, 3, 4, 5].copyWithin(0, 3, 4) // [4, 2, 3, 4, 5]
[1, 2, 3].fill(4) // [4, 4, 4]
[4, 5, 8, 12].find(isPrime) // 5
[4, 5, 8, 12].findIndex(isPrime) // 2
[4, 5, 8, 12].keys() // iterator from 0 to 3
[4, 5, 8, 12].values() // iterator from 4 to 12
```

**⛏ &nbsp; ES6 Katas: Set**

Hacer las siguientes katas:
- [`Array.from()`](http://tddbin.com/#?kata=es6/language/array-api/from)
- [`Array.of()`](http://tddbin.com/#?kata=es6/language/array-api/of)
- [`[].fill()`](http://tddbin.com/#?kata=es6/language/array-api/fill)
- [`[].find()`](http://tddbin.com/#?kata=es6/language/array-api/find)
- [`[].findIndex()`](http://tddbin.com/#?kata=es6/language/array-api/findIndex)
- [`[].entries()`](http://tddbin.com/#?kata=es6/language/array-api/entries), [`[].keys()`](http://tddbin.com/#?kata=es6/language/array-api/keys) & [`[].values()`](http://tddbin.com/#?kata=es6/language/array-api/values) returns [_iterator_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Iteration_protocols#iterator)
