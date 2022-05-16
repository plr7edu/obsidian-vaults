-   In this step, I will show you how to clean Arch Linux by removing the cache files in your /home/user folder

1. As we use our system, the cache will fill up and take up a lot of space. So, the first thing you probably would want to do is to clean cache in your user directory. If you want to check the size of your cache folder, you can do it with this command :-

### `sudo du -sh ~/.cache/

![[Untitled picture9.png|500]]

2. To clean it, you need to remove all files inside it:

### `rm -rf ~/.cache/*

[[4 - Remove old config files]]

