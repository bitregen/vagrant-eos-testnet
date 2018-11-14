### VBox kernel module not loaded
Vbox not working, `"kernel module not loaded"`  
[StackExchange thread](https://unix.stackexchange.com/questions/361617/virtualbox-is-complaining-that-the-kernel-module-is-not-loaded)  
***Fixed by disabling secure boot in BIOS***  

`vboxdrv.sh: failed: modprobe vboxdrv failed. Please use 'dmesg' to find out why.`
[StackExchange thread](https://askubuntu.com/questions/900118/vboxdrv-sh-failed-modprobe-vboxdrv-failed-please-use-dmesg-to-find-out-why)

### Vagrant ssh hangs
[StackExchange thread](https://askubuntu.com/questions/716467/vagrant-ssh-terminal-freezes)  
_Attempted fix by re-configuring vbox_
```
$ sudo /sbin/vboxconfig
```

_Attempted fix by destroying a duplicate machine_
```
$ vagrant destroy 27
```

_Tried to learn more about the error by outputting ssh logs_
```
$ vagrant ssh -- -v
```
***Fixed by enabling Virtualization under CPU settings in BIOS***
