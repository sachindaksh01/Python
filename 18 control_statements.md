# 🐍 Python Programming Notes – Lecture 18

## 🛑 Control Flow Statements in Python

Control statements help manage the flow of loops. Python provides three important ones:

- `break` – exits the loop early
- `continue` – skips the rest of the current iteration
- `pass` – does nothing (placeholder)

We'll learn to use them in both `for` and `while` loops.

---

## 🔚 The `break` Statement

Used to **exit the loop immediately**, even if the condition is still `True`.

### 🧠 Example 1: Stop when number is found

```python
numbers = [1, 3, 5, 7, 9, 10, 13]
for num in numbers:
    if num == 10:
        print("Found 10!")
        break
    print("Checked:", num)
```

### 🧠 Example 2: Stop user guessing game

```python
secret = 7
while True:
    guess = int(input("Guess the number: "))
    if guess == secret:
        print("Correct!")
        break
    print("Try again")
```

---

## 🔄 The `continue` Statement

Used to **skip the rest of the loop** and start the next iteration.

### 🧠 Example 3: Skip even numbers

```python
for i in range(1, 6):
    if i % 2 == 0:
        continue
    print(i)
```

### 🧠 Example 4: Skip blank user input

```python
while True:
    name = input("Enter your name (type 'exit' to stop): ")
    if name == "exit":
        break
    if name.strip() == "":
        continue
    print("Hello,", name)
```

---

## 🧘 The `pass` Statement

Used when a statement is syntactically required but you don’t want to do anything yet.

### 🧠 Example 5: Placeholder inside a loop

```python
for i in range(5):
    if i == 2:
        pass  # maybe plan to add something later
    else:
        print(i)
```

---

## 🧪 Practice Set – Control Statements

### 🔰 Basic

1. 🚪 Write a `for` loop that breaks when number is divisible by 7.
2. ❌ Create a loop that skips negative numbers in a list.
3. ⬅️ Build a loop to print only odd numbers from 1 to 20 using `continue`.

### ⚙️ Intermediate

4. 🛒 Iterate over a shopping list but skip empty items.
5. ➖ Create a loop that prints numbers from 1 to 10 but stops after 6 using `break`.



---

## 📝 Summary

- ✅ `break` exits the loop immediately
- ✅ `continue` skips the current iteration
- ✅ `pass` does nothing (used as a placeholder)

Use these to build smarter, more flexible loops!

---

> 🎯 Next Lecture: `Functions in Python` — how to organize reusable blocks of code!

