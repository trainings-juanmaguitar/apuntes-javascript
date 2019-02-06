# [Modules](https://hacks.mozilla.org/2015/08/es6-in-depth-modules/)

- Módulos nativos, alternativa a [CommonJS](http://www.commonjs.org/) y [AMD](http://requirejs.org/docs/whyamd.html)
- Módulos pueden exportar múltiples valores (no cómo los otros tipos de módulos)
- Se analiza estáticamente para cargar dependencias
- Las dependencias se cargan asíncronamente, pero se puede optimizar con un "module bundler" ([rollup](http://rollupjs.org/) or [webpack](https://webpack.github.io/))

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