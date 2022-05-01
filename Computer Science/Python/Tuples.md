---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**::tuples ()

---

### Tuple Data Type

```python
>>> eggs = ('hello', 42, 0.5)
>>> eggs[0]
'hello'
```

```python
>>> eggs[1:3]
(42, 0.5)
```

```python
>>> len(eggs)
3
```

The main way that tuples are different from lists is that tuples, like strings, are immutable.

---

### Converting Types with the list() and tuple() Functions

```python
>>> tuple(['cat', 'dog', 5])
('cat', 'dog', 5)
```

```python
>>> list(('cat', 'dog', 5))
['cat', 'dog', 5]
```

```python
>>> list('hello')
['h', 'e', 'l', 'l', 'o']
```

---
---
