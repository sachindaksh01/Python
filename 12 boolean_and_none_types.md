# 🐍 Python Programming Notes – Lecture 12

## ✅ Boolean and None Types in Python

This lecture covers two fundamental Python data types:

- **Boolean** (`True` and `False`)
- **NoneType** (`None` – represents no value)

---

## 1️⃣ Boolean Type

### 🔹 Boolean Values

```python
is_sunny = True
is_raining = False
print(is_sunny)     # True
print(is_raining)   # False
```

Booleans are often used to **control flow** using `if`, `while`, and other logic-based conditions.

---

## 2️⃣ Boolean Expressions

Python uses **comparison operators** that return Boolean values:

| Operator | Meaning               | Example   | Output |
| -------- | --------------------- | --------- | ------ |
| `==`     | Equal to              | `10 == 5` | False  |
| `!=`     | Not equal to          | `10 != 5` | True   |
| `>`      | Greater than          | `10 > 5`  | True   |
| `<`      | Less than             | `10 < 5`  | False  |
| `>=`     | Greater than or equal | `5 >= 5`  | True   |
| `<=`     | Less than or equal    | `3 <= 5`  | True   |

---

## 3️⃣ Boolean Operators

### 🔸 `and`, `or`, `not`

```python
a = True
b = False
print(a and b)   # False
print(a or b)    # True
print(not a)     # False
```

---

## 4️⃣ Boolean in Control Flow

```python
age = 18

if age >= 18:
    print("You are eligible to vote.")
else:
    print("You are not eligible to vote.")
```

---

## 5️⃣ None Type

`None` is a special constant in Python used to represent **no value / nothing**.

### 🔹 Declaration and Checking

```python
x = None
print(x)               # None
print(type(x))         # <class 'NoneType'>
```

### 🔹 Using `is` to check for None

```python
x = None
if x is None:
    print("x has no value")
```

---

## 🧪 Practice Set 12: Boolean and None

1. ✅ Write a program that returns `True` if a number is positive.
2. 🔍 Declare a variable with `None` and print its type.
3. 🔁 Check if two numbers are equal using `==` and print the result.
4. 📭 Write a function that returns `True` if a string is empty.
5. 🔍 Check if a number exists in a list using `in` and Boolean.
6. ⚡ Use a Boolean in an `if` statement to decide output.
7. 🔁 Check if a number is even or odd using Boolean logic.
8. 📌 Use `is` to compare two variables, one of which is `None`.

---

## 📝 Summary

- ✅ Booleans are `True` or `False`, used for logical decisions
- ✅ Use comparison and logical operators to form Boolean expressions
- ✅ `None` means no value is assigned
- ✅ Use `is` to check for `None` safely

---

> 🎯 Next Lecture: Python Operators — Dive deeper into arithmetic, logical, assignment and bitwise operators!

