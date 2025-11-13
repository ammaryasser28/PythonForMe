# 🧩 Set Methods in Python

## 🎯 Introduction
Python provides many **built-in methods** to perform different operations on sets,  
such as adding, removing, and performing mathematical operations (union, intersection, etc.).

Let’s explore all of them one by one 👇

---

## 1️⃣ add()
Adds a single element to the set.

```python
fruits = {"apple", "banana"}
fruits.add("cherry")
print(fruits)
```
🖥️ Output:
```python
{'apple', 'banana', 'cherry'}
```

## 2️⃣ update()
Adds multiple elements (from a list, tuple, or another set).
```python
numbers = {1, 2, 3}
numbers.update([4, 5, 6])
print(numbers)
```
🖥️ Output:
```python
{1, 2, 3, 4, 5, 6}
```

## 3️⃣ remove()
- Removes a specific element.
- ⚠️ Raises an error if the element doesn’t exist.
```python
colors = {"red", "green", "blue"}
colors.remove("green")
print(colors)
```
🖥️ Output:
```python
{'red', 'blue'}
```

## 4️⃣ discard()
Removes a specific element without raising an error if it’s missing.
```python
colors = {"red", "green", "blue"}
colors.discard("yellow")
print(colors)
```
🖥️ Output:
```python
{'red', 'green', 'blue'}
```

## 5️⃣ pop()
Removes and returns a random element.
```python
nums = {10, 20, 30}
removed = nums.pop()
print("Removed:", removed)
print("Remaining:", nums)
```
🖥️ Output:
```python
Removed: 10
Remaining: {20, 30}
```

## 6️⃣ clear()
Removes all elements from the set.
```python
items = {"pen", "book", "bag"}
items.clear()
print(items)
```
🖥️ Output:
```python
set()
```

## 7️⃣ union() or |
Combines all elements from two or more sets (no duplicates).
```python
a = {1, 2, 3}
b = {3, 4, 5}
print(a.union(b))
```
🖥️ Output:
```python
{1, 2, 3, 4, 5}
```

## 8️⃣ intersection() or &
Returns elements common to both sets.
```python
a = {1, 2, 3}
b = {2, 3, 4}
print(a.intersection(b))
```
🖥️ Output:
```python
{2, 3}
```

## 9️⃣ difference() or -
Returns elements that are only in the first set.
```python
a = {1, 2, 3}
b = {2, 3, 4}
print(a.difference(b))
```
🖥️ Output:
```python
{1}
```

## 🔟 symmetric_difference() or ^
Returns elements that are in one set only, not both.
```python
a = {1, 2, 3}
b = {3, 4, 5}
print(a.symmetric_difference(b))
```
🖥️ Output:
```python
{1, 2, 4, 5}
```

## 11️⃣ issubset()
Returns True if all elements of one set exist in another.
```python
a = {1, 2}
b = {1, 2, 3}
print(a.issubset(b))
```
🖥️ Output:
```python
True
```

## 12️⃣ issuperset()
Returns True if the set contains all elements of another.
```python
a = {1, 2, 3}
b = {1, 2}
print(a.issuperset(b))
```
🖥️ Output:
```python
True
```

## 13️⃣ isdisjoint()
Returns True if sets have no elements in common.
```python
a = {1, 2}
b = {3, 4}
print(a.isdisjoint(b))
```
🖥️ Output:
```python
True
```

## 🧾 Summary Table
| Method                         | Description                        | Example           | Output          |    |                     |
| ------------------------------ | ---------------------------------- | ----------------- | --------------- | -- | ------------------- |
| `add()`                        | Adds one element                   | `s.add(4)`        | `{..., 4}`      |    |                     |
| `update()`                     | Adds multiple elements             | `s.update([5,6])` | `{...,5,6}`     |    |                     |
| `remove()`                     | Removes element (error if missing) | `s.remove(3)`     | Removes 3       |    |                     |
| `discard()`                    | Removes element (safe)             | `s.discard(10)`   | No error        |    |                     |
| `pop()`                        | Removes a random element           | `s.pop()`         | Random item     |    |                     |
| `clear()`                      | Removes all elements               | `s.clear()`       | `set()`         |    |                     |
| `union()` / `                  | `                                  | Combine sets      | `a              | b` | All unique elements |
| `intersection()` / `&`         | Common elements                    | `a & b`           | Shared elements |    |                     |
| `difference()` / `-`           | Unique in first set                | `a - b`           | Unique to a     |    |                     |
| `symmetric_difference()` / `^` | In one set only                    | `a ^ b`           | Not shared      |    |                     |
| `issubset()`                   | Checks if smaller set is inside    | `a.issubset(b)`   | True/False      |    |                     |
| `issuperset()`                 | Checks if set contains another     | `a.issuperset(b)` | True/False      |    |                     |
| `isdisjoint()`                 | Checks if no elements overlap      | `a.isdisjoint(b)` | True/False      |    |                     |

