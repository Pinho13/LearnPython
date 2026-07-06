# Comparison Operators

Comparison operators are used to compare any two values.

<div align="center">

| Operator |           Name           |  Example |
|:--------:|:------------------------:|:--------:|
|    ==    |          Equal           |  x == y  |
|    !=    |         Not equal        |  x != y  |
|     >    |       Greater than       |  x > y   |
|     <    |         Less than        |  x < y   |
|    >=    | Greater than or equal to |  x >= y  |
|     <=   |   Less than or equal to  |  x <= y |

</div>

The result of a comparison is always either ```True``` or ```False```:

```py
print(5 == 5) # Output: True
print(10 != 9) # Output: True
print( 20 < 10) # Output: False
print( 20 > 10) # Output: True
```

You can also compare other data types:

```py
print("Hello" == "Bye") # Output: False
print(True != False) # Output: True
print(2.2 != 2.2) # Output: False
print(10 == 10.1) # Output: False
print(False == 0) # Output: True
print((10 >= 10) != True) # Output: False
print(type(1) == type(1.0)) # Output: False
```
> Note: 0 represents ```False``` and 1 represents ```True``` that is why you can compare them to numbers

<p align="center">
    <image src="images/BooleanMeme.jpeg" width="400px" />
</p>

Variables work as expect:

```py
x = "Hello"
y = False

print(x == y) # Output: False
```

As you've seen, comparisons are the foundation of conditional logic. Whenever you want your program to perform different actions based on one or more values, the first step is to compare those values.

<p align="center">
    <image src="images/ComparisonOperatorsMeme.jpeg" width="300px" />
</p>

Next topic: [Logical Operators](LogicalOperators.md)