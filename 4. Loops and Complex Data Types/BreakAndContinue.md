# Break and Continue

Sometimes you may want to change the normal flow of a loop. Python provides the `break` and `continue` statements for this purpose.

- `break` immediately exits the loop.
- `continue` skips the current iteration and moves on to the next one.

These statements can be used in both `for` and `while` loops.

## The `break` Statement

Use `break` when you want to stop a loop before it finishes.

For example:

```py
for number in range(10):
    if number == 5:
        break

    print(number)
```

Output:

```text
0
1
2
3
4
```

As soon as `number` becomes `5`, the `break` statement is executed and the loop ends immediately.

`break` is also commonly used with `while` loops.

```py
while True:
    password = input("Password: ")

    if password == "python":
        break

print("Access granted!")
```

In this example, the loop continues asking for the password until the correct one is entered.

## The `continue` Statement

Use `continue` when you want to skip the rest of the current iteration without stopping the loop.

For example:

```py
for number in range(6):
    if number == 3:
        continue

    print(number)
```

Output:

```text
0
1
2
4
5
```

When `number` is `3`, the `print()` statement is skipped, and the loop continues with the next iteration.

Another example:

```py
names = ["Alice", "", "Bob", "", "Charlie"]

for name in names:
    if name == "":
        continue

    print(name)
```

Output:

```text
Alice
Bob
Charlie
```

Here, empty strings are ignored, and only the valid names are printed.

<p align="center">
    <image src="images/BreakMeme.jpeg" width="500px" />
</p>

Next topic: [Exercises](Exercises.md)