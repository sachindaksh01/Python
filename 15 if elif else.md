# 🐍 Python Programming Notes – Lecture 15

## 🧠 Conditional Statements in Python

Conditional statements allow your program to make decisions based on conditions. Python supports `if`, `elif`, and `else` to perform different actions depending on different conditions.

---

## 1️⃣ Introduction to `if`, `elif`, and `else`

### Basic Syntax
```python
if condition:
    # block of code if condition is True
elif another_condition:
    # block of code if previous condition is False and this one is True
else:
    # block of code if all above conditions are False
```

---

## 2️⃣ Simple `if` Statement
```python
age = 20
if age >= 18:
    print("You are an adult.")
```
✅ Runs only if the condition is True.

---

## 3️⃣ `if-else` Statement
```python
num = int(input("Enter a number: "))
if num % 2 == 0:
    print("Even")
else:
    print("Odd")
```
✅ Executes one of two blocks.

---

## 4️⃣ `if-elif-else` Statement
```python
score = int(input("Enter your score: "))
if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
elif score >= 60:
    print("Grade: D")
else:
    print("Grade: F")
```
✅ Checks multiple conditions in sequence.

---

## 5️⃣ Nested `if` Statements
```python
age = 18
citizen = True

if age >= 18:
    if citizen:
        print("Eligible to vote")
    else:
        print("Only citizens can vote")
else:
    print("You must be 18 or older")
```
✅ An `if` inside another `if`.

---

## 6️⃣ Logical Conditions in `if`
```python
username = "admin"
password = "1234"

if username == "admin" and password == "1234":
    print("Access granted")
else:
    print("Access denied")
```
✅ You can combine multiple conditions using `and`, `or`, `not`.

---

## 7️⃣ Real-Life Example: Temperature Alert
```python
temp = float(input("Enter temperature: "))

if temp > 35:
    print("It's very hot!")
elif temp < 10:
    print("It's very cold!")
else:
    print("Weather is pleasant")
```

---

## 🧪 Practice Set: Conditional Statements

1. 🔢 Write a program to check if a number is positive, negative, or zero.
2. 🎓 Accept marks and print the grade using `if-elif-else`.
3. 👤 Check if the user is eligible to vote based on age.
4. 📅 Check whether a given year is a leap year.
5. 🔑 Create a basic login system with username and password.
6. ⚖️ Compare two numbers and print the largest.
7. 🔁 Write a BMI calculator and categorize the result.

---

## 📝 Summary
- ✅ Use `if` for decision making
- ✅ Use `elif` for multiple conditions
- ✅ Use `else` as fallback
- ✅ Combine conditions with `and`, `or`, `not`

---

> 🎯 Next Lecture: Looping in Python — Learn to use `for`, `while`, and control statements!

