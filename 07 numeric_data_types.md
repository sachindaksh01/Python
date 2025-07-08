# 🐍 Python Programming Notes - Lecture 7

## 🔢 Numeric Data Types in Python

In Python, there are three main types of numbers:

### 1️⃣ `int` (Integer)
- Whole numbers (positive or negative)
- No decimal point
```python
x = 10
y = -5
```

### 2️⃣ `float` (Floating-point)
- Numbers with decimal points
```python
a = 3.14
b = -0.99
```

### 3️⃣ `complex` (Complex Number)
- Includes a real and an imaginary part
- Written as `a + bj`
```python
z = 2 + 3j
print(z.real)      # 2.0
print(z.imag)      # 3.0
```

---

## ➕ Arithmetic Operations
Python supports all common math operations on numbers.

| Operation        | Symbol | Example               | Output  |
|------------------|--------|------------------------|---------|
| Addition         | `+`    | `5 + 3`                | `8`     |
| Subtraction      | `-`    | `10 - 4`               | `6`     |
| Multiplication   | `*`    | `6 * 7`                | `42`    |
| Division         | `/`    | `10 / 4`               | `2.5`   |
| Floor Division   | `//`   | `10 // 4`              | `2`     |
| Modulus          | `%`    | `10 % 3`               | `1`     |
| Exponentiation   | `**`   | `2 ** 3`               | `8`     |

---

## 🌊 Float Examples
```python
a = 5.5
b = 2.0
print(a * b)    # Output: 11.0
```

---

## 🧠 Complex Number Operations
```python
c1 = 2 + 3j
c2 = 1 + 4j

print(c1 + c2)  # Output: (3+7j)
print(c1 - c2)  # Output: (1-1j)
print(c1 * c2)  # Output: (-10+11j)
print(c1 / c2)  # Output: (0.8235...+0.2941...j)
```

---

## 🔄 Type Conversion
```python
x = 5.9
print(int(x))       # Output: 5

num = 3
print(float(num))   # Output: 3.0
```

---

## 🎯 Useful Built-in Functions
```python
abs(-10)       # 10
round(3.567)   # 4
pow(2, 3)      # 8
```

---

## 🧪 Practice Set 7: Numeric Data Types

1. ✏️ Add two integers and print the result.
2. ➕ Perform all basic arithmetic operations with float values.
3. 📐 Use `**` to calculate the square of a number.
4. 🧊 Convert a float to an int and see the result.
5. 🔬 Create a complex number and print its real and imaginary parts.
6. 📏 Write a program to calculate the area of a circle using `π = 3.14` and radius = 7.
7. 🔁 Use `round()` to round a float to the nearest integer.

---

## 📝 Summary
- `int`, `float`, and `complex` are Python’s numeric data types
- All support arithmetic and type conversion
- Complex numbers are built-in and easy to use

---

> 🎯 Next Lecture: [08 List and Method](https://github.com/sachindaksh01/Python/blob/main/07%20numeric_data_types.md)

