obj-m += hp-wmi.o

all:
	make -C /lib/modules/${kernelver}/build M=$(PWD) modules

clean:
	make -C /lib/modules/${kernelver}/build M=$(PWD) clean
