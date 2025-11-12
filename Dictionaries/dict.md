# 📘 Dictionaries in Python

## 🎯 Introduction
A **Dictionary** in Python is a **collection of key–value pairs**.  
It is **unordered**, **mutable**, and **does not allow duplicate keys**.

You create a dictionary using curly braces `{}`.

```python
person = {
    "name": "Amr",
    "age": 21,
    "country": "Egypt"
}
```
## 🧱 Dictionary Structure
| Term      | Description                | Example  |
| --------- | -------------------------- | -------- |
| **Key**   | The unique identifier      | `"name"` |
| **Value** | The data assigned to a key | `"Amr"`  |
Each key must be unique, and each key maps to exactly one value.

## 🔍 Accessing Dictionary Items
You can access values using their keys:
```python
person = {"name": "Amr", "age": 21, "country": "Egypt"}

print(person["name"])       # Amr
print(person.get("age"))    # 21
```
⚠️ Using get() is safer — it returns None if the key doesn’t exist.

## ✏️ Changing Values
```python
person["age"] = 22
print(person)  # {'name': 'Amr', 'age': 22, 'country': 'Egypt'}
```

## ➕ Adding New Items
```python
person["job"] = "Developer"
print(person)
# {'name': 'Amr', 'age': 22, 'country': 'Egypt', 'job': 'Developer'}
```

## ➖ Removing Items
| Method          | Description                         | Example                 |
| --------------- | ----------------------------------- | ----------------------- |
| `pop(key)`      | Removes the item with the given key | `person.pop("age")`     |
| `popitem()`     | Removes the **last inserted** item  | `person.popitem()`      |
| `del dict[key]` | Deletes an item by key              | `del person["country"]` |
| `clear()`       | Removes **all items**               | `person.clear()`        |
```python
person = {"name": "Amr", "age": 21, "country": "Egypt"}

person.pop("age")
print(person)  # {'name': 'Amr', 'country': 'Egypt'}
```

## 🧩 Looping Through Dictionaries
- Loop over keys:
```python
for key in person:
    print(key)
```
- Loop over values:
```python
for value in person.values():
    print(value)
```
- Loop over both keys and values:
```python
for key, value in person.items():
    print(key, ":", value)
```
🖥️ Output:
```python
name : Amr
age : 21
country : Egypt
```
## 🧾 Summary Table
| Operation         | Description            | Example                   | Output            |
| ----------------- | ---------------------- | ------------------------- | ----------------- |
| Create Dictionary | Define key-value pairs | `{"a":1, "b":2}`          | `{'a':1, 'b':2}`  |
| Access Value      | Get value by key       | `person["name"]`          | `"Amr"`           |
| Use `get()`       | Safer access           | `person.get("age")`       | `21`              |
| Change Value      | Modify a key’s value   | `person["age"] = 22`      | Updates the value |
| Add Item          | Add new key-value      | `person["job"] = "Dev"`   | Adds item         |
| Remove Key        | Remove one key         | `person.pop("age")`       | Removes key       |
| Remove Last       | Remove last inserted   | `person.popitem()`        | Removes last pair |
| Loop Keys         | Iterate keys           | `for k in dict:`          | Each key          |
| Loop Values       | Iterate values         | `for v in dict.values()`  | Each value        |
| Loop Items        | Iterate pairs          | `for k,v in dict.items()` | Key and value     |
| Clear             | Remove all             | `dict.clear()`            | `{}`              |


