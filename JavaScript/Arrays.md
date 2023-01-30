```js
let myArray = ['one', 2, 'three', true, false, undefined, null];
```

## Bracket notation

```js
let myVar = myArray[0] // value is 'one'
```

## Operations

```js
myArray[2] = 'III';
```

- `.push()` - **adds** elements to the **end** of the array
- `.pop()` - **removes** elements from the **end** of the array
- `.unshift()` - **adds** elements to the **beginning** of the array
- `.shift()` - **removes** elements from the **beginning** of the array
- `.splice()` - first parameter is the **index** of the array, second is the **number of elements to delete**, third (one or more elements) is **element(s) to add in that place**
- `.slice()` - copies/**extracts** elements to a **new** array - index to **start** extraction, index to **stop** extraction (up to but not including)
- spread operator `...` - 