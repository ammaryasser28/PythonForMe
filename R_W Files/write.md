# 📝 Python Writing Files

## 🎯 Introduction
In Python, you can **write data to files** using the built-in `open()` function along with file **modes**.  
Writing to files is essential for storing information permanently.

---

## 🧱 File Modes for Writing

| Mode | Description |
|------|-------------|
| `'w'` | Write mode → **creates a new file** or **overwrites** existing content |
| `'a'` | Append mode → **adds content** to the end of the file without deleting existing data |
| `'x'` | Exclusive creation → **creates a new file**, raises an error if it already exists |
| `'w+'` | Write & read → write and then read from the file |
| `'a+'` | Append & read → append and then read |

---

## 🔍 Writing to a File

```python
# Open a file in write mode
file = open("example.txt", "w")

# Write text to the file
file.write("Hello, Python!\n")
file.write("Writing files is easy.\n")

# Close the file
file.close()
```
🖥️ Result in example.txt:
```
Hello, Python!
Writing files is easy.
```
💡 Always close the file after writing to save changes.

## 🧩 Using with Statement (Recommended)
The with statement automatically closes the file after writing.
```
with open("example.txt", "w") as file:
    file.write("Python is powerful.\n")
    file.write("It makes file handling easy.\n")
```
🖥️ Result:
```
Python is powerful.
It makes file handling easy.
```

## 🧩 Appending to a File
```
with open("example.txt", "a") as file:
    file.write("Appending a new line.\n")
```
🖥️ Result (example.txt now contains):
```
Python is powerful.
It makes file handling easy.
Appending a new line.
```

## 🧩 Writing Multiple Lines
You can write a list of strings using writelines():
```
lines = ["Line 1\n", "Line 2\n", "Line 3\n"]

with open("example.txt", "w") as file:
    file.writelines(lines)
```
🖥️ Result:
```
Line 1
Line 2
Line 3
```
💡 Important: writelines() does not add newline characters automatically.

Include \n at the end of each line.

## 🧾 Summary Table
| Method                | Description                   | Example                          |
| --------------------- | ----------------------------- | -------------------------------- |
| `open(filename, 'w')` | Write mode → overwrite file   | `open("file.txt", "w")`          |
| `open(filename, 'a')` | Append mode → add at end      | `open("file.txt", "a")`          |
| `write()`             | Write text to file            | `file.write("Hello\n")`          |
| `writelines()`        | Write multiple lines          | `file.writelines(["a\n","b\n"])` |
| `close()`             | Close the file                | `file.close()`                   |
| `with open()`         | Automatically handles closing | `with open("f.txt","w") as f:`   |
