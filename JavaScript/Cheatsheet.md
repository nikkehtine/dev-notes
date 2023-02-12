## Comments

```js
// This is a single-line comment

/* This comment can span multiple lines.
   Lorem ipsum dolor sit amet */
```

## Variables, constants

- `var` - **variable** that can be declared multiple times
- `let` - **variable** that can be declared only once, but you can change its value
- `const` - **constant**, which can be declared only once and won't change its value

It is recommended to use `let` for variables.

A good practice is using `camelCase` for variables and `SCREAMING_SNAKE_CASE` for constants.

Another good practice is ending each line with a semicolon `;`.

```js
let myVariable; // You can declare a variable without assigning value
myVariable = 42;

const MY_CONSTANT;
```

## Console logging

```js
console.log("Hello World");
console.log(myVariable);
```

## Mathematical operations

```js
let myVar = 1 + 2; // The value is 3

myVar++; // Increments above variable - same as adding 1
// The value is 4

myVar *= 3; // The value is 12

// Prefix and postfix
let a = 1;
console.log(a++); // 'a' prints to the console, then increments
// Statement prints 1
console.log(a); // 'a' was incremented above after being printed
// Statement prints 2
console.log(++a); // 'a' increments, then prints to the console
// Statement prints 3
```
