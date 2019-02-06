# [`=>` arrow Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)

- syntaxis más corta con `=>`
- siempre anónimas
- Lexically bind `this`
- Muy útil para event handlers y callbacks
- Muy útil para programación funcional (higher order functions(


4 versiones:

```javascript
    (arg1, arg2, ...) => expr
    (arg1, arg2, ...) => { stmt1; stmt2; ... }
    singleArg => expr
    singleArg => { stmt1; stmt2; ... }
```

### value of `this`

antes (ES5)

```javascript
var self = this;
this.element.addEventListener('click', function(event) {
  self.registerClick(event.target.id);
});
```

después (ES2015)

```javascript
this.element.addEventListener('click', event => {
  this.registerClick(event.target.id);
});
```

### higher order functions

antes (ES5)

```javascript
[1,3,4,5,6,7].filter(function(n) { return n % 2 } )
  .map(function(n, i) { return n + i } );
// [1, 4, 7, 10]
```

después (ES2015)

```javascript
[1,2,3,4,5,6,7].filter(n => n % 2).map((n, i) => n+i);
```

Más info: 
- [ECMAScript 6 equivalents in ES5: Arrow Functions](https://github.com/addyosmani/es6-equivalents-in-es5#arrow-functions)  
- [ES6 In Depth: Arrow functions](https://hacks.mozilla.org/2015/06/es6-in-depth-arrow-functions/)  
- [Understanding ECMAScript 6 arrow functions](https://www.nczonline.net/blog/2013/09/10/understanding-ecmascript-6-arrow-functions/)


**⛏ &nbsp; ES6 Katas: Arrow Functions**

Hacer las siguientes katas:
- [basics](http://tddbin.com/#?kata=es6/language/arrow-functions/basics)
- [function binding](http://tddbin.com/#?kata=es6/language/arrow-functions/binding)

