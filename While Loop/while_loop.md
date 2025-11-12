# 🔁 While Loop in Python

## 🎯 Introduction
A **while loop** in Python is used to **repeat a block of code** as long as a certain condition is **True**.  
It’s mainly used when you **don’t know beforehand** how many times the loop should run.

---

## 🧱 Syntax

```python
while condition:
    # code to execute
```
- The code inside the loop runs while the condition is True.
- When the condition becomes False, the loop stops.

## 🧩 Example 1 — Basic While Loop
```python
count = 1

while count <= 5:
    print("Count is:", count)
    count += 1
```
🖥️ Output:
```python
Count is: 1
Count is: 2
Count is: 3
Count is: 4
Count is: 5
```
💡 The loop runs 5 times because the condition count <= 5 is True until count becomes 6.

## ⚠️ Infinite Loop
If you forget to update the variable inside the loop, it will run forever.
```python
i = 1

while i <= 10:
    print(i)
    if i == 5:
        break
    i += 1
```
🖥️ Output:
```python
1
2
3
4
5
```
💡 The loop stops when i == 5 because of the break statement.

## 🧩 Example 3 — Using continue
continue skips the current iteration and goes to the next one.
```python
i = 0

while i < 5:
    i += 1
    if i == 3:
        continue
    print(i)
```
🖥️ Output:
```python
1
2
4
5
```
💡 When i == 3, Python skips the print() and continues to the next iteration.

## 🧩 Example 4 — While Loop with else
- The else block runs when the condition becomes False,
- unless the loop is exited using break.
```python
i = 1

while i <= 3:
    print("Number:", i)
    i += 1
else:
    print("Loop finished successfully!")
```
🖥️ Output:
```python
Number: 1
Number: 2
Number: 3
Loop finished successfully!
```

## 🧾 Summary Table
| Concept     | Description                            | Example                  | Output             |
| ----------- | -------------------------------------- | ------------------------ | ------------------ |
| Basic While | Runs while condition is True           | `while x < 5:`           | Repeats block      |
| Increment   | Update variable to avoid infinite loop | `x += 1`                 | Keeps loop safe    |
| `break`     | Stops loop immediately                 | `if x == 3: break`       | Loop ends early    |
| `continue`  | Skips one iteration                    | `if x == 2: continue`    | Skips printing 2   |
| `else`      | Runs after loop ends normally          | `while x < 3: ... else:` | Executes when done |

