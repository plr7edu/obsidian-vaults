1. Create a mount directory for boot

### `mkdir -p /mnt/boot/efi`

2.  Mount EFI partition.

### `mount /dev/sda1 /mnt/boot/efi`

<mark>( In Dual Boot mount windows EFI partition)</mark>

- use gdisk -l or fdisk -l to determine your EFI partition

![[2021-12-21_053753.png]]

[[11 - Fstab]]
