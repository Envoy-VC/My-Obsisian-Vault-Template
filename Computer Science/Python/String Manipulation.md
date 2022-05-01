---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**::string manipulation 

---

## Manipulating Strings

### Escape Characters

| Escape character | Prints as            |
| ---------------- | -------------------- |
| `\'`             | Single quote         |
| `\"`             | Double quote         |
| `\t`             | Tab                  |
| `\n`             | Newline (line break) |
| `\\`             | Backslash            |

Example:

```python
>>> print("Hello there!\nHow are you?\nI\'m doing fine.")
Hello there!
How are you?
I'm doing fine.
```

---

### Raw Strings

A raw string completely ignores all escape characters and prints any backslash that appears in the string.

```python
>>> print(r'That is Carol\'s cat.')
That is Carol\'s cat.
```

Note: mostly used for regular expression definition (see `re` package)

---

### Multiline Strings with Triple Quotes

```python
>>> print('''Dear Alice,
>>>
>>> Eve's cat has been arrested for catnapping, cat burglary, and extortion.
>>>
>>> Sincerely,
>>> Bob''')
Dear Alice,

Eve's cat has been arrested for catnapping, cat burglary, and extortion.

Sincerely,
Bob
```

To keep a nicer flow in your code, you can use the `dedent` function from the `textwrap` standard package.

```python
>>> from textwrap import dedent
>>>
>>> def my_function():
>>>     print('''
>>>         Dear Alice,
>>>
>>>         Eve's cat has been arrested for catnapping, cat burglary, and extortion.
>>>
>>>         Sincerely,
>>>         Bob
>>>         ''').strip()
```

This generates the same string than before.

---

### Indexing and Slicing Strings


```python
>>> spam = 'Hello world!'

>>> spam[0]
'H'
```

```python
>>> spam[4]
'o'
```

```python
>>> spam[-1]
'!'
```

Slicing:

```python

>>> spam[0:5]
'Hello'
```

```python
>>> spam[:5]
'Hello'
```

```python
>>> spam[6:]
'world!'
```

```python
>>> spam[6:-1]
'world'
```

```python
>>> spam[:-1]
'Hello world'
```

```python
>>> spam[::-1]
'!dlrow olleH'
```

```python
>>> spam = 'Hello world!'
>>> fizz = spam[0:5]
>>> fizz
'Hello'
```

---

### The in and not in Operators with Strings

```python
>>> 'Hello' in 'Hello World'
True
```

```python
>>> 'Hello' in 'Hello'
True
```

```python
>>> 'HELLO' in 'Hello World'
False
```

```python
>>> '' in 'spam'
True
```

```python
>>> 'cats' not in 'cats and dogs'
False
```

---

### The in and not in Operators with list

```python
>>> a = [1, 2, 3, 4]
>>> 5 in a
False
```

```python
>>> 2 in a
True
```

---

### The upper(), lower(), isupper(), and islower() String Methods

`upper()` and `lower()`:

```python
>>> spam = 'Hello world!'
>>> spam = spam.upper()
>>> spam
'HELLO WORLD!'
```

```python
>>> spam = spam.lower()
>>> spam
'hello world!'
```

isupper() and islower():

```python
>>> spam = 'Hello world!'
>>> spam.islower()
False
```

```python
>>> spam.isupper()
False
```

```python
>>> 'HELLO'.isupper()
True
```

```python
>>> 'abc12345'.islower()
True
```

```python
>>> '12345'.islower()
False
```

```python
>>> '12345'.isupper()
False
```

---

### The isX String Methods

- **isalpha()** returns True if the string consists only of letters and is not blank.
- **isalnum()** returns True if the string consists only of letters and numbers and is not blank.
- **isdecimal()** returns True if the string consists only of numeric characters and is not blank.
- **isspace()** returns True if the string consists only of spaces,tabs, and new-lines and is not blank.
- **istitle()** returns True if the string consists only of words that begin with an uppercase letter followed by only lowercase letters.

---

### The startswith() and endswith() String Methods

```python
>>> 'Hello world!'.startswith('Hello')
True
```

```python
>>> 'Hello world!'.endswith('world!')
True
```

```python
>>> 'abc123'.startswith('abcdef')
False
```

```python
>>> 'abc123'.endswith('12')
False
```

```python
>>> 'Hello world!'.startswith('Hello world!')
True
```

```python
>>> 'Hello world!'.endswith('Hello world!')
True
```

---

### The join() and split() String Methods

join():

```python
>>> ', '.join(['cats', 'rats', 'bats'])
'cats, rats, bats'
```

```python
>>> ' '.join(['My', 'name', 'is', 'Simon'])
'My name is Simon'
```

```python
>>> 'ABC'.join(['My', 'name', 'is', 'Simon'])
'MyABCnameABCisABCSimon'
```

split():

```python
>>> 'My name is Simon'.split()
['My', 'name', 'is', 'Simon']
```

```python
>>> 'MyABCnameABCisABCSimon'.split('ABC')
['My', 'name', 'is', 'Simon']
```

```python
>>> 'My name is Simon'.split('m')
['My na', 'e is Si', 'on']
```

---

### Justifying Text with rjust(), ljust(), and center()

rjust() and ljust():

```python
>>> 'Hello'.rjust(10)
'     Hello'
```

```python
>>> 'Hello'.rjust(20)
'               Hello'
```

```python
>>> 'Hello World'.rjust(20)
'         Hello World'
```

```python
>>> 'Hello'.ljust(10)
'Hello     '
```

An optional second argument to rjust() and ljust() will specify a fill character other than a space character. Enter the following into the interactive shell:

```python
>>> 'Hello'.rjust(20, '*')
'***************Hello'
```

```python
>>> 'Hello'.ljust(20, '-')
'Hello---------------'
```

center():

```python
>>> 'Hello'.center(20)
'       Hello       '
```

```python
>>> 'Hello'.center(20, '=')
'=======Hello========'
```

---

### Removing Whitespace with strip(), rstrip(), and lstrip()

```python
>>> spam = '    Hello World     '
>>> spam.strip()
'Hello World'
```

```python
>>> spam.lstrip()
'Hello World '
```

```python
>>> spam.rstrip()
'    Hello World'
```

```python
>>> spam = 'SpamSpamBaconSpamEggsSpamSpam'
>>> spam.strip('ampS')
'BaconSpamEggs'
```

---

### Copying and Pasting Strings with the pyperclip Module (need pip install)

```python
>>> import pyperclip

>>> pyperclip.copy('Hello world!')

>>> pyperclip.paste()
'Hello world!'
```

---
---
