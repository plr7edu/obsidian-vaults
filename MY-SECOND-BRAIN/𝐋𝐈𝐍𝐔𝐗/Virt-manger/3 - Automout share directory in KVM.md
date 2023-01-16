# Virtual Matchine :-

1. Open terminal and type following command. 

```bash
sudo vim /etc/fstab
```

2. Type Following line to fstab 

```
/sharepoint /home/test/share  9p trans=virtio,version=9p2000.L,rw 0       0
```

![[2022-11-13_22-44.png]]

3. Then write and quit. (:wq) 
4. Reboot.