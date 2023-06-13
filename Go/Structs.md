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

## Updating structs

```go
s.name = "Circle"
s.size = 35
```
