# Lists

A **list** is an ordered collection of values. Unlike variables, which store a single value, a list can store multiple values in a single variable.

Lists are created using square brackets (`[]`), with each element separated by a comma:

```py
fruits = ["apple", "banana", "orange"]
numbers = [1, 2, 3, 4, 5]
mixed = ["John", 18, True, 1.75]
empty = []
```

Each of the values stored in a list can be accessed by its position, this is called the **index**.

Indexes start at **0**:

```py
fruits = ["apple", "banana", "orange"]

first_value = fruits[0]
second_value = fruits[1]
last_value = fruits[2]

print(first_value) # Output: apple
print(second_value) # Output: banana
print(last_value) # Output: orange
```

You can also use negative indexes to access elements from the last of the list:

```py
fruits = ["apple", "banana", "orange"]

print(fruits[-1]) # Output: orange
```

However if you try accessing an invalid index, you will get an error:

```py
fruits = ["apple", "banana", "orange"]

print(fruits[5])
```

Output:

```text
IndexError: list index out of range
```

## Modifying Elements

Lists are mutable, which means you can change the value of their elements after the list is created:

```py
fruits = ["apple", "banana", "orange"]

fruits[1] = "grape"

print(fruits) # Output: ['apple', 'grape', 'orange']
```

## Adding Elements

Collection data types come with built-in methods that make it easy to interact with and modify them. You can call a method by writing the variable name, followed by a dot (`.`), and then the method name.

To add an element to the end of the list, use the `append()` function:

```py
fruits = ["apple", "banana"]

fruits.append("orange")

print(fruits) # Output: ['apple', 'banana', 'orange']
```

## Removing Elements

Use `remove()` to remove an element by its value.

```py
fruits = ["apple", "banana", "orange"]

fruits.remove("banana")

print(fruits) # Output: ['apple', 'orange']
```

You can also use `pop()` to remove an element by its index.

```py
numbers = [10, 20, 30]

numbers.pop(1)

print(numbers) # Output: [10, 30]
```

If no index is provided, `pop()` removes the last element.

```py
numbers = [10, 20, 30]

numbers.pop()

print(numbers) # Output: [10, 20]
```

## List Length

Use `len()` to find the number of elements in a list.

```py
fruits = ["apple", "banana", "orange"]

print(len(fruits)) # Output: 3
```

## Membership

Use the `in` operator to check whether an element exists in a list.

```py
fruits = ["apple", "banana", "orange"]

print("banana" in fruits)   # Output: True
print("grape" in fruits)    # Output: False
```

## List Summary

Lists are one of the most commonly used data types in Python. They are useful whenever you need to store and manipulate a collection of related values.

Lists are:
- Accessed by index (starting at 0)
- Ordered
- Mutable (can be changed)
- Allow duplicates

[Go Back](../ComplexDataTypes.md)