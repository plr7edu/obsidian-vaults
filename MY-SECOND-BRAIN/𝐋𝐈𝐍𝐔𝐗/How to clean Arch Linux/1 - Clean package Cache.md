- Pacman, a package manager of Arch Linux, stores all downloaded packages in /var/cache/pacman/pkg/ and it does not remove the old or uninstalled versions automatically.

-   Showing the size of downloaded packages in my Arch Linux

### ``du -sh /var/cache/pacman/pkg`

![[Untitled picture 1.png]]

### 1. Cleaning the cache Manually

-   One option is to remove cached packages that are not currently installed :-

#### `sudo pacman –Sc`

![[Untitled picture1 1.png]]

#### The other option is to remove all the package from the cache, including those that are installed :-

### `sudo pacman –Scc



![[Untitled picture3 1.png]]

### 2.  Cleaning the cache Automatically
- Another way to clean the /var/cache/pacman/pkg/ directory is to use a script that automatically deletes all cached versions of installed and uninstalled packages, except for the most recent 3 versions. The script is called paccache. You can install it with the pacman-contrib package.

### `sudo pacman -S pacman-contrib

- For available, options check the help menu of paccache.

### `paccache –h

![[Untitled picture4 1.png]]

## Run paccache monthly
- A very useful way to use this script is to have it run automatically once a month using the [systemd timer](https://wiki.archlinux.org/index.php/Systemd/Timers#Timer_units). Basically, you need to create the file paccache.timer in /etc/systemd/system/, which will trigger /usr/lib/systemd/system/paccache.service.

1.  So, you create a paccache.timer file with nano

### `sudo nano /etc/systemd/system/paccache.timer

2. Then, to run this script monthly, paste the following content into this file 

> [Unit]
> Description=Clean-up old pacman pkg
> 
> [Timer]
> OnCalendar=monthly
> Persistent=true
> 
> [Install]
> WantedBy=multi-user.target

3. After that, start the systemd service

### `sudo systemctl enable paccache.timer

### `sudo systemctl start paccache.timer

4. Finally, you can check the service status.

### `sudo systemctl status paccache.timer

![[Untitled picture5 1.png]]

- So, you should see the message that it is active. 
- Now, paccache will run every month and clean the cache of your old and uninstalled packages.

## Run paccache after pacman (Additional)

- Alternatively to this timer, you can also run paccache every time after you run pacman. So, you need to [create a Hook](https://wiki.archlinux.org/index.php/Pacman#Hooks) for that.

1. Just create a file /usr/share/libalpm/hooks/paccache.hook

### `sudo nano /usr/share/libalpm/hooks/paccache.hook

2.  After that, add this content on the file.

> [Trigger]
> Operation = Upgrade
> Operation = Install
> Operation = Remove
> Type = Package
> Target = *
> 
> [Action]
> Description = Cleaning pacman cache with paccache …
> When = PostTransaction
> Exec = /usr/bin/paccache -r

- Now, if I remove a package using pacman, paccache will also be executed.


![[Untitled picture6 1.png]]

[[2 - Remove unused packages (Orphans)]]
