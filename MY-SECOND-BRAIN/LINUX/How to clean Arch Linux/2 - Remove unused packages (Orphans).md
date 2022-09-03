-   When you install and remove packages in Arch Linux, some unused orphans packages may remain on your system. To find them you need to run this command :-

### `sudo pacman -Qtdq`

![[Untitled picture7.png]]

1. As you can see, by executing the above command, you will be able to know which packages are orphans. To remove them, you need to modify the command with the remove action :-

### `sudo pacman -Rns $(pacman -Qtdq)

![[Untitled picture8.png]]

[[3 - Clean the Cache in your home directory]]
