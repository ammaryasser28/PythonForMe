# 🎀 Tuples in Python

## 🎯 Introduction
A **Tuple** is a collection of items stored in a single variable (similar to a list)  
but the main difference is that **tuples are immutable**, meaning you **cannot change** their elements once created.

Tuples use **round brackets** `()`.

```python
my_tuple = (10, 20, 30)
names = ("Ahmed", "Amr", "Omar")
mixed = (1, "Python", 3.14, True)
```

## ✅ Tuple Characteristics
| Feature                   | Description                                 |
| ------------------------- | ------------------------------------------- |
| Ordered                   | Items have indexes                          |
| Immutable                 | You **cannot** modify, add, or remove items |
| Allows Duplicates         | Values can repeat                           |
| Can Store Different Types | Numbers, strings, etc.                      |

## 🔢 Indexing and Slicing
```python
my_tuple = (10, 20, 30, 40, 50)

print(my_tuple[0])    # 10
print(my_tuple[-1])   # 50
print(my_tuple[1:4])  # (20, 30, 40)
```

## ❗ Immutability (Cannot Change Items)
```python
my_tuple = (1, 2, 3)
# my_tuple[1] = 10   # ❌ Error
```

## ✏️ But You Can Convert to List to Edit
```python
t = (1, 2, 3)
x = list(t)
x[1] = 10
t = tuple(x)
print(t)   # (1, 10, 3)
```

## ➕ Concatenation and Repetition
```python
a = (1, 2)
b = (3, 4)

print(a + b)     # (1, 2, 3, 4)
print(a * 2)     # (1, 2, 1, 2)
```



