# ⚖️ Comparison Operators in Python

## 🎯 Introduction
Comparison operators are used to **compare two values**.  
They return a **Boolean value** — either `True` or `False`.

These operators are very important in **conditions**, **loops**, and **decision making**.

---

## 🔍 List of Comparison Operators

| Operator | Meaning | Example | Result |
|-----------|----------|----------|---------|
| `==` | Equal to | `5 == 5` | `True` |
| `!=` | Not equal to | `5 != 3` | `True` |
| `>` | Greater than | `7 > 4` | `True` |
| `<` | Less than | `2 < 9` | `True` |
| `>=` | Greater than or equal | `5 >= 5` | `True` |
| `<=` | Less than or equal | `4 <= 6` | `True` |

---

## 🧩 Examples

```python
x = 10
y = 20

print(x == y)   # False
print(x != y)   # True
print(x > y)    # False
print(x < y)    # True
print(x >= 10)  # True
print(y <= 15)  # False
```
🖥️ Output:
```python
False
True
False
True
True
False
```

## ⚡ Comparing Strings
Python can also compare strings alphabetically (based on Unicode order).
```python
print("apple" == "apple")  # True
print("apple" != "banana") # True
print("car" > "bus")       # True (c comes after b)
```

## 🔄 Comparing Different Data Types
You can compare numbers with floats — Python automatically converts types when possible.
```python
print(10 == 10.0)  # True
print(10 > 9.5)    # True
```
⚠️ Comparing incompatible types like int and str raises an error:
```python
# print(10 > "5")  ❌  → TypeError
```

## 🧠 Using in Conditions
Comparison operators are often used in if statements:
```python
age = 18

if age >= 18:
    print("You can vote!")
else:
    print("You are too young.")
```
🖥️ Output:
```python
You can vote!
```

## 🧾 Summary Table
| Operator | Description      | Example  | Output |
| -------- | ---------------- | -------- | ------ |
| `==`     | Equal            | `3 == 3` | `True` |
| `!=`     | Not Equal        | `5 != 2` | `True` |
| `>`      | Greater Than     | `7 > 4`  | `True` |
| `<`      | Less Than        | `2 < 5`  | `True` |
| `>=`     | Greater or Equal | `6 >= 6` | `True` |
| `<=`     | Less or Equal    | `4 <= 6` | `True` |

