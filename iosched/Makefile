KERNEL_DIR=
CROSS_COMPILE=

obj-m := fiops-iosched.o sio-iosched.o sioplus-iosched.o vr-iosched.o zen-iosched.o

PWD := $(shell pwd)

default:
	$(MAKE) ARCH=arm CROSS_COMPILE=$(CROSS_COMPILE) -C $(KERNEL_DIR) SUBDIRS=$(PWD) modules

clean:
	$(MAKE) -C $(KERNEL_DIR) SUBDIRS=$(PWD) clean
