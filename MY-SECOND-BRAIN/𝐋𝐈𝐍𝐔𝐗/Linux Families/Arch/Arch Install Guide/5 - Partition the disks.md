1. Check partition list.

### `lsblk / fdisk -l`

![[2021-12-20_121307.png]]

2. There are various partitioning tools one can use for partitioning Arch

-    cfdisk (Easy)
-    gdisk  (Directly compatible with UEFI bootmode)
-    fdisk

![[2021-12-20_150755.png|1000]]

## cfdisk
<mark>(IF YOU DUAL BOOT NOT CREATE A EFI PARTITION)</mark>


1. Create new partition

> [New] > 100M (EFI)  - /dev/sda1
> [New]> 14.9G ( For LVM) - /dev/sda2

2. Change partition type

> [Type] > 100M (System EFI)  - /dev/sda1
> [Type]> 14.9G ( Linux LVM) - /dev/sda2

[[6- Format the partition]]
