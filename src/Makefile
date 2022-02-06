obj-m :=rkp-ipid.o xmurp-ua.o
KERNEL :=/usr/src/linux-headers-`uname -r`
PWD :=$(shell pwd)
modules :
	$(MAKE) -C $(KERNEL) M=$(PWD) modules
.PHONEY:clean
clean :
	rm -f *.o *.ko *.mod *.mod.c modules.order Module.symvers 
