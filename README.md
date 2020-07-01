# Hello World Example

Starts a FreeRTOS task to print "Hello World"

Configure the development environment as indicated in https://docs.espressif.com/projects/esp8266-rtos-sdk/en/latest/get-started/

This is an example of a build:

<code>
make

Toolchain path: /hd/esp/xtensa-lx106-elf/bin/xtensa-lx106-elf-gcc
Toolchain version: crosstool-ng-1.22.0-100-ge567ec7
Compiler version: 5.2.0
Python requirements from /hd/esp/ESP8266_RTOS_SDK/requirements.txt are satisfied.
Project is not inside a git repository, or git repository has no commits
will not use 'git describe' to determine PROJECT_VER.
App "hello-world" version: 1
To flash all build output, run 'make flash' or:
python /hd/esp/ESP8266_RTOS_SDK/components/esptool_py/esptool/esptool.py --chip esp8266 --port /dev/ttyUSB0 --baud 115200 --before default_reset --after hard_reset write_flash -z --flash_mode dio --flash_freq 40m --flash_size 2MB 0x0 /hd/esp/hello_world/build/bootloader/bootloader.bin 0x10000 /hd/esp/hello_world/build/hello-world.bin 0x8000 /hd/esp/hello_world/build/partitions_singleapp.bin
</code>
