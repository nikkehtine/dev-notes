# C# Basics [📝](https://learn.microsoft.com/en-us/dotnet/csharp/)

[C# basics on Exercism](https://exercism.org/tracks/csharp/concepts/basics)

## Hello world

```cs
Console.WriteLine("Hello World!");
//class   method    input
/* Multi
line
comments */
```

## Variables

```cs
int explicitVar = 10; // Explicitly typed
var implicitVar = 10; // Implicitly typed
```

## Functions

C# is an object-oriented language and requires all [functions](https://learn.microsoft.com/en-us/dotnet/csharp/methods) to be defined in a _class_, which are defined using the [`class` keyword](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/classes#declaring-classes). Objects (or _instances_) are created by using the `new` keyword.

```cs
class Calculator
{
    // ...
}

var calculator = new Calculator();
```

A function within a class is referred to as a _method_. Each [method](https://docs.microsoft.com/en-us/dotnet/csharp/methods) can have zero or more parameters. All parameters must be explicitly typed, there is no type inference for parameters. Similarly, the return type must also be made explicit. Values are returned from methods using the [`return` keyword](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/return). To allow a method to be called by code in other files, the `public` access modifier must be added.

```cs
class Calculator
{
    public int Add(int x, int y)
    {
        return x + y;
    }
}
```

Methods are invoked using dot (`.`) syntax on an instance, specifying the method name to call and passing arguments for each of the method's parameters. Arguments can optionally specify the corresponding parameter's name.

```csharp
var calculator = new Calculator();
var sum_v1 = calculator.Add(1, 2);
var sum_v2 = calculator.Add(x: 1, y: 2);
```

If the method to be called is defined in the same class as the method that calls it, the class name can be omitted.
