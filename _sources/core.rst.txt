core
====

Core fundamental definitions of Porth that are used by all layers of abstraction. This stuff should just work regardless of the target platform.

@ptr
----
Load a ptr.
    - signature: [place: ptr] -- [byte: ptr]


@@ptr
-----
Load a ptr to a ptr.
    - signature: [place: ptr] -- [byte: ptr]

..  +----------------------------------------------------------+
..  |                        warning::                         |
..  |           idk what f***ing magic this thing do           |
..  +----------------------------------------------------------+

@bool
-----
Load a bool.
    - signature: [place: ptr] -- [byte: bool]


@int
----
Load an int.
    - signature: [place: ptr] -- [byte: int]


@addr
-----
Load an addr.
    - signature: [place: ptr] -- [byte: addr]

.. note::
 addr - address of the procedure.


!ptr
----
Store a ptr.
    - signature: [byte: ptr] [place: ptr]


!bool
-----
Store a ptr.
    - signature: [byte: bool] [place: ptr]


!int
----
Store an int.
    - signature: [byte: int] [place: ptr]


!addr
-----
Store an addr. Accepts addr ptr respectively.
    - signature: [byte: addr] [place: ptr]


ptr+
----
Sums up ptr and int.
    - signature: ptr int -- ptr


ptr-
----
Subtracts int from ptr.
    - signature: ptr int -- ptr


ptr!=
-----
Not equal comparison.
    - signature: ptr ptr -- bool


ptr=
----
Equal comparison.
    - signature: ptr ptr -- bool


ptr<
----
Less than comparison.
    - signature: ptr ptr -- bool


+ptr
----
Sums up int and ptr.
    - signature: int ptr -- ptr


ptr-diff
--------
Difference between two pointers.
    - signature: ptr ptr -- int


/ div
------
Division.
    - signature: [a: int] [b: int] -- [a / b: int]


% mod
------
Modulus.
    - signature: [a: int] [b: int] -- [a % b: int]


imod
----
IDIV modulus.
    - signature: [a: int] [b: int] -- [a % b: int]


idiv
----
IDIV.
    - signature: [a: int] [b: int] -- [a / b: int]


emod
----
Sum of moduluses of 2 numbers.
    - signature: [a: int] [b: int] -- [(a % b) + (b % a): int]


lnot
----
Logical 'not'.
    - signature: bool -- bool


land
----
Logical 'and'.
    - signature: bool bool -- bool


lor
---
Logical 'or'.
    - signature: bool bool -- bool


inc64-by
--------
Increment 64-bit int by value.
    - signature: [int64: ptr] [b: int]


inc64
-----
Increment 64-bit int by 1.
    - signature: [int64: ptr]


dec64
-----
Decrement 64-bit int by 1.
    - signature: [int64: ptr]


inc32
-----
Increment 32-bit int by 1.
    - signature: [int32: ptr]


dec32
-----
Decrement 32-bit int by 1.
    - signature: [int32: ptr]


inc8
-----
Increment 8-bit int by 1.
    - signature: [int8: ptr]


dec8
-----
Decrement 8-bit int by 1. Accepts int8 as 'ptr'.
    - signature: [int8: ptr]


neg
---
Negate number.
    - signature: [a: int] -- [-a: int]


?null
-----
Null check.
    - signature: ptr -- bool


toggle
------
Toggles logical.
    - signature: [logical: ptr]
