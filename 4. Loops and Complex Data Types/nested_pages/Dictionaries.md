# Dictionaries

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

## Accessing Values

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

## Modifying Values

Assign a new value to an existing key to update it.

```py
student = {
    "name": "John",
    "age": 18
}

student["age"] = 19

print(student) # Output: {'name': 'John', 'age': 19}
```

## Adding Key-Value Pairs

Assign a value to a new key to add it to the dictionary.

```py
student = {
    "name": "John",
    "age": 18
}

student["passed"] = True

print(student) # Output: {'name': 'John', 'age': 18, 'passed': True}
```

## Removing Key-Value Pairs

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

## Dictionary Length

As all complex data types, use `len()` to find the number of key-value pairs in a dictionary.

```py
student = {
    "name": "John",
    "age": 18,
    "passed": True
}

print(len(student)) # Output: 3
```

## Membership

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

## Key Differences from Lists

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

## Dictionary Summary

Dictionaries are useful for storing data that has a natural relationship between names (keys) and values.

Dictionaries are:

- Accessed by keys
- Mutable (can be changed)
- Store key-value pairs
- Require unique keys
- Preserve insertion order (since python 3.7)

[Go Back](../ComplexDataTypes.md)