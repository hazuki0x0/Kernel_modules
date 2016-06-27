KERNEL_DIR=
CROSS_COMPILE=


obj-m := tcp_westwood.o

PWD := $(shell pwd)

default:
	$(MAKE) ARCH=arm CROSS_COMPILE=$(CROSS_COMPILE) -C $(KERNEL_DIR) SUBDIRS=$(PWD) modules

clean:
	$(MAKE) -C $(KERNEL_DIR) SUBDIRS=$(PWD) clean
