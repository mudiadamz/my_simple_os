# The SIMPLE KERNEL

I tried to build my own simple operating system from scratch, thanks to Osdev (https://wiki.osdev.org/Bare_Bones), with its thorough explanation, the instruction is very very clear and up to date, i can follow and able for the first time, after several attempts trying to develop an OS and always failed even just to compile, this is my first OS from scratch that actually works and output something on a window.

## How to build and Run

1. Build and Run the OS binary

```
./build.sh
# Copy myos.bin to your main Windows OS
# Make sure you have Qemu on your Windows, then run
qemu-system-i386 -kernel myos.bin
```

2. Run the cd rom version with Grub

To build a cd rom version, which you can actually run on a real machine (but don't it may erase your data!). To build cd rom format, first switch to the `cdrom` branch, then run the `build.sh`. To run on Qemu, do the same thing except run ISO format instead. And also you need to have grub utility on your WSL disto.

```
sudo apt install xorriso grub-pc-bin
./build.sh
# Copy myos.iso to your main Windows OS
# Make sure you have Qemu on your Windows, then run
qemu-system-i386 -cdrom myos.iso
```

## Why Windows Subsystem for Linux
Because I have been using Windows for quite a number of years, I have tried using several Linux distros, but don't get the appeal, especially with the HiDPI display on my laptop, every Linux destroys fonts just very small.

This code is built on WSL which is actually 100% pure Linux (probably), i am using windows as main computer because it's better, for text editing, etc. But for compilation it runs on WSL Debian.

## Thanks to
- The OSDEV https://wiki.osdev.org/Bare_Bones
- And i wrote a blog about it here https://www.techgalery.com/2020/12/how-to-build-simple-os-using-windows.html
