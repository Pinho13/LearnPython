# Important Functions

Python provides many built-in functions that are very useful. We have already seen a few of them, such as ```print()``` and ```type()```. Below is a list of some important functions that will be helpful as you continue learning:

* ```print()``` - displays text in the terminal
* ```type()``` - returns the type of a value
* ```input()``` - receives input from the user
* ```len()``` - returns the length of a string
* ```round()``` - rounds a float

> The functions discussed earlier will be skipped here. If needed, please refer back to the previous topics.

## input()

This function pauses the program and waits for the user to type something. Whatever the user enters is then returned by the function and can be stored in a variable for later use:

```py
text = input()

print(text)
```

This function can also take a string as a parameter. The string will be displayed to the user before they are asked for input:

```py
name = input("Enter your name: ")

print(name)
```

You can also use this function directly inside ```print()``` if the value is not going to be reused:

```py
print(input("Enter your name: "))
```

If you want to get integers (or other types of numbers) from the user, be careful: input() always returns a string. You will need to convert it to the correct type before using it in calculations.

```py
number = input("Enter your number: ")

print(type(number)) # Output: <class 'str'>
```

In this example you can just cast it to an int so you can use it in calculations and such.

```py
number_1 = int(input("Enter the first number: "))
number_2 = int(input("Enter the second number: "))

print(number_1 + number_2)
```

<p align="center">
    <image src="images/InputFunctionMeme.png" width="400px"/>
</p>


## len()

This function returns the number of elements in a value. For example, it can count the number of characters in a string, or the number of items in a list (we’ll learn about lists later).

```py
number_of_char = len("Hello world!")

print(number_of_char) # Output: 12
```

## round()

This function rounds a float to the nearest integer. Be careful: Python uses a method called **banker’s rounding**. This means that if a number is exactly halfway between two integers, it rounds to the nearest even number.

```py
print(round(2.3)) # Output: 2
print(round(2.5)) # Output: 2
print(round(2.7)) # Output: 3
print(round(3.5)) # Output: 4
print(round(3.3333)) # Output: 3
print(round(3.75)) # Output: 4
```

Next Topic: [Comments](Comments.md)