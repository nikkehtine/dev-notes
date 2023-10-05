# Randomness [📝](https://pkg.go.dev/math/rand)

[Randomness on Exercism](https://exercism.org/tracks/go/concepts/randomness)

```go
import "math/rand"

n := rand.Intn(100) // n is a random int, 0 <= n < 100
```

```go
f := rand.Float64() // f is a random float64, 0.0 <= f < 1.0
```

```go
x := []string{"a", "b", "c", "d", "e"}
// shuffling the slice put its elements into a random order
rand.Shuffle(len(x), func(i, j int) {
	x[i], x[j] = x[j], x[i]
})
```
