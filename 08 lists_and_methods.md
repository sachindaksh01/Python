# 🐍 Python Programming Notes - Lecture 8

## 📦 Lists and List Methods

In Python, a **list** is a collection of items stored in a single variable. Lists are **ordered**, **mutable** (can be changed), and can hold **multiple data types**.

---

## 1️⃣ Creating a List
```python
shopping_list = ["milk", "eggs", "bread"]
print(shopping_list)
# Output: ['milk', 'eggs', 'bread']
```

---

## 2️⃣ Accessing List Items
```python
print(shopping_list[0])   # milk
print(shopping_list[-1])  # bread
```

---

## 3️⃣ Updating List Items
```python
shopping_list[1] = "butter"
print(shopping_list)
# Output: ['milk', 'butter', 'bread']
```

---

## 4️⃣ Common List Methods with Examples

### 🔹 `append()` – Adds item at the end
```python
shopping_list.append("jam")
# ['milk', 'butter', 'bread', 'jam']
```

### 🔹 `pop()` – Removes last or specified index
```python
shopping_list.pop(1)
# ['milk', 'bread', 'jam']
```

### 🔹 `remove()` – Removes first occurrence of value
```python
shopping_list.remove("jam")
# ['milk', 'bread']
```

### 🔹 `clear()` – Removes all items
```python
shopping_list.clear()
# []
```

### 🔹 `copy()` – Copies the list
```python
backup = shopping_list.copy()
```

### 🔹 `count()` – Counts occurrence of an item
```python
shopping_list = ["milk", "milk", "eggs"]
print(shopping_list.count("milk"))
# Output: 2
```

### 🔹 `extend()` – Merges another list
```python
shopping_list.extend(["butter", "cheese"])
# ['milk', 'milk', 'eggs', 'butter', 'cheese']
```

### 🔹 `index()` – Returns first index of value
```python
print(shopping_list.index("eggs"))
# Output: 2
```

### 🔹 `insert()` – Inserts item at given index
```python
shopping_list.insert(1, "juice")
# ['milk', 'juice', 'milk', 'eggs', 'butter', 'cheese']
```

### 🔹 `reverse()` – Reverses the list
```python
shopping_list.reverse()
```

### 🔹 `sort()` – Sorts the list
```python
shopping_list.sort()
```

---

## 🧪 Practice Set 8: List Operations

1. 📋 Create a list of your 5 favorite fruits.
2. ➕ Add 2 more items using `append()`.
3. ❌ Remove an item using `pop()` and `remove()`.
4. 🔁 Reverse the list using `reverse()`.
5. 🧮 Count how many times a fruit appears using `count()`.
6. 📚 Sort the list alphabetically using `sort()`.
7. 🧩 Insert an item at index 2.
8. 🔗 Combine it with another list using `extend()`.
9. 🎯 Find the index of a fruit using `index()`.
10. 🧹 Clear the list using `clear()`.

---

## 📝 Summary
- Lists are mutable, ordered, and flexible.
- Methods like `append()`, `remove()`, `sort()` help manage list content.
- Perfect for working with collections like shopping items, to-do lists, etc.

---

> 🎯 Next Lecture: [Tuples in Python — Learn about fixed, ordered collections](https://github.com/sachindaksh01/Python/blob/main/09%20%20Tuple%20and%20Methods.md).

