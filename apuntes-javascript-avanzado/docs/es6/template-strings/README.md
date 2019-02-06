# [` `` ` template Strings](https://hacks.mozilla.org/2015/05/es6-in-depth-template-strings-2/)

- Se utilizan back-ticks ` `` `
- Soporte multilinea
- placeholders `${ expression }`

```javascript
`string text`

`string text line 1
 string text line 2`

`string text ${expression} string text`
```

### placeholders y multilinea

antes (ES5)

```javascript
var name = "juanma";
var getSuitableDrink = function(who) {
  return who === 'juanma' ? 'beer' : 'cocktail'
};

console.log( 'Hello, '+name+'!\nFancy a '+getSuitableDrink()+'?' );

// Hello, juanma!
// Fancy a beer?
```

después (ES2015)

```javascript
var name = "juanma";
var getSuitableDrink = function(who) {
  return who === 'juanma' ? 'beer' : 'cocktail'
};

console.log( `Hello, ${ name }!
  Fancy a ${ getSuitableDrink() }?` );
```


Más info: 

- [Template Strings](https://hacks.mozilla.org/2015/05/es6-in-depth-template-strings-2/)
- [ECMAScript 6 equivalents in ES5: Template Literals](https://github.com/addyosmani/es6-equivalents-in-es5#template-literals)  

**⛏ &nbsp; ES6 Katas: Template Strings**

Hacer las siguientes katas:
- [basics](http://tddbin.com/#?kata=es6/language/template-strings/basics)
- [multiline](http://tddbin.com/#?kata=es6/language/template-strings/multiline)
- [tagged template strings](http://tddbin.com/#?kata=es6/language/template-strings/tagged)
- [`raw` property](http://tddbin.com/#?kata=es6/language/template-strings/raw)
