# Sets

A **set** is an unordered collection of unique values. Unlike lists and tuples, a set does **not** allow duplicate elements.

Sets are created using curly braces (`{}`), with each element separated by a comma:

```py
fruits = {"apple", "banana", "orange"}
numbers = {1, 2, 3, 4, 5}
mixed = {"John", 18, True, 1.75}
empty = set()
```

> **Note:** An empty set is created using `set()`, **not** `{}`. The expression `{}` creates an empty dictionary.

If you add duplicate values to a set, they are automatically removed:

```py
numbers = {1, 2, 2, 3, 3, 3}

print(numbers) # Output: {1, 2, 3}
```

Since sets are **unordered**, their elements do not have indexes. This means you cannot access elements by position:

```py
fruits = {"apple", "banana", "orange"}

print(fruits[0])
```

Output:

```text
TypeError: 'set' object is not subscriptable
```

> **Note:** Since sets are unordered, the order of their elements may be different each time you print them.

## Adding Elements

Use `add()` to insert a new element into a set.

```py
fruits = {"apple", "banana"}

fruits.add("orange")

print(fruits) # Output: {'apple', 'banana', 'orange'}
```

If the element already exists, nothing happens:

```py
fruits = {"apple", "banana"}

fruits.add("banana")

print(fruits) # Output: {'apple', 'banana'}
```

## Removing Elements

Use `remove()` to remove an element from a set.

```py
fruits = {"apple", "banana", "orange"}

fruits.remove("banana")

print(fruits) # Output: {'apple', 'orange'}
```

Trying to remove an element that doesn't exist raises an error:

```py
fruits.remove("grape")
```

Output:

```text
KeyError: 'grape'
```

### Key Differences from Lists

Although both lists and sets can store multiple values, they behave quite differently.

The main differences are:

- Sets are **unordered**, while lists preserve the order of their elements.
- Sets **do not allow duplicate values**.
- Sets are optimized for **fast membership checks** (checking if an element is `in` the set).
- Sets support mathematical set operations such as union, intersection, and difference.

### Union

The **union** of two sets contains every unique element from both sets.

```py
set1 = {1, 2, 3}
set2 = {3, 4, 5}

print(set1 | set2) # Output: {1, 2, 3, 4, 5}
```

### Intersection

The **intersection** of two sets contains only the elements that appear in both sets.

```py
set1 = {1, 2, 3}
set2 = {3, 4, 5}

print(set1 & set2) # Output: {3}
```

### Difference

The **difference** of two sets contains the elements that are in the first set but not in the second.

```py
set1 = {1, 2, 3}
set2 = {3, 4, 5}

print(set1 - set2) # Output: {1, 2}
```

Notice that order matters for the difference operation:

```py
print(set2 - set1) # Output: {4, 5}
```

## Set Summary

Sets are useful whenever you need to store **unique** values or compare groups of values using set operations.

Sets are:

- Unordered
- Mutable (can be changed)
- Do not allow duplicates
- Not accessed by index
- Support union (`|`), intersection (`&`), and difference (`-`)

<p align="center">
    <image src="../images/SetsMeme.jpg" width="500px" />
</p>

[Go Back](../ComplexDataTypes.md)