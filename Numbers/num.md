# 🔢 Numbers in Python

## 🎯 Introduction
Python provides several **numeric data types** used to work with numbers.  
You can use them in math operations such as addition, subtraction, multiplication, etc.

---

## 🧱 Types of Numbers in Python

| Type | Description | Example |
|------|-------------|---------|
| `int` | Whole numbers (no decimals) | `10`, `-5`, `1000` |
| `float` | Numbers with decimals | `3.14`, `-0.5`, `2.0` |
| `complex` | Numbers with imaginary part | `3+4j`, `5j` |

---

## 🔍 Checking Number Types
Use `type()` to know the variable's type:

```python
x = 10
y = 3.14
z = 2 + 5j

print(type(x))
print(type(y))
print(type(z))
```
🖥️ Output:
```python
<class 'int'>
<class 'float'>
<class 'complex'>
```

## 🔁 Convert Between Number Types
- Convert to Integer:
```python
print(int(3.9))     # 3
print(int("15"))    # 15
```

- Convert to Float:
```python
print(float(5))     # 5.0
print(float("3.14")) # 3.14
```

 - Convert to Complex:
```python
print(complex(3))     # (3+0j)
print(complex(3, 5))  # (3+5j)
```

## 📏 Getting Absolute Value
```python
print(abs(-10))  # 10
```

## 🧮 Rounding Numbers
```python
print(round(3.14159, 2))  # 3.14
print(round(7.5))         # 8
```

## ⚙️ min() and max()
```python
print(min(2, 5, 1, 9))  # 1
print(max(2, 5, 1, 9))  # 9
```
