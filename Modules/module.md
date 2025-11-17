# 📦 Python Modules

## 🎯 Introduction
A **module** in Python is simply a file that contains Python code  
(functions, variables, classes, etc.).  
Modules help you:
- Organize your code  
- Reuse functions  
- Split large projects into smaller files  
- Use built-in Python features

---

## 🧱 Creating Your Own Module

### ✔️ 1. Create a file named `mymodule.py`

```python
# mymodule.py

def say_hello(name):
    return f"Hello, {name}!"

x = 10
```

### ✔️ 2. Import the module in another file
```python
import mymodule

print(mymodule.say_hello("Amr"))
print(mymodule.x)
```
🖥️ Output:
```python
Hello, Amr!
10
```

### 📥 Importing From Modules
🔹 import module_name
```python
import math

print(math.sqrt(25))
```

🔹 from module_name import something
```python
from math import sqrt

print(sqrt(16))
```

🔹 Import Multiple Items
```python
from math import sin, cos, pi
```

🔹 Import Everything (NOT recommended)
```python
from math import *
```

### 📁 Using Aliases (as)
```python
import math as m

print(m.pi)
```

### 📦 Built-in Python Modules
🔹 math
```python
import math
print(math.floor(3.7))  
print(math.ceil(3.1))
```

🔹 random
```python
import random
print(random.randint(1, 5))
```

🔹 datetime
```python
import datetime
print(datetime.datetime.now())
```

🔹 os
```python
import os
print(os.getcwd())
```

🔹 sys
```python
import sys
print(sys.version)
```

### 🗂️ Package vs Module
| Term        | Meaning                                     |
| ----------- | ------------------------------------------- |
| **Module**  | A single Python file (`file.py`)            |
| **Package** | A folder containing modules + `__init__.py` |

### 📦 Installing External Modules (PIP)
✔️ Install
```python
pip install requests
```
✔️ Use
```python
import requests

r = requests.get("https://example.com")
print(r.status_code)
```

### 🧠 Why Use Modules?
| Benefit          | Description                  |
| ---------------- | ---------------------------- |
| Reusability      | Write once → use everywhere  |
| Organization     | Clean and readable project   |
| Avoid repetition | Reuse functions              |
| Scalability      | Large apps become manageable |

### 🧾 Summary Table
| Command/Concept        | Description             | Example                 |
| ---------------------- | ----------------------- | ----------------------- |
| `import module`        | Import full module      | `import math`           |
| `from module import x` | Import specific item    | `from math import pi`   |
| `as`                   | Give alias              | `import math as m`      |
| Custom module          | User-created `.py` file | `import mymodule`       |
| Package                | Folder + `__init__.py`  | `import package.module` |
| Install module         | External modules        | `pip install numpy`     |

