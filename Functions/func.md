# 🧩 Functions in Python

## 🎯 Introduction
A **function** is a reusable block of code that runs only when it is called.  
Functions help make code **organized**, **clean**, and **efficient**.

---

## ✅ Defining and Calling a Function

### Syntax:
```python
def function_name():
    # code to execute
```

Example:
```python
def say_hello():
    print("Hello Python!")

say_hello()   # Calling the function
```
Output:
```python
Hello Python!
```

## 🎁 Functions with Parameters
Parameters allow you to send data into the function.
```python
def greet(name):
    print(f"Hello {name}!")

greet("Amr")
```
Output:
```
Hello Amr!
```

## 🎚️ Default Parameter Value
```python
def welcome(country="Egypt"):
    print(f"Welcome from {country}")

welcome()            # Uses default value
welcome("Morocco")   # Uses given value
```
Output:
```python
Welcome from Egypt
Welcome from Morocco
```

## 🔄 Function with Return Value
return is used to send result back.
```python
def add(a, b):
    return a + b

result = add(5, 3)
print(result)
```
Output:
```python
8
```

## 🧱 Multiple Return Values
```python
def operations(x, y):
    return x+y, x-y, x*y

a, b, c = operations(10, 5)
print(a, b, c)
```
Output:
```python
15 5 50
```

## 📦 Packing & Unpacking Arguments
*args → Multiple Positional Arguments
```python
def sum_all(*numbers):
    return sum(numbers)

print(sum_all(1,2,3,4,5))   # 15
```
**kwargs → Multiple Named Arguments
```python
def display_info(**info):
    print(info)

display_info(name="Amr", age=20)
```
Output:
```python
{'name': 'Amr', 'age': 20}
```

## 🧾 Summary Table
| Concept            | Description                   | Example       | Result                  |
| ------------------ | ----------------------------- | ------------- | ----------------------- |
| `def`              | Define a function             | `def f():`    | Creates function        |
| Calling a function | Execute function code         | `f()`         | Runs function           |
| Parameter          | Input variable                | `def f(x):`   | `x` receives value      |
| Default Parameter  | Parameter with fallback value | `def f(x=5)`  | Used if no value passed |
| `return`           | Send result back              | `return x+y`  | Returns value           |
| Multiple Returns   | Return many values            | `return a, b` | Tuple output            |
| `*args`            | Accept many values            | `*numbers`    | Tuple of values         |
| `**kwargs`         | Accept many named values      | `**info`      | Dict of values          |
