# Logical Operators

Logical operators are used to combine comparison statements to make more complex conditions.

<div align="center">

| Operator | Name | Example |
|:--------:|:----:|:-------:|
| and | Returns `True` if both statements are true | x < 5 and x < 10 |
| or  | Returns `True` if one statement is true | x < 5 or x < 4 |
| not | Reverses the statement result | not (x < 5)|

</div>

Logical operators also always return either `True` or `False`:

```py
print(True and True)    # Output: True
print(True and False)   # Output: False
print(True or False)    # Output: True
print(False or False)   # Output: False
print(not True)         # Output: False
print(not False)        # Output: True
```

Here are some more realistic use cases:

```py
age = 20
has_ticket = True

print(age >= 18 and has_ticket)      # Output: True
print(age >= 21 or has_ticket)       # Output: True
print(not has_ticket)                # Output: False
print(age < 18 and has_ticket)       # Output: False
```

You can chain as many conditions together with logical operators as you want. However, as always, try to keep your expressions clear and easy to read:

```py
age = 20
minimum_age_required = 18
ticket_price = 6.5
wallet = 10
has_ticket = False

can_enter = age >= minimum_age_required and (has_ticket or wallet >= ticket_price)


print(can_enter) # Output: True
```
<br>

<p align="center">
    <image src="images/LogicalOperatorsMeme.png" width="400px" />
</p>

Next topic: [If Statements](IfStatements.md)