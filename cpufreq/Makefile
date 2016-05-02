KERNEL_DIR=
CROSS_COMPILE=

symsearch-y := search.o hijack.o
obj-m := symsearch.o powersuspend.o cpufreq_gov_msm.o cpufreq_hotplugx.o cpufreq_intelliactive.o cpufreq_intellimm.o cpufreq_lionheart.o cpufreq_pegasusq.o cpufreq_smartass2.o cpufreq_smartassH3.o cpufreq_smartassH3.boost.o cpufreq_smartmax.o cpufreq_wheatley.o 

PWD := $(shell pwd)

default:
	$(MAKE) ARCH=arm CROSS_COMPILE=$(CROSS_COMPILE) -C $(KERNEL_DIR) SUBDIRS=$(PWD) modules

clean:
	$(MAKE) -C $(KERNEL_DIR) SUBDIRS=$(PWD) clean
