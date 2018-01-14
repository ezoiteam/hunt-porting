# Porting of Hunt on Windows

Porting project of Hunt on Windows.

Hunt is a part of bsdgames, which could not be run on Windows.
So we make a porting using Cygwin and msys2.

See [bsdgames](https://packages.debian.org/wheezy/bsdgames).

## Instructions

### Get the source code

### Environments

You should have Cygwin on Windows or msys2 on Windows with the ``ncurses`` lib.

### Make

Just get into the root directory of this repo and type `make`.

## Contents

patch.c at hunt/, hunt.c and otto.c at hunt/hunt.


### patch.h

Included by **otto.c**.

Some definations like `sigblock`, `sigmask`, etc, are added here.

These code are copied from **glibc**.


### hunt.c

Add check `ip->ifa_broadaddr` against `NULL`.


### otto.c

Include ../patch.h.

## Run

First you should disable the network cards until only one of them is available, and then open hunt.exe via programs like mintty.exe.
