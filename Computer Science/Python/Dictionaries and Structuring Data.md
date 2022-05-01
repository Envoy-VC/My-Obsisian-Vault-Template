---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**::all about dictionaries

---

## Dictionaries and Structuring Data

Example Dictionary:

```python
myCat = {'size': 'fat', 'color': 'gray', 'disposition': 'loud'}
```

---

### The keys(), values(), and items() Methods

values():

```python
>>> spam = {'color': 'red', 'age': 42}
>>> for v in spam.values():
>>>     print(v)
red
42
```

keys():

```python
>>> for k in spam.keys():
>>>     print(k)
color
age
```

items():

```python
>>> for i in spam.items():
>>>     print(i)
('color', 'red')
('age', 42)
```

Using the keys(), values(), and items() methods, a for loop can iterate over the keys, values, or key-value pairs in a dictionary, respectively.

```python

>>> spam = {'color': 'red', 'age': 42}
>>>
>>> for k, v in spam.items():
>>>     print('Key: {} Value: {}'.format(k, str(v)))
Key: age Value: 42
Key: color Value: red
```

---

### Checking Whether a Key or Value Exists in a Dictionary

```python
>>> spam = {'name': 'Zophie', 'age': 7}
```

```python
>>> 'name' in spam.keys()
True
```

```python
>>> 'Zophie' in spam.values()
True
```

```python
>>> # You can omit the call to keys() when checking for a key
>>> 'color' in spam
False
```

```python
>>> 'color' not in spam
True
```

---

### The get() Method

Get has two parameters: key and default value if the key did not exist

```python
>>> picnic_items = {'apples': 5, 'cups': 2}

>>> 'I am bringing {} cups.'.format(str(picnic_items.get('cups', 0)))
'I am bringing 2 cups.'
```

```python
>>> 'I am bringing {} eggs.'.format(str(picnic_items.get('eggs', 0)))
'I am bringing 0 eggs.'
```

---

### The setdefault() Method

Let's consider this code:

```python
spam = {'name': 'Pooka', 'age': 5}

if 'color' not in spam:
    spam['color'] = 'black'
```

Using `setdefault` we could write the same code more succinctly:

```python
>>> spam = {'name': 'Pooka', 'age': 5}
>>> spam.setdefault('color', 'black')
'black'
```

```python
>>> spam
{'color': 'black', 'age': 5, 'name': 'Pooka'}
```

```python
>>> spam.setdefault('color', 'white')
'black'
```

```python
>>> spam
{'color': 'black', 'age': 5, 'name': 'Pooka'}
```

---

### Merge two dictionaries

```python
# in Python 3.5+:
>>> x = {'a': 1, 'b': 2}
>>> y = {'b': 3, 'c': 4}
>>> z = {**x, **y}
>>> z
{'c': 4, 'a': 1, 'b': 3}

# in Python 2.7
>>> z = dict(x, **y)
>>> z
{'c': 4, 'a': 1, 'b': 3}
```

---
---
