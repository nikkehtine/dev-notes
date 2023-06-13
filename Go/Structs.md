[Structs on Exercism](https://exercism.org/tracks/go/concepts/structs)

Structs can be compared to _classes_ in object-oriented programming.

```go
type Shape struct {
  name string
  size int
}
```

## Creating structs

```go
s := Shape {
  name: "Square",
  size: 25,
}
```

You can create an instance of a `struct` without using the field names, as long as you define the fields *in order*:

```go
s := Shape {
  "Oval",
  20,
}
```

However, this syntax is considered *brittle code* since it can break when a field is added, especially when the new field is of a different type.

### _New_ functions

These functions are usually called `New` or have their names starting with `New`, but since they are just regular functions, you can give them any name you want. They might remind you of constructors in other languages, but in Go they are just regular functions.

```go
func NewShape(name string) Shape {
	return Shape{
		name: name,
		size: 100, //default-value for size is 100
	}
}
```

### `new` builtin

Another way of creating a new instance of a struct is by using the `new` built-in:

```go
s := new(Shape) // s will be of type *Shape (pointer to shape)
```

## Updating structs

```go
s.name = "Circle"
s.size = 35
```
