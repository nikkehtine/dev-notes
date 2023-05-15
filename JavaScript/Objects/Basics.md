```js
let duck = {
	name: "Aflac",
	numLegs: 2,
};
```

## Access a property

```js
console.log(duck.name); // Aflac
```

## Create a method

```js
let duck = {
	name: "Aflac",
	numLegs: 2,
	sayName: function () {
		return "The name of this duck is " + duck.name + ".";
	},
};

duck.sayName(); // 'The name of this duck is Aflac.'
```

## `this` keyword

```js
let duck = {
	name: "Aflac",
	numLegs: 2,
	sayName: function () {
		return "The name of this duck is " + this.name + ".";
	},
};

duck.sayName(); // 'The name of this duck is Aflac.'
```

[[Constructors]]
