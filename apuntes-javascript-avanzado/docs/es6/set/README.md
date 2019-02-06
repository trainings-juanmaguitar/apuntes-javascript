# [`Set`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set)

- New **data structure** for handling collections
- Store unique values of any type, whether primitive values or object references
- Efficient and clean

```javascript
var s = new Set();
s.add("hello").add("goodbye").add("hello");
s.size === 2;
s.has("hello") === true;
s.delete("hello");
s.has("hello") === false;
```

**⛏ &nbsp; ES6 Katas: Set**

Hacer las siguientes katas:
- [basics](http://tddbin.com/#?kata=es6/language/set/basics)
- [`set.add()`](http://tddbin.com/#?kata=es6/language/set/add)
- [`set.delete()`](http://tddbin.com/#?kata=es6/language/set/delete)
- [the API](http://tddbin.com/#?kata=es6/language/set/api)
- [`set.clear()`](http://tddbin.com/#?kata=es6/language/set/clear)
