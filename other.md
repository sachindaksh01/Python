Bahut badhiya! 👏
Aapka ye doubt clear karna **bahut zaroori** hai, kyunki `lambda` function Python me chhoti aur powerful cheez hai 💪
Chalo simple example ke saath **step-by-step** samajhte hain 👇

---

## 🔹 **Lambda Function — Basic Definition**

👉 **Syntax:**

```python
lambda arguments: expression
```

* `lambda` → keyword (batata hai ye ek anonymous function hai)
* `arguments` → input values (jaise variables)
* `expression` → woh formula ya calculation jo return hoti hai

---

## 🧠 **Example 1: Simple addition**

```python
add = lambda x: x + 5
print(add(10))
```

➡️ Output:

```
15
```

📝 Explanation:

* `lambda x:` → input variable `x`
* `x + 5` → return hone wali value
  So this is same as:

```python
def add(x):
    return x + 5
```

---

## 🧩 **Example 2: Multiple arguments**

```python
multiply = lambda a, b: a * b
print(multiply(4, 3))
```

➡️ Output:

```
12
```

📝 Ye same hai:

```python
def multiply(a, b):
    return a * b
```

---

## 🧮 **Example 3: With condition (if–else)**

```python
check = lambda x: "Even" if x % 2 == 0 else "Odd"
print(check(5))
```

➡️ Output:

```
Odd
```

📝 Matlab:

* Agar `x` even hai → “Even” return karo
* Warna → “Odd”

---

## 🧰 **Example 4: Use inside `apply()` (DataFrame ke saath)**

```python
df['Marks'] = df['Marks'].apply(lambda x: x + 5 if pd.notnull(x) else x)
```

🧾 Meaning:

* Har value `x` par check karo: agar NaN nahi hai to `x + 5`
* Agar NaN hai to value ko as it is rakho

---

## 💡 Shortcut yaad rakhne ka tarika:

> 🔸 **lambda** = "function without a name"
> 🔸 **Syntax** = `lambda input : output`

---

## ⚡ Quick Practice:

Try yourself 👇

```python
square = lambda n: n ** 2
print(square(6))     # ?
```

Aap batao, iska output kya hoga?
