# dreal3-win
dReal solver v3.17 on Win10 Msys/MinGW-w64

More info:
https://github.com/dreal/dreal3


Binaries Usage:

Download and unzip dreal-3.17-mingw-w64-bin.zip

Run run.cmd

dreal smt2\nra\01.smt2

dreal smt2\nra\02.smt2

......


Build from source：

1.Install Required Toolchain

Msys2/MinGW-w64:

http://repo.msys2.org/distrib/x86_64/msys2-x86_64-20161025.exe

Code::Blocks:

http://sourceforge.net/projects/codeblocks/files/Binaries/17.12/Windows/codeblocks-17.12-setup.exe

2.Build Required Third Party Libraries

https://github.com/dreal-deps/ibex-lib

Patching:

https://github.com/ibex-team/ibex-lib/issues/306

Update:

The Waf build system is too old , need update to 1.9.1

https://waf.io/

Bulid:

/usr/bin/python2 ./waf configure --enable-shared --with-optim --with-affine --with-filib

/usr/bin/python2 ./waf install

3.Build dReal3 on Code::Blocks

Load the codeblocks projcets file from src/dreal/dreal.cbp

Build it.

