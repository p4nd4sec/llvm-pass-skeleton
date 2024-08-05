# llvm-pass-skeleton

A completely useless LLVM pass.
It's for LLVM 17.

## Build:
```sh
cd llvm-pass-skeleton
mkdir build
cd build
cmake ..
make
cd ..
```    
## Add environtment variables:
```sh
export LLVM_DIR=`llvm build path`/lib/cmake/llvm cmake ..
```
or
```sh
LLVM_DIR=`llvm build path`/lib/cmake/llvm cmake ..
```    
## Run:
```sh
clang -fpass-plugin=`echo build/skeleton/SkeletonPass.*` something.c
```

## Acknowledgments

* https://www.cs.cornell.edu/~asampson/blog/llvm.html
* https://polarply.medium.com/build-your-first-llvm-obfuscator-80d16583392b
