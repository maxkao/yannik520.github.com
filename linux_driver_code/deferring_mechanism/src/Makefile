obj-m := tasklet.o work_queue.o

KERNELDIR ?= /lib/modules/$(shell uname -r)/build
PWD := $(shell pwd)

default:
	$(MAKE) -C $(KERNELDIR) M=$(PWD) modules
clean:
	@rm -f *.ko *.mod.* *.o *.order *.symvers
