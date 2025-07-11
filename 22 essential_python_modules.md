# 🚀 Python Programming Notes – Lecture 22

> **Essential Modules in Python:** Explore the power of built-in modules like `calendar`, `random`, `os`, and `time` for everyday programming tasks.

---

## 🗓️ calendar — Work with Dates and Calendars

The `calendar` module lets you handle dates, weeks, months, and leap years easily.

```python
import calendar
```

### 🔹 Useful Features:

- 📆 **Display Month Calendar**
  ```python
  print(calendar.month(2025, 7))
  ```
- 🕳️ **Check Leap Year**
  ```python
  print(calendar.isleap(2024))
  ```
- 🗓️ **Display Full Year Calendar**
  ```python
  print(calendar.calendar(2025))
  ```
- 📅 **Get Day of the Week**
  ```python
  print(calendar.weekday(2025, 7, 7))  # Output: 0 (Monday)
  ```

---

## 🎲 random — Generate Randomness

The `random` module helps in generating random numbers, picking random elements, or shuffling data.

```python
import random
```

### 🔹 Most Used Functions:

- 🎯 **Random Integer Between Two Numbers**
  ```python
  print(random.randint(1, 10))
  ```
- 🧠 **Pick a Random Element from a List**
  ```python
  print(random.choice(['apple', 'banana', 'cherry']))
  ```
- 🔀 **Shuffle a List Randomly**
  ```python
  items = [1, 2, 3, 4]
  random.shuffle(items)
  print(items)
  ```
- 💧 **Generate Random Float Between 0 and 1**
  ```python
  print(random.random())
  ```

---

## 💻 os — Interact with the Operating System

The `os` module helps in working with the file system, directories, and environment settings.

```python
import os
```

### 🔹 Common Functions:

- 📍 **Current Working Directory**
  ```python
  print(os.getcwd())
  ```
- 📂 **List Directory Contents**
  ```python
  print(os.listdir())
  ```
- 🏗️ **Create a New Directory**
  ```python
  os.mkdir("new_folder")
  ```
- ✏️ **Rename File/Folder**
  ```python
  os.rename("old.txt", "new.txt")
  ```
- ❌ **Delete a File**
  ```python
  os.remove("data.txt")
  ```

> ⚠️ Always check if file/folder exists before removing or renaming.

---

## ⏱️ time — Time & Delays

The `time` module helps in tracking execution time, creating pauses, or formatting time.

```python
import time
```

### 🔹 Most Used Functions:

- ⏰ **Current Time (seconds since epoch)**
  ```python
  print(time.time())
  ```
- 🧭 **Readable Current Time**
  ```python
  print(time.ctime())
  ```
- 💤 **Pause Execution**
  ```python
  time.sleep(2)  # Waits for 2 seconds
  ```
- ⏱️ **Measure Execution Time**
  ```python
  start = time.time()
  # some task
  end = time.time()
  print("Execution time:", end - start)
  ```

---

## 📝 Quick Recap Table

| 📦 Module  | 🔍 Use Case                        | 🛠️ Common Features                       |
| ---------- | ---------------------------------- | ----------------------------------------- |
| `calendar` | Work with dates & months           | Month/year view, leap year, weekdays      |
| `random`   | Random values & simulations        | randint, choice, shuffle, random          |
| `os`       | File system & directory management | cwd, listdir, mkdir, rename, remove       |
| `time`     | Delay & performance measurement    | time, sleep, ctime, execution measurement |

---

> 📌 **Up Next:** Lecture 23 – Handling User Input & Errors Gracefully

