## Passing by value

In the example below, when we pass the variable `val` to the function `MultiplyByTwo`, we passed a copy of `val`. Because of this, `newVal` has the updated value `4` but the original variable `val` is still `2`. Behind the scene, Go essentially makes a copy of the original value so that only this copy, a.k.a. `v`, is modified by the function.

```go
val := 2
func MultiplyByTwo(v int) int {
  v = v * 2
  return v
}
newVal := MultiplyByTwo(val)
// newval is 4, val is still 2 because only a copy of its value was passed into the function
```

## Passing by reference (Pointers)

By passing `pointer` arguments into a function, we could modify the underlying data passed into the function instead of only operating on a copy of the data.

Pointer types can be recognized by the `*` in front of the type in the function signature.

```go
func HandlePointers(x, y *int) {
    // Some logic to handle integer values referenced by pointers x and y
}
```

### Exceptions

Note that `slices` and `maps` are exceptions to the above-mentioned rule. When we pass a `slice` or a `map` as arguments into a function, they are treated as pointer types even though there is no explicit `*` in the type. This means that if we pass a slice or map into a function and modify its underlying data, the changes will be reflected on the original slice or map.
