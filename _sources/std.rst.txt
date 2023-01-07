std
===

The main standard library that you probably want to include into your Porth program.

nth_argv
--------
Get nth argument. Accepts index as 'int'. Returns string as 'ptr'.
   signature: int -- ptr

cstrlen
-------
Get length of c-string. Accepts c-string as 'ptr'. Returns length as 'int'.
    signature: ptr -- int

cstreq
------
Compares two c-strings. Accepts c-string1 as 'ptr' c-string2 as 'ptr' respectively. Returns state as 'bool'.
    signature: ptr ptr -- bool

cstr-to-str
-----------
Converts c-string to string. Accepts c-string as 'ptr'. Returns string as 'int ptr'.
    signature: ptr -- int ptr

fputs
-----
Print the element on top of the stack in a free form to **formatter** and remove it from the stack.
    signature: int ptr int

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
