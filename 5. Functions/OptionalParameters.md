# Optional Parameters

Sometimes it makes sense for a function to have a **default value** for one or more of its parameters. These are called **optional parameters**.

To define an optional parameter, assign it a value in the function definition.

```py
def greet(name="World"):
    print(f"Hello, {name}!")
```

Now, the function can be called with or without an argument.

```py
greet("Alice")
greet()
```

Output:

```text
Hello, Alice!
Hello, World!
```

You can also have a mix of required and optional parameters.

```py
def power(base, exponent=2):
    return base ** exponent

print(power(5))
print(power(5, 3))
```

Output:

```text
25
125
```

Here, `exponent` defaults to `2`. If a different value is provided, it replaces the default.

## Parameter Order

Required parameters must come **before** optional parameters.

This is valid:

```py
def introduce(name, age=18):
    print(f"{name} is {age} years old.")
```

This is **not** valid:

```py
def introduce(name="John", age):
    print(f"{name} is {age} years old.")
```

Output:

```text
SyntaxError: non-default argument follows default argument
```

## Named Arguments

By default, arguments are matched to parameters by their position.

```py
def introduce(name, age):
    print(f"{name} is {age} years old.")

introduce("Alice", 20)
```

However, you can also assign arguments by their parameter names.

```py
introduce(age=20, name="Alice")
```

Output:

```text
Alice is 20 years old.
```

When using named arguments, the order no longer matters because each argument is explicitly assigned to a parameter.

You can also combine positional and named arguments.

```py
introduce("Alice", age=20)
```

However, all positional arguments must come before any named arguments.

This is **not** valid:

```py
introduce(name="Alice", 20)
```

Output:

```text
SyntaxError: positional argument follows keyword argument
```

<p align="center">
    <image src="images/OptionalParametersMeme.jpeg" width="500px" />
</p>

Next topic: [Variable Scope](VariableScope.md)