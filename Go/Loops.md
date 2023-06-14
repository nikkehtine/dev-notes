## `for` loop

```go
for i := 0; i < 10; i++ {
  sum += i
}
```

The init and post statements are optional.

```go
for ; sum < 10; {
  sum += sum
}
```

## `while` loop

That's also `for`.

```go
for sum < 1000 {
  sum += sum
}
```

## Infinite loop

```go
for {
}
```
