# raosxd
A tiny bootloader which prints the first three lines of the "Never gonna give you up" refrain.
It is written completely in the hex editor, using the full 512 bytes dedicated to him.

*Note: There is nothing more it can do.*

![Alt Text](https://github.com/Flederossi/raosxd/blob/main/assets/screenshot.png)

## Boot it using QEMU
First install [QEMU](https://www.qemu.org) on your system, then run in the root folder:

- 32 bit: 
```
qemu-system-i386 image/boot.bin
```
- 64 bit:
```
qemu-system-x86_64 image/boot.bin
```

*Note: No compilation required :)*

## Boot it on a real machine
To run it on real hardware there are two methods.
### Method 1 (Terminal):
Flash the binary to a USB stick by using dd:

- Linux: 
```
sudo dd if=image/boot.bin of=/dev/[your usb] bs=512 status=progress
```

**Important: Be sure you entered the right name of the usb you want the system to be on before executing this command. If you choose the wrong device your data could be damaged or wiped completely. I take no responsibility for loss of data, do it at your own risk. If you don't know what you are doing, I recommend using the qemu boot instead.**

Then select the USB in the boot menu to boot raosxd.

### Method 2 (GUI):
Flash the latest ISO image from the releases tab to a USB stick by using programs like [Balena Etcher](https://www.balena.io/etcher/) or [Rufus](https://rufus.ie/).

## Source Code
If you are interested in how this thing works, you can use my hex dump [tx](https://github.com/Flederossi/tx) or any other hex editor on the *boot.bin* file to view the code.

- tx:
```
tx image/boot.bin
```

## Credit: Rick Astley (singer of the song)
- YouTube: https://www.youtube.com/@RickAstleyYT
- Spotify: https://open.spotify.com/artist/0gxyHStUsqpMadRV0Di1Qt
- Twitter: https://twitter.com/rickastley
