# 🐍 Python Programming Notes – Lecture 19

## 🧩 Functions in Python (Basics to Advanced)

Functions help us organize code into reusable blocks. They improve modularity, readability, and maintainability.

---

## 🔹 What is a Function?

A **function** is a block of code that performs a specific task when called.

---

## 🎯 Why Use Functions?

- ✅ **Code Reusability**: Define once, use many times
- ✅ **Modularity**: Break code into smaller, manageable parts
- ✅ **Maintainability**: Easier to test and update
- ✅ **Cleaner Code**: Increases readability and reduces duplication

---

## 🔧 Defining a Function

```python
def function_name():
    # function body (indented)
    print("Hello from function")
```

- `def`: Keyword to define the function
- `function_name`: Descriptive name
- `()`: Can include parameters
- `:`: Marks the start of the function body

### 🧠 Example:

```python
def greet():
    print("Welcome to Python!")

greet()  # Function call
```

---

## 📥 Parameters and Arguments

### 🧠 Function with Parameters

```python
def greet_user(name):
    print("Hello,", name)

greet_user("Alice")
```

- **Parameter**: `name`
- **Argument**: "Alice"

---

## 🔁 Returning Values from Functions

Use `return` to send output back to the caller.

### 🧠 Example:

```python
def add(a, b):
    return a + b

result = add(10, 5)
print("Sum:", result)
```

### 🔄 Returning Multiple Values:

```python
def calculate(a, b):
    return a + b, a - b, a * b

s, d, m = calculate(8, 3)
```

---

## ⚙️ Types of Arguments

### 1. **Positional Arguments**

Passed in the same order as parameters:

```python
def show(name, age):
    print(name, age)

show("John", 25)
```

### 2. **Keyword Arguments**

Passed using parameter names:

```python
show(age=25, name="John")
```

### 3. **Default Arguments**

Provide default values:

```python
def greet(name, message="Hello"):
    print(message, name)

greet("Asha")  # Uses default message
```

### 4. **Mixing Positional & Keyword**

```python
def info(name, age, city="Delhi"):
    print(f"{name}, {age} yrs, from {city}")

info("Neha", 22)
info("Ravi", 25, city="Mumbai")
```

---

## 🌡️ Practical Examples

### ✅ 1. Convert Celsius to Fahrenheit

```python
def convert(temp, to_celsius=True):
    if to_celsius:
        return (temp - 32) * 5/9
    else:
        return (temp * 9/5) + 32
```

### ✅ 2. Personalized Greeting

```python
def greet(name, age=None):
    if age:
        print(f"Hello {name}, age {age}!")
    else:
        print(f"Hello {name}!")
```

---

## 🧪 Practice Set – Defining & Calling Functions (Moderate to High)

1. ✏️ Write a function to return the average of 3 numbers.
2. 🧮 Create a function that returns the factorial of a number.
3. 🔍 Write a function to check if a number is **prime**.
4. 🆚 Create a function to find the largest among 3 given numbers.
5. 📦 Write a function that calculates the volume of a box (length, width, height). Use default height = 10.
6. 🔄 Build a function that takes a string and returns it reversed.
7. 🔁 Create a function that returns the Fibonacci sequence up to `n` terms.
8. 💸 Write a function to calculate final price after discount. Use `discount=10%` as default.
9. 🎓 Function that accepts student details (name, grade) and prints a report card.
10. 🔠 Write a function that takes a sentence and returns a count of each vowel.

---

## 📝 Summary

- ✅ Use `def` to define a function
- ✅ Call using function name with parentheses
- ✅ Use `return` to send result
- ✅ Support positional, keyword, and default arguments
- ✅ Functions improve code reusability, structure, and clarity

---

> 🎯 Next Lecture: Advanced Function Concepts – `*args`, `**kwargs`, Lambda Functions, and Scope

