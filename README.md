# hunt-patch

patch.c at hunt/, hunt.c and otto.c at hunt/hunt.


## patch.h

Included by **otto.c**.

Some defination like `sigblock`, `sigmask`, etc, are added here.

These code are copyed from **glibc**.


## hunt.c

Add check `ip->ifa_broadaddr` against `NULL`.


## otto.c

Include ../patch.h.


# TODO    <del>TO DEBUG</del>

`hunt: sendto: Network is unreachable`
