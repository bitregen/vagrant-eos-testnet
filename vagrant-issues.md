# VirtualBox and Vagrant installation issues compendium 

## Ubuntu 18.04

The following issues were reported on Ubuntu 18.04

### 1. VBox kernel module not loaded
Vbox not working:  
```
kernel module not loaded
```  
[StackExchange thread](https://unix.stackexchange.com/questions/361617/virtualbox-is-complaining-that-the-kernel-module-is-not-loaded)  
***Fixed by disabling secure boot in BIOS***  

### 2. modprobe vboxdrv failed
```
vboxdrv.sh: failed: modprobe vboxdrv failed. Please use 'dmesg' to find out why.
```  
[StackExchange thread](https://askubuntu.com/questions/900118/vboxdrv-sh-failed-modprobe-vboxdrv-failed-please-use-dmesg-to-find-out-why)  

### 3. Vagrant ssh hangs
[StackExchange thread](https://askubuntu.com/questions/716467/vagrant-ssh-terminal-freezes)  
_Attempted fix by re-configuring vbox:_  
```
$ sudo /sbin/vboxconfig
```

_Attempted fix by destroying a duplicate machine:_
```
$ vagrant destroy 27
```

_Tried to learn more about the error by outputting ssh logs:_
```
$ vagrant ssh -- -v
```
***Fixed by enabling Virtualization under CPU settings in BIOS***
