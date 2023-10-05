# Python basics

[Python basics on Exercism](https://exercism.org/tracks/python/concepts/basics)

## Variables

```python
my_first_variable = "Hello, World!"
```

## Constants

```python
MY_CONSTANT = "Do not reassign me!"
```

## Functions

```python
def add_two_numbers(number_one, number_two):
	result = number_one + number_two
	return result
```

## Comments

```python
# This is a comment
```

Python doesn't support multi-line comments

### Docstrings

The first statement of a function body can optionally be a [_docstring_](https://docs.python.org/3/tutorial/controlflow.html#tut-docstrings), which concisely summarizes the function or object's purpose. Docstring conventions are laid out in [PEP257](https://www.python.org/dev/peps/pep-0257/).

```python
# An example from PEP257 of a multi-line docstring.
def complex(real=0.0, imag=0.0):
    """Form a complex number.

    Keyword arguments:
    real -- the real part (default 0.0)
    imag -- the imaginary part (default 0.0)
    """

    if imag == 0.0 and real == 0.0:
        return complex_zero
```
