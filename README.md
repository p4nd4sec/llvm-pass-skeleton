# llvm-pass-skeleton

A completely useless LLVM pass.
It's for LLVM 17.

Build:

    $ cd llvm-pass-skeleton
    $ mkdir build
    $ cd build
    $ cmake ..
    $ make
    $ cd ..
    
Add environtment variables:

    $ LLVM_DIR=`llvm build path`/lib/cmake/llvm cmake ..
    
Run:

    $ clang -fpass-plugin=`echo build/skeleton/SkeletonPass.*` something.c
