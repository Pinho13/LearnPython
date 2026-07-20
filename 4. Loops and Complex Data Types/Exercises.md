# Exercises

## 1. Count to N

Given a positive integer `n`, print all numbers from **1** to `n`, each on a new line.

| Input | Output |
|:------|:-------|
| 5 | 1 / 2 / 3 / 4 / 5 |
| 3 | 1 / 2 / 3 |

## 2. Sum of Numbers

Given a positive integer `n`, print the sum of all numbers from **1** to `n`.

| Input | Output |
|:------|:-------|
|   5   |   15   |
|   10  |   55   |

## 3. Remove Duplicates

Given a list of numbers, print a new list containing only the unique values.

| Input | Output |
|:------|:-------|
| `[1, 2, 2, 3, 1]` | `[1, 2, 3]` |
| `[5, 5, 5]` | `[5]` |

> **Hint:** Try casting the `list` to a `set`. Ex.: `set([1, 2, 3])`

## 4. Shopping List

Keep asking the user to enter items for a shopping list.

When the user enters `done`, stop asking for input and print the complete list.

| Example Input | Example Output |
|:--------------|:---------------|
| milk / eggs / bread / done | `['milk', 'eggs', 'bread']` |

## 5. Character Frequency

Given a string, count how many times each character appears.

| Input | Output |
|:------|:-------|
| hello | `{'h': 1, 'e': 1, 'l': 2, 'o': 1}` |
| aab | `{'a': 2, 'b': 1}` |

## 6. Common Elements

Given two lists, print a list containing only the elements that appear in both.

| Input | Output |
|:------|:-------|
| `[1, 2, 3]` / `[2, 3, 4]` | `[2, 3]` |
| `[5, 6]` / `[1, 2]` | `[]` |

## 7. Prime Number Checker

Given an integer greater than **1**, determine whether it is a prime number.

| Input | Output |
|:------|:-------|
|   7   |  Prime |
| 12 | Not prime |

## 8. Count Character Occurrences

Given a list of words and a character, count how many times the character appears in all the words combined.

| Input | Output |
|:------|:-------|
| `["apple", "banana", "pear"]` / `a` | `6` |
| `["hello", "world"]` / `l` | `3` |

> **Hint:** The `count()` method can be used to count how many times a character appears in a string. Ex.: `"hello".count("l")`

## 9. Longest Common Prefix

Given a list of words, print the **longest common prefix** shared by all of them.

A **prefix** is a sequence of characters at the beginning of a word.

| Input | Output |
|:------|:-------|
| `["april", "apple"]` | `ap` |
| `["flower", "flow", "flight"]` | `fl` |
| `["dog", "racecar", "car"]` | `""` |

> **Note:** If the words have no common prefix, print an empty string (`""`).

Next topic: [What are Functions](../5.%20Functions/WhatAreFunctions.md)