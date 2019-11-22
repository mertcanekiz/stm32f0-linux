# STM32F0 Blink

An example project for programming STM32F0 Discovery board on Linux using ARM GNU Toolchain.

### Dependencies
* [ARM GNU Toolchain](https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads) (`arm-none-eabi`)
* [CMake](https://cmake.org)

If you are on arch linux, you can use this command:
```
sudo pacman -S cmake arm-none-eabi-gcc arm-none-eabi-binutils arm-none-eabi-newlib arm-none-eabi-gdb
```

### How to build
You can either use the `Makefile` in the top level:
```
make
```
or you can use CMake:
```
mkdir build && cd build
cmake ..
make
```

Either option includes a `flash` target in order to download the program to the board:
```
make flash
```
