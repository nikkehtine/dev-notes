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
