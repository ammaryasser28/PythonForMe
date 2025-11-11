# 🔀 If Condition in Python

## 🎯 Introduction
`if` statements are used to **make decisions** in Python.  
They allow your program to **execute code only if a certain condition is true**.

---

## ✅ Basic `if` Statement

```python
x = 10

if x > 5:
    print("x is greater than 5")
```
# 🔀 If Condition in Python

## 🎯 Introduction
`if` statements are used to **make decisions** in Python.  
They allow your program to **execute code only if a certain condition is true**.

---

## ✅ Basic `if` Statement
```python
x = 10

if x > 5:
    print("x is greater than 5")
```
Output:
```python
x is greater than 5
```

## 🟨 if - else
```python
age = 16

if age >= 18:
    print("You can drive")
else:
    print("You cannot drive")
```
Output:
```python
You cannot drive
```

## 🟦 if - elif - else
```python
score = 75

if score >= 90:
    print("Excellent")
elif score >= 70:
    print("Good")
else:
    print("Try Again")
```
Output:
```python
Good
```

## 🎛️ Nested If (If Inside If)
```python
x = 20

if x > 10:
    if x < 30:
        print("x is between 10 and 30")
```

## 🔗 Using Logical Operators (and, or, not)
```python
age = 22
has_license = True

if age >= 18 and has_license:
    print("Allowed to drive")
```
```python
temp = 35

if temp < 20 or temp > 30:
    print("Weather Not Comfortable")
```
```python
is_admin = False

if not is_admin:
    print("Access Denied")
```

## 📝 Comparison Operators Recap
| Operator | Meaning          | Example  | Result     |
| -------- | ---------------- | -------- | ---------- |
| `==`     | Equal            | `x == 5` | True/False |
| `!=`     | Not Equal        | `x != 5` | True/False |
| `>`      | Greater Than     | `x > 5`  | True/False |
| `<`      | Less Than        | `x < 5`  | True/False |
| `>=`     | Greater or Equal | `x >= 5` | True/False |
| `<=`     | Less or Equal    | `x <= 5` | True/False |

## 🧾 Summary Table
| Keyword / Concept | Purpose                            | Example                |
| ----------------- | ---------------------------------- | ---------------------- |
| `if`              | Run code only if condition is True | `if x > 5:`            |
| `else`            | Run when `if` is False             | `else:`                |
| `elif`            | Additional conditions              | `elif x == 5:`         |
| Nested If         | If inside another if               | `if x > 0: if x < 10:` |
| `and`             | Both conditions must be True       | `x > 5 and x < 10`     |
| `or`              | At least one condition True        | `x == 0 or x == 1`     |
| `not`             | Reverse condition                  | `not x == 5`           |


