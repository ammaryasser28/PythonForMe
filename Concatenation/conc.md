# 🔗 Concatenation in Python

## 🎯 Introduction
**Concatenation** means **joining strings together**.  
In Python, you can combine (concatenate) text, variables, and even numbers (after converting them to strings).

You’ll use concatenation a lot when printing messages or building text dynamically.

---

## 🧠 Basic String Concatenation
You can concatenate strings using the **`+`** operator.

```python
first_name = "Amr"
last_name = "Yasser"

full_name = first_name + " " + last_name
print(full_name)
```
🖥️ Output:
```
Amr Yasser
```
✅ Python joins the strings into one, and " " adds a space between them.

## ⚠️ Important: You Can Only Concatenate Strings
You cannot concatenate strings with numbers directly.
```
age = 20

# ❌ This will cause an error
print("My age is " + age)
```
🖥️ Error:
```
TypeError: can only concatenate str (not "int") to str
```
✅ To fix this, you must convert numbers to strings using str():
```
age = 20
print("My age is " + str(age))
```
🖥️ Output:
```
My age is 20
```
