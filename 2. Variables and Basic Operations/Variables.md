# Variables

Variables are easy to understand. They are simply containers with a name that store values.

<p align="center">
    <image src="images/VariablesVisualization.png" />
</p>

Let’s use the same example from before:

```py
print("Hello, world!")
```

We can, for example, turn ```"Hello, world!"``` into a variable like this:

```py
message = "Hello, world!"

print(message)
```

Now, every time we use ```message``` in our code, we are referring to the string ```"Hello, world!"```.

To create a variable, you simply write the variable name, followed by an equals sign (```=```), and then the value you want to assign to it, as shown in the example above.

There are a few rules to name variables:
* Variable names can only contain **letters**, **digits** and **underscores** (```_```)
* A variable name cannot start with a digit
* Variable names are case-sensitive (```myVar``` is different than ```myvar```)

Avoid using python keywords as variable names:

```py
# This is wrong
print = "Hello, world!"
```

Apart from that, you can use variables just like you would use the values themselves.

```py
print(5 + 10) # Result is 15
```

This is the same as:

```py
number_1 = 5
number_2 = 10

print(number_1 + number_2) # Result is 15
``` 

Which is also the same as:

```py
number_1 = 5
number_2 = 10

number_3 = number_1 + number_2

print(number_3) # Result is 15
``` 

Be mindful when naming variables and try to choose names that clearly describe what they represent.

<p align="center">
    <image src="images/ChoosingVariableNameMeme.jpg" width="400px"/>
</p>

Next topic: [Basic Data Types](BasicDataTypes.md)