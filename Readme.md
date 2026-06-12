# 🇬🇧  CMake C Project Template

This is a modern and reusable CMake template for C projects. It is designed to provide a clean and scalable starting point for developing C applications.

## Features

- Modern CMake structure
- C language support (C11 by default)
- Easy switch between C standards (C99, C11, C17)
- Strict compiler warnings enabled:
  - -Wall
  - -Wextra
  - -Wpedantic
- Clean project layout (src / include)
- Out-of-source build support (build directory separated from source)

## Project Structure

```bash
project/
│
├── src/ # Source files (.c)
├── include/ # Header files (.h)
├── CMakeLists.txt
└── build/ # Generated build files (not tracked in git)

```

## Build Instructions

```bash
cmake -S . -B build
cmake --build build

```

## Changing C Standard

By default, the project uses C11:

```bash
target_compile_features(target PRIVATE c_std_11)
```

You can change it to:

- C99 → c_std_99
- C11 → c_std_11
- C17 → c_std_17

