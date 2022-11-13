# Host Machine :-

1. Create a Directory for share

```bash
mkdir virt-manager-share
```

2.  Add read write execute permision to that directory

```bash
chmod 777 virt-manager-share/
```

3. Open virt-manager  and go "open" "show virtual matchine console and details" and select "show vitual hadware details" 

![[2022-11-13_22-31.png]]

 ![[2022-11-13_22-21.png]]

4. Select "Filesystem"  and change following details

	Driver : virtio-9p
	Source path : home/plr/virt-manager-share
	Target path : /sharepoint

5. Finish &  Apply  and start the VM.


# VM Matchine : -

1. Open Terminal and make share directory

```bash
mkdir share
```

2. Type following command

```bash
sudo mount -t 9p -o trans=virtio /sharepoint share
```
