# 🗒️ Comments and How to Use It in Python

## 🎯 Introduction
**Comments** in Python are lines of text that are ignored by the interpreter.  
They are used to:
- Explain what your code does.
- Leave notes for yourself or other developers.
- Temporarily disable a line of code without deleting it.

Comments **are not executed**, they are just for humans to read.

---

## 🧠 Types of Comments in Python

### 1. 🟢 Single-line Comment
- Single-line comments start with the `#` symbol.  
- Everything after `#` on that line will be ignored by Python.

```python
# This is a comment explaining the next line
print("Hello Python")  # You can also write a comment at the end of a line
```
✅ Notes:
- Anything after # on the same line won’t be executed.
- You can use comments anywhere in your code.

### 2. 🟣 Multi-line Comments
- Python doesn’t have a specific syntax for multi-line comments,
- but you can achieve the same effect in two ways 👇

Method 1️⃣ — Using # on each line:
```
# This is the first line of the comment
# This is the second line
# This is the third line
```
Method 2️⃣ — Using Triple Quotes (''' or """)
- You can use triple quotes to write multi-line comments.
- This is especially useful for long explanations or documentation.
```
"""
This is an example of
a multi-line comment
using triple quotes
"""
print("Python is awesome!")
```

⚠️ Note:
- If the triple quotes are not used as a docstring (inside a function or class),
- Python will simply ignore them — just like a comment.

🧩 Practical Example
```
# A simple program that calculates the sum of two numbers

num1 = 10  # first number
num2 = 5   # second number

# calculate the result
result = num1 + num2

print(result)  # print the result
```

## 💬 Why Use Comments?
- Makes your code easier to understand.
- Helps others (and your future self) read your code.
- Useful for debugging or disabling temporary code.

## 🚫 Common Mistakes

❌ Writing a comment right after code without a space:
```
print("Hi")#Wrong
```
✅ Correct:
```
print("Hi")  # Correct
```
❌ Forgetting to close triple quotes:
```
"""
This will cause an error
print("Hi")
```

## 🧾 Comments vs Docstrings
| Feature             | Comments           | Docstrings                    |
| ------------------- | ------------------ | ----------------------------- |
| Purpose             | Explain code logic | Document functions or classes |
| Syntax              | `#` or `'''`       | `"""` inside a function/class |
| Executed by Python? | No                 | Accessible with `help()`      |

🔹 Example of a Docstring:
```
def say_hello():
    """This function prints a hello message."""
    print("Hello!")

help(say_hello)
```


