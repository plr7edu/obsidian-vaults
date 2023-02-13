- To verify the boot mode, list the [efivars](https://wiki.archlinux.org/title/Efivars) directory :-

### `# ls /sys/firmware/efi/efivars`

- If the command shows the directory without error, then the system is booted in UEFI mode.

- If the directory does not exist, the system may be booted in [BIOS](https://en.wikipedia.org/wiki/BIOS) (or [CSM](https://en.wikipedia.org/wiki/Compatibility_Support_Module)) mode.
![[2021-12-20_055833.png|1000]]

[[3 - Connect to the Internet]]
