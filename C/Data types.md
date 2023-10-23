# Data types

[C data types - Mbed Handbook](https://os.mbed.com/handbook/C-Data-Types)

```c
int age = 21;
float gpa = 2.05;
char grade = 'C';
char name[] = "John";
```

```c
char a = 'C';   // single character    %c
char b[] = "S"; // array of characters %s

float c = 3.141592;           // 4 bytes  6 - 7 digits   %f
double d = 3.141592653589793; // 8 bytes  15 - 16 digits %lf

bool e = true;  // 1 byte %d
  // #include <stdbool.h> (>=C99)

char f = 120;          // 1 byte (-128 to 127) %d or %c
unsigned char g = 256; // 1 byte (0 to 255)    %d or %c

short h = 32767;          // 2 bytes (-32 768 to 32 767) %d
unsigned short i = 65535; // 2 bytes (0 to 65 535)       %d
// (short int)

int j = 2147483647;          // 4 bytes (-2 147 483 648 to 2 147 483 647) %d
unsigned int k = 4294967295; // 4 bytes (0 to 4 294 967 295)              %u
// on modern systems this is already a long

long long l = 9223372036854775807; // 8 bytes (-9 quintillion to 9 quintillion) %lld
unsigned long long m = 18446744073709551615U; // 8 bytes (0 to 18 quintillion) %llu
```

## Format specifiers

```c
printf("Hello %s\n", name);
```

| Sequence | Description         |
| -------- | ------------------- |
| `%s`     | string              |
| `%d`     | decimal             |
| `%c`     | character           |
| `%f`     | float               |
| `%.1f`   | decimal precision   |
| `%1`     | minimum field width |
| `%-`     | left align          |

```c
printf("Item 1: $%8.2f\n", item1);
// Item 1: $  100.99
```

## Escape sequences [🌐](https://en.wikipedia.org/wiki/Escape_sequences_in_C#Table_of_escape_sequences)

```c
printf("I like pizza!\n");
```

| Sequence     | Explanation                     |
| ------------ | ------------------------------- |
| `\n`         | new line                        |
| `\t`         | tab                             |
| `\\`         | backslash                       |
| `\'` or `\"` | single or double quotation mark |
| `\b`         | backspace                       |
