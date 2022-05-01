---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**::all about lists in python

---

## Lists

```python
>>> spam = ['cat', 'bat', 'rat', 'elephant']

>>> spam
['cat', 'bat', 'rat', 'elephant']
```

---

### Getting Individual Values in a List with Indexes

```python
>>> spam = ['cat', 'bat', 'rat', 'elephant']
>>> spam[0]
'cat'
```

```python
>>> spam[1]
'bat'
```

```python
>>> spam[2]
'rat'
```

```python
>>> spam[3]
'elephant'
```

---

### Negative Indexes

```python
>>> spam = ['cat', 'bat', 'rat', 'elephant']
>>> spam[-1]
'elephant'
```

```python
>>> spam[-3]
'bat'
```

```python
>>> 'The {} is afraid of the {}.'.format(spam[-1], spam[-3])
'The elephant is afraid of the bat.'
```

---

### Getting Sub lists with Slices

```python
>>> spam = ['cat', 'bat', 'rat', 'elephant']
>>> spam[0:4]
['cat', 'bat', 'rat', 'elephant']
```

```python
>>> spam[1:3]
['bat', 'rat']
```

```python
>>> spam[0:-1]
['cat', 'bat', 'rat']
```

```python
>>> spam = ['cat', 'bat', 'rat', 'elephant']
>>> spam[:2]
['cat', 'bat']
```

```python
>>> spam[1:]
['bat', 'rat', 'elephant']
```

Slicing the complete list will perform a copy:

```python
>>> spam2 = spam[:]
['cat', 'bat', 'rat', 'elephant']
>>> spam.append('dog')
>>> spam
['cat', 'bat', 'rat', 'elephant', 'dog']
>>> spam2
['cat', 'bat', 'rat', 'elephant']
```

---

### Getting a List’s Length with len()

```python
>>> spam = ['cat', 'dog', 'moose']
>>> len(spam)
3
```

---

### Changing Values in a List with Indexes

```python
>>> spam = ['cat', 'bat', 'rat', 'elephant']
>>> spam[1] = 'aardvark'

>>> spam
['cat', 'aardvark', 'rat', 'elephant']

>>> spam[2] = spam[1]

>>> spam
['cat', 'aardvark', 'aardvark', 'elephant']

>>> spam[-1] = 12345

>>> spam
['cat', 'aardvark', 'aardvark', 12345]
```

---

### List Concatenation and List Replication

```python
>>> [1, 2, 3] + ['A', 'B', 'C']
[1, 2, 3, 'A', 'B', 'C']

>>> ['X', 'Y', 'Z'] * 3
['X', 'Y', 'Z', 'X', 'Y', 'Z', 'X', 'Y', 'Z']

>>> spam = [1, 2, 3]

>>> spam = spam + ['A', 'B', 'C']

>>> spam
[1, 2, 3, 'A', 'B', 'C']
```

---

### Removing Values from Lists with del Statements

```python
>>> spam = ['cat', 'bat', 'rat', 'elephant']
>>> del spam[2]
>>> spam
['cat', 'bat', 'elephant']
```

```python
>>> del spam[2]
>>> spam
['cat', 'bat']
```

---

### Using for Loops with Lists

```python
>>> supplies = ['pens', 'staplers', 'flame-throwers', 'binders']
>>> for i, supply in enumerate(supplies):
>>>     print('Index {} in supplies is: {}'.format(str(i), supply))
Index 0 in supplies is: pens
Index 1 in supplies is: staplers
Index 2 in supplies is: flame-throwers
Index 3 in supplies is: binders
```

---

### Looping Through Multiple Lists with zip()

```python
>>> name = ['Pete', 'John', 'Elizabeth']
>>> age = [6, 23, 44]
>>> for n, a in zip(name, age):
>>>     print('{} is {} years old'.format(n, a))
Pete is 6 years old
John is 23 years old
Elizabeth is 44 years old
```

### The in and not in Operators

```python
>>> 'howdy' in ['hello', 'hi', 'howdy', 'heyas']
True
```

```python
>>> spam = ['hello', 'hi', 'howdy', 'heyas']
>>> 'cat' in spam
False
```

```python
>>> 'howdy' not in spam
False
```

```python
>>> 'cat' not in spam
True
```

---

### The Multiple Assignment Trick

The multiple assignment trick is a shortcut that lets you assign multiple variables with the values in a list in one line of code. So instead of doing this:

```python
>>> cat = ['fat', 'orange', 'loud']

>>> size = cat[0]

>>> color = cat[1]

>>> disposition = cat[2]
```

You could type this line of code:

```python
>>> cat = ['fat', 'orange', 'loud']

>>> size, color, disposition = cat
```

The multiple assignment trick can also be used to swap the values in two variables:

```python
>>> a, b = 'Alice', 'Bob'
>>> a, b = b, a
>>> print(a)
'Bob'
```

```python
>>> print(b)
'Alice'
```

---

### Augmented Assignment Operators

| Operator    | Equivalent        |
| ----------- | ----------------- |
| `spam += 1` | `spam = spam + 1` |
| `spam -= 1` | `spam = spam - 1` |
| `spam *= 1` | `spam = spam * 1` |
| `spam /= 1` | `spam = spam / 1` |
| `spam %= 1` | `spam = spam % 1` |

Examples:

```python
>>> spam = 'Hello'
>>> spam += ' world!'
>>> spam
'Hello world!'

>>> bacon = ['Zophie']
>>> bacon *= 3
>>> bacon
['Zophie', 'Zophie', 'Zophie']
```

---

### Finding a Value in a List with the index() Method

```python
>>> spam = ['Zophie', 'Pooka', 'Fat-tail', 'Pooka']

>>> spam.index('Pooka')
1
```

---

### Adding Values to Lists with the append() and insert() Methods

**append()**:

```python
>>> spam = ['cat', 'dog', 'bat']

>>> spam.append('moose')

>>> spam
['cat', 'dog', 'bat', 'moose']
```

**insert()**:

```python
>>> spam = ['cat', 'dog', 'bat']

>>> spam.insert(1, 'chicken')

>>> spam
['cat', 'chicken', 'dog', 'bat']
```

---

### Removing Values from Lists with remove()

```python
>>> spam = ['cat', 'bat', 'rat', 'elephant']

>>> spam.remove('bat')

>>> spam
['cat', 'rat', 'elephant']
```

If the value appears multiple times in the list, only the first instance of the value will be removed.

---

### Removing Values from Lists with pop()

```python
>>> spam = ['cat', 'bat', 'rat', 'elephant']

>>> spam.pop()
'elephant'

>>> spam
['cat', 'bat', 'rat']

>>> spam.pop(0)
'cat'

>>> spam
['bat', 'rat']
```

---

### Sorting the Values in a List with the sort() Method

```python
>>> spam = [2, 5, 3.14, 1, -7]
>>> spam.sort()
>>> spam
[-7, 1, 2, 3.14, 5]
```

```python
>>> spam = ['ants', 'cats', 'dogs', 'badgers', 'elephants']
>>> spam.sort()
>>> spam
['ants', 'badgers', 'cats', 'dogs', 'elephants']
```

You can also pass True for the reverse keyword argument to have sort() sort the values in reverse order:

```python
>>> spam.sort(reverse=True)
>>> spam
['elephants', 'dogs', 'cats', 'badgers', 'ants']
```

If you need to sort the values in regular alphabetical order, pass str. lower for the key keyword argument in the sort() method call:

```python
>>> spam = ['a', 'z', 'A', 'Z']
>>> spam.sort(key=str.lower)
>>> spam
['a', 'A', 'z', 'Z']
```

You can use the built-in function `sorted` to return a new list:

```python
>>> spam = ['ants', 'cats', 'dogs', 'badgers', 'elephants']
>>> sorted(spam)
['ants', 'badgers', 'cats', 'dogs', 'elephants']
```

---
---