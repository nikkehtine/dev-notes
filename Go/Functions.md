[Functions on Exercism](https://exercism.org/tracks/go/concepts/functions)

```go
// No parameters
func PrintHello() {
    fmt.Println("Hello")
}

// One parameter
func PrintHelloName(name string) {
  fmt.Println("Hello " + name)
}
```

Parameters of the same type can be declared together, followed by a single type declaration.

```go
func PrintGreetingName(greeting, name string) {
  fmt.Println(greeting + " " + name)
}
```

If multiple values are to be returned from a function, they are comma separated.

```go
func Hello(name string) string {
  return "Hello " + name
}

func HelloAndGoodbye(name string) (string, string) {
  return "Hello " + name, "Goodbye " + name
}
```

## Variadic Functions

[Variadic functions on Exercism](https://exercism.org/tracks/go/concepts/variadic-functions)

Usually, functions in Go accept only a fixed number of arguments. However, it is also possible to write variadic functions in Go.

A variadic function is a function that accepts a variable number of arguments.

If the type of the last parameter in a function definition is prefixed by ellipsis `...`, then the function can accept any number of arguments for that parameter.

```go
func find(a int, b ...int) {
    // ...
}
```

In the above function, parameter `b` is variadic and we can pass 0 or more arguments to `b`.

```go
find(5, 6)
find(5, 6, 7)
find(5)
```

> **Note**
> The variadic parameter must be the last parameter of the function.

The way variadic functions work is by converting the variable number of arguments to a slice of the type of the variadic parameter.

Here is an example of an implementation of a variadic function:

```go
func find(num int, nums ...int) {
    fmt.Printf("type of nums is %T\n", nums)

    for i, v := range nums {
        if v == num {
            fmt.Println(num, "found at index", i, "in", nums)
            return
        }
    }

    fmt.Println(num, "not found in ", nums)
}

func main() {
    find(89, 90, 91, 95)
    // Output:
    // type of nums is []int
    // 89 not found in  [90 91 95]

    find(45, 56, 67, 45, 90, 109)
    // Output:
    // type of nums is []int
    // 45 found at index 2 in [56 67 45 90 109]

    find(87)
    // Output:
    // type of nums is []int
    // 87 not found in  []
}
```

Sometimes you already have a slice and want to pass that to a variadic function. This can be achieved by passing the slice followed by `...`. That will tell the compiler to use the slice as is inside the variadic function. The step described above where a slice is created will simply be omitted in this case.

```go
list := []int{1,2,3}
find(1, list...) // "find" defined as shown above
```

## Named Return Values and Naked Return

As well as parameters, return values can optionally be named. If named return values are used, a `return` statement without arguments will return those values. This is known as a 'naked' return.

```go
func SumAndMultiplyThenMinus(a, b, c int) (sum, mult int) {
    sum, mult = a+b, a*b
    sum -= c
    mult -= c
    return
}
```
