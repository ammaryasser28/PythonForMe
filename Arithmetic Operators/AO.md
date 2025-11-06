# ➕ Arithmetic Operators in Python

## 🎯 Introduction
Arithmetic operators are used to perform **mathematical operations** on numbers such as addition, subtraction, multiplication, etc.

Python supports multiple arithmetic operators that work on both `int` and `float` values.

---

## 🧮 List of Arithmetic Operators

| Operator | Name | Example | Result |
|---------|------|---------|--------|
| `+` | Addition | `10 + 5` | `15` |
| `-` | Subtraction | `10 - 5` | `5` |
| `*` | Multiplication | `10 * 5` | `50` |
| `/` | Division | `10 / 5` | `2.0` *(Always returns float)* |
| `//` | Floor Division | `10 // 3` | `3` *(removes decimals)* |
| `%` | Modulus (Remainder) | `10 % 3` | `1` |
| `**` | Exponent (Power) | `2 ** 3` | `8` |

---

## 🧩 Examples

```python
a = 10
b = 3

print(a + b)   # 13
print(a - b)   # 7
print(a * b)   # 30
print(a / b)   # 3.3333333333
print(a // b)  # 3
print(a % b)   # 1
print(a ** b)  # 1000
```

## 🔥 Floor Division //
```python
print(9 // 2)   # 4  (not 4.5)
print(-9 // 2)  # -5  (rounds down, not toward zero)
```
Note: Floor division always rounds down, not just chops decimals.

## 🧮 Modulus % — Remainder
```python
print(10 % 3)   # 1
print(20 % 6)   # 2
print(15 % 5)   # 0   (exact division)
```
- Useful for:
Checking even/odd numbers
```python
print(6 % 2 == 0)  # True (even)
```

## ⚡ Exponent Operator **
```python
print(2 ** 3)   # 8
print(3 ** 2)   # 9
print(10 ** 0)  # 1
```

## 🧾 Summary Table
| Operator | Purpose        | Example  | Output |
| -------- | -------------- | -------- | ------ |
| `+`      | Add numbers    | `7 + 2`  | `9`    |
| `-`      | Subtract       | `7 - 2`  | `5`    |
| `*`      | Multiply       | `7 * 2`  | `14`   |
| `/`      | Divide (float) | `7 / 2`  | `3.5`  |
| `//`     | Floor division | `7 // 2` | `3`    |
| `%`      | Get remainder  | `7 % 2`  | `1`    |
| `**`     | Power          | `2 ** 4` | `16`   |

