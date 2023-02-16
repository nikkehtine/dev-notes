**Length**

```js
var name = "Lovelace";
var nameLen = name.length;
console.log(nameLen); //Output: 8
```

**Bracket notation**

```js
console.log(name[0]);
// Output: L

console.log(name[2]); // 3rd letter of 'name'
// Output: v

console.log(name[name.length - 1]); // Last letter of 'name'
// Output: e
```

**String immutability**

```js
var myStr = "Jello World";

// This will produce an ERROR
myStr[0] = "H";

myStr = "Hello World";

```
