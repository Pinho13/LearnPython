# Complex Data Types

So far, you've learned about Python's basic data types. However, sometimes a single value isn't enough, and you need a way to store multiple values in one variable. To make this possible, Python provides several **collection data types**, which allow you to group and organize related values together.

Here are the ones we will be going over:
- Lists - [1, 2, 3]
- Tuples - (1, 2, 3)
- Sets - {1, 2, 3}
- Dictionaries - {"one": 1, "two": 2, "three": 3}

All of them can store different data types at the same time.

These data types are used to store multiple values in the same variable. Although they have many similarities, they differ in how they store and manage data, making each one suitable for different situations.

## Lists

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

### Modifying Elements

Lists are mutable, which means you can change the value of their elements after the list is created:

```py
fruits = ["apple", "banana", "orange"]

fruits[1] = "grape"

print(fruits) # Output: ['apple', 'grape', 'orange']
```

### Adding Elements

Collection data types come with built-in methods that make it easy to interact with and modify them. You can call a method by writing the variable name, followed by a dot (`.`), and then the method name.

To add an element to the end of the list, use the `append()` function:

```py
fruits = ["apple", "banana"]

fruits.append("orange")

print(fruits) # Output: ['apple', 'banana', 'orange']
```

### Removing Elements

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

### List Length

Use `len()` to find the number of elements in a list.

```py
fruits = ["apple", "banana", "orange"]

print(len(fruits)) # Output: 3
```

### Membership

Use the `in` operator to check whether an element exists in a list.

```py
fruits = ["apple", "banana", "orange"]

print("banana" in fruits)   # Output: True
print("grape" in fruits)    # Output: False
```

### List Summary

Lists are one of the most commonly used data types in Python. They are useful whenever you need to store and manipulate a collection of related values.

Lists are:
- Accessed by index (starting at 0)
- Ordered
- Mutable (can be changed)
- Allow duplicates

## Tuples

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

### Immutability

Unlike lists, tuples are **immutable**, which means their elements cannot be changed after the tuple is created.

```py
fruits = ("apple", "banana", "orange")

fruits[1] = "grape"
```

Output:

```text
TypeError: 'tuple' object does not support item assignment
```

### Tuple Summary

Because tuples are immutable, they are often used to store data that should not change throughout the execution of a program. Lists, on the other hand, are better suited for collections that need to be modified.

Tuples are:
- Accessed by index (starting at 0)
- Ordered
- Immutable (cannot be changed)
- Allow duplicates

## Sets

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

### Adding Elements

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

### Removing Elements

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

#### Union

The **union** of two sets contains every unique element from both sets.

```py
set1 = {1, 2, 3}
set2 = {3, 4, 5}

print(set1 | set2) # Output: {1, 2, 3, 4, 5}
```

#### Intersection

The **intersection** of two sets contains only the elements that appear in both sets.

```py
set1 = {1, 2, 3}
set2 = {3, 4, 5}

print(set1 & set2) # Output: {3}
```

#### Difference

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

### Set Summary

Sets are useful whenever you need to store **unique** values or compare groups of values using set operations.

Sets are:

- Unordered
- Mutable (can be changed)
- Do not allow duplicates
- Not accessed by index
- Support union (`|`), intersection (`&`), and difference (`-`)

## Dictionaries

A **dictionary** stores data as **key-value pairs**. Instead of accessing values by their position, like in a list or tuple, you access them using their **keys**.

Dictionaries are created using curly braces (`{}`), where each key is followed by a colon (`:`) and its corresponding value:

```py
student = {
    "name": "John",
    "age": 18,
    "passed": True
}

empty = {}
```

In this example:

- `"name"`, `"age"`, and `"passed"` are the **keys**.
- `"John"`, `18`, and `True` are the **values**.

### Accessing Values

Use a key inside square brackets (`[]`) to access its corresponding value.

```py
student = {
    "name": "John",
    "age": 18,
    "passed": True
}

print(student["name"])   # Output: John
print(student["age"])    # Output: 18
```

Trying to access a key that doesn't exist raises an error.

```py
print(student["height"])
```

Output:

```text
KeyError: 'height'
```

### Modifying Values

Assign a new value to an existing key to update it.

```py
student = {
    "name": "John",
    "age": 18
}

student["age"] = 19

print(student) # Output: {'name': 'John', 'age': 19}
```

### Adding Key-Value Pairs

Assign a value to a new key to add it to the dictionary.

```py
student = {
    "name": "John",
    "age": 18
}

student["passed"] = True

print(student) # Output: {'name': 'John', 'age': 18, 'passed': True}
```

### Removing Key-Value Pairs

Use `pop()` to remove a key and its associated value.

```py
student = {
    "name": "John",
    "age": 18,
    "passed": True
}

student.pop("passed")

print(student) # Output: {'name': 'John', 'age': 18}
```

Trying to remove a key that doesn't exist raises an error.

```py
student.pop("height")
```

Output:

```text
KeyError: 'height'
```

### Dictionary Length

As all complex data types, use `len()` to find the number of key-value pairs in a dictionary.

```py
student = {
    "name": "John",
    "age": 18,
    "passed": True
}

print(len(student)) # Output: 3
```

### Membership

Use the `in` operator to check whether a **key** exists in a dictionary.

```py
student = {
    "name": "John",
    "age": 18
}

print("name" in student)   # Output: True
print("grade" in student)  # Output: False
```

> **Note:** The `in` operator checks for **keys**, not values.

### Key Differences from Lists

Although dictionaries and lists both store multiple values, they are designed for different purposes.

The main differences are:

- Dictionaries store **key-value pairs**, while lists store individual values.
- Dictionary values are accessed using **keys**, while list elements are accessed using **indexes**.
- Keys must be **unique**, but multiple keys can have the same value.
- Dictionaries are ideal for storing related pieces of information about an object.

For example, compare these two ways of storing information about a student:

Using a list:

```py
student = ["John", 18, True]

print(student[0])  # Output: John
```

Using a dictionary:

```py
student = {
    "name": "John",
    "age": 18,
    "passed": True
}

print(student["name"])  # Output: John
```

The dictionary version is much easier to read because each value has a meaningful name.

### Dictionary Summary

Dictionaries are useful for storing data that has a natural relationship between names (keys) and values.

Dictionaries are:

- Accessed by keys
- Mutable (can be changed)
- Store key-value pairs
- Require unique keys
- Preserve insertion order (since python 3.7)