# 🧱 2D Lists in Python

## 🎯 What Are 2D Lists?
A **2D List** (Two-Dimensional List) is a list that contains **other lists inside it**.  
It works like a table with **rows and columns**.

Example:

```python
matrix = [
    [1, 2, 3],      # Row 0
    [4, 5, 6],      # Row 1
    [7, 8, 9]       # Row 2
]
```
## 📌 Accessing Elements
- Use two indexes:
- First index → Row
- Second index → Column
```
matrix[0][1]
```
🖥️ Output:
```
2
```

## 🔄 Looping Through a 2D List
- 1️⃣ Loop Through Rows
```
for row in matrix:
    print(row)
```
- 2️⃣ Loop Through All Elements
```
for row in matrix:
    for item in row:
        print(item)
```

## ✏️ Editing Values
```
matrix[1][2] = 99
print(matrix)
```
🖥️ Output:
```
[
 [1, 2, 3],
 [4, 5, 99],
 [7, 8, 9]
]
```

