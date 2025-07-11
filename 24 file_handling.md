# 📂 Python Programming Notes – Lecture 24

## 🗃️ File Handling in Python

File handling allows Python programs to read from and write to files stored on your computer.

---

## 🔑 Key Concepts

| Mode | Description              |
| ---- | ------------------------ |
| `r`  | Read (default)           |
| `a`  | Append                   |
| `w`  | Write (overwrites)       |
| `x`  | Create (error if exists) |
| `t`  | Text mode (default)      |

---

## 📘 Opening Files

```python
f = open("file.txt", "r")
```

### 🧠 Smart Shortcut:

```python
f = open("file.txt")  # "rt" mode by default
```

### 📂 Open file from another location:

```python
f = open("D:\\notes\\file.txt", "r")
```

---

## 📖 Reading Files

### 🔹 Entire Content

```python
f = open("file.txt", "r")
print(f.read())
```

### 🔹 First N Characters

```python
print(f.read(10))
```

### 🔹 First Line

```python
print(f.readline())
```

### 🔹 Loop Through Lines

```python
for line in f:
    print(line)
```

---

## ✅ Always Close Files

```python
f.close()
```

---

## 📝 Writing to Files

### 🔹 Append (keep old content)

```python
f = open("file.txt", "a")
f.write("New line added!\n")
f.close()
```

### 🔹 Overwrite

```python
f = open("file.txt", "w")
f.write("New content!\n")
f.close()
```

---

## 🆕 Creating Files

```python
f = open("newfile.txt", "x")  # Error if exists
```

### ✅ Safe Way:

```python
f = open("newfile.txt", "w")  # Creates if doesn't exist
```

---

## ❌ Deleting Files and Folders

```python
import os

# Remove file
os.remove("file.txt")

# Check before removing
if os.path.exists("file.txt"):
    os.remove("file.txt")
else:
    print("The file does not exist")

# Remove empty folder
os.rmdir("empty_folder")
```

---

## 🛠️ Mini Project: Create and Remove Files

```python
import os

def create_files(n, t):
    for i in range(1, n+1):
        filename = f"Folder {i}.{t}"
        open(filename, 'x')
        print(f"Created {filename} with message: \"\"")
    print('All files created successfully!')

def remove_files():
    for i in os.listdir('.'):
        if i == 'main.py':
            continue
        os.remove(i)
    print('All files removed successfully!')

print('Welcome to the File Creator and Remover!')
while True:
    choice = input('Do you want to create or remove files? (c/r): ').strip().lower()
    if choice == 'c':
        n = int(input('Enter the number of files to create: '))
        t = input('Enter the file type (e.g., txt, md): ')
        create_files(n, t)
    elif choice == 'r':
        remove_files()
    else:
        print('Invalid choice. Please enter "c" to create or "r" to remove files.')

    try:
        cont = input('Do you want to continue? (y/n): ').strip().lower()
    except:
        print('Invalid input. Exiting the program.')
    else:
        if cont != 'y':
            break
```

---

## ✨ Bonus: `with` Statement (Context Manager)

Using `with` automatically closes your file after work is done.

### ✅ Best Practice

```python
with open("file.txt", "r") as f:
    content = f.read()
    print(content)
# File is automatically closed
```

---

## 🧾 Summary Table

| 🔧 Task           | ✅ Method                 |
| ----------------- | ------------------------ |
| Open a file       | `open("file.txt", "r")`  |
| Read all data     | `read()`                 |
| Read line-by-line | `readline()` / loop      |
| Write text        | `write()`                |
| Append text       | `a` mode                 |
| Create file       | `x` or `w` mode          |
| Close file        | `close()` / `with` block |
| Delete file       | `os.remove()`            |
| Delete folder     | `os.rmdir()`             |

---

> 🧠 **File handling is a core skill for reading logs, saving data, and automation in real-world Python projects.**

