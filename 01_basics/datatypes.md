# object Types / Data types

- Number: 1234, 3.14415, 3+4j, 0b111, Decimal(), Fraction()
  - Examples:
    - `1234` (int)
    - `3.14415` (float)
    - `3+4j` (complex)
    - `0b111` is binary literal for 7 (`int('0b111', 2) == 7`)
    - `from decimal import Decimal; Decimal('0.1')` for exact decimals
    - `from fractions import Fraction; Fraction(1, 3)` for rational numbers

- String: 'spam', "Bob's", b'a\x01c', u'sp\xc4m'
  - Examples:
    - `s = 'spam'`
    - `s[0] == 's'`
    - `"Bob's"` contains an apostrophe without escaping
    - `b'a\x01c'` is a bytes literal; `b'a\x01c'[0] == 97`
    - `f"Name: {name}"` is an f-string for interpolation

- List: [1,2,3], ['spam','eggs',100], []
  - Examples:
    - `lst = [1, 2, 3]`
    - `lst.append(4)` -> `[1, 2, 3, 4]`
    - `lst[0]` -> `1`
    - lists are mutable: `lst[0] = 10`

- Tuple: (1, 2, 3), ('a',)
  - Immutable ordered sequence: `(1,2) + (3,) == (1,2,3)`

- Dict: {'a': 1, 'b': 2}
  - Mapping type: `d = {'a':1}; d['a'] == 1; d.get('c', 0) == 0`

- Set: {1, 2, 3}
  - Unique unordered collection: `{1,2} | {2,3} == {1,2,3}`

- Bool/None: True, False, None
  - `isinstance(True, int)  # True` (bool is a subclass of int)

- Bytes/bytearray: b'data', bytearray(b'data')
  - Bytes are immutable; `bytearray` is mutable.

Quick REPL checks (copy-paste into Python):

```python
1234
3.14
(3+4j).imag
int('0b111', 2)

s = 'spam'
s[1]

lst = [1,2,3]
lst.append(4)

(1,2) + (3,)

d = {'a':1}
d['a']

{1,2} & {2,3}
```

End of quick inline examples.