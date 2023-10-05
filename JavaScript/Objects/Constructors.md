# Objects - Constructors

## Constructor function

```js
function Bird() {
	this.name = "Albert";
	this.color = "blue";
	this.numLegs = 2;
}
```

## Use a constructor to create objects

```js
let blueBird = new Bird();
```

## Extend constructors to receive arguments

```js
function Bird(name, color) {
	this.name = name;
	this.color = color;
	this.numLegs = 2;
}

let swan = new Bird("Carlos", "white");
```

## Verify an object's constructor

```js
let Bird = function (name, color) {
	this.name = name;
	this.color = color;
	this.numLegs = 2;
};

let crow = new Bird("Alexis", "black");

crow instanceof Bird; // true
```

```js
let canary = {
	name: "Mildred",
	color: "Yellow",
	numLegs: 2,
};

canary instanceof Bird; // false
```

## Use prototype properties

Since `numLegs` will probably have the same value for all instances of `Bird`, you essentially have a duplicated variable `numLegs` inside each `Bird` instance.

A better way is to use the `prototype` of `Bird`. Properties in the `prototype` are shared among ALL instances of `Bird`.

```js
Bird.prototype.numLegs = 2;
```

```js
Bird.prototype = {
	numLegs: 2,
	eat: function () {
		console.log("nom nom nom");
	},
	describe: function () {
		console.log("My name is " + this.name);
	},
};
```

### Check an object's prototype

```js
Bird.prototype.isPrototypeOf(duck); //true
```

### Prototype chain

```js
Object.prototype.isPrototypeOf(Bird.prototype);
```

## Constructor property

```js
let duck = new Bird();
let beagle = new Dog();

console.log(duck.constructor === Bird); // true
console.log(beagle.constructor === Dog); // true
```

### Set constructor property when changing prototype

There is one crucial side effect of manually setting the prototype to a new object - it erases the `constructor` property. This property can be used to check which constructor function created the instance, but since the property has been overwritten, it now gives false results.

```js
Bird.prototype = {
	constructor: Bird, // redeclare the constructor property
	numLegs: 2,
	eat: function () {
		console.log("nom nom nom");
	},
	describe: function () {
		console.log("My name is " + this.name);
	},
};
```

## Dry code (Don't Repeat Yourself)

```js
function Animal() {}

Animal.prototype = {
	constructor: Animal,
	describe: function () {
		console.log("My name is " + this.name);
	},
};
```

```js
Bird.prototype = {
	constructor: Bird,
};

Dog.prototype = {
	constructor: Dog,
};
```

## Inheriting behaviors from a supertype

```js
let animal = Object.create(Animal.prototype);
```

### Setting child's prototype to an instance of the parent

```js
Bird.prototype = Object.create(Animal.prototype);
```

```js
Bird.prototype.constructor = Bird;
duck.constructor; // Bird()
```
