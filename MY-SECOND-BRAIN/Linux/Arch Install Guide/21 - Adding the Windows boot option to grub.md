(If os-prober package didn't Work)

1. Open the configuration file (With nano or vim)

> nano /boot/grub/grub.cfg

> 	menuentry "Windows Boot Manager (on /dev/sdb1)" {
> 	  insmod part_gpt
> 	  insmod fat
> 	  insmod search_fs_uuid
> 	  insmod chain
> 	  search --fs-uuid --set=root $hints_string $fs_uuid
> 	  chainloader /EFI/Microsoft/Boot/bootmgfw.efi
> 	}

2. Replace $hints_string by the output of :- 

### `sudo grub-probe --target=fs_uuid /boot/efi/EFI/Microsoft/Boot/bootmgfw.efi`
3. Replace $fs_uuid by the output of :-

### `sudo grub-probe --target=hints_string /boot/efi/EFI/Microsoft/Boot/bootmgfw.efi`

![[2021-12-29_093146.png]]

> menuentry "Windows Boot Manager (on /dev/sdb1)" {
>     insmod part_gpt
>     insmod fat
>     insmod search_fs_uuid
>     insmod chain
>     search --fs-uuid --set=root --hint-bios=hd1,gpt1 --hint-efi=hd1,gpt1 --hint-baremetal=ahci1,gpt1 C850-B041
>     chainloader /EFI/Microsoft/Boot/bootmgfw.efi
> }


