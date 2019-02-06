# [String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)

String object extended with:

- New static methods: [`raw()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/raw)
- New instance methods: [`startsWith()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/startsWith), [`endsWith()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/endsWith), [`includes()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/includes), [`repeat()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/repeat), ...


```javascript
String.raw`Line 1\nLine 2\nLine 3` // 'Line 1\\nLine 2\\nLine 3'
'Hello world'.startsWith('Hello') // true
'Hello world'.endsWith('world') // true
'Hello world'.includes('orl') // true
'Hello world'.repeat(2) // 'Hello worldHello world'
```

**⛏ &nbsp; ES6 Katas: String**

Hacer las siguientes katas:
- [`string.includes()`](http://tddbin.com/#?kata=es6/language/string-api/includes)
- [`string.repeat(count)`](http://tddbin.com/#?kata=es6/language/string-api/repeat)
- [`string.startsWith()`](http://tddbin.com/#?kata=es6/language/string-api/startswith)
- [`string.endsWith()`](http://tddbin.com/#?kata=es6/language/string-api/endswith)
