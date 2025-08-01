snd-hda-codec-realtek-objs := patch_realtek.o
obj-m += snd-hda-codec-realtek.o

ccflags-y := -I$(PWD)/inc

all:
	make -C /lib/modules/${kernelver}/build M=$(PWD) modules

clean:
	make -C /lib/modules/${kernelver}/build M=$(PWD) clean
