# 🗕️ Python Programming Notes – Lecture 21

## 🕰️ Working with Dates in Python

Python makes it easy to work with dates and times using the `datetime` module.

---

## 🔹 Importing the datetime Module

```python
import datetime
```

This gives access to all date/time-related features like current date, specific date creation, formatting, and differences.

---

## 📆 Getting the Current Date and Time

```python
now = datetime.datetime.now()
print("Current Date and Time:", now)
```

🗞 Example Output:
```
Current Date and Time: 2025-07-07 09:30:15.123456
```

---

## 📅 Creating a Specific Date

```python
specific_date = datetime.datetime(2023, 12, 25)  # YYYY, MM, DD
print("Specific Date:", specific_date)
```
✅ Output:
```
Specific Date: 2023-12-25 00:00:00
```

---

## 🧹 Extracting Date Components

```python
print("Year:", now.year)
print("Month:", now.month)
print("Day:", now.day)
```

✅ Output:
```
Year: 2025
Month: 7
Day: 7
```

---

## 🗓️ Formatting Dates with `strftime()`

You can format date objects into readable strings using `.strftime()`.

```python
formatted_date = now.strftime("%Y-%m-%d")
print("Formatted Date:", formatted_date)
```

### 🔹 Most Common Format Codes:

| Code | Meaning | Example |
|------|---------|---------|
| `%Y` | Full year | 2025 |
| `%y` | Year (2 digits) | 25 |
| `%m` | Month (01-12) | 07 |
| `%B` | Month name full | July |
| `%b` | Month name short | Jul |
| `%d` | Day of the month (01-31) | 07 |
| `%A` | Full weekday name | Monday |
| `%a` | Short weekday name | Mon |
| `%H` | Hour (00-23) | 13 |
| `%I` | Hour (01-12) | 01 |
| `%p` | AM/PM | AM |
| `%M` | Minute (00-59) | 45 |
| `%S` | Second (00-59) | 22 |
| `%f` | Microsecond (000000-999999) | 123456 |
| `%j` | Day of year (001-366) | 188 |
| `%U` | Week number (Sunday first day) | 27 |
| `%W` | Week number (Monday first day) | 27 |
| `%x` | Locale's date | 07/07/25 |
| `%X` | Locale's time | 13:45:22 |
| `%c` | Locale's date and time | Mon Jul 7 13:45:22 2025 |
| `%%` | Literal `%` | % |

### 🧠 Full Example:
```python
print(now.strftime("Today is %A, %B %d, %Y at %I:%M %p"))
```
✅ Output:
```
Today is Monday, July 07, 2025 at 09:30 AM
```

---

## 🔀 Date Arithmetic (Finding Difference)

```python
x = datetime.datetime(2024, 1, 1)
y = datetime.datetime(2024, 3, 1)
rem = y - x
print("Total Days Between Dates:", rem.days)
```
✅ Output:
```
Total Days Between Dates: 60
```

---

## 📚 Practice Questions

1. 🦓 Get the current time in "Hour:Minute AM/PM" format using `strftime`.
2. 🎂 Ask the user for their birthdate and print the day of the week they were born.
3. 🧾 Create a program to calculate how many days are left until New Year.
4. 🗓️ Format today's date as "DD-MM-YYYY".
5. 🔀 Input two dates from the user and calculate the number of days between them.

---

## 📌 Summary

- `datetime` module allows us to work with dates and times.
- Use `datetime.datetime.now()` for current date & time.
- Use `.strftime()` to format dates into custom strings.
- Use `datetime.datetime(Y, M, D)` to create specific dates.
- Subtract dates to get the number of days between them.

---

> 🎯 Next Lecture: Python Time Module and Scheduling Basics

