# For Loops

Often, we know how many iterations a loop needs to perform before it starts. In these cases, we use a `for` loop. It iterates over a sequence, executing a block of code once for each element.

The basic syntax is:

```py
for variable in sequence:
    # Code to repeat
```

- `variable` - You can name this whatever you like. It represents the current element of the sequence during each iteration.
- `sequence` - The collection being iterated over, such as a list, tuple, string, set, dictionary, or the result of `range()`.

## Iterating Over a String

A string is a sequence of characters, so you can iterate over each character:

```py
text = "Python"

for character in text:
    print(character)
```

Output:

```text
P
y
t
h
o
n
```

## Iterating Over a List

You can also iterate over every element in a list.

```py
fruits = ["apple", "banana", "orange"]

for fruit in fruits:
    print(fruit)
```

Output:

```text
apple
banana
orange
```

The loop variable (`fruit` in this example) takes the value of each element, one at a time.

## The `range()` Function

Sometimes you don't want to iterate over a sequence, you simply want to repeat an action a certain number of times.

The `range()` function generates a sequence of numbers.

```py
for number in range(5):
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

Notice that `range(5)` starts at `0` and stops before `5`.

You can also specify a starting value:

```py
for number in range(3, 8):
    print(number)
```

Output:

```text
3
4
5
6
7
```

And you can specify a step:

```py
for number in range(2, 11, 2):
    print(number)
```

Output:

```text
2
4
6
8
10
```

A negative step counts backwards:

```py
for number in range(5, 0, -1):
    print(number)
```

Output:

```text
5
4
3
2
1
```

You can also use this function to iterate over lists by accesing their elements by index:

```py
fruits = ["apple", "banana", "orange"]

for i in range(3):
    print(fruits[i])
```
> **Note:** It is common to use i as the loop variable. It is short for index.

Output:

```text
apple
banana
orange
```

Although `while` loops can be used in many of the same situations as `for` loops, `for` loops are usually the better choice when iterating over a sequence. They are less prone to infinite loops because the iteration is handled automatically, reducing the chance of forgetting to update the loop condition.

<p align="center">
    <image src="images/ForLoopMeme.png" width="400px" />
</p>

Next topic: [Break and Continue](BreakandContinue.md)