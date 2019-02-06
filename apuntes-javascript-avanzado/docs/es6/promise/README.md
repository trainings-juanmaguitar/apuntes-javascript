# [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

- Native implementation of promises. Yay!
- [Promises/A+](https://promisesaplus.com/) spec compliant


```javascript
var promise = new Promise(function(resolve, reject) {
  // Do something asynchronous and call resolve with the
  // result or reject with the error
});

promise.then(function(result) {
  // Use the result of the async call
}, function(error) {
  // Process the error
});
```

```javascript
var allPromise = Promise.all([getLocation, getTemperature]);
allPromise.then(function([location, temperature]) {
  console.log('The location is ', location,
        'and the temperature is', temperature);
}, function(error) {
  // Process the error
});

var racePromise = Promise.race([getGoogleAds, getYahooAds, getBindAds]);
racePromise.then(function(ads) {
  page.addAds(ads);
});
```

**⛏ &nbsp; ES6 Katas: Operador Spread**

Hacer las siguientes katas:
- [basics](http://tddbin.com/#?kata=es6/language/promise/basics)
- [creation](http://tddbin.com/#?kata=es6/language/promise/creation)
- [chaining `then`](http://tddbin.com/#?kata=es6/language/promise/chaining-then)