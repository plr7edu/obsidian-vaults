
What is GRUB ?

- Grub is a bootloader.

## Bootloader

-  A boot loader is a piece of software started by the firmware (BIOS or UEFI).

- It is responsible for loading the kernel with the wanted kernel parameters, and initial RAM disk based on configuration files.

- In the case of UEFI, the kernel itself can be directly launched by the UEFI using the EFI boot stub.

- A separate boot loader or boot manager can still be used for the purpose of editing kernel parameters before booting.

---

1. Install Grub and necessary packages for bootloader

### `pacman -S grub efibootmgr dosfstools os-prober mtools`

2. Install Grub 

### `grub-install --target=x86_64-efi --bootloader-id=grub_uefi --recheck`

![[2021-12-27_041556.png|800]]

3. Set GRUB Language to English

### `cp /usr/share/locale/en\@quot/LC_MESSAGES/grub.mo /boot/grub/locale/en.mo`

4. Generate GRUB Configuration File.

### `grub-mkconfig -o /boot/grub/grub.cfg`

![[2021-12-27_044037.png]]

[[16 - Reboot]]
