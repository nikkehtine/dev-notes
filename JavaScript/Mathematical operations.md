```js
let myVar = 1 + 2; // The value is 3
```

## Incrementing

```js
myVar++;
```

- Increments above variable - same as adding 1
- The value is `4`

### Decrementing

It can also go the other way:

```js
myVar--;
```

- Decrements above variable - same as adding 1
- The value is `3`

## Multiplying

```js
myVar *= 4; // 3 * 4 = 12
```

## Prefix and postfix increment

```js
let a = 1;
```

**Postfix**

```js
console.log(a++);
```

- `a` first prints to the console, then increments
- Statement prints `1`

```js
console.log(a);
```

- `a` was already incremented above after being printed
- Statement prints `2`

**Prefix**

```js
console.log(++a); // 'a' increments, then prints to the console
// Statement prints 3
```

- `a` increments, then prints to the console
- Statement prints `3`
