# C Basics

## Good resources

- [Modern C](https://inria.hal.science/hal-02383654/file/ModernC.pdf)
- [Learn-C.org](https://learn-c.org/)
- [GNU C Manual](https://www.gnu.org/software/gnu-c-manual/gnu-c-manual.html)
- [C reference card](https://users.ece.utexas.edu/~adnan/c-refcard.pdf)

## Hello World

```c
#include <stdio.h>

int main() {
  printf("Hello, World!\n");
  return 0;
}
```

## Comments

```c
// This is a comment
/* This one is
also a comment */
```

## [[Data types|Variables]]

```c
int x; // declaration
x = 123; // initialization
int y = 321; // declaration + initialization
```

## Constants

```c
const float PI = 3.141592;
```

## Arithmetic operators

| Operator | Name           |
| -------- | -------------- |
| `+`      | addition       |
| `-`      | subtraction    |
| `*`      | multiplication |
| `/`      | division       |
| `%`      | modulus        |
| `++`     | increment      |
| `--`     | decrement      |

```c
int x = 5;
int y = 2;

int z = x / y;           // 2
float z = x / y;         // 2.000000
float z = x / (float) y; // 2.500000

int z = x % y;           // 1

// Augmented assignment operators
x++;    // 6
y += 2; // 4
x--;    // 5
y -= 2; // 2
```
