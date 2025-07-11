# 🐍 Python Programming Notes – Lecture 10

## 🗂️ Dictionaries in Python

A **dictionary** is an unordered, mutable collection that stores data in **key-value pairs**. It's perfect for structured data like user profiles, student records, and more.

---

## 1️⃣ Creating a Dictionary

```python
student = {
    "name": "Aarav",
    "age": 16,
    "grade": "A"
}
```

📌 Use curly braces `{}` with key: value format.

---

## 2️⃣ Accessing Items

```python
print(student["name"])     # Aarav
print(student.get("age"))  # 16
```

✅ `.get()` avoids errors if key is missing.

---

## 3️⃣ Changing Items

```python
student["age"] = 17
print(student)
```

---

## 4️⃣ Adding New Items

```python
student["city"] = "Delhi"
print(student)
```

---

## 5️⃣ Removing Items

```python
student.pop("grade")           # By key
student.popitem()              # Last inserted item
# del student["name"]         # Using del
```

---

## 6️⃣ Looping Through Dictionary

```python
for key, value in student.items():
    print(f"{key}: {value}")
```

---

## 7️⃣ Copying a Dictionary

```python
student_copy = student.copy()
```

---

## 8️⃣ Nested Dictionaries

```python
students = {
    "Aarav": {"age": 16, "marks": 85},
    "Riya": {"age": 15, "marks": 90}
}
print(students["Riya"]["marks"])
# Output: 90
```

---

## 🔧 Useful Dictionary Methods

### 🔹 `clear()` – Removes all items

```python
student.clear()
```

### 🔹 `fromkeys()` – Create dictionary with default values

```python
names = ["John", "Emma"]
d = dict.fromkeys(names, 0)
print(d)  # {'John': 0, 'Emma': 0}
```

### 🔹 `items()` – Returns key-value pairs

```python
print(student.items())
```

### 🔹 `keys()` and `values()`

```python
print(student.keys())     # dict_keys([...])
print(student.values())   # dict_values([...])
```

### 🔹 `setdefault()` – Adds key with default if not exists

```python
student.setdefault("school", "DPS")
```

### 🔹 `update()` – Updates/adds multiple key-value pairs

```python
student.update({"age": 18, "marks": 92})
```

---

## 🧪 Practice Set 10: Dictionary Exercises

1. 👩‍🎓 Create a dictionary to store names and ages. Add, update, and delete entries.
2. 🧮 Write a program to loop through a dictionary and print keys and values.
3. 🧊 Use `fromkeys()` to create a dictionary with default values.
4. 🔄 Use `update()` to change multiple fields at once.
5. 🧰 Create and access a nested dictionary with student info.
6. 🔐 Use `get()` and `setdefault()` safely to retrieve/add keys.
7. 🧹 Remove keys using `pop()`, `popitem()`, and `del`.
8. 🧪 Copy a dictionary and verify it is independent using `.copy()`.

---

## 📝 Summary

- ✅ Use `{}` to create key-value pairs
- ✅ Access with `[]` or `.get()`
- ✅ Use `.update()`, `.pop()`, `.clear()`, `.copy()` for operations
- ✅ Nest dictionaries for structured data

---

> 🎯 Next Lecture: Sets in Python — Handle unordered collections of unique values

