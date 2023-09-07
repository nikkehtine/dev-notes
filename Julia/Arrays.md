# Arrays [📝](https://docs.julialang.org/en/v1/manual/arrays/)

```julia
a = [1, 2, 3]
```

You can specify the element type:

```julia
a = Float32[1, 2.3, 4//5]
# 3-element Vector{Float32}:
# 1.0
# 2.3
# 0.8
```

## Properties [📝](https://docs.julialang.org/en/v1/manual/arrays/#Basic-Functions)

- **`eltype(a)`** - `Float32` - the type of elements
- **`length(a)`** - `3` - the number of elements
- **`ndim(a)`** - `1` - the number of dimensions
