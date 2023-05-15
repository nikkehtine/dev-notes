```js
const tekkenCharacter = {
	player: "Hwoarang",
	fightingStyle: "Tae Kwon Doe",
	human: true,
};
```

## Adding key-value pairs

```js
tekkenCharacter.origin = "South Korea";

tekkenCharacter["hair color"] = "dyed orange";

const eyes = "eye color";
tekkenCharacter[eyes] = "brown";
```

**Result:**

```js
{
  player: 'Hwoarang',
  fightingStyle: 'Tae Kwon Doe',
  human: true,
  origin: 'South Korea',
  'hair color': 'dyed orange',
  'eye color': 'brown'
};
```

## Modifying an objected nested within an object

```js
let userActivity = {
	id: 23894201352,
	date: "January 1, 2017",
	data: {
		totalUsers: 51,
		online: 42,
	},
};

userActivity.data.online = 45;
```

## Accessing property names with bracket notation

```js
function grabData(property) {
	return tekkenCharacter[property];
}

console.log(grabData("eye color")); // 'dyed orange'
```

## Deleting properties

```js
delete tekkenCharacter.human;
```

## Checking if object has a property

```js
users.hasOwnProperty("Alan");
"Alan" in users;
// both should return true
```

## Iterate through the keys of an object

```javascript
const refrigerator = {
	milk: 1,
	eggs: 12,
};

for (const food in refrigerator) {
	console.log(food, refrigerator[food]);
}
```

> **NOTE:** Objects do not maintain an ordering to stored keys like arrays do; thus a key's position on an object, or the relative order in which it appears, is irrelevant when referencing or accessing that key.

## Generate an array of all object keys

```js
console.log(Object.keys(refrigerator)); // [ 'milk', 'eggs' ]
```

## Modify an array stored in an object

```js
let user = {
	name: "Kenneth",
	age: 28,
	data: {
		username: "kennethCodesAllDay",
		joinDate: "March 26, 2016",
		friends: ["Sam", "Kira", "Tomo"],
	},
};

user.data.friends.push("Pete");

console.log(user.data.friends); // [ 'Sam', 'Kira', 'Tomo', 'Pete' ]
```
