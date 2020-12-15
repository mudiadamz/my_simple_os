# The SIMPLE KERNEL

I tried to build my own simple operating system from scratch, thanks to Osdev (https://wiki.osdev.org/Bare_Bones), with its thorough explanation, the instruction is very very clear and up to date, i can follow and able for the first time, after several attempts trying to develop an OS and always failed even just to compile, this is my first OS from scratch that actually works and output something on a window.

## How to build and Run

```
./build.sh
qemu-system-i386 -kernel myos.bin
```

## Why Windows Subsystem for Linux
Because I have been using Windows for quite a number of years, I have tried using several Linux distros, but don't get the appeal, especially with the HiDPI display on my laptop, every Linux distros fonts just very small.

This code is built on WSL which is actually 100% pure Linux (probably), i am using windows as main computer because it's better, for text editing, etc. But for compilation it runs on WSL Debian.

## Thanks to
- The OSDEV https://wiki.osdev.org/Bare_Bones
- And i wrote a blog about it here https://www.techgalery.com/2020/12/how-to-build-simple-os-using-windows.html
