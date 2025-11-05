# 🧰 String Methods in Python

## 🎯 Introduction
Python provides many **built-in string methods** that make it easy to manipulate and analyze text.  
These methods **do not change the original string**, because strings in Python are **immutable**.  
They return **new strings** instead.

---

## 🧱 Basic String Methods

### 🔹 `upper()`
Converts all characters to uppercase.

```python
name = "python"
print(name.upper())
```
🖥️ Output:
```python
PYTHON
```

### 🔹 lower()
Converts all characters to lowercase.
```python
text = "HELLO"
print(text.lower())
```
🖥️ Output:
```python
hello
```

### 🔹 title()
Converts the first letter of each word to uppercase.
```python
sentence = "hello world from python"
print(sentence.title())
```
🖥️ Output:
```python
Hello World From Python
```

### 🔹 capitalize()
Converts only the first character of the string to uppercase.
```python
text = "python is fun"
print(text.capitalize())
```
🖥️ Output:
```python
Python is fun
```

### 🔹 strip()
Removes spaces from the beginning and end of the string.
```python
name = "   Amr Yasser   "
print(name.strip())
```
🖥️ Output:
```python
Amr Yasser
```
- ✅ Use lstrip() to remove spaces from the left
- ✅ Use rstrip() to remove spaces from the right

### 🔹 replace(old, new)
Replaces part of a string with another.
```python
text = "I love Java"
print(text.replace("Java", "Python"))
```
🖥️ Output:
```python
I love Python
```

### 🔹 split()
Splits a string into a list of words.
```python
sentence = "I love Python programming"
print(sentence.split())
```
🖥️ Output:
```python
['I', 'love', 'Python', 'programming']
```
You can also specify a separator:
```python
text = "apple,banana,orange"
print(text.split(","))
```
🖥️ Output:
```python
['apple', 'banana', 'orange']
```

### 🔹 join()
Joins a list of strings into one string.
```python
words = ["Python", "is", "awesome"]
print(" ".join(words))
```
🖥️ Output:
```python
Python is awesome
```

### 🔹 count()
Counts how many times a substring appears in a string.
```python
text = "python python PYTHON"
print(text.count("python"))
```
🖥️ Output:
```python
2
```

###🔹 find() and index()
Find the position of a substring in a string.
```python
text = "I love Python"
print(text.find("Python"))  # 7
```
🖥️ Output:
```pyhon
7
```
🧩 Difference:
- find() → returns -1 if not found
- index() → raises an error if not found
```python
text = "Python"
print(text.find("x"))   # -1
print(text.index("x"))  # ❌ ValueError
```

### 🔹 startswith() / endswith()
Check if a string starts or ends with a specific substring.
```python
name = "Python Programming"

print(name.startswith("Python"))  # True
print(name.endswith("ing"))       # True
```

###🔹 swapcase()
Switches uppercase letters to lowercase and vice versa.
```python
text = "PyThOn"
print(text.swapcase())
```
🖥️ Output:
```python
pYtHoN
```

### 🔹 isalpha() / isdigit() / isalnum()
Check what type of characters are in the string.
```python
print("Hello".isalpha())  # True
print("1234".isdigit())   # True
print("Hi123".isalnum())  # True
```
🖥️ Output:
```python
True
True
True
```

### 🔹 `zfill(width)`
Adds **leading zeros** to the string until it reaches the given length.
```python
num = "50"
print(num.zfill(5))
```
🖥️ Output:
```python
00050
```

###🔹 center(width, char)
Centers the string between a certain number of characters.
```python
name = "Python"
print(name.center(11, "-"))
```
🖥️ Output:
```python
---Python---
```

###🔹 rjust(width, char) and ljust(width, char)
- rjust() → Aligns text to the right
- ljust() → Aligns text to the left
```python
text = "Hi"
print(text.rjust(6, "*"))
print(text.ljust(6, "*"))
```
🖥️ Output:
```python
****Hi
Hi****
```

###🔹 splitlines()
Splits a multi-line string into a list.
```python
text = """Hello
World
Python"""
print(text.splitlines())
```
🖥️ Output:
```python
['Hello', 'World', 'Python']
```

###🔹 expandtabs(size)
Controls how many spaces a tab \t is equal to.
```python
text = "Hello\tPython"
print(text.expandtabs(10))
```
🖥️ Output:
```python
Hello     Python
```

###🔹 istitle()
Returns True if each word is capitalized.
```python
print("Hello World".istitle())  # True
print("hello world".istitle())  # False
```

###🔹 isspace()
Returns True if the string contains only spaces.
```python
print("   ".isspace())  # True
print(" A ".isspace())  # False
```

###🔹 islower()
Returns True if all characters are lowercase.
```python
print("python".islower())  # True
print("Python".islower())  # False
```

###🔹 isidentifier()
Checks if a string can be used as a valid variable name.
```python
print("name".isidentifier())   # True
print("user_1".isidentifier()) # True
print("1user".isidentifier())  # False
print("@var".isidentifier())   # False
```

# 🧾 Full Summary Table

| Method | Description | Example | Output | Notes |
|--------|-------------|---------|--------|-------|
| `upper()` | Converts all letters to uppercase | `"python".upper()` | `PYTHON` | Does not modify original string |
| `lower()` | Converts all letters to lowercase | `"HELLO".lower()` | `hello` | Returns new string |
| `title()` | Capitalizes the first letter of each word | `"hello world".title()` | `Hello World` | Useful for names/titles |
| `capitalize()` | Capitalizes the first character only | `"hello world".capitalize()` | `Hello world` | Only first word affected |
| `strip()` | Removes spaces from both sides | `"  hi  ".strip()` | `hi` | Use `lstrip()` & `rstrip()` for sides |
| `replace(old, new)` | Replaces text | `"I love C".replace("C", "Python")` | `I love Python` | Can replace multiple occurrences |
| `split()` | Splits string into list | `"a b c".split()` | `['a', 'b', 'c']` | Default separator is space |
| `join(list)` | Joins elements of a list | `" ".join(['Python','is','fun'])` | `Python is fun` | Separator comes first |
| `count(substring)` | Counts occurrences of substring | `"hi hi".count("hi")` | `2` | Case-sensitive |
| `find(substring)` | Returns index of substring | `"Hello".find("l")` | `2` | Returns `-1` if not found |
| `index(substring)` | Returns index of substring | `"Hello".index("l")` | `2` | Raises error if not found |
| `startswith(sub)` | Checks if string starts with substring | `"Python".startswith("Py")` | `True` | Case-sensitive |
| `endswith(sub)` | Checks if string ends with substring | `"Python".endswith("on")` | `True` | Used often in file checks |
| `swapcase()` | Swaps upper ↔ lower | `"PyThOn".swapcase()` | `pYtHoN` | Useful for toggling case |
| `isalpha()` | Checks if all chars are letters | `"Hello".isalpha()` | `True` | No spaces or numbers allowed |
| `isdigit()` | Checks if all chars are digits | `"123".isdigit()` | `True` | `"12.5"` → `False` |
| `isalnum()` | Letters or digits | `"A1".isalnum()` | `True` | No spaces |
| `zfill(width)` | Pads string with zeros | `"50".zfill(5)` | `00050` | Affects left side only |
| `center(width, char)` | Centers text | `"Hi".center(6,"-")` | `--Hi--` | Default padding is space |
| `rjust(width, char)` | Right-aligns text | `"Hi".rjust(6,"*")` | `****Hi` | Useful for output formatting |
| `ljust(width, char)` | Left-aligns text | `"Hi".ljust(6,"*")` | `Hi****` | Used for table formatting |
| `splitlines()` | Splits based on line breaks | `"a\nb".splitlines()` | `['a', 'b']` | Detects all newline types |
| `expandtabs(size)` | Convert tab to spaces | `"a\tb".expandtabs(4)` | `a   b` | Default tab = 8 spaces |
| `istitle()` | Checks Title Case | `"Hello World".istitle()` | `True` | Each word must be capitalized |
| `islower()` | Checks if all characters lowercase | `"python".islower()` | `True` | Must contain alphabetic chars |
| `isspace()` | Checks if string is only whitespace | `"   ".isspace()` | `True` | Newlines count as space |
| `isidentifier()` | Valid Python variable name? | `"user_1".isidentifier()` | `True` | Must follow variable rules |
