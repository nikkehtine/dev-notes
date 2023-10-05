# Kotlin basics [📝](https://kotlinlang.org/docs/home.html)

[Basic syntax | Kotlin Documentation](https://kotlinlang.org/docs/basic-syntax.html)

[Android Developers - Kotlin Basics course](https://developer.android.com/courses/android-basics-kotlin/course)

---

## Hello World

```kotlin
fun main() {
	println("Hello World!")
}
```

`print()` prints a line; `println()` prints a line and ends it with a new line symbol

## Variables

```kotlin
// Read-only local variables are defined using the keyword `val`; they can be assigned a value only once
val name = "Rover"
// Variables that can be reassigned use the `var` keyword
var age = 5
```

- Use `${}` to surround variables and calculations in the text of print statements

```kotlin
println("Happy birthday, ${name}!")
// output: Happy Birthday, Rover!
```

## Functions

```kotlin
// A type annotation is required on a value parameter
fun printBorder(border: String, timesToRepeat: Int) {
	repeat(timesToRepeat) {
		print(border)
	}
}
```

- Use a `repeat() {}` statement to repeat a set of instructions several times
