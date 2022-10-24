core
====

Core fundamental definitions of Porth that are used by all layers of abstraction. This stuff should just work regardless of the target platform.

@ptr
----
TBD

@@ptr
-----
TBD

@bool
-----
TBD

@int
----
TBD

@addr
-----
TBD

!ptr
----
TBD

!bool
-----
TBD

!int
----
TBD

!addr
-----
TBD

ptr+
----
TBD

ptr-
----
TBD

ptr!=
-----
TBD

ptr=
----
TBD

ptr<
----
TBD

+ptr
----
TBD

ptr-diff
--------
TBD

/ div
------
Division. Accepts number1 as 'int' number2 as 'int' respectively. Returns result as 'int'.
    signature: int int -- int

% mod
------
Modulus. Accepts number1 as 'int' number2 as 'int' respectively. Returns modulus as 'int'.
    signature: int int -- int

imod
----
IDIV modulus. Accepts number1 as 'int' number2 as 'int' respectively. Returns modulus as 'int'.
    signature: int int -- int

idiv
----
IDIV private. Accepts number1 as 'int' number2 as 'int' respectively. Returns private as 'int'.
    signature: int int -- int

emod
----
Sum of moduluses of 2 numbers. Accepts number1 as 'int' number2 as 'int' respectively. Returns sumofmods as 'int'.
    signature: int int -- int

lnot
----
Logical 'not'. Accepts logical as 'bool'. Returns 'bool'.
    signature: bool -- bool

land
----
Logical 'and'. Accepts logical1 as 'bool' logical2 as 'bool' respectively. Returns 'bool'.
    signature: bool bool -- bool

lor
---
Logical 'or'. Accepts logical1 as 'bool' logical2 as 'bool' respectively. Returns 'bool'.
    signature: bool bool -- bool

inc64-by
--------
Increment 64-bit int by value. Accepts int64 as 'ptr' incby as 'int' respectively.
    signature: ptr int

inc64
-----
Increment 64-bit int by 1. Accepts int64 as 'ptr'.
    signature: ptr
