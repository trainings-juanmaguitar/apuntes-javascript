# [Modules](https://hacks.mozilla.org/2015/08/es6-in-depth-modules/)

- Native modules, alternative to [CommonJS](http://www.commonjs.org/) and [AMD](http://requirejs.org/docs/whyamd.html)
- Modules can export multiple values (unlike the others)
- Statically analyzed to load dependencies
- Dependencies are loaded asynchronously, but can be optimized with a module bundler ([rollup](http://rollupjs.org/) or [webpack](https://webpack.github.io/))

```javascript
// -------- jquery.js --------
export default function jQuery() {
  /* code */
}

// -------- code.js --------
import $ from 'jquery';
$('body').addClass('yay');

```

```javascript
// --------- http.js --------
export function get(url) {
  /* code */
}

export function post(url, body) {
  /* code */
}

// -------- code.js --------
import { get, post } from 'http';
import { TIMEOUT as HTTP_TIMEOUT } from 'http';
import * as http from 'http';

get('/my/url').then(function(result) {
  /* code */
});

HTTP_TIMEOUT; // 1000;
http.post('/my/url', 'body');
```

Do the following katas to assure the understanding of Modules
- [`import` statement](http://tddbin.com/#?kata=es6/language/modules/import)