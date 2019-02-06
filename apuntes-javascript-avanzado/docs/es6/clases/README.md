# [Clases](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

- Basic support
- `class` and [`extends`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/extends) keywords
- [`constructor`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/constructor) definition
- [`static`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/static) method definitions

BEFORE

```javascript
var Shape = function( id, x, y ) {
  this.id = id;
  this.x = x;
  this.y = y;
};
Shape.prototype.toString = function( x, y ) {
  return "Shape(" + this.id + ")"
};

var Rectangle = function( id, x, y, width, height ) {
  Shape.call( this, id, x, y );
};
Rectangle.prototype = Object.create(Shape.prototype);
Rectangle.prototype.constructor = Rectangle;
Rectangle.prototype.toString = function() {
  return "Rectangle > " + Shape.prototype.toString.call( this );
};
```

AFTER

```javascript
class Shape {
  constructor (id, x, y) {
    this.id = id;
    this.x = x;
    this.y = y;
    // or Object.assign(this, {id, x, y});
  }
  toString () {
    return `Shape(${this.id})`
  }
}

class Rectangle extends Shape {
  constructor (id, x, y, width, height) {
    super(id, x, y)
  }
  toString () {
    return "Rectangle > " + super.toString()
  }
}
```


- [Examples Classes](https://googlechrome.github.io/samples/classes-es6/index.html)
- [ES6 | Classes and Inheritance](https://medium.com/ecmascript-2015/es6-classes-and-inheritance-607804080906#.yly3wqbsq)  

**⛏ &nbsp; ES6 Katas: Clases**

Hacer las siguientes katas:
- [creation](http://tddbin.com/#?kata=es6/language/class/creation)
- [accessors](http://tddbin.com/#?kata=es6/language/class/accessors)
- [static](http://tddbin.com/#?kata=es6/language/class/static)
- [extends](http://tddbin.com/#?kata=es6/language/class/extends)
- [more extends](http://tddbin.com/#?kata=es6/language/class/more-extends)
- [super in method](http://tddbin.com/#?kata=es6/language/class/super-in-method)
- [super in constructor](http://tddbin.com/#?kata=es6/language/class/super-in-constructor)
