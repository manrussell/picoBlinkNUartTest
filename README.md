# picoBlinkNUartTest
Raspberry pi pico Blink and Uart Test on ubuntu 22.04 and VSCode

How to build...

Compiler that worked was:
    gcc-arm-none-eabi-9-2020-q2-update/bin/arm-none-eabi-gcc


$ mkdir build
$ cd build
$ cmake ..
$ make -j8

Leds should flash...

Serial output...
    Use VSCode's serial termianl or minicom...
    $ sudo minicom -D /dev/ttyACM0 -b 115200


Note the hardcoded path in setting.json and launch.json for OpenOcd, This was because 
I wanted to use the Rapberrypi pico's OpenOCD fork, but not install it globally in /usr/bin and break other OpenOCD builds
E.g. 
    1) path to openocd TCL
    2) path to openOcd

How to build OpenOCD...
...

Commandline version to runthe tools...
OpenOCD
GDB
