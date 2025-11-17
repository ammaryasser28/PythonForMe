# ⚠️ Python Errors

## 📌 Introduction
Errors in Python happen when the interpreter cannot understand or execute your code.  
Python shows an error message that helps you know **what the problem is** and **where it happened**.

There are two main categories:

1. **Syntax Errors** – mistakes in the code structure.
2. **Runtime Errors (Exceptions)** – errors that occur while the code is running.

---

## 1️⃣ Syntax Errors
These appear when you write code that Python cannot parse.

### 🔥 Example: Missing colon
```python
if True
    print("Hello")
```
❗ Error:
```
SyntaxError: invalid syntax
```
- 📝 Why?
Because the if statement must end with :.

## 2️⃣ NameError
- Occurs when you try to use a variable that doesn’t exist.
```python
print(age)
```
Error:
```python
NameError: name 'age' is not defined
```

## 3️⃣ TypeError
- Happens when an operation is applied to an incompatible data type.
```python
print("Age: " + 20)
```
Error:
```python
TypeError: can only concatenate str (not "int") to str
```

## 4️⃣ ValueError
- Occurs when a function receives the right data type but the wrong value.
```python
int("hello")
```
Error:
```python
ValueError: invalid literal for int() with base 10: 'hello'
```

## 5️⃣ IndexError
- Happens when trying to access a list index that doesn’t exist.
```python
nums = [1, 2, 3]
print(nums[5])
```
Error:
```python
IndexError: list index out of range
```

## 6️⃣ KeyError
- Occurs when accessing a dictionary with a missing key.
```python
user = {"name": "Amr"}
print(user["age"])
```
Error:
```python
KeyError: 'age'
```

## 7️⃣ ZeroDivisionError
- Triggered when dividing by zero.
```python
print(10 / 0)
```
Error:
```python
ZeroDivisionError: division by zero
```

## 8️⃣ AttributeError
- Occurs when trying to use a method or attribute that doesn’t exist.
```python
name = "Amr"
name.push()
```
Error:
```python
AttributeError: 'str' object has no attribute 'push'
```

## 9️⃣ ImportError
- Happens when Python cannot import a module.
```python
import my_missing_module
```
Error:
```python
ImportError: No module named 'my_missing_module'
```

## ✅ Summary Table
| Error Type          | Meaning                  | Example         |
| ------------------- | ------------------------ | --------------- |
| `SyntaxError`       | Wrong code structure     | Missing `:`     |
| `NameError`         | Variable not defined     | `print(x)`      |
| `TypeError`         | Wrong data type          | `"a" + 1`       |
| `ValueError`        | Wrong value              | `int("abc")`    |
| `IndexError`        | Invalid list index       | `arr[10]`       |
| `KeyError`          | Missing dictionary key   | `dict["age"]`   |
| `ZeroDivisionError` | Division by zero         | `10/0`          |
| `AttributeError`    | Missing attribute/method | `"text".push()` |
| `ImportError`       | Cannot import a module   | `import x`      |



