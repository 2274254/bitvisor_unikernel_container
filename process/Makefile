CFLAGS += -Iprocess/lib

bins-1 += debug helpinit log panic recvexample sendexample sendint hello unikernelctl
bins-1 += unikernel #kernel
#bins-1 += osv
bins-1 += serialtest shell
bins-$(CONFIG_IDMAN) += idman
bins-$(CONFIG_STORAGE) += storage
bins-$(CONFIG_VPN) += vpn
asubdirs-1 += lib
bins-$(CONFIG_IP) += echoctl
bins-$(CONFIG_PCI_MONITOR) += monitor

unikernelbins =
#unikernelbins += osv
unikernelbins += kernel

debug-objs = debug.o
help-objs = help.o
idman-objs = idman.o
idman-libs = idman/lib/$(outa) crypto/$(outa)
init-objs = init.o
log-objs = log.o
panic-objs = panic.o
recvexample-objs = recvexample.o
sendexample-objs = sendexample.o
sendint-objs = sendint.o
serialtest-objs = serialtest.o
shell-objs = shell.o
storage-objs = storage.o
storage-libs = storage/lib/$(outa) crypto/$(outa)
vpn-objs = vpn.o
vpn-libs = vpn/lib/$(outa) crypto/$(outa)
echoctl-objs = echoctl.o
monitor-objs = monitor.o
hello-objs = hello.o
unikernelctl-objs = unikernelctl.o
#osv-objs = osv.o
unikernel-objs = unikernel.o
unikernel-libs = unikernel/lib/$(outa)
#kernel-objs = kernel.elf

kernel-uklobjs = kernel.elf
#osv-uklobjs = osv.o
