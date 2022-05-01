---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**:: Boolean Operators , Evaluation and merging comparison and Boolean operators

---

### Boolean Operators

There are three Boolean operators: and, or, and not.

The _and_ Operator’s _Truth_ Table:

| Expression        | Evaluates to |
| ----------------- | ------------ |
| `True and True`   | `True`       |
| `True and False`  | `False`      |
| `False and True`  | `False`      |
| `False and False` | `False`      |

The _or_ Operator’s _Truth_ Table:

| Expression       | Evaluates to |
| ---------------- | ------------ |
| `True or True`   | `True`       |
| `True or False`  | `True`       |
| `False or True`  | `True`       |
| `False or False` | `False`      |

The _not_ Operator’s _Truth_ Table:

| Expression  | Evaluates to |
| ----------- | ------------ |
| `not True`  | `False`      |
| `not False` | `True`       |

---

### Boolean evaluation

Never use `==` or `!=` operator to evaluate boolean operation. Use the `is` or `is not` operators,
or use implicit boolean evaluation.

NO (even if they are valid Python):

```python
>>> True == True
True
```

```python
>>> True != False
True
```

YES (even if they are valid Python):

```python
>>> True is True
True
```

```python
>>> True is not False
True
```

These statements are equivalent:

```Python
>>> if a is True:
>>>    pass
>>> if a is not False:
>>>    pass
>>> if a:
>>>    pass
```

And these as well:

```Python
>>> if a is False:
>>>    pass
>>> if a is not True:
>>>    pass
>>> if not a:
>>>    pass
```

---

### Mixing Boolean and Comparison Operators

```python
>>> (4 < 5) and (5 < 6)
True
```

```python
>>> (4 < 5) and (9 < 6)
False
```

```python
>>> (1 == 2) or (2 == 2)
True
```

You can also use multiple Boolean operators in an expression, along with the comparison operators:

```python
>>> 2 + 2 == 4 and not 2 + 2 == 5 and 2 * 2 == 2 + 2
True
```