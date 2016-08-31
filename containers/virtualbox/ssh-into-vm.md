## SSH into a VM 

Find your VM

```
♪  ~  VBoxManage list vms                                                
"Solus1" {3a1db666-df40-4fb0-b94f-266e8ce978b5}
```

Map it to localhost on an alternate port (with the VM powered down):

```
♪  ~  VBoxManage modifyvm "Solus1" --natpf1 "host2guest-ssh,tcp,,2222,,22"
```

