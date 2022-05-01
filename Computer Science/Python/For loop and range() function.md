---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**::for loop, range() and for else

---

### for Loops and the range() Function

```python
>>> print('My name is')
>>> for i in range(5):
>>>     print('Jimmy Five Times ({})'.format(str(i)))
My name is
Jimmy Five Times (0)
Jimmy Five Times (1)
Jimmy Five Times (2)
Jimmy Five Times (3)
Jimmy Five Times (4)
```

The _range()_ function can also be called with three arguments. The first two arguments will be the start and stop values, and the third will be the step argument. The step is the amount that the variable is increased by after each iteration.

```python
>>> for i in range(0, 10, 2):
>>>    print(i)
0
2
4
6
8
```

You can even use a negative number for the step argument to make the for loop count down instead of up.

```python
>>> for i in range(5, -1, -1):
>>>     print(i)
5
4
3
2
1
0
```

---

### For else statement

This allows to specify a statement to execute in case of the full loop has been executed. Only
useful when a `break` condition can occur in the loop:

```python
>>> for i in [1, 2, 3, 4, 5]:
>>>    if i == 3:
>>>        break
>>> else:
>>>    print("only executed when no item of the list is equal to 3")
``` 
---
---
