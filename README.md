# llvm-ptr-hide
Code pointer hiding work based on LLVM 3.5.0 (and the jumptable support).

- Build:
```
mkdir build; cd build
cmake -G "Unix Makefiles" -DLLVM_TARGETS_TO_BUILD="X86" -DCMAKE_BUILD_TYPE=Release ../llvm-ptr-hide
make
```
- Usage:
```
../build/bin/clang -fcph *.c -o <target>
or
../build/bin/clang -fcph *.c -S
```
