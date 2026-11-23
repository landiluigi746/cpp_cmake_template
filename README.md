# C++ CMake Project Template

This is a small C++ template that uses CMake as build system and vcpkg as dependency manager.
It also provides already defined formatting rules with clang-format.

## Dependencies

To use this template you need:

- a C++ compiler (C++23 is the standard used by default, you can change it in the [CMake config](CMakeLists.txt))
- CMake (3.16+)
- vcpkg
- clang-format (optional, used to format code)

## Getting started

To get started with this template, either clone it or generate a new repo from this one.
Then, create a `.env` file with env variables (see an example configuration [here](.env.sample)).

To prepare the local environment (CMake build files), run the following command:

```bash
cmake --preset=<preset> # preset can be debug or release
```

Then, to compile the project run:

```bash
# use --parallel $(nproc) to compile using all cores
cmake --build build-<preset> # preset can be debug or release
```
