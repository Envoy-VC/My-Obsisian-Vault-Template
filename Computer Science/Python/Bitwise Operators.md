---
banner: ""
banner_icon: 
---

---
**Tags**:: #python
**Links**::[[🐍 Python]]
**Description**:: Bitwise AND OR XOR

---

# Bitwise Operators
| Operator  | Description         | Syntax     |
| --------- | ------------------- | ---------- |
| &         | Bitwise AND         | `x & y`    |
| \|        | Bitwise OR          | `x \| y`   |
| ~         | Bitwise NOT         |  `x ~ y`   |
| ^         | Bitwise XOR         | `x ^ y`    |
| >>        | Bitwise right shift |  `x>>`     |
| <<        | Bitwise left shift  |  `x<<`     |

  
Bitwise **AND** operator: Returns 1 if both the bits are 1 else 0.

```python

a = 10 = 1010 (Binary)

b = 4 =  0100 (Binary)

  

a & b = 1010

         &

        0100

      = 0000

      = 0 (Decimal)

```


Bitwise **or** operator: Returns 1 if either of the bit is 1 else 0.

```python

a = 10 = 1010 (Binary)

b = 4 =  0100 (Binary)

  

a | b = 1010

         |

        0100

      = 1110

      = 14 (Decimal)

```

Bitwise **not** operator: Returns one’s complement of the number.

```python

  

a = 10 = 1010 (Binary)

  

~a = ~1010

   = -(1010 + 1)

   = -(1011)

   = -11 (Decimal)

```


Bitwise **XOR** operator: Returns 1 if one of the bits is 1 and the other is 0 else returns false.

```python

a = 10 = 1010 (Binary)

b = 4 =  0100 (Binary)

  

a ^ b = 1010

         ^

        0100

      = 1110

      = 14 (Decimal)

```


**Shift Operators** -
These operators are used to shift the bits of a number left or right thereby multiplying or dividing the number by two respectively. They can be used when we have to multiply or divide a number by two.

**Bitwise right shift**: Shifts the bits of the number to the right and fills 0 on voids left( fills 1 in the case of a negative number) as a result. Similar effect as of dividing the number with some power of two.

```python

a = 10 = 0000 1010 (Binary)

a >> 1 = 0000 0101 = 5

  

Example 2:

a = -10 = 1111 0110 (Binary)

a >> 1 = 1111 1011 = -5

```

**Bitwise left shift**: Shifts the bits of the number to the left and fills 0 on voids right as a result. Similar effect as of multiplying the number with some power of two.

```python

a = 5 = 0000 0101 (Binary)

a << 1 = 0000 1010 = 10

a << 2 = 0001 0100 = 20

```

---
---

