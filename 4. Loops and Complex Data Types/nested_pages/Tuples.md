# Tuples

A **tuple** is an ordered collection of values. Like a list, a tuple can store multiple values in a single variable.

Tuples are created using parentheses (`()`), with each element separated by a comma:

```py
fruits = ("apple", "banana", "orange")
numbers = (1, 2, 3, 4, 5)
mixed = ("John", 18, True, 1.75)
empty = ()
```

Just like lists, each element in a tuple can be accessed by its **index** in the same way.

Only the key differences from lists will be mentioned.

## Immutability

Unlike lists, tuples are **immutable**, which means their elements cannot be changed after the tuple is created.

```py
fruits = ("apple", "banana", "orange")

fruits[1] = "grape"
```

Output:

```text
TypeError: 'tuple' object does not support item assignment
```

## Tuple Summary

Because tuples are immutable, they are often used to store data that should not change throughout the execution of a program. Lists, on the other hand, are better suited for collections that need to be modified.

Tuples are:
- Accessed by index (starting at 0)
- Ordered
- Immutable (cannot be changed)
- Allow duplicates

<p align="center">
    <image src="../images/TuplesMeme.png" width="600px" />
</p>


[Go Back](../ComplexDataTypes.md)