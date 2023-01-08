std
===

The main standard library that you probably want to include into your Porth program.

nth_argv
--------
Get nth argument.
   - signature: int -- ptr

cstrlen
-------
Get length of c-string.
    signature: ptr -- int

cstreq
------
Compares two c-strings.
    signature: ptr ptr -- bool

cstr-to-str
-----------
Converts c-string to string.
    signature: ptr -- int ptr

fputs
-----
Print the element on top of the stack in a free form to **file descriptor* and remove it from the stack.
    signature: [string: int ptr] [fd: int]

puts
----
Print the element(string) on top of the stack in a free form to **stdout** and remove it from the stack.
    signature: int ptr

eputs
-----
Print the element(string) on top of the stack in a free form to **stderr** and remove it from the stack.
    signature: int ptr

Str.count
---------
TBD

Str.data
--------
TBD

@Str.count
----------
TBD

@Str.data
---------
TBD

!Str.count
----------
TBD

!Str.data
---------
TBD
