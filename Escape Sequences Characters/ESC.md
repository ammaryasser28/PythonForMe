# 🔤 Escape Sequences Characters in Python

## 🎯 Introduction
**Escape Sequences** are special characters used inside strings to represent actions or symbols that are hard (or impossible) to type directly.

They **start with a backslash (`\`)** and are used to:
- Add new lines or tabs.
- Include special characters (like quotes or backslashes) inside strings.
- Control how text appears when printed.

---

## 🧠 Basic Syntax
```python
print("Hello\nWorld")
```
🖥️ Output:
```
Hello
World
```
Here, \n means new line → it tells Python to move to the next line.

## 🔡 Common Escape Characters
| Escape | Description                             | Example                            | Output                 |
| ------ | --------------------------------------- | ---------------------------------- | ---------------------- |
| `\\`   | Backslash                               | `print("This is a backslash: \\")` | This is a backslash: \ |
| `\'`   | Single quote                            | `print('It\'s Python!')`           | It's Python!           |
| `\"`   | Double quote                            | `print("He said \"Hello!\"")`      | He said "Hello!"       |
| `\n`   | New line                                | `print("Line1\nLine2")`            | Line1<br>Line2         |
| `\t`   | Tab (adds spaces)                       | `print("Name:\tAmr")`              | Name: Amr              |
| `\r`   | Carriage return (moves cursor to start) | `print("12345\rHi")`               | Hi345                  |
| `\b`   | Backspace (deletes previous character)  | `print("Helloo\b")`                | Hello                  |
| `\f`   | Form feed (page break - rarely used)    | `print("Hello\fWorld")`            | HelloWorld            |
| `\v`   | Vertical tab (rarely used)              | `print("Hello\vWorld")`            | HelloWorld            |



