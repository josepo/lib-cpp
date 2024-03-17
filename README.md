# lib-cpp

Linking a shared library in C++

Folder `lib` includes a small C++ app that can be built into a shared library by doing:

```
$lib> g++ -c -shared hello.cpp -o libhello.so
```

To build the main program from the root folder:

```
$> g++ main.cpp -L./lib -lhello -o main
```
