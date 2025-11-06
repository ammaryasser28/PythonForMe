# 🎨 String Formatting in Python

## 🎯 Introduction
String formatting allows you to **combine text with variables** in a clean and readable way.  
Instead of using long concatenation, Python provides multiple ways to format strings.

---

## 1) ➕ Concatenation (Basic)
Using `+` to join strings:

```python
name = "Amr"
age = 21

print("My name is " + name + " and I am " + str(age) + " years old.")
```
🖥️ Output:
```python
My name is Amr and I am 21 years old.
```
⚠️ Not recommended when variables become many.

## 2) 🟡 Using format() Method
Basic Example:
```python
name = "Amr"
age = 21
print("My name is {} and I am {} years old.".format(name, age))
```
Numbered Placeholders:
```python
print("My name is {1} and I am {0} years old.".format(age, name))
```
Named Placeholders:
```python
print("My name is {username} and I am {userage} years old.".format(username="Amr", userage=21))
```

## 3) 🔵 f-Strings (Recommended — Python 3.6+)
Fastest + cleanest formatting:
```python
name = "Amr"
age = 21
print(f"My name is {name} and I am {age} years old.")
```
🖥️ Output:
```python
My name is Amr and I am 21 years old.
```

## 4) 🎯 Formatting Numbers
Decimal Places:
```python
price = 19.98765
print(f"Price: {price:.2f}")
```
🖥️ Output:
```python
Price: 19.99
```
Add Commas to Large Numbers:
```python
num = 1000000
print(f"{num:,}")
```
🖥️ Output:
```python
1,000,000
```
Aligning Text:
```python
print(f"|{'Python':^10}|")  # Center
print(f"|{'Python':<10}|")  # Left
print(f"|{'Python':>10}|")  # Right
```
🖥️ Output:
```python
|  Python  |
|Python    |
|    Python|
```

## 5) 🏦 Formatting with format() Style Codes
| Code   | Meaning                 | Example                    | Output       |
| ------ | ----------------------- | -------------------------- | ------------ |
| `:.2f` | 2 decimal numbers       | `"{:.2f}".format(3.14159)` | `3.14`       |
| `:,`   | Adds commas             | `"{:,}".format(1000000)`   | `1,000,000`  |
| `:>10` | Right align in width 10 | `"{:>10}".format("Hi")`    | `        Hi` |
| `:<10` | Left align in width 10  | `"{:<10}".format("Hi")`    | `Hi        ` |
| `:^10` | Center align            | `"{:^10}".format("Hi")`    | `    Hi    ` |

## 🧾 Summary Table
| Method            | Usage                     | Example                   | Output                  | Notes                             |
| ----------------- | ------------------------- | ------------------------- | ----------------------- | --------------------------------- |
| `+` Concatenation | Join strings manually     | `"Hi " + name`            | `Hi Amr`                | Must convert numbers with `str()` |
| `.format()`       | Insert variables by `{}`  | `"Hello {}".format(name)` | Inserted value          | Flexible but longer               |
| f-Strings         | Insert variables directly | `f"Hello {name}"`         | Inserted value          | Fastest & recommended             |
| `:.2f`            | Format decimals           | `f"{num:.2f}"`            | Rounded value           | Controls precision                |
| `:,`              | Add commas                | `f"{num:,}"`              | `1,000,000`             | Useful for money                  |
| `:> < ^`          | Align text                | `f"{text:^10}"`           | Centered / left / right | Useful in tables                  |

