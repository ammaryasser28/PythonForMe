# 🧰 List Methods in Python

## 🎯 Introduction
Python lists come with many built-in methods that allow you to **add**, **remove**, **search**, **sort**, and **manipulate** list elements easily.

Below are the most commonly used list methods.

---

## ➕ Adding Items

### append()
Adds an item to the **end** of the list.
```python
my_list = [1, 2, 3]
my_list.append(4)
print(my_list)   # [1, 2, 3, 4]
```

### insert()
Adds an item at a specific index.
```python
my_list = ["A", "C"]
my_list.insert(1, "B")
print(my_list)   # ["A", "B", "C"]
```

### extend()
Adds multiple items at once.
```python
numbers = [1, 2]
numbers.extend([3, 4, 5])
print(numbers)   # [1, 2, 3, 4, 5]
```

---

## ➖ Removing Items

### remove()
Removes the first occurrence of a value.
```python
x = [1, 2, 2, 3]
x.remove(2)
print(x)   # [1, 2, 3]
```

### pop()
Removes an item by index (default last).
```python
x = [10, 20, 30]
x.pop(1)
print(x)   # [10, 30]
```

### clear()
Removes all items.
```python
x = [4, 5, 6]
x.clear()
print(x)   # []
```

---

## 🔍 Searching

### index()
Returns the index of a value.
```python
names = ["Ali", "Omar", "Amr"]
print(names.index("Amr"))   # 2
```

### count()
Counts how many times a value appears.
```python
x = [1, 1, 2, 3]
print(x.count(1))   # 2
```

---

## 🔁 Sorting and Reversing

### sort()
Sorts the list ascending.
```pyhton
nums = [4, 2, 8, 1]
nums.sort()
print(nums)   # [1, 2, 4, 8]
```

### sort(reverse=True)
Sorts descending.
```python
nums = [4, 2, 8, 1]
nums.sort(reverse=True)
print(nums)   # [8, 4, 2, 1]
```

### reverse()
Reverses list order (NOT sorting).
```python
nums = [1, 2, 3]
nums.reverse()
print(nums)   # [3, 2, 1]
```

---

## 📝 Copying Lists

### copy()
Creates a shallow copy of the list.
```python
a = [1, 2, 3]
b = a.copy()
print(b)   # [1, 2, 3]
```

---

## 🧾 Summary Table
| Method               | Purpose                 | Example                   | Result                      |
| -------------------- | ----------------------- | ------------------------- | --------------------------- |
| `append(x)`          | Add one item to end     | `[1,2].append(3)`         | `[1,2,3]`                   |
| `insert(i,x)`        | Insert at index         | `list.insert(1,"A")`      | Insert "A" at index 1       |
| `extend(iterable)`   | Add multiple items      | `[1].extend([2,3])`       | `[1,2,3]`                   |
| `remove(x)`          | Remove first occurrence | `list.remove(2)`          | Removes first matching 2    |
| `pop(i)`             | Remove item by index    | `list.pop(1)`             | Removes element at index 1  |
| `clear()`            | Empty list              | `list.clear()`            | `[]`                        |
| `index(x)`           | Find index of item      | `list.index("Ali")`       | Returns index               |
| `count(x)`           | Count occurrences       | `list.count(2)`           | Returns count of 2          |
| `sort()`             | Sort ascending          | `list.sort()`             | Sorted list                 |
| `sort(reverse=True)` | Sort descending         | `list.sort(reverse=True)` | Reverse sorted              |
| `reverse()`          | Reverse order           | `list.reverse()`          | List reversed               |
| `copy()`             | Copy list               | `list.copy()`             | New list with same elements |


