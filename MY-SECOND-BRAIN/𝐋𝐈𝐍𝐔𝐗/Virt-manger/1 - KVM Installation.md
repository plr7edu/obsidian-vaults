1. Checking support for KVM

``` bash
$ LC_ALL=C lscpu | grep Virtualization
```

![[2022-11-13_20-01.png]]

2. Install need packages

Arch =

```bash
sudo pacman -S qemu virt-manager ebtables
```

3. Enable libvirtd deamon 

```bash
sudo systemctl enable libvirtd
```

4. Start libvirtd deamon

```bash
sudo systemctl start libvirtd
```

5. Add member to `libvirt` user group

```bash
sudo usermod -G libvirt -a plr
```
