# Arithmetic Operators

Arithmetic operators are symbols used to perform mathematical operations in Python.


<div align="center">

| Operator |       Name      | Example |
|:--------:|:---------------:|:-------:|
|     +    |    Addition     |  x + y  |
|     -    |   Subtraction   |  x - y  |
|     *    | Multiplication  |  x * y  |
|     /    |    Division     |  x / y  |
|     %    |     Modulus     |  x % y  |
|     **   | Exponentiation  |  x ** y  |
|     //   |  Floor division |  x // y  |

</div>

> Note: The **modulus** operator (**%**) returns the remainder of a division between two numbers.

> Note: **Floor division** (**//**) divides two numbers and returns the result rounded down to the nearest integer.

You can combine arithmetic operators to perform more complex calculations:

```py
print(5 + 10 * 2)
```

But be careful, always be clear when making more complex calculations.

Use parentheses to clarify your intent and control the order of operations:

```py
print(6 / (2 * (1 + 2))) # Output: 1

print((6 / 2) * (1 + 2)) # Output: 9
```


<p align="center">
    <image src="images/OrderOfOperationsMeme.jpeg" />
</p>

Next Topic: [Important Functions](ImportantFunctions.md)
