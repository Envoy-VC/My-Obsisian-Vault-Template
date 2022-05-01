---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**::Basic Functions

---

### The print() Function

```python
>>> print('Hello world!')

Hello world!

```

```python

>>> a = 1

>>> print('Hello world!', a)

Hello world! 1

```

---

### The input() Function

Example Code:

```python
>>> print('What is your name?')   # ask for their name

>>> myName = input()

>>> print('It is good to meet you, {}'.format(myName))

What is your name?

Al

It is good to meet you, Al

```

  ---

### The len() Function

Evaluates to the integer value of the number of characters in a string:

```python
>>> len('hello')

5
```

Note: test of emptiness of strings, lists, dictionary, etc., should **not** use len, but prefer direct

Boolean evaluation.

```python
>>> a = [1, 2, 3]

>>> if a:

>>>     print("the list is not empty!")
```

---

### The str(), int(), and float() Functions

Integer to String or Float:

```python
>>> str(29)

'29'
```

```python
>>> print('I am {} years old.'.format(str(29)))

I am 29 years old.
```

```python
>>> str(-3.14)

'-3.14'
```

Float to Integer:

```python
>>> int(7.7)

7
```

```python
>>> int(7.7) + 1

8
```

---
