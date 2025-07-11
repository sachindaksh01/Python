# 🐍 Python Programming Notes – Lecture 16

## 🔁 Introduction to Loops in Python

A **loop** is used to repeat a block of code multiple times. Python provides two main types of loops:

- `for` loop
- `while` loop

They are very useful when we want to perform a task repeatedly without writing the same code again and again.

---

## 🔄 Why Use Loops?

Imagine needing to print 100 student names. Instead of writing 100 `print()` statements, you can use a loop that runs 100 times and prints them automatically.

---

## 🔁 `for` Loop vs `while` Loop

| Feature          | `for` Loop                            | `while` Loop                     |
| ---------------- | ------------------------------------- | -------------------------------- |
| Best Used When   | Number of iterations is known         | Condition is to be checked       |
| Structure        | `for i in range():`                   | `while condition:`               |
| Stops When       | Sequence ends                         | Condition becomes False          |
| Example Use Case | Looping through lists, strings, range | Repeating until user exits input |

---

## 🔂 `for` Loop Syntax

```python
for variable in sequence:
    # block of code
```

✅ `variable` takes each value from the `sequence` one by one.

### Example: Printing Items in a List

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

---

## 🔠 Iterating Over Strings

```python
name = "Python"
for char in name:
    print(char)
```

---

## 🔢 Using `range()` with for Loop

```python
for i in range(5):
    print(i)
```

⏩ Output: 0, 1, 2, 3, 4 (range stops before 5)

### `range(start, stop)`

```python
for i in range(1, 6):
    print(i)
```

⏩ Output: 1 to 5

---

## 🔁 Nested for Loops

Useful for working with tables (like multiplication tables).

```python
for i in range(1, 4):
    for j in range(1, 3):
        print(f"i: {i}, j: {j}")
```

---

## 🌍 Real-Life Examples Using `for` Loop

### 🧾 Example 1: Print Employee Names

```python
employees = ["Ravi", "Neha", "Ankit"]
for name in employees:
    print("Employee:", name)
```

### 📅 Example 2: Print Days of the Week

```python
days = ["Mon", "Tue", "Wed", "Thu", "Fri"]
for day in days:
    print("Today is:", day)
```

### 📦 Example 3: Inventory Count

```python
items = ["Pen", "Notebook", "Pencil"]
for item in items:
    print(f"Counting item: {item}")
```

### 🧮 Example 4: Sum of Prices

```python
prices = [100, 200, 150]
total = 0
for price in prices:
    total += price
print("Total Bill:", total)
```

---

## 🧪 Practice Set – For Loop

### 🔰 Beginner

1. 📃 Print numbers from 1 to 10 using a `for` loop
2. 🧍 Print all names in a list of students
3. 📖 Print each letter in the word "Python"

### ⚙️ Intermediate

4. ➕ Find the sum of numbers in the list [5, 10, 15, 20]
5. 🔁 Print even numbers from 1 to 20
6. 🧾 Print a shopping list using `for` loop

### 🚀 Advanced

7. ➗ Print a multiplication table of 5
8. 🔄 Print numbers from 10 to 1 (reverse loop)
9. ➗ Find the factorial of a number using `for` loop
10. 🔡 Count the number of vowels in a sentence

```python
sentence = "Welcome to Python!"
vowels = "aeiouAEIOU"
count = 0
for char in sentence:
    if char in vowels:
        count += 1
print("Total vowels:", count)
```

---

## 📝 Summary

- ✅ Loops save time and reduce repetitive code
- ✅ Use `for` loop to iterate over sequences (list, string, range)
- ✅ `range()` helps to loop for a fixed number of times
- ✅ Nest loops to work with grids or tables

---

> 🎯 Next Lecture: `while` Loop — Learn how to use condition-controlled loops for repetition!

