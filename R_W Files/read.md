# 📘 Python Reading Files

Working with files is an essential skill in Python.  
You often need to read data from text files, logs, configurations, or datasets.

Python makes this very easy using the built-in `open()` function.

---

## 🔹 1. The `open()` Function

Basic syntax:

```python
file = open("filename.txt", "mode")
```
Common Modes:
| Mode   | Description                                     |
| ------ | ----------------------------------------------- |
| `"r"`  | Read (default). File must exist.                |
| `"w"`  | Write. Creates file or overwrites existing one. |
| `"a"`  | Append. Adds to the end of the file.            |
| `"x"`  | Create file (error if exists).                  |
| `"rb"` | Read in binary mode.                            |
| `"rt"` | Read in text mode (default).                    |

##  🔹 2. Reading a File
- 👉 read()
Reads the whole file as one string.
```python
file = open("test.txt", "r")
content = file.read()
print(content)
file.close()
```

- 👉 readline()
Reads one line at a time.
```python
file = open("test.txt", "r")
line = file.readline()
print(line)
file.close()
```

- 👉 readlines()
Reads all lines and returns them as a list.
```python
file = open("test.txt", "r")
lines = file.readlines()
print(lines)
file.close()
```

## 🔹 3. Best Practice: Using with
Using with automatically closes the file for you.
```python
with open("test.txt", "r") as file:
    content = file.read()
    print(content)
```

## 🔹 4. Looping Through File Lines
Using a loop to read line-by-line:
```python
with open("data.txt", "r") as f:
    for line in f:
        print(line.strip())
```

## 🔹 5. Reading Binary Files (images, videos, etc.)
```python
with open("image.png", "rb") as file:
    data = file.read()
```

## 🔹 6. File Exists? (Optional Trick)
```python
import os

if os.path.exists("file.txt"):
    print("File found")
else:
    print("File does not exist")
```

## 🧾 Summary Table
| Method        | Meaning            | Returns         |
| ------------- | ------------------ | --------------- |
| `read()`      | Reads entire file  | String          |
| `readline()`  | Reads one line     | String          |
| `readlines()` | Reads all lines    | List of strings |
| `with open()` | Auto-handles close | Best practice   |


