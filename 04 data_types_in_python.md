# 🐍 Python Programming Notes - Lecture 4

## 🧩 Data Types in Python

> 🧠 Data types define what kind of value a variable can hold.

Python automatically detects the type based on the value you assign — no need to declare it manually.

---

## 🔤 Common Python Data Types

| Data Type   | Description                            | Example                        |
|-------------|----------------------------------------|--------------------------------|
| `int`       | Whole numbers                          | `age = 25`                     |
| `float`     | Decimal numbers                        | `pi = 3.14`                    |
| `str`       | Text (string)                          | `name = "Alice"`              |
| `bool`      | Logical value: `True` or `False`       | `is_adult = True`             |
| `list`      | Mutable collection of items            | `fruits = ["apple", "banana"]`|
| `tuple`     | Immutable collection of items          | `colors = ("red", "blue")`    |
| `dict`      | Key-value pairs                        | `user = {"name": "Sam"}`     |
| `set`       | Unordered, unique items                | `nums = {1, 2, 3}`             |

---

## 📦 Examples

### 🔢 Integer & Float
```python
age = 25         # Integer
price = 9.99     # Float
```

### 🔠 String
```python
name = "Alice"
greeting = 'Hello!'
```

### ✅ Boolean
```python
is_student = True
is_tired = False
```

### 📋 List
```python
numbers = [1, 2, 3, 4]
fruits = ["apple", "banana", "cherry"]
```

### 📦 Tuple
```python
dimensions = (1920, 1080)
days = ("Mon", "Tue", "Wed")
```

### 🗂️ Dictionary
```python
student = {
    "name": "Aanya",
    "age": 16,
    "grade": "A"
}
```

### 🔘 Set
```python
unique_numbers = {1, 2, 3, 2, 1}
print(unique_numbers)  # Output: {1, 2, 3} - duplicates removed
```

---

## 🕵️‍♂️ Checking Data Types
Use the `type()` function:
```python
x = 10
print(type(x))   # <class 'int'>
```

---

## 👨‍💻 Practice Set 4: Data Types in Python

1. ✏️ Create a string, an integer, and a float. Print each variable and its type.
2. 🔁 Convert the string "123" into an integer using `int()` and print the result.
3. 📋 What’s the difference between a list and a tuple? Try creating both.
4. 🧠 Create a dictionary of 3 key-value pairs. Print one of the values.
5. 🔍 Use `type()` to check and print the data types of: a list, a tuple, a set, and a dictionary.

---

## 📝 Summary

- `int`, `float`, `str`, `bool` — for numbers, text, and logic
- `list`, `tuple`, `set`, `dict` — for collections
- Use `type()` to check data type of any variable

---

> 🎯 Next Lecture: [05 Type Conversion in Python — How to switch between data types](https://github.com/sachindaksh01/Python/blob/main/05%20type_conversion.md)

