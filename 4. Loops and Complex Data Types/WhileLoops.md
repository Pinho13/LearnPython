# While Loops

Sometimes you need to repeat the same action several times. Python uses **loops** to execute a block of code repeatedly.

A `while` loop repeatedly executes a block of code as long as a condition is `True`.

The basic syntax is:

```py
while condition:
    # Code to repeat
```

Just like `if` statements, notice the colon (`:`) and the indentation. The indented code belongs to the loop and will be executed repeatedly while the condition is `True`.

For example:

```py
count = 1

while count <= 5:
    print(count)
    count += 1
```

Output:

```text
1
2
3
4
5
```

In this example:

- `count` starts at `1`.
- The condition `count <= 5` is checked.
- If it is `True`, the loop executes.
- `count` is increased by `1`.
- The condition is checked again.

This process repeats until the condition becomes `False`.

## Infinite Loops

If the condition never becomes `False`, the loop will run forever.

For example:

```py
count = 1

while count <= 5:
    print(count)
```

Since `count` is never updated, the condition is always `True`, creating an **infinite loop**.

To stop a program stuck in an infinite loop, you usually need to interrupt it manually (for example, by pressing **Ctrl + C** in the terminal).

## User Input

`while` loops are commonly used when you don't know in advance how many times something should repeat.

For example, keep asking the user for a password until they enter the correct one:

```py
password = ""

while password != "python":
    password = input("Password: ")

print("Access granted!")
```

## Nested While Loops

Like `if` statements, `while` loops can be nested.

```py
row = 1

while row <= 3:
    column = 1

    while column <= 4:
        print("*", end="")
        column += 1

    print()
    row += 1
```

Output:

```text
****
****
****
```

<p align="center">
    <image src="images/WhileLoopsMeme.jpeg" width="500px" />
</p>

Next topic: [For Loops](ForLoops.md)