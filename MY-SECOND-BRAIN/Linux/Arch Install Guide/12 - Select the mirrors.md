1. Synchronized the servers

### `pacman -Syyy`

![[2021-12-22_084058.png]]

2. Download reflector package

### `Pacman -S reflector`

![[2021-12-22_091247.png|1000]]


3. Get reflector help page (Check reflector is working)

![[2021-12-22_164558.png|1000]]

If reflector prints "No module named Reflector" Error then install python3 package (sudo pacman -S python3)`

4. Sort the five most recently synchronized mirrors with 6 hours servers have been update by download speed and overwrite the local mirrorlist :- 

### `reflector --verbose --latest 10 -a 10 --sort rate --save /etc/pacman.d/mirrorlist`

5. Check mirror list

### `cat /etc/pacman.d/mirrorlist`

![[2021-12-22_171922.png]]

[[13 - Install the base packages]]
