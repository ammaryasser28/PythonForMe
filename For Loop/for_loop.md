# 🔁 For Loop in Python

## 🎯 Introduction
A **for loop** in Python is used to **iterate (loop)** over a sequence such as a **list, tuple, string, dictionary, or range**.  
It executes a block of code **once for each item** in the sequence.

---

## 🧱 Syntax

```python
for variable in sequence:
    # code to execute
```
- variable → a name that takes each value from the sequence.
- sequence → the object you’re looping through (like a list or string).

## 🧩 Example 1 — Looping Through a List
```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
```
🖥️ Output:
```python
apple
banana
cherry
```
💡 The loop runs 3 times — once for each item in the list.

## 🧩 Example 2 — Looping Through a String
```python
for letter in "Python":
    print(letter)
```
🖥️ Output:
```python
P
y
t
h
o
n
```

## 🧩 Example 3 — Using range()
The range() function generates a sequence of numbers.
```python
for i in range(5):
    print(i)
```
🖥️ Output:
```python
0
1
2
3
4
```
💡 range(5) starts from 0 and goes up to 4 (not including 5).

## 🧮 Example 4 — Using Range with Start & End
``` python
for i in range(2, 6):
    print(i)
```
🖥️ Output:
```python
2
3
4
5
```
💡 The range starts at 2 and stops before 6.

## 🧩 Example 5 — Using break
Stops the loop immediately when a condition is met.
```python
for num in range(1, 6):
    if num == 4:
        break
    print(num)
```
🖥️ Output:
```python
1
2
3
```
💡 The loop stops when num == 4.

## 🧩 Example 6 — Using continue
Skips the current iteration and moves to the next one.
```python
for num in range(1, 6):
    if num == 3:
        continue
    print(num)
```
🖥️ Output:
```python
1
2
4
5
```
💡 When num == 3, Python skips the print statement.

## 🧩 Example 7 — Using else with a For Loop
The else block runs when the loop finishes normally (no break used).
```python
for i in range(3):
    print("Loop:", i)
else:
    print("Loop finished successfully!")
```
🖥️ Output:
```python
Loop: 0
Loop: 1
Loop: 2
Loop finished successfully!
```

## 🧩 Example 8 — Nested For Loops
You can use a for loop inside another for loop.
```python
for x in range(1, 4):
    for y in range(1, 3):
        print(f"({x}, {y})")
```
🖥️ Output:
```python
(1, 1)
(1, 2)
(2, 1)
(2, 2)
(3, 1)
(3, 2)
```

## 🧾 Summary Table
| Concept              | Description           | Example                      | Output              |
| -------------------- | --------------------- | ---------------------------- | ------------------- |
| Loop List            | Iterate through items | `for x in [1,2,3]: print(x)` | 1 2 3               |
| Loop String          | Iterate through chars | `for c in "Hi": print(c)`    | H i                 |
| Range                | Loop numbers          | `for i in range(5)`          | 0 → 4               |
| Range with Start/End | Custom range          | `range(2,6)`                 | 2 → 5               |
| Break                | Stop loop early       | `if i == 3: break`           | Stops               |
| Continue             | Skip one iteration    | `if i == 2: continue`        | Skips 2             |
| Else                 | Run when done         | `for...else:`                | Executes after loop |
| Nested Loop          | Loop inside loop      | `for x in... for y in...`    | Pair outputs        |


