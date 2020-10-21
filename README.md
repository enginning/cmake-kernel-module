A simple hello world kernel module, that can be build with cmake.
Utilize Kbuild through cmake, and do it in a build directory.


Usage:
1) clone it.
2) create a folder: mkdir build
3) navigate into build: cd build
4) run cmake: cmake ../
5) build it: make



Expected behavior: 

cmake ../ shall do:
```
$ cmake ../
-- The C compiler identification is GNU 9.2.1
-- Check for working C compiler: /usr/lib64/ccache/cc
-- Check for working C compiler: /usr/lib64/ccache/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Kernel release: 5.3.13-300.fc31.x86_64
-- Kernel headers: /usr/src/kernels/5.3.13-300.fc31.x86_64
-- Configuring done
-- Generating done
-- Build files have been written to: /home/ca/Code/cmake-kernel-module/build
```
make shall do:
```
make
Scanning dependencies of target driver
[100%] Generating hello.ko
[100%] Built target driver
```

Among others the hello.ko is now present. 


Thoughts and comments are welcome. 
