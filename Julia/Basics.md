[Julia docs](https://docs.julialang.org/en)

## Variables [📝](https://docs.julialang.org/en/v1/manual/variables/)

```julia
x = 10
```

Julia accepts certain Unicode characters for names:

```julia
∑ = 12

안녕하세요 = "Hello"
```

## Constants

```julia
const my_const = "Can't redeclare me!"
```

## Functions [📝](https://docs.julialang.org/en/v1/manual/functions/)

```julia
function f(x,y)
	x + y
end
```

The same function declaration, in a more compact form:

```julia
f(x,y) = x + y
```

## Comments [📝](https://docs.julialang.org/en/v1/base/punctuation/)

```julia
# This is a single line comment.

#= And this comment can
span multiple lines. =#
```

### Docstrings [📝](https://docs.julialang.org/en/v1/manual/documentation/)

```julia
"Tell whether there are too foo items in the array."
foo(xs::Array) = ...
```

```julia
"""
    bar(x[, y])

Compute the Bar index between `x` and `y`.

If `y` is unspecified, compute the Bar index between all pairs of columns of `x`.
"""
function bar(x, y) ...

```
