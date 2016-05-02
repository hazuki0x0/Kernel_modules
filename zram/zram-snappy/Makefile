KERNEL_DIR=/opt/9.2.A.0.295/kernel
CROSS_COMPILE=/opt/arm-2013.11/bin/arm-none-linux-gnueabi-

zram-y	:=	zram_drv.o zram_sysfs.o
zsmalloc-y 		:= zsmalloc-main.o
snappy_compress-objs := csnappy_compress.o
snappy_decompress-objs := csnappy_decompress.o
obj-m := zram.o zsmalloc.o csnappy_compress.o csnappy_decompress.o

PWD := $(shell pwd)

default:
	$(MAKE) ARCH=arm CROSS_COMPILE=$(CROSS_COMPILE) -C $(KERNEL_DIR) SUBDIRS=$(PWD) modules

clean:
	$(MAKE) -C $(KERNEL_DIR) SUBDIRS=$(PWD) clean
