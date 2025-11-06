# 📋 Lists in Python

## 🎯 Introduction
A **List** in Python is a **collection of items** stored in a single variable.  
Lists are **ordered**, **changeable (mutable)**, and allow **duplicate values**.

You define a list using **square brackets** `[]`.

```python
my_list = [1, 2, 3, 4]
names = ["Ahmed", "Amr", "Omar"]
mixed = [10, "Python", 3.14, True]
```

## ✅ List Characteristics
| Feature                   | Description                           |
| ------------------------- | ------------------------------------- |
| Ordered                   | Items have indexes                    |
| Mutable                   | You can change elements               |
| Allows Duplicates         | Same values can appear multiple times |
| Can Store Different Types | Numbers, strings, floats, etc.        |

## 🔢 Indexing (Access Elements)
| Type              | Explanation    | Example       | Result     |
| ----------------- | -------------- | ------------- | ---------- |
| Positive Indexing | Starts from 0  | `my_list[0]`  | First item |
| Negative Indexing | Starts from -1 | `my_list[-1]` | Last item  |
```python
my_list = ["A", "B", "C", "D"]
print(my_list[0])   # A
print(my_list[-1])  # D
```

## ✂️ Slicing Lists
```python
my_list = [10, 20, 30, 40, 50]
print(my_list[1:4])   # [20, 30, 40]
print(my_list[:3])    # [10, 20, 30]
print(my_list[2:])    # [30, 40, 50]
print(my_list[::-1])  # Reverse → [50, 40, 30, 20, 10]
```

## 📝 Changing List Items
```python
my_list = [1, 2, 3]
my_list[1] = 10
print(my_list)   # [1, 10, 3]
```

Syntax: list[start:end] (end index not included)
