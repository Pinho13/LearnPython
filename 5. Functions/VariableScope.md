# Variable Scope

Variables are only accessible within certain parts of a program. This is known as their **scope**.

Functions create their own scope, meaning variables created inside a function are generally not accessible outside of it.

## Local Variables

A variable created inside a function is called a **local variable**.

```py
def greet():
    message = "Hello!"
    print(message)

greet()
```

Output:

```text
Hello!
```

However, trying to access `message` outside the function results in an error.

```py
print(message)
```

Output:

```text
NameError: name 'message' is not defined
```

This happens because `message` only exists while the function is executing.

## Global Variables

A variable created outside any function is called a **global variable**.

```py
language = "Python"

def greet():
    print(f"Welcome to {language}!")

greet()
```

Output:

```text
Welcome to Python!
```

Global variables can be accessed from anywhere in the program, including inside functions.

## Local vs Global Variables

A local variable can have the same name as a global variable.

In this case, the local variable takes priority inside the function.

```py
language = "Python"

def greet():
    language = "Java"
    print(language)

greet()
print(language)
```

Output:

```text
Java
Python
```

Changing the local variable does **not** affect the global one.

## Modifying Global Variables

If you assign a value to a variable inside a function, Python creates a new local variable by default.

```py
count = 10

def increase():
    count = count + 1

increase()
```

Output:

```text
UnboundLocalError: local variable 'count' referenced before assignment
```

Python assumes `count` is a local variable because it is assigned a value inside the function.

To modify a global variable inside a function, use the `global` keyword.

```py
count = 10

def increase():
    global count
    count += 1

increase()

print(count)
```

Output:

```text
11
```

> **Note:** Although the `global` keyword exists, it is generally considered good practice to avoid modifying global variables whenever possible. Instead, prefer passing values as parameters and returning the updated result.

<p align="center">
    <image src="images/VariableScopeMeme.png" width="400px" />
</p>