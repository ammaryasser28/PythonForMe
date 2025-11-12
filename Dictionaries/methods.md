# 🧩 Dictionary Methods in Python

## 🎯 Introduction
Dictionaries in Python have many built-in methods that make it easy to **manipulate, update, and retrieve** data efficiently.  
Here’s a detailed explanation of the most important ones.

---

## 🧱 Common Dictionary Methods

### 1️⃣ clear()
Removes **all items** from the dictionary.

```python
info = {"name": "Amr", "age": 21}
info.clear()
print(info)  # {}
```
### 2️⃣ update()
Updates the dictionary with new key-value pairs or modifies existing keys.
```python
info = {"name": "Amr", "age": 21}
info.update({"age": 22, "country": "Egypt"})
print(info)
# {'name': 'Amr', 'age': 22, 'country': 'Egypt'}
```

### 3️⃣ copy()
Returns a shallow copy of the dictionary.
```python
original = {"a": 1, "b": 2}
copied = original.copy()
print(copied)  # {'a': 1, 'b': 2}
```

### 4️⃣ fromkeys()
Creates a new dictionary using given keys and a single default value.
```python
keys = ("name", "age", "job")
new_dict = dict.fromkeys(keys, "Not Specified")
print(new_dict)
# {'name': 'Not Specified', 'age': 'Not Specified', 'job': 'Not Specified'}
```

### 5️⃣ get()
- Returns the value for a specified key.
- If the key doesn’t exist → returns None (or a default value if provided).
```python
person = {"name": "Amr", "age": 21}
print(person.get("age"))          # 21
print(person.get("country"))      # None
print(person.get("country", "N/A"))  # N/A
```

### 6️⃣ items()
Returns all dictionary items as (key, value) tuples.
```python
person = {"name": "Amr", "age": 21}
print(person.items())
# dict_items([('name', 'Amr'), ('age', 21)])
```

### 7️⃣ keys()
Returns all keys in the dictionary.
```python
person = {"name": "Amr", "age": 21}
print(person.keys())  # dict_keys(['name', 'age'])
```

### 8️⃣ values()
Returns all values in the dictionary.
```python
person = {"name": "Amr", "age": 21}
print(person.values())  # dict_values(['Amr', 21])
```

### 9️⃣ pop()
Removes an item by key and returns its value.
```python
person = {"name": "Amr", "age": 21}
removed = person.pop("age")
print(removed)  # 21
print(person)   # {'name': 'Amr'}
```

### 🔟 popitem()
Removes and returns the last inserted (key, value) pair.
```python
person = {"name": "Amr", "age": 21}
item = person.popitem()
print(item)  # ('age', 21)
print(person)  # {'name': 'Amr'}
```

## 🧾 Summary Table
| Method       | Description                     | Example                      | Output                       |
| ------------ | ------------------------------- | ---------------------------- | ---------------------------- |
| `clear()`    | Removes all items               | `person.clear()`             | `{}`                         |
| `update()`   | Adds or updates keys            | `person.update({"age": 22})` | Updated dict                 |
| `copy()`     | Returns a shallow copy          | `new = person.copy()`        | `{'name': 'Amr', 'age': 21}` |
| `fromkeys()` | Creates new dict from keys      | `dict.fromkeys(keys, 0)`     | `{'a': 0, 'b': 0}`           |
| `get()`      | Returns value or default        | `person.get("age", "N/A")`   | `21`                         |
| `items()`    | Returns list of key-value pairs | `person.items()`             | `dict_items([...])`          |
| `keys()`     | Returns all keys                | `person.keys()`              | `dict_keys([...])`           |
| `values()`   | Returns all values              | `person.values()`            | `dict_values([...])`         |
| `pop()`      | Removes key and returns value   | `person.pop("age")`          | `21`                         |
| `popitem()`  | Removes last inserted pair      | `person.popitem()`           | `('key', value)`             |
