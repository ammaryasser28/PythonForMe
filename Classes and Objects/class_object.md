# 🏷️ Python Classes & Objects

## 🎯 Introduction
Python is an **object-oriented programming (OOP)** language.  
Classes and objects are the **core concepts** of OOP in Python.

- **Class:** A blueprint for creating objects.  
- **Object:** An instance of a class.

---

## 🧱 1️⃣ Classes & Objects

### Creating a Class

```python
class Person:
    # Class attribute
    species = "Human"

    # Constructor
    def __init__(self, name, age):
        self.name = name
        self.age = age

# Creating objects
person1 = Person("Alice", 25)
person2 = Person("Bob", 30)

print(person1.name)  # Alice
print(person2.age)   # 30
print(person1.species)  # Human
```
💡 self refers to the instance of the class and is used to access attributes and methods.

## 🧩 2️⃣ Class Functions (Methods)
Instance Methods
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    # Instance method
    def greet(self):
        print(f"Hello, my name is {self.name} and I am {self.age} years old.")

person = Person("Alice", 25)
person.greet()
```
🖥️ Output:
```python
Hello, my name is Alice and I am 25 years old.
```
Class Methods
```python
class Person:
    species = "Human"

    @classmethod
    def show_species(cls):
        print(f"All persons are {cls.species}")

Person.show_species()
```
🖥️ Output:
```python
All persons are Human
```
Static Methods
```python
class Math:
    @staticmethod
    def add(a, b):
        return a + b

print(Math.add(5, 3))  # 8
```
💡 Static methods do not use self or cls and behave like normal functions inside a class.

## 🧱 3️⃣ Class Inheritance
Inheritance allows a class (child) to inherit attributes and methods from another class (parent).
```python
# Parent class
class Person:
    def __init__(self, name):
        self.name = name

    def greet(self):
        print(f"Hello, my name is {self.name}")

# Child class
class Student(Person):
    def __init__(self, name, student_id):
        super().__init__(name)  # Call parent constructor
        self.student_id = student_id

    def show_id(self):
        print(f"My student ID is {self.student_id}")

# Create object
s1 = Student("Alice", "S123")
s1.greet()      # Inherited method
s1.show_id()    # Child method
```
🖥️ Output:
```python
Hello, my name is Alice
My student ID is S123
```

## 🧾 Summary Table
| Concept         | Description                 | Example                    | Output                |
| --------------- | --------------------------- | -------------------------- | --------------------- |
| Class           | Blueprint for objects       | `class Person:`            | -                     |
| Object          | Instance of class           | `p = Person()`             | -                     |
| `__init__`      | Constructor method          | `def __init__(self, name)` | Sets attributes       |
| Instance Method | Works on object             | `def greet(self)`          | Access object data    |
| Class Method    | Works on class              | `@classmethod`             | Access class data     |
| Static Method   | Independent of object/class | `@staticmethod`            | Like normal function  |
| Inheritance     | Child class inherits parent | `class Student(Person)`    | Access parent methods |
| `super()`       | Call parent methods         | `super().__init__()`       | Initialize parent     |

