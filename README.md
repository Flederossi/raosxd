# raosxd
A tiny bootloader that prints the first three lines of the "Never gonna give you up" refrain.

*It is written completely in the hex editor, using the full 512 bytes dedicated to him.*

## Boot it using QEMU
First install https://www.qemu.org on your system, then run in the root folder:

`qemu-system-x86_64 image/boot.bin`
