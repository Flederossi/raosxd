# raosxd
A tiny bootloader which prints the first three lines of the "Never gonna give you up" refrain.
It is written completely in the hex editor, using the full 512 bytes dedicated to him.

*Note: There is nothing more it can do.*

![Alt Text](https://github.com/Flederossi/raosxd/blob/main/assets/screenshot.png)

## Boot it using QEMU
First install https://www.qemu.org on your system, then run in the root folder:

`qemu-system-x86_64 image/boot.bin`

*Note: No compilation required :)*

## Source
If you are interested in how this thing works, you can use my hex dump https://github.com/Flederossi/tx to view the source code. ^^
