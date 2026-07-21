# Exercises

> **Note:** The symbol `/` is used to indicate a line separation, like a paragraph for each part of the output.

## 1. Maximum of Three

Write a function that receives three numbers and returns the largest of them.

| Input | Output |
|:------|:-------|
| 5 / 3 / 8 | 8 |
| -2 / -7 / -1 | -1 |

## 2. Distance Between Two Points

Write a function that receives two points `(x1, y1)` and `(x2, y2)` and returns the distance between them.

The distance between two points is given by:

<p align="center">
    <image src="images/DistanceFormula.png" width="400px" />
</p>

| Input | Output |
|:------|:-------|
| `(0, 0)` / `(3, 4)` | 5.0 |
| `(1, 2)` / `(4, 6)` | 5.0 |

## 3. Primitive Calculator

Create four functions:

- `add(a, b)`
- `subtract(a, b)`
- `multiply(a, b)`
- `divide(a, b)`

Then, ask the user for two numbers and an operator (`+`, `-`, `*`, `/`) and call the appropriate function.

| Input | Output |
|:------|:-------|
| `5` / `+` / `3` | `8` |
| `12` / `/` / `4` | `3.0` |

## 4. Remove Even Numbers

Write a function that receives a list of integers and removes all even numbers.

| Input | Output |
|:------|:-------|
| `[1, 2, 3, 4, 5]` | `[1, 3, 5]` |
| `[2, 4, 6]` | `[]` |

## 5. Sort a List

Write your own function that sorts a list of integers in ascending order.

Do **not** use Python's built-in `sort()` method or the `sorted()` function.

| Input | Output |
|:------|:-------|
| `[5, 2, 8, 1]` | `[1, 2, 5, 8]` |
| `[9, 4, 7]` | `[4, 7, 9]` |

## 6. Mini Statistics

Write functions to calculate:

- the minimum
- the maximum
- the average
- the median

Then write another function that prints all of these statistics for a given list.

| Input | Output |
|:------|:-------|
| `[5, 2, 8, 1]` | Min: 1 / Max: 8 / Average: 4.0 / Median: 3.5 |

## 7. Prime Factorization

Write a function that receives a positive integer and returns a list containing its **prime factors**.

A **prime factor** is a prime number that divides another number exactly (without leaving a remainder). The product of all the prime factors is equal to the original number.

For example:

- 12 = 2 × 2 × 3
- 84 = 2 × 2 × 3 × 7

| Input | Output |
|:------|:-------|
| 12 | `[2, 2, 3]` |
| 84 | `[2, 2, 3, 7]` |

## 8. Caesar Cipher

Write two functions:

- `encrypt(text, shift)`
- `decrypt(text, shift)`

Each letter should be shifted by the given amount in the alphabet.

| Input | Output |
|:------|:-------|
| hello / 3 | khoor |
| abc / 1 | bcd |

> **Hint:** You may find `ord()` and `chr()` useful.

## 9. Tic-Tac-Toe Winner

Given a 3×3 Tic-Tac-Toe board, write a function that determines whether `X` has won, `O` has won, or if there is no winner.

| Input | Output |
|:------|:-------|
| `[['X','X','X'],['O','','O'],['','','']]` | X wins |
| `[['X','O','X'],['','O','O'],['X','O','']]` | O wins |

> **Hint:** Check all rows, columns, and diagonals.
