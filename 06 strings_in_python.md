# 🐍 Python Programming Notes - Lecture 6

## 📚 Working with Strings in Python

> Strings are sequences of characters used to represent text data. Python provides powerful tools and methods to work with strings efficiently.

---

## 1️⃣ String Basics

### 🔤 Declaring Strings
```python
name = "Alice"
greeting = 'Hello!'
quote = '''This is a multi-line
string.'''
```

### ✅ Strings are Immutable
Once created, they cannot be modified directly.

---

## 2️⃣ String Indexing
```python
text = "Python"
print(text[0])    # Output: P
print(text[-1])   # Output: n
```

---

## 3️⃣ String Slicing
```python
text = "Programming"
print(text[:5])     # Output: Progr
print(text[3:8])    # Output: gram
print(text[::-1])   # Output: gnimmargorP
```

---

## 4️⃣ String Concatenation
```python
first = "Hello"
second = "World"
result = first + " " + second
print(result)  # Output: Hello World
```

---

## 5️⃣ String Modification with Slicing
```python
text = "Jython"
modified = "P" + text[1:]
print(modified)  # Output: Python
```

---

## 6️⃣ Case Methods
```python
text = "hello world"
print(text.upper())      # HELLO WORLD
print(text.lower())      # hello world
print(text.capitalize()) # Hello world
print(text.title())      # Hello World
print(text.swapcase())   # HELLO WORLD -> hello world
```

---

## 7️⃣ Alignment and Padding
```python
text = "hello"
print(text.center(10, "-"))  # --hello---
print(text.ljust(10, "-"))    # hello-----
print(text.rjust(10, "-"))    # -----hello
print("42".zfill(5))          # 00042
```

---

## 8️⃣ Searching and Substrings
```python
text = "hello world"
print(text.find("world"))     # 6
print(text.rfind("l"))        # 9
print(text.index("hello"))    # 0
print(text.startswith("hello"))  # True
print(text.endswith("world"))    # True
```

---

## 9️⃣ Splitting and Joining
```python
text = "apple,banana,grape"
print(text.split(","))       # ['apple', 'banana', 'grape']
print(", ".join(["a", "b"]))  # a, b
```

---

## 🔟 Cleaning and Trimming
```python
text = "  hello world  "
print(text.strip())   # hello world
print(text.lstrip())  # hello world
print(text.rstrip())  # hello world
```

---

## 🔠 Replace Text
```python
text = "I love apples"
print(text.replace("apples", "oranges"))  # I love oranges
```

---

## 1️⃣1️⃣ Validation Methods
```python
print("hello123".isalnum())  # True
print("hello".isalpha())     # True
print("123".isdigit())       # True
```

---

## 1️⃣2️⃣ Encoding and Translation
```python
text = "hello"
print(text.encode())  # b'hello'

# Translation
table = str.maketrans("a", "b")
print("apple".translate(table))  # bpple
```

---

## 🧪 Practice Set 6: String Operations

1. Create a string and print its length.
2. Print the first and last characters of a string.
3. Extract the word "Python" from "I am learning Python."
4. Reverse a string using slicing.
5. Concatenate first name and last name with space.
6. Convert a sentence to uppercase, lowercase, and title case.
7. Replace all spaces in a sentence with underscores.
8. Check if a string starts with "Hello" and ends with "!".
9. Center a word with * on both sides up to 20 characters.
10. Split a string by commas and print the resulting list.
11. Join a list ["a", "b", "c"] with hyphens.
12. Find the index of the word "code" in a sentence.
13. Replace "Java" with "Python" in the sentence "I like Java."
14. Check if a string is a palindrome.
15. Convert string "123" to int and validate with isdigit().

---

> 🎯 Next Lecture: Python Operators — Master arithmetic, comparison, logical, and bitwise operators.

