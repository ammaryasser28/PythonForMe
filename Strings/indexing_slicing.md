# 🔤 Indexing and Slicing in Python

## 🎯 Introduction
A **string** is a sequence of characters inside quotes (`" "` or `' '`).  
In Python, strings are **indexable and sliceable**, meaning you can access specific characters or parts of the string easily.

---

## 🧠 String Indexing
Each character in a string has an **index (position)**.  
Indexes start from **0** for the first character.

Example:
```python
name = "Python"
```
| Character | P  | y  | t  | h  | o  | n  |
| --------- | -- | -- | -- | -- | -- | -- |
| Index     | 0  | 1  | 2  | 3  | 4  | 5  |
| Negative  | -6 | -5 | -4 | -3 | -2 | -1 |

🔹 Accessing Characters

You can access any character by its index using square brackets [].
```python
name = "Python"

print(name[0])  # P
print(name[1])  # y
print(name[-1]) # n (last character)
print(name[-2]) # o
```
🖥️ Output:
```python
P
y
n
o
```

## ✂️ String Slicing
Slicing means taking a part of a string (substring) using the format:
```python
string[start:end]
```
- start → the index where slicing begins (included)
- end → the index where slicing stops (excluded)

Example:
```python
name = "Python"
print(name[0:4])  # Pyth
```
🖥️ Output:
```python
Pyth
```

🔸 Omitting Start or End

If you leave out the start or end index, Python uses defaults:
```python
name = "Python"

print(name[:4])   # from start to index 3 → Pyth
print(name[2:])   # from index 2 to the end → thon
print(name[:])    # entire string → Python
```
🖥️ Output:
```python
Pyth
thon
Python
```

🔹 Using Negative Indexes

You can slice from the end using negative indexes:
```python
name = "Python"

print(name[-3:])   # hon
print(name[:-2])   # Pytho
```
🖥️ Output:
```python
hon
Pytho
```

🔸 Adding a Step Value

You can also add a step (the third value) to skip characters:
```python
string[start:end:step]
```
Example:
```python
name = "Python"

print(name[0:6:2])   # Pto
print(name[::-1])    # Reverse string → nohtyP
```
🖥️ Output:
```python
Pto
nohtyP
```

## 🧾 Summary
| Concept           | Example         | Result  |
| ----------------- | --------------- | ------- |
| Indexing          | `"Hello"[1]`    | `e`     |
| Negative Indexing | `"Hello"[-1]`   | `o`     |
| Basic Slice       | `"Hello"[1:4]`  | `ell`   |
| Slice from Start  | `"Hello"[:3]`   | `Hel`   |
| Slice to End      | `"Hello"[2:]`   | `llo`   |
| Slice with Step   | `"Hello"[::2]`  | `Hlo`   |
| Reverse String    | `"Hello"[::-1]` | `olleH` |
