# Strings

Although strings are a basic data type, they behave similarly to lists of characters.

Just like in lists, each character in a string can be accessed by its index:

```py
text = "Python"

print(text[0]) # Output: P
print(text[1]) # Output: y
print(text[5]) # Output: n
```

### Immutability

Like tuples, strings are **immutable**, which means their characters cannot be modified.

```py
text = "Python"

text[0] = "J"
```

Output:

```text
TypeError: 'str' object does not support item assignment
```

If you want to "modify" a string, you must create a new one. This is usually done by **slicing** the string leaving that character out.

### Slicing

Since strings behave like sequences of characters, you can extract parts of them using **slicing**.

The basic syntax is:

```py
string[start:stop]
```

- `start` is the index of the first character to include.
- `stop` is the index where the slice ends (**not included**).

For example:

```py
text = "Python"

print(text[0:2]) # Output: Py
print(text[2:6]) # Output: thon
print(text[1:4]) # Output: yth
```

If you omit the `start` index, the slice begins at the start of the string.

```py
text = "Python"

print(text[:3]) # Output: Pyt
```

If you omit the `stop` index, the slice continues to the end of the string.

```py
text = "Python"

print(text[2:]) # Output: thon
```

Negative indexes work as well:

```py
text = "Python"

print(text[-3:])  # Output: hon
print(text[:-2])  # Output: Pyth
```

You can also provide a third value, called the **step**, which determines how many characters to skip.

```py
text = "Python"

print(text[::2])  # Output: Pto
print(text[1::2]) # Output: yhn
```

A negative step traverses the string backwards.

```py
text = "Python"

print(text[::-1]) # Output: nohtyP
```
