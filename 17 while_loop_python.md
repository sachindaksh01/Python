# 🐍 Python Programming Notes – Lecture 17

## 🔁 Introduction to `while` Loop in Python

A ``** loop** is used to repeatedly execute a block of code **as long as a condition remains True**. It is best used when we don’t know in advance how many times the loop needs to run.

---

## 🧠 Key Concepts

- ✅ The loop checks the condition **before** each iteration.
- ✅ If the condition is `True`, the code inside runs.
- ✅ If the condition becomes `False`, the loop stops.

---

## 🔤 Syntax of `while` Loop

```python
while condition:
    # code block
```

Ensure the condition becomes False eventually to avoid **infinite loops**.

---

## 🧮 Example 1: Print Numbers 1 to 5

```python
count = 1
while count <= 5:
    print(count)
    count += 1
```

---

## 🔄 How `while` Loop Works

1. **Initialize**: Set a starting value.
2. **Check Condition**: Loop runs if condition is `True`.
3. **Execute**: Run the code block.
4. **Update**: Modify variables so condition may become `False`.

---

## ⬇️ Example 2: Countdown from 10

```python
number = 10
while number > 0:
    print(number)
    number -= 1
print("Liftoff!")
```

---

## ➕ Example 3: Sum from 1 to n

```python
n = 5
sum_numbers = 0
counter = 1
while counter <= n:
    sum_numbers += counter
    counter += 1
print("Sum:", sum_numbers)
```

---

## ❗ Example 4: Input Validation

```python
user_input = ""
while user_input != "yes":
    user_input = input("Type 'yes' to continue: ")
print("Thank you!")
```

✅ Useful for checking form input, login attempts, etc.

---

## ⚠️ Infinite Loop Warning

```python
# This causes infinite loop
count = 1
while count <= 5:
    print(count)
    # Missing: count += 1
```

Always update the variable to avoid infinite loops.

---

## 🧪 Practice Set – `while` Loop (Beginner Friendly)

1. 🔢 Print numbers from 1 to 10 using a `while` loop.
2. ➕ Calculate the sum of first 10 even numbers.
3. 🔁 Continue taking user input until they type 'exit'.
4. 🔁 Reverse a number using a `while` loop.
5. 🔢 Find the sum of digits of a number using a `while` loop.
6. 📉 Countdown from 10 to 1 using a `while` loop.
7. 🧮 Create a number guessing game that stops when the correct guess is entered (basic version).

---

## 📝 Summary

- ✅ `while` loop runs **while** the condition is `True`
- ✅ Ideal for **input validation**, **uncertain iterations**, and **counting**
- ✅ Always ensure a way to make the condition `False`

---

> 🎯 Next Lecture: `break`, `continue`, and `pass` Statements — Control the flow inside loops with special keywords.

