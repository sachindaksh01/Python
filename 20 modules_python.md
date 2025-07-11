# 📦 Python Programming Notes – Lecture 20

## 📚 Modules and Importing in Python

Modules help in organizing Python code into manageable files and enable **reusability**, **modularity**, and **clean project structure**.

---

## 🔸 What is a Module?
- A **module** is simply a `.py` file containing functions, variables, classes, or runnable code.
- You can use your own module or import built-in and external ones.

### 🧠 Why Use Modules?
- ✅ Reusability – Code can be reused in multiple programs.
- ✅ Readability – Logical separation of functionalities.
- ✅ Collaboration – Easier to divide work in teams.

---

## 🛠️ Creating a Custom Module
### Create a file named `mymodule.py`
```python
# mymodule.py
def greet(name):
    return f"Hello, {name}!"

def add_numbers(a, b):
    return a + b

PI = 3.14159
```

### Create a second file `main.py` and import it
```python
import mymodule

print(mymodule.greet("Sachin"))
print(mymodule.add_numbers(5, 3))
print("PI:", mymodule.PI)
```
✅ Output:
```
Hello, Sachin!
8
PI: 3.14159
```

---

## 📥 Importing Modules in Python

### 🔹 1. Import entire module
```python
import math
print(math.sqrt(16))
```

### 🔹 2. Import specific items
```python
from math import sqrt
print(sqrt(25))
```

### 🔹 3. Import with alias
```python
import math as m
print(m.pi)
```

### 🔹 4. Import all (Not recommended)
```python
from math import *
print(sqrt(64))
```

---

## 📦 `pip install` External Modules
Some modules need to be installed first using `pip` (Python package manager).

### 🔹 Install a package:
```bash
pip install numpy
```

### 🔹 Use the package:
```python
import numpy as np
arr = np.array([1, 2, 3])
print(arr)
```

### 🔹 Uninstall a package:
```bash
pip uninstall numpy
```

---

## 🧰 Useful Built-in Modules
- `math`: Mathematical functions
- `random`: Random number generation
- `datetime`: Work with date and time
- `os`: Interact with the operating system
- `sys`: Access system-specific parameters

---

## 🔍 Other Module Utilities

### 📌 `dir()` Function
Returns all attributes and methods of a module.
```python
import math
print(dir(math))
```

### 📌 `__name__` Variable
Used to check whether a module is run directly or imported.
```python
def welcome():
    print("Welcome to Dream Topper")

if __name__ == "__main__":
    welcome()
```
✅ Output (only when run directly):
```
Welcome to Dream Topper
```

---

## ✅ Real-life Example
### `math_tools.py`
```python
def square(x):
    return x ** 2

def cube(x):
    return x ** 3
```

### `main.py`
```python
import math_tools
print(math_tools.square(4))  # 16
print(math_tools.cube(4))    # 64
```

---

## 🧪 Practice Questions

1. 🔢 Create a custom module `calculator.py` with functions for add, subtract, multiply, and divide. Use it in `main.py`.
2. 📐 Make a `geometry.py` module with `area_of_circle()` and `area_of_rectangle()` functions.
3. 🎲 Use the `random` module to create a dice roll simulator.
4. 📅 Write a program using `datetime` to print the current date and time.
5. 📦 Install and use the `emoji` module to print a smiley using Python.

---

## 📝 Summary
- 📁 A module is a `.py` file that can be imported in other scripts.
- 🔧 Use `import`, `from`, `as` to load modules.
- 🎒 Built-in modules (math, os, random, etc.) come with Python.
- 🌍 Use `pip` to install external modules like `numpy`, `pandas`, `emoji`.
- 💡 Use `__name__ == "__main__"` to manage script vs module behavior.

---

> 🎯 Next Lecture: Python Packages and Virtual Environments

