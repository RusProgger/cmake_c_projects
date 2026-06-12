🇬🇧 # CMake C Project Template

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

``` 
project/
│
├── src/ # Source files (.c)
├── include/ # Header files (.h)
├── CMakeLists.txt
└── build/ # Generated build files (not tracked in git)

```

