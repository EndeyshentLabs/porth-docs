linux
=====

Linux specific definitions.

write
-----
Write(2) syscall wrapper.
    - signature: [fd: int] [buf: ptr] [count: int] -- [errno: int]


read
----
Read(2) syscall wrapper.
    - signature: [fd: int] [buf: ptr] [count: int] -- [errno: int]


openat
------
Openat(2) syscall wrapper.
    - signature: [dirfd: int] [pathname: int] [flags: ptr] [mode: int] -- [errno: int]


fstat
-----
Fstat(2) syscall wrapper.
    - signature: [statbuf: ptr] [fd: int] -- [errno: int]


stat
----
Stat(2) syscall wrapper.
    - signature: [pathname: ptr] [statbuf: ptr] -- [errno: int]


close
-----
Close(2) syscall wrapper.
    - signature: [fd: int] -- [errno: int]


exit
----
Exit(3) syscall wrapper.
    - signature: [status: int]


mmap
----
Mmap(2) syscall wrapper.
    - signature: [offset: int] [fd: int] [flags: int] [prot: int] [length: int] [addr: ptr] -- [errno: int]


clock_nanosleep
---------------
Clock_nanosleep(2) syscall wrapper.
    - signature: [remain: ptr] [request: ptr] [flags: int] [clockid: int] -- [errno: int]


clock_gettime
-------------
Clock_gettime(2) syscall wrapper.
    - signature: [clockid: ptr] [tp: int] -- [errno: int]


fork
----
Fork(2) syscall wrapper.
    - signature: -- [pid|errno: int]


getpid
------
Getpid(2) syscall wrapper.
    - signature: -- [pid: int]


execve
------
Execve(2) syscall wrapper.
    - signature: [envp: ptr] [argv: ptr] [pathname: ptr] -- [errno: int]


wait4
-----
Wait4(2) syscall wrapper.
    - signature: [rusage: ptr] [options: int] [wstatus: ptr] [pid: int] -- [pid|errno: int]


rename
------
Rename(2) syscall wrapper.
    - signature: [newpath: ptr] [oldpath: ptr] -- [errno: int]


fcntl
-----
Fcntl(2) syscall wrapper.
    - signature: [arg: int] [cmd: int] [fd: int] -- [errno: int]


kill
----
Kill(2) syscall wrapper.
    - signature: [sig: int] [pid: int] -- [errno: int]


dup2
----
Dup2(2) syscall wrapper.
    - signature: [newfd: int] [oldfd: int] -- [errno: int]


socket
------
Socket(2) syscall wrapper.
    - signature: [protocol: int] [type: int] [domain: int] -- [newfd|errno: int]


bind
----
Bind(2) syscall wrapper.
    - signature: [addrlen: int] [addr: ptr] [sockfd: int] -- [errno: int]


listen
------
Listen(2) syscall wrapper.
    - signature: [backlog: int] [sockfd: int] -- [errno: int]


accept
------
Accept(2) syscall wrapper.
    - signature: [addrlen: ptr] [addr: ptr] [sockfd: int] -- [newfd|errno: int]


getcwd
------
Getcwd(3) syscall wrapper.
    - signature: [size: int] [buf: ptr] -- [buf|errno: int]


chroot
------
Chroot(2) syscall wrapper.
    - signature: [path: ptr] -- [errno: int]


ioctl
-----
Ioctl(2) syscall wrapper.
    - signature: int [request: int] [fd: int] -- [errno: int]

WIFSTOPPED
----------
TBD



WIFCONTINUED
------------
TBD



WTERMSIG
--------
TBD


WIFEXITED
---------
TBD


WEXITSTATUS
-----------
TBD



isatty
------
Checks, is programm ran in terminal or not.
    - signature: [fd: int] -- [errno: int] [is a tty?: bool]
