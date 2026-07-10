# Exercises

> Note: The symbol // is used to indicate a line separation, like a paragraph for each part of the output.

## 1. Length Printer

Given a string, print its length.

| Input        | Output |
|:-------------|:-------|
| Banana       | 6      |
| Hello world! | 12     |

[Solution](solutions/1.Length_Printer.py)

## 2. Divider

Given two positive numbers, divide them and round the result to 2 decimal places.

| Input  | Output |
|--------|--------|
| 1 / 3  | 0.33   |
| 3 / 17 | 0.18   |

[Solution](solutions/2.Divider.py)

## 3. Average Calculator

Given three integer numbers, print their average rounded to 1 decimal place.

| Input      | Output |
|------------|--------|
| 1 / 3 / 5  | 3.0    |
| 3 / 17 / 6 | 8.7    |

[Solution](solutions/3.Average_Calculator.py)

## 4. Hypotenuse Calculator

Given the length of two sides of a right-angled triangle, make a hypotenuse calculator. Round the result to 3 decimal places.

| Input  | Output |
|--------|--------|
| 3 / 8  | 8.544  |
| 1 / 17 | 17.029 |

> Note: Taking the square root of a number is the same as raising it to the power of **0.5**.

[Solution](solutions/4.Hypotenuse_Calculator.py)

## 5. Repeated Digit Sum

Given a single-digit number n, compute and output the result of n + nn + nnn.

| Input | Output                    |
|:------|:--------------------------|
| 5     | 5 + 55 + 555 = 615        |
| 17    | 17 + 1717 + 171717 = 2091 |

[Solution](solutions/5.Repeated_Digit_Sum.py)

## 6. Quadratic Formula

Given three numbers (a, b and c), make a quadratic formula calculator. The result should be rounded to 5 decimal places. 

| Input      | Output                                            |
|:-----------|---------------------------------------------------|
| 1 / -5 / 6 | First Result:  3.0 // Second Result:  2.0         |
| 1 / -3 / 1 | First Result:  2.61803 // Second Result:  0.38197 |

[Solution](solutions/6.Quadratic_Formula.py)

## 7. String Repeater

Given a string and a number n, repeate that string n times.

| Input | Output                   |
|:------|--------------------------|
| ter   | terterterterterter       |
| aqui  | aquiaquiaquiaquiaquiaqui |

[Solution](solutions/7.String_Repeater.py)

## 8. Change

You are a cashier. Given an amount of change to give to a customer, write a Python program that calculates how many banknotes of each value are needed.

The available banknotes are 50€, 20€, 10€, and 5€.

Your program should output the number of banknotes in the following format: ```# 50 / # 20 / # 10 / # 5```

Replace each ```#``` with the number of banknotes of that value.

Extra - In case banknotes are not sufficient, print the remaining change.

Example:

| Input        | Output                                          |
|:-------------|:------------------------------------------------|
| 245          | 4 50 / 2 20 / 0 10 / 1 5                        |
| 356          | 7 50 / 0 20 / 0 10 / 1 5 // Remaining change: 1 |

[Solution](solutions/8.Change.py)

## 9. Future Time

It is currently 18:07. If you go to sleep now, and you are given the number of hours and minutes you will sleep for, write a Python program that calculates and displays the time shown on the clock when you wake up.

Example:

| Input        | Output                                                             |
|:-------------|:-------------------------------------------------------------------|
| 04:20        | Wake-Up time: 22:27                                                |
| 03:63        | Wake-Up time: 22:10                                                |
| 27:45        | Wake-Up time: 21:52 // Not the same day, 1 day(s) after you slept. |

[Solution](solutions/9.Future_Time.py)
