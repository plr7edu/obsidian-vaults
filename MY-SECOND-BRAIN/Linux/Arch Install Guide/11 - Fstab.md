-  This file at boot time will tell the distribution  where the find partitions.

1. Create a Directory for fstab

### `mkdir /mnt/etc`

2. Generate an fstab file

### `genfstab -U -p /mnt >> /mnt/etc/fstab`

3.  Check fstab file

## `cat /mnt/etc/fstab`

![[2021-12-21_220557.png|1000]]

[[12 - Select the mirrors]]
