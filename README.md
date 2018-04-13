# Porting of Hunt on Windows

Porting project of Hunt on Windows.

Hunt is a part of bsdgames, which could not be run on Windows.
So we make a porting using Cygwin and msys2.

See [bsdgames](https://packages.debian.org/wheezy/bsdgames).

## Instructions

### Get the source code

### Environments

You should have Cygwin on Windows or msys2 on Windows with the ``ncurses-devel`` lib.

### Apply patches

`patch -p0 < patch_file.patch`

### Make

Generate the makefile, then `make`.


## Run

First you should disable the network cards until only one of them is available, and then open hunt.exe via programs like mintty.exe.
