# 🐍 Python Programming Notes – Lecture 13

## ➕ Arithmetic and Assignment Operators

Operators are special symbols used to perform operations on variables and values. In this lecture, we’ll cover:

- **Arithmetic Operators** (for math)
- **Assignment Operators** (to assign values)

---

## 1️⃣ Arithmetic Operators

These operators perform basic math operations.

| Operator | Name           | Example   | Output |
| -------- | -------------- | --------- | ------ |
| `+`      | Addition       | `10 + 5`  | `15`   |
| `-`      | Subtraction    | `10 - 5`  | `5`    |
| `*`      | Multiplication | `10 * 5`  | `50`   |
| `/`      | Division       | `10 / 5`  | `2.0`  |
| `%`      | Modulus        | `10 % 3`  | `1`    |
| `**`     | Exponentiation | `2 ** 3`  | `8`    |
| `//`     | Floor Division | `10 // 3` | `3`    |

### 🔹 Example

```python
x = 10
y = 3

print(x + y)   # 13
print(x - y)   # 7
print(x * y)   # 30
print(x / y)   # 3.33...
print(x % y)   # 1
print(x ** y)  # 1000
print(x // y)  # 3
```

---

## 2️⃣ Assignment Operators

These operators assign values and also combine with arithmetic.

| Operator | Description             | Example   | Equivalent To |
| -------- | ----------------------- | --------- | ------------- |
| `=`      | Assign value            | `x = 5`   |               |
| `+=`     | Add and assign          | `x += 3`  | `x = x + 3`   |
| `-=`     | Subtract and assign     | `x -= 2`  | `x = x - 2`   |
| `*=`     | Multiply and assign     | `x *= 4`  | `x = x * 4`   |
| `/=`     | Divide and assign       | `x /= 2`  | `x = x / 2`   |
| `%=`     | Modulus and assign      | `x %= 3`  | `x = x % 3`   |
| `**=`    | Exponent and assign     | `x **= 2` | `x = x ** 2`  |
| `//=`    | Floor divide and assign | `x //= 2` | `x = x // 2`  |

### 🔹 Example

```python
x = 10
x += 5
print(x)  # 15

x *= 2
print(x)  # 30

x -= 10
print(x)  # 20

x //= 3
print(x)  # 6
```

---

## 🧪 Practice Set 13: Arithmetic and Assignment Operators

1. 🔢 Write a program to add, subtract, multiply, and divide two numbers.
2. 🔁 Use the modulus operator to find the remainder of `17 % 5`.
3. 📈 Write a program to calculate the power of a number using `**`.
4. 🧮 Use floor division to divide two numbers and round down.
5. 🔁 Demonstrate the use of `+=`, `*=`, and `-=` on a single variable.
6. 🔁 Swap two numbers using a temporary variable and then without using one.
7. 📐 Calculate area and perimeter of a rectangle (length × width).
8. ✏️ Assign values to multiple variables in one line: `a, b, c = 1, 2, 3`

---

## 📝 Summary

- ✅ Arithmetic operators perform basic math like `+`, `-`, `*`, `/`
- ✅ Assignment operators combine logic with `=` (e.g., `+=`, `-=`)
- ✅ Use these for mathematical operations and updating variables

---

> 🎯 Next Lecture: Logical and Bitwise Operators — Learn how Python compares and manipulates bits

