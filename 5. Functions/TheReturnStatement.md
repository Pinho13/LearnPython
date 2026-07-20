# The Return Statement

## Functions in Math

Before learning about functions in Python, let's relate them to something you may already know: **functions in mathematics**.

Consider the following mathematical function:

```text
f(x) = 8x + 1
```

This function takes an input (`x`) and produces an output.

For example:

```text
f(0) = 1
```

Here, the input is `0`, and after applying the function, the output is `1`.

Functions can also have multiple inputs:

```text
f(x, y) = 8x + y
```

Here:

- Inputs: `x` and `y`
- Function body: `8x + y`
- Output: the result of evaluating `8x + y`

Python functions are similar. They **can receive** zero or more inputs (called **parameters**), execute a block of code, and **can** produce an output using the `return` statement.

## Syntax

To **define** a function in Python, use the following syntax:

<p align="center">
    <image src="images/FunctionSyntax.png" width="600px" />
</p>

Both the **parameters** and the **`return` statement** are optional.

Not all functions need inputs, some simply perform a specific task. Likewise, not all functions need to return a value, as shown in the example from the previous [section](WhatAreFunctions.md).

## Parameters

**Parameters** are variables listed in a function's definition. They allow you to pass information into a function, making it more flexible and reusable.

For example, this function receives one parameter:

```py
def greet(name):
    print(f"Hello, {name}!")
```

When calling the function, you provide a value for the parameter. This value is called an **argument**.

```py
greet("Alice")
greet("Bob")
```

Output:

```text
Hello, Alice!
Hello, Bob!
```

The same function can now be used with different values without changing its code.

### Multiple Parameters

A function can have as many parameters as needed.

```py
def rectangle_area(width, height):
    return width * height

print(rectangle_area(5, 8))
print(rectangle_area(3, 10))
```

Output:

```text
40
30
```

The values passed to a function are matched to its parameters in order.

```py
def introduce(name, age):
    print(f"{name} is {age} years old.")

introduce("Alice", 20)
```

Output:

```text
Alice is 20 years old.
```

If you swap the arguments, the result changes:

```py
introduce(20, "Alice")
```

Output:

```text
20 is Alice years old.
```

### No Parameters

Not every function needs parameters.

Some functions perform a task without requiring any external information.

```py
def print_separator():
    print("-" * 20)

print_separator()
print("Menu")
print_separator()
```

Output:

```text
--------------------
Menu
--------------------
```

## Returning a Value

The `return` statement is used to send a value back to wherever the function was called.

For example:

```py
def celsius_to_fahrenheit(celsius):
    return celsius * 9 / 5 + 32

result = celsius_to_fahrenheit(20)

print(result)
```

Output:

```text
68.0
```

Here, the function returns the converted temperature, which is then stored in the variable `result`.

Since the function returns a value, it can be used anywhere a normal value can be used.

For example, you can print the returned value directly:

```py
print(celsius_to_fahrenheit(30))
```

Or use it in an expression:

```py
average = (celsius_to_fahrenheit(20) + celsius_to_fahrenheit(30)) / 2

print(average)
```

Output:

```text
77.0
```

## Returning Early

When Python reaches a `return` statement, the function immediately stops executing.

```py
def absolute(number):
    if number >= 0:
        return number

    return -number

print(absolute(5))
print(absolute(-5))
```

Output:

```text
5
5
```

Once a `return` statement is executed, any code below it is skipped.

```py
def example():
    print("Before return")

    return

    print("After return")

example()
```

Output:

```text
Before return
```

The second `print()` is never executed because the function has already returned.

A function with no `return` or with an empty `return` will return the value `None`.

<p align="center">
    <image src="images/ReturnStatementMeme.jpg" width="400px" />
</p>

