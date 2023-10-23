# Asynchronous JavaScript

```js
console.log("START");
console.log("This is synchronous");
console.log("END");
```

```
START
This is synchronous
END
```

---

```js
console.log("START");
setTimeout(() => console.log("This is asynchronous"), 5000);
console.log("END");
```

```
START
END
This is asynchronous
```

## Promises

```js
const promise = new Promise((resolve, reject) => {
	let fileLoaded = true;
	if (fileLoaded) {
		resolve("File loaded");
	} else {
		reject("File not loaded");
	}
});
```
