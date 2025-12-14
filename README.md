# cpp-template
A C++ project template with CMake

Uses CPM for package management.

To build, use:

```cmake -S . -B build -G "[Compiler]"```

For tests, add: ```-DENABLE_TESTS=ON```
For benchmarks, add: ```-DENABLE_BENCHMARKS=ON```