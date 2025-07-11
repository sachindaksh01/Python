# 🐍 Python Programming Notes – Lecture 14

## 🔍 Comparison, Logical, Identity & Membership Operators

This lecture includes all the core comparison and logic-based operators in Python:

- Comparison Operators
- Logical Operators
- Identity Operators
- Membership Operators

---

## 1️⃣ Comparison Operators

Used to compare two values. Always returns `True` or `False`.

| Operator | Description           | Example | Result |
| -------- | --------------------- | ------- | ------ |
| `==`     | Equal to              | 5 == 3  | False  |
| `!=`     | Not equal to          | 5 != 3  | True   |
| `<`      | Less than             | 5 < 3   | False  |
| `>`      | Greater than          | 5 > 3   | True   |
| `<=`     | Less than or equal    | 5 <= 3  | False  |
| `>=`     | Greater than or equal | 5 >= 3  | True   |

### 🔹 Example:

```python
x = 5
y = 3
print(x == y)  # False
print(x >= y)  # True
```

---

## 2️⃣ Logical Operators

Used to combine multiple conditions.

| Operator | Description                          | Example          |
| -------- | ------------------------------------ | ---------------- |
| `and`    | Returns True if both conditions true | x > 5 and x < 10 |
| `or`     | Returns True if one condition true   | x > 5 or x < 3   |
| `not`    | Reverses the result                  | not(x > 5)       |

### 🔹 Example:

```python
x = 10
y = 20

if x > 5 and y > 10:
    print("Both conditions are True")

if x < 5 or y > 15:
    print("At least one condition is True")

if not (x < y):
    print("x is not less than y")
```

---

## 3️⃣ Identity Operators

Used to compare object references (memory locations).

| Operator | Description             | Example    |
| -------- | ----------------------- | ---------- |
| `is`     | True if same object     | a is b     |
| `is not` | True if not same object | a is not b |

### 🔹 Example:

```python
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)       # True
print(a is c)       # False
print(a == c)       # True (value-wise equal)
```

---

## 4️⃣ Membership Operators

Used to check if a value exists in a sequence.

| Operator | Description                      | Example            |
| -------- | -------------------------------- | ------------------ |
| `in`     | True if value is in the sequence | 'a' in 'apple'     |
| `not in` | True if value not in sequence    | 4 not in [1, 2, 3] |

### 🔹 Example:

```python
fruits = ["apple", "banana", "cherry"]

print("banana" in fruits)      # True
print("grape" not in fruits)   # True
```

---

## 🧪 Practice Set 14

1. ✏️ Write a program that checks if two numbers are equal using `==`.
2. 🔢 Use comparison operators to find the largest of three numbers.
3. 🔁 Create a program that checks if a number is in a given range.
4. 🔐 Use `and` and `or` to combine multiple conditions.
5. 🔄 Write a program that reverses a condition using `not`.
6. 🧠 Use `is` and `is not` to compare two objects.
7. 🔍 Use `in` to check if a value exists in a list or string.
8. 📘 Check if a key exists in a dictionary using `in` and `not in`.
9. 💡 Combine identity and value comparison (`is` and `==`) for two lists.
10. ✅ Use logical operators to decide if a person can vote and drive.

---

## 📝 Summary

- ✅ **Comparison Operators**: `==`, `!=`, `>`, `<`, `>=`, `<=`
- ✅ **Logical Operators**: `and`, `or`, `not`
- ✅ **Identity Operators**: `is`, `is not` (same memory or not)
- ✅ **Membership Operators**: `in`, `not in` (value inside container or not)

---

> 🎯 Next Lecture: Bitwise Operators — Learn how Python works at the binary level for operations like `&`, `|`, `^`, `~`, `<<`, `>>`

