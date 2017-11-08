# Porting of Hunt on Windows

Porting project of Hunt on Windows.

Hunt is a part of bsd-games, and it used to can be only run on Linux/Unix.
So we make a porting base on Cygwin and msys2.

## Instructions

### make

### Environments

You should have Cygwin on Windows or msys on Windows with the ``ncurses`` lib.

### Make

Just get into the root directory of this repo and type `make`.

## Contents

patch.c at hunt/, hunt.c and otto.c at hunt/hunt.


## patch.h

Included by **otto.c**.

Some defination like `sigblock`, `sigmask`, etc, are added here.

These code are copyed from **glibc**.


## hunt.c

Add check `ip->ifa_broadaddr` against `NULL`.


## otto.c

Include ../patch.h.
