# 🐍 Python Programming Notes - Lecture 9

## 🔐 Tuples in Python

Tuples are ordered collections used to store multiple items in a single variable. Unlike lists, tuples are **immutable** — you cannot modify their values once created.

---

## 1️⃣ Creating a Tuple

```python
# Tuple of fruits
fruits = ("apple", "banana", "mango")
print(fruits)
```

✅ Tuples use parentheses `()` instead of square brackets `[]`.

---

## 2️⃣ Accessing Tuple Elements

```python
print(fruits[0])     # apple
print(fruits[-1])    # mango
```

✅ Tuples support positive and negative indexing like lists.

---

## 3️⃣ Tuple is Immutable

```python
# fruits[1] = "orange"  ❌ Error: Tuples cannot be changed
```

To update a tuple, convert it to a list, change it, and convert it back:

```python
fruits = ("apple", "banana", "mango")
temp = list(fruits)
temp[1] = "orange"
fruits = tuple(temp)
print(fruits)
# Output: ('apple', 'orange', 'mango')
```

---

## 4️⃣ Tuple Unpacking

```python
student = ("Aarav", 18, "Grade A")
name, age, grade = student
print(name)   # Aarav
print(age)    # 18
print(grade)  # Grade A
```

🎯 Each variable gets one item from the tuple.

---

## 5️⃣ Looping Through a Tuple

```python
colors = ("red", "green", "blue")
for color in colors:
    print(color)
```

---

## 6️⃣ Joining Tuples

```python
a = (1, 2, 3)
b = (4, 5)
c = a + b
print(c)  # Output: (1, 2, 3, 4, 5)
```

---

## 7️⃣ Checking Membership

```python
animals = ("dog", "cat", "rabbit")
print("cat" in animals)     # True
print("lion" not in animals)  # True
```

---

## 8️⃣ Tuple Methods

### 🔹 `count()` — Returns number of times a value appears

```python
nums = (1, 2, 2, 3, 2)
print(nums.count(2))  # Output: 3
```

### 🔹 `index()` — Returns the first index of a value

```python
nums = (5, 3, 7, 3)
print(nums.index(3))  # Output: 1
```

---

## 🔁 Tuple with Mixed Data Types

```python
info = ("Python", 3.11, True)
print(type(info))  # <class 'tuple'>
```

---

## 📏 Tuple Length

```python
letters = ("a", "b", "c")
print(len(letters))  # Output: 3
```

---

## 🧪 Practice Set 9: Tuple Exercises

1. 📚 Create a tuple of your 5 favorite books. Print the first and last book.
2. 🔗 Combine two tuples (e.g., favorite foods and drinks) into one.
3. 🔁 Count how many times a certain value appears in a tuple.
4. 🧪 Convert a tuple to a list, modify an item, and convert it back to a tuple.
5. 📤 Unpack a tuple into variables and print each one.

---

## 📝 Summary

- ✅ Tuples are immutable and use parentheses `()`
- ✅ Use indexing and unpacking to access elements
- ✅ Common methods: `.count()`, `.index()`
- ✅ Tuples are faster and safer for fixed collections

---

> 🎯 Next Lecture 10 : [Dictionaries in Python](https://github.com/sachindaksh01/Python/blob/main/10%20%20dictionaries_in_python.md) — Learn about unordered, unique collections.

