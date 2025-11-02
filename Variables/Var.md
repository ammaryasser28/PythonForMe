# 🧮 Variables in Python

## 🎯 Introduction
**Variables** are containers that store data values.  
They allow you to save information, use it later, and manipulate it in your code.

Think of a variable like a box with a name — you can put something inside it, take it out, or change what’s inside.

---

## 🧠 Creating Variables
You create a variable by writing a **name**, then using the **assignment operator (`=`)**, and then giving it a **value**.
```python
name = "Amr"
age = 20
country = "Egypt"
```
✅ Explanation:
- name, age, and country are variable names.
- The = symbol assigns the value on the right to the variable on the left.


## 🧾 Rules for Variable Names
To create valid variable names in Python, follow these rules:
| Rule                                               | Example                | Valid? |
| -------------------------------------------------- | ---------------------- | ------ |
| Must start with a letter or underscore `_`         | `name`, `_user`        | ✅ Yes  |
| Cannot start with a number                         | `1name`                | ❌ No   |
| Can contain only letters, numbers, and underscores | `user_name`, `user1`   | ✅ Yes  |
| Case-sensitive                                     | `Name` ≠ `name`        | ✅ Yes  |
| No spaces or special characters                    | `user-name`, `my name` | ❌ No   |

🧩 Example
```
# Define variables
username = "Osama"
age = 36
country = "Egypt"

# Print the values
print(username)
print(age)
print(country)
```
🖥️ Output:
```
Osama
36
Egypt
```


## 🔁 Reassigning Variables
You can change the value of a variable at any time:
```
x = 10
x = 20
print(x)  # Output: 20
```
✅ The last value assigned is the one Python keeps.


## 📦 Multiple Assignments
Python allows assigning multiple variables in one line:
```
a, b, c = 1, 2, 3
print(a, b, c)
```
🖥️ Output:
```
1 2 3
```
You can also assign the same value to multiple variables:
```
x = y = z = 100
print(x, y, z)
```
🖥️ Output:
```
100 100 100
```


## 🧮 Variable Types
Python automatically detects the type of value stored in a variable.
```
name = "Osama"   # str (string)
age = 36         # int (integer)
score = 99.5     # float (decimal number)
is_student = True  # bool (boolean)
```
You can check the variable type using the type() function:
```
print(type(name))      # <class 'str'>
print(type(age))       # <class 'int'>
print(type(score))     # <class 'float'>
print(type(is_student))# <class 'bool'>
```


## 🧹 Naming Conventions (Best Practices)
✅ Use descriptive names:
```
user_name = "Amr"
total_price = 150.75
```
❌ Avoid meaningless names:
```
x = "Amr"
tp = 150.75
```
✅ Follow snake_case style for variable names (recommended in Python):
```
first_name = "Osama"
```

