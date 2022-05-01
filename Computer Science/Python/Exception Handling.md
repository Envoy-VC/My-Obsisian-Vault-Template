---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**::try , except and finally

---

## Exception Handling

### Basic exception handling

```python
>>> def spam(divideBy):
>>>     try:
>>>         return 42 / divideBy
>>>     except ZeroDivisionError as e:
>>>         print('Error: Invalid argument: {}'.format(e))
>>>
>>> print(spam(2))
>>> print(spam(12))
>>> print(spam(0))
>>> print(spam(1))
21.0
3.5
Error: Invalid argument: division by zero
None
42.0
```

---

### Final code in exception handling

Code inside the `finally` section is always executed, no matter if an exception has been raised or
not, and even if an exception is not caught.

```python
>>> def spam(divideBy):
>>>     try:
>>>         return 42 / divideBy
>>>     except ZeroDivisionError as e:
>>>         print('Error: Invalid argument: {}'.format(e))
>>>     finally:
>>>         print("-- division finished --")
>>> print(spam(2))
-- division finished --
21.0
>>> print(spam(12))
-- division finished --
3.5
>>> print(spam(0))
Error: Invalid Argument division by zero
-- division finished --
None
>>> print(spam(1))
-- division finished --
42.0
```

---
---
