# Arrays - Operations

```js
let myArray = ["one", 2, ["the universe", 42], true, false, undefined, null];
```

```js
myArray[2] = "III"; // Replaces the third element with 'III'
```

- `.push()` - **adds** elements to the **end** of the array
- `.pop()` - **removes** elements from the **end** of the array
- `.shift()` - **removes** elements from the **beginning** of the array
- `.unshift()` - **adds** elements to the **beginning** of the array
- `.splice()` - first parameter is the **index** of the array, second is the **number of elements to delete**, third (one or more elements) is **element(s) to add in that place**
- `.slice()` - copies/**extracts** elements to a **new** array - index to **start** extraction, index to **stop** extraction (up to but not including)
- spread operator `...` - spreads out elements of an iterable object
