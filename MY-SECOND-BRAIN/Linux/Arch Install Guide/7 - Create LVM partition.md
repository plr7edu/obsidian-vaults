1. Create Physical Volume on the LVM partition

> pvcreate partiton

### `pvcreate /dev/sda2``

![[2021-12-20_155630.png]]

2. Then add Volume Group on it to add various other Logical volumes

> vgcreate name partiton

### `vgcreate archvol /dev/sda2`

![[2021-12-20_160428.png]]

3. Now lets create logical volumes for root and home.

**(Root / )  : -

> lvcreate -L (Size) (Volume group name) -n (Logical volume name)

### `lvcreate -L 75GB archvol -n lv_root`

![[2021-12-20_161715.png]]

**(Home /home) :-

### ``lvcreate -l 100%FREE archvol -n lv_home``

![[2021-12-20_162022.png]]

[[8 - Active LVM configuration]]



