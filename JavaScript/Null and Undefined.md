# Null and undefined

[Null and Undefined on Exercism](https://exercism.org/tracks/javascript/concepts/null-undefined)

## `null`

The primitive value `null` is used as an intentional "empty value" for variables of any type

You can check whether a variable is null by using the **strict equality operator** `===`

```javascript
let name = null;
name === null;
// => true
```

## `undefined`

`undefined` appears in different contexts.

- If a variable is declared without a value (initialization), it is `undefined`.
- If you try to access a value for a non-existing key in an object, you get `undefined`.
- If a function does not return a value, the result is `undefined`.
- If an argument is not passed to a function, it is `undefined`, unless that argument has a default value.

## Optional chaining

With the optional chaining operator `?.` you can ensure that JavaScript only tries to access the nested key if the parent was not `null` or `undefined`. Otherwise, `undefined` is returned.

```javascript
const obj = {
	address: {
		street: "Trincomalee Highway",
		city: "Batticaloa",
	},
};

obj.address.zipCode;
// => undefined

obj.residence.street;
// => TypeError: Cannot read property 'street' of undefined

obj.residence?.street;
// => undefined
```

## Nullish coalescing

`??` returns the right-hand side operand only when the left-hand side operand is `null` or `undefined`. Otherwise, the left-hand side operand is returned.

```javascript
let amount = null;
amount = amount ?? 1;
// => 1

amount = 0;
amount = amount ?? 1;
// => 0
```
