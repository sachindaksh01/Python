# 🐍 Python Programming Notes - Lecture 5

## 🔁 Type Conversion in Python

> 🔧 Type conversion means changing a value from one data type to another.

---

## ✌️ Two Types of Conversion

### 1️⃣ Implicit Conversion
Python automatically converts smaller data types into larger ones to avoid data loss.

#### 🔹 Example 1: int to float
```python
num_int = 10
num_float = 5.5
result = num_int + num_float
print(result)  # Output: 15.5
```

#### 🔹 Example 2: bool to int
```python
x = True
y = 5
z = x + y
print(z)  # Output: 6 (True = 1)
```

---

### 2️⃣ Explicit Conversion (Typecasting)
You decide how to convert a value using built-in functions.

| Function    | Description                         |
|-------------|-------------------------------------|
| `int()`     | Converts to integer                 |
| `float()`   | Converts to float                   |
| `str()`     | Converts to string                  |
| `list()`    | Converts to list                    |
| `tuple()`   | Converts to tuple                   |
| `set()`     | Converts to set                     |

#### 🔹 Example 1: float to int
```python
num = 7.8
converted = int(num)
print(converted)  # Output: 7
```

#### 🔹 Example 2: int to string
```python
age = 25
age_str = str(age)
print("I am " + age_str + " years old.")
```

#### 🔹 Example 3: string to list
```python
name = "Alice"
name_list = list(name)
print(name_list)  # Output: ['A', 'l', 'i', 'c', 'e']
```

#### 🔹 Example 4: list to string
```python
char_list = ['H', 'e', 'l', 'l', 'o']
string = ''.join(char_list)
print(string)  # Output: Hello
```

#### 🔹 Example 5: int to float and back
```python
x = 5
y = float(x)
print(y)  # Output: 5.0

z = int(y)
print(z)  # Output: 5
```

#### 🔹 Example 6: set to list
```python
my_set = {1, 2, 3, 3, 2}
my_list = list(my_set)
print(my_list)  # Output: [1, 2, 3]
```

#### 🔹 Example 7: dict keys to list
```python
student = {"name": "Alice", "age": 20}
keys_list = list(student.keys())
print(keys_list)  # Output: ['name', 'age']
```

---

## 🧪 Practice Set 5: Type Conversion

1. 🧮 Convert an integer to a string and concatenate it with another string.
2. 🔢 Convert a float to an integer and print it.
3. 📚 Convert a list to a tuple and print the result.
4. 🌊 Convert the string "3.14" into a float.
5. ✅ Convert boolean `True` into an integer and print the result.
6. 🔁 Convert a set into a list and print both.
7. 🗝️ Convert a dictionary's keys into a list and print it.
8. 🧾 Convert a float value to string and format it to 2 decimal places.

---

## 📝 Summary

- 🧠 Python handles implicit conversion automatically.
- 🧰 Use functions like `int()`, `float()`, `str()`, `list()` etc. for explicit conversion.
- 🔄 Useful for working with different types of data together.

---

> 🎯 Next Lecture: [05 String in Python](https://github.com/sachindaksh01/Python/blob/main/06%20strings_in_python.md)
