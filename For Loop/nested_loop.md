# 🔁 Nested Loops in Python

## 📌 Introduction
A **nested loop** is a loop inside another loop.  
The inner loop runs completely **for every single iteration** of the outer loop.

This is useful when working with:
- 2D lists  
- Patterns  
- Combinations  
- Multi-level iterations  

---

## 🧩 Basic Example

```python
for i in range(3):
    for j in range(2):
        print(i, j)
```
▶️ Output
```python
0 0
0 1
1 0
1 1
2 0
2 1
```

## 📘 How Nested Loops Work
- Outer Loop
Controls rows, cycles, or main structure.
- Inner Loop
Controls columns, repeated tasks, or nested structure.
```python
Outer Loop → i = 0
    Inner Loop → j = 0, 1, 2...

Outer Loop → i = 1
    Inner Loop → j = 0, 1, 2...

Outer Loop → i = 2
    Inner Loop → j = 0, 1, 2...
```
