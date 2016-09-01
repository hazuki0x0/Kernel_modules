#Kernel Modules
kernel module souce codes
* CPU governors
* I/O schedulers
* frandom
* zram(lz4,snappy)

This modules modified for Locked Bootloader's Kernel.

Using symsearch.ko for search address in kernel.

##How to build

Step 1: Build the kernel you want to create a module

Step 2: Rewrite in the Makefile

    KERNEL_DIR= <Your kernel source>
    CROSS_COMPILE= <Your gcc compiler>

Step 3: Make Modules

`$ make`
