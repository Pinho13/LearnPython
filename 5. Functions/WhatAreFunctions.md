# What are Functions

As programs grow larger, you may find yourself writing the same code multiple times. Instead of copying and pasting it multiple times, you can group it into a **function**.

A **function** is a reusable block of code that performs a specific task. Once a function has been defined, it can be called whenever that task needs to be performed.

For example, suppose you need to convert degrees celsius to fahrenheit for an experiment.

Without a function:

```py
celsius = 20
fahrenheit = celsius * 9 / 5 + 32
print(fahrenheit)

celsius = 35
fahrenheit = celsius * 9 / 5 + 32
print(fahrenheit)

celsius = -10
fahrenheit = celsius * 9 / 5 + 32
print(fahrenheit)
```

With a function:

```py
def celsius_to_fahrenheit(celsius):
    fahrenheit = celsius * 9 / 5 + 32
    print(fahrenheit)

celsius_to_fahrenheit(20)
celsius_to_fahrenheit(35)
celsius_to_fahrenheit(-10)
```

Output:

```text
68.0
95.0
14.0
```

Notice that the formula for the conversion is written only once, making the program shorter, easier to read, and easier to maintain.

Functions are useful because they:

- Avoid repeating code.
- Make programs easier to read.
- Make code easier to test and maintain.
- Break large problems into smaller, manageable pieces.

<p align="center">
    <image src="images/FunctionsMeme.png" width="400px" />
</p>

Next topic: [The Return Statement](TheReturnStatement.md)