
**(Root / )  : -

1. Format logical Volume use for root file system.

### `mkfs.ext4 /dev/archvol/lv_root`

![[2021-12-20_214138.png]]

2. Mount logical Volume use for root file system.

### `mount /dev/archvol/lv_root /mnt`

**(Home /home) :-

3. Format logical Volume use for home file system.`

### `mkfs.ext4 /dev/archvol/lv_home`

![[2021-12-21_043646.png]]

4. Create a mount directory for home

### `mkdir /mnt/home`

5. Mount logical Volume use for home file system.

### `mount /dev/archvol/lv_home /mnt/home`

[[10 - Mount the EFI partition (UEFI)]]
