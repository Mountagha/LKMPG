obj-m += hello-1.o
obj-m += hello-2.o
obj-m += hello-3.o
obj-m += hello-4.o
obj-m += hello-5.o
obj-m += startstop.o
startstop-objs := start.o stop.o
obj-m += chardev.o
obj-m += procfs1.o
obj-m += procfs2.o
obj-m += procfs3.o
obj-m += procfs4.o
obj-m += hello-sysfs.o
obj-m += sleep.o
obj-m += print_string.o
obj-m += kbleds.o
obj-m += file_sched.o
obj-m += chardev2.o
obj-m += syscall.o

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
	rm other/ioctl other/cat_noblock
