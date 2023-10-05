# Basics

**[Go documentation](https://go.dev/learn/)**

[Go basics on Exercism](https://exercism.org/tracks/go/concepts/basics) | [Effective Go (Go Docs)](https://go.dev/doc/effective_go)

## Packages

- A package is a collection of source files located in the same directory.
- All source files in a directory must share the same package name.
- It is conventional for the package name to be the last directory in the import path. For example, the files in the ["math/rand" package](https://golang.org/src/math/rand/) begin with the statement `package rand`.
- When a package is imported, only entities (functions, types, variables, constants) whose names start with a capital letter can be used / accessed.
- The recommended style of naming in Go is that identifiers will be named using `camelCase`, except for those meant to be accessible across packages which should be `PascalCase`.

```go
package lasagna
```

```go
package main
```

### Importing packages

```go
import (
	"fmt"
	t "time" // You can alias package time as t
)
```

## Variables

Go is statically-typed, which means all variables must have a defined type at compile-time.

```go
var explicit int // Explicitly typed
```

```go
implicit := 10   // Implicitly typed as an int
```

## Constants

```go
const Age = 21
```

## Functions

```go
package greeting

// Hello is a public function.
func Hello (name string) string {
    return hi(name)
}

// hi is a private function.
func hi (name string) string {
    return "hi " + name
}
```

## Comments

```go
// This is a single line comment

/* This is a multi line comment
   This is a multi line comment
   This is a multi line comment */
```

## Numbers

- `int`: e.g. `0`, `255`, `2147483647`
- `float64`: e.g. `0.0`, `3.14`

## Arithmetic operators

| Operator | Example        |
| -------- | -------------- |
| `+`      | `4 + 6 == 10`  |
| `-`      | `15 - 10 == 5` |
| `*`      | `2 * 3 == 6`   |
| `/`      | `13 / 3 == 4`  |
| `%`      | `13 % 3 == 1`  |

For integer division, the remainder is dropped (e.g. `5 / 2 == 2`).

```go
var x int = 42

// this line produces an error
value := float32(2.0) * x // invalid operation: mismatched types float32 and int

// you must convert int type to float32 before performing arithmetic operation
value := float32(2.0) * float32(x)
```
