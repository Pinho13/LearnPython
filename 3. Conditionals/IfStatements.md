# If Statements

## If ...

An `if` statement allows your program to execute code only when a condition is `True`.

To make an if statement you have to write `if` followed by a condition and `:`:

```py
age = 20

if age >= 18:
    print("You are an adult") # Output: You are an adult
```

Notice the space before the print() statement. This is called indentation. In Python, indentation is significant, it tells the interpreter which lines of code belong to the if statement.

If the condition is `False`, the indented code is skipped:

```py
age = 15

if age >= 18:
    print("You are an adult")

print("Program finished") # Output: Program finished
```

You can use any expression that evaluates to `True` or `False`:

```py
temperature = 28
is_sunny = True

if temperature > 25 and is_sunny:
    print("It's a great day to go outside!")
```

If you forget to indent the code, Python will raise an error:

```py
if True:
print("Hello")
```

Output:

```text
IndentationError: expected an indented block
```

## If ... else

Sometimes you may want different outcomes depending if it is `True` or `False`.

For that we have the `else` keyword:

```py
age = 16

if age >= 18:
    print("You are an adult")
else:
    print("You are a minor") # Output: You are a minor
```

An `else` statement lets you specify what should happen when the `if` condition is `False`.

Only one of the two blocks will execute. If the `if` condition is `True`, the `else` block is skipped. Otherwise, the `else` block runs.

Just like `if` statements, the code inside the `else` block must be indented:

```py
is_logged_in = False

if is_logged_in:
    print("Welcome back!")
else:
    print("Please log in.")
```

The `else` block doesn't have a condition. It simply runs whenever the `if` condition is `False`.

## If ... elif ... else

An `elif` statement lets you check another condition if the previous `if` (or `elif`) condition was `False`.

Python evaluates the conditions from top to bottom. As soon as it finds one that is `True`, it executes that block and skips the rest:

```py
grade = 85

if grade >= 90:
    print("Grade: A")
elif grade >= 70:
    print("Grade: B") # Output: Grade: B
elif grade >= 50:
    print("Grade: C")
else:
    print("Grade: F")
```

You can have as many `elif` statements as you need:

```py
temperature = 12

if temperature >= 30:
    print("It's hot.")
elif temperature >= 20:
    print("It's warm.")
elif temperature >= 10:
    print("It's cool.")
elif temperature >= 0:
    print("It's cold.")
else:
    print("It's freezing.")
```

The `else` block is not required and only runs if all of the above have been skipped.

Conditions are checked in order, so their order matters. Consider this example:

```py
age = 66
if age >= 18:
    print("Adult") # Output: Adult
elif age >= 65:
    print("Senior")
```

Even though `66` is a senior, this example illustrates an important rule: once the first condition is `True`, Python skips every remaining `elif` and `else` block.

You can nest as many `if` statements as you like:

```py
age = 20
has_ticket = True

if age >= 18:
    print("You are old enough to enter")

    if has_ticket:
        print("You may enter the cinema")
```

Output:

```text
You are old enough to enter.
You may enter the cinema.
```

Try to avoid nesting too many if statements. Deeply nested code can become difficult to read and understand. Whenever possible, simplify your conditions or combine them using logical operators.

For example, instead of writing:

```py
if age >= 18:
    if has_ticket:
        print("You may enter")
```

Just write:

```py 
if age >= 18 and has_ticket:
    print("You may enter.")
```

Both examples produce the same result, but the second is shorter, easier to read, and generally preferred.

<p align="center">
    <image src="images/IfStatementsMeme.png" width="600px" />
</p>

Next topic: [Exercises](Exercises.md)