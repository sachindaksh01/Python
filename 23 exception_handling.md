# ⚠️ Python Programming Notes – Lecture 23

## 🧯 Exception Handling in Python

Exception handling lets you gracefully manage **runtime errors** in your Python code and avoid crashing the program.

---

## 📌 Why Use Exception Handling?

- ✅ Prevents program crash
- ✅ Gives meaningful error messages
- ✅ Allows cleanup even if errors occur

---

## 🔹 Basic Syntax: try-except

```python
try:
    # Code that might raise an error
except ExceptionType:
    # Code to handle the error
```

### 📍 Example: Handle Invalid Input

```python
try:
    number = int(input("Enter a number: "))
    print("You entered:", number)
except ValueError:
    print("❌ Invalid input! Please enter a valid integer.")
```

---

## 🔹 try-except-else

`else` block runs **only if no error** occurs in try block.

```python
try:
    number = int(input("Enter a number: "))
except ValueError:
    print("❌ Invalid input!")
else:
    print("✅ You entered a valid number:", number)
```

---

## 🔹 try-finally

`finally` block always executes — good for **cleanup operations**.

```python
try:
    file = open("example.txt", "r")
    print(file.read())
except FileNotFoundError:
    print("📂 File not found!")
finally:
    print("📌 Program complete.")
```

---

## 🔁 Combined Structure: try-except-else-finally

```python
try:
    x = int(input("Enter a number: "))
except ValueError:
    print("❌ Not a number!")
else:
    print("✅ Input accepted.")
finally:
    print("🔚 End of program.")
```

---

## 🧪 Practice Example: Safe Input with Cleanup

```python
try:
    number = int(input("Enter a number: "))
except ValueError:
    print("❌ Invalid input! Please enter a number.")
else:
    print("🎉 Success! You entered:", number)
finally:
    print("🧹 Cleanup complete. Program ends.")
```

---

## 🔎 Summary

| Concept   | Description                           |
| --------- | ------------------------------------- |
| `try`     | Code that may throw error             |
| `except`  | Handles specific error types          |
| `else`    | Executes if no exception in try block |
| `finally` | Executes always, used for cleanup     |

> 🎯 Exception handling is essential for writing **robust and user-friendly Python programs**.

---

📘 **Next Lecture:** Custom Exceptions & Raising Your Own Errors

