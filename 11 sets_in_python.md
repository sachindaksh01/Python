# 🐍 Python Programming Notes – Lecture 11

## 🔘 Sets in Python

A **set** is an unordered collection of unique items. Sets are useful when you need to store only unique values, like IDs or tags.

---

## 1️⃣ Creating a Set

```python
fruits = {"apple", "banana", "orange"}
print(fruits)

numbers = set([1, 2, 3, 4])
print(numbers)
```

📌 Sets are created using `{}` or `set()` constructor.

---

## 2️⃣ Accessing Set Items

```python
for item in fruits:
    print(item)

if "apple" in fruits:
    print("Apple is in the set")
```

❌ You cannot access items by index in a set.

---

## 3️⃣ Adding and Removing Items

```python
fruits.add("grapes")             # Add item
fruits.remove("banana")          # Remove item
fruits.discard("pear")           # Safe remove (no error if not present)
```

---

## 4️⃣ Set Operations

### 🔹 `union()` or `|` – Combine elements

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
print(set1.union(set2))   # {1, 2, 3, 4, 5}
print(set1 | set2)         # {1, 2, 3, 4, 5}
```

### 🔹 `intersection()` or `&` – Common elements

```python
print(set1.intersection(set2))  # {3}
print(set1 & set2)              # {3}
```

### 🔹 `difference()` or `-` – In set1 but not in set2

```python
print(set1.difference(set2))    # {1, 2}
print(set1 - set2)              # {1, 2}
```

### 🔹 `symmetric_difference()` or `^` – In either but not both

```python
print(set1.symmetric_difference(set2))  # {1, 2, 4, 5}
print(set1 ^ set2)                      # {1, 2, 4, 5}
```

---

## 5️⃣ Useful Set Methods

### 🔸 `clear()` – Remove all items

```python
set1.clear()
```

### 🔸 `copy()` – Return a shallow copy

```python
copy_set = set1.copy()
```

### 🔸 `issubset()` – Check if all elements exist in another set

```python
print({1, 2}.issubset({1, 2, 3}))  # True
```

### 🔸 `issuperset()` – Check if set contains all elements of another

```python
print({1, 2, 3}.issuperset({1, 2}))  # True
```

### 🔸 `pop()` – Remove random element

```python
val = set1.pop()
print(val)
```

---

## 🧪 Practice Set 11: Set Exercises

1. 🧮 Create a set of 5 numbers and add/remove items using `add()` and `discard()`.
2. 🔁 Create two sets and find their union and intersection.
3. ➖ Use `difference()` to find what is in the first set but not the second.
4. 🔄 Check if a set is a subset/superset of another.
5. 🧼 Use `clear()` and `copy()` methods.
6. 🔁 Perform `symmetric_difference()` between two sets.
7. 🔎 Write a loop to print all elements in a set.

---

## 📝 Summary

- ✅ Sets are unordered collections with **unique** values
- ✅ Use `{}` or `set()` to create sets
- ✅ No indexing; use loops or membership test (`in`)
- ✅ Powerful operations: `union()`, `intersection()`, `difference()`, `symmetric_difference()`
- ✅ Methods like `add()`, `remove()`, `clear()`, `copy()`, `issubset()` are commonly used

---

> 🎯 Next Lecture: [Boolean and None Types in Python](https://github.com/sachindaksh01/Python/blob/main/12%20boolean_and_none_types.md)

