# 🧮 Sets in Python

## 🎯 Introduction
A **Set** in Python is a **collection of unique and unordered items**.  
It is **mutable**, meaning you can add or remove elements, but **it doesn’t allow duplicates**.

Sets are mainly used for **mathematical operations** like **union, intersection, difference**, etc.

---

## 🧱 Creating a Set
```python
my_set = {1, 2, 3, 4}
print(my_set)
```
🖥️ Output:
```python
{1, 2, 3, 4}
```
💡 Notice that sets use curly braces {}, just like dictionaries —
but they don’t have key-value pairs.

## ⚠️ Duplicates Are Not Allowed
```python
nums = {1, 2, 2, 3}
print(nums)
```
🖥️ Output:
```python
{1, 2, 3}
```
💡 The duplicate 2 was removed automatically.

## 🧩 Using set() Constructor
You can create a set from a list or string:
```python
letters = set("hello")
print(letters)
```
🖥️ Output:
```python
{'h', 'e', 'l', 'o'}
```
💡 Duplicate letters are removed, and the order is not guaranteed.

## 🔍 Accessing Set Elements
- You cannot access items by index because sets are unordered.
- But you can loop through them:
```python
fruits = {"apple", "banana", "cherry"}

for fruit in fruits:
    print(fruit)
```
🖥️ Output:
```python
apple
banana
cherry
```
