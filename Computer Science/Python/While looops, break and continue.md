---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**::while loops, break and continue

---

### while Loop Statements

```python
spam = 0
while spam < 5:
    print('Hello, world.')
    spam = spam + 1
```

---

### break Statements

If the execution reaches a break statement, it immediately exits the while loop’s clause:

```python
while True:
    print('Please type your name.')
    name = input()
    if name == 'your name':
        break
print('Thank you!')
```

---

### continue Statements

When the program execution reaches a continue statement, the program execution immediately jumps back to the start of the loop.

```python
while True:
    print('Who are you?')
    name = input()
    if name != 'Joe':
        continue
    print('Hello, Joe. What is the password? (It is a fish.)')
    password = input()
    if password == 'swordfish':
        break
print('Access granted.')
```

---
---
