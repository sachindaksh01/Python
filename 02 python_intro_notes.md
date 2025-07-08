# 🐍 Python Programming Notes - Lecture 2

## 🧑‍🏫 Introduction to Python

### 🔸 What is Python?

Python is a high-level, beginner-friendly programming language created by **Guido van Rossum** in 1991.

#### ✅ Uses of Python:

- 🌐 Web development (server-side)
- 🧠 Data analysis & Machine Learning
- 🛠️ Software development
- 📊 Mathematics and big data
- 📜 Scripting & Automation

### 💡 Why Python?

- ✅ Works on Windows, Mac, Linux, Raspberry Pi
- ✅ Syntax is simple and similar to English
- ✅ Fewer lines of code compared to other languages
- ✅ Interpreted language (code runs instantly)
- ✅ Supports multiple styles: procedural, object-oriented, functional

### 📌 Good to Know:

- We'll use **Python 3**, the latest major version.
- Code can be written in text editors or **IDEs** like Thonny, PyCharm, VS Code, etc.

### 🔍 Python Syntax Highlights:

- 📎 Uses **indentation** (spaces) to define blocks (like loops, functions, classes)
- 🔄 No need for `{}` or `;` like other languages
- ✍️ Simple and readable structure

---

## 💻 Python Installation & Setup

### 1️⃣ Installing Python:

1. Go to [python.org](https://www.python.org/downloads/)
2. Download and install the latest version
3. ✅ **Important:** Check the box **"Add Python to PATH"**

#### 🔍 Verify Installation:

- Open terminal or CMD
- Run: `python --version` or `python3 --version`

---

### 2️⃣ Setting Up IDEs

#### 🔹 Jupyter Notebook (For Data Science Students)

- 📦 Install **Anaconda** (includes Python + Jupyter + data science libraries)
- Use it if you're working on **data analytics**, **machine learning**, or **visualizations**

**Alternative:** Install Jupyter manually using pip:

```bash
pip install jupyter
jupyter notebook
```

- Opens in your browser
- Great for writing code + markdown

#### 🔹 Jupyter Lab

- Advanced version of Jupyter Notebook
- 🗂️ Supports multi-tab interface and visualizations

**Notebook vs Lab:**

| Tool             | Use Case                           |
| ---------------- | ---------------------------------- |
| Jupyter Notebook | Simple, beginner-friendly UI       |
| Jupyter Lab      | Pro users, more features, IDE-like |

#### 🔹 Other IDEs

- 🧠 PyCharm: Full-featured professional IDE
- 🧑‍💻 VS Code: Lightweight, highly customizable

---

## 👨‍💻 First Python Program

```python
# This is a simple Python program
print("Hello, World!")
```

### 🗒️ Comments

- `#` for single-line comments
- Triple quotes (`'''` or `"""`) for multi-line comments

### 📐 Indentation

Python uses indentation (spaces) instead of `{}`:

✅ Correct:

```python
if 5 > 2:
    print("Five is greater than two.")
```

❌ Incorrect (will cause `IndentationError`):

```python
if 5 > 2:
print("Five is greater than two.")
```

---

## 🧪 Practice Set 1: Basics

1. Print `"Hello, World!"`
2. Add comments to explain your code
3. Print multiple lines using `\n`
4. Explain indentation with examples
5. Print a triangle using asterisks (`*`)
6. Try improper indentation – observe the error
7. Comment out code and check output
8. Write a multi-line comment about what your program does



---

🚀 Next Lecture: [Variable in Python](https://github.com/sachindaksh01/Python/blob/main/03%20variables_in_python.md)
