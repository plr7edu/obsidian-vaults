- You can do even more cleaning by removing duplicated and empty files and directories. To keep some order in your system, I also recommend removing broken symlinks, e.i. links that lead to non-existing filer or folders. They do not take much space, but they clutter your system. To remove such things, you can use the program rmlint. Install It.

### `sudo pacman -S rmlint`

![[Untitled picture12.png]]

![[Untitled picture13.png]]

-   This program will list everything it finds and creates a shell script to remove this lint. The script can be found in the home folder. Open it using a text editor, scroll down and check what files it will remove.

![[Untitled picture17.png]]

![[Untitled picture14.png|1000]]

You can remove some of these files manually, or if you agree with suggested remove action you can go back to the terminal and execute this script. Again, make sure you have a backup of all files before you run this script. <mark>This action will be irreversible.</mark>

### `sh -c rmlint.sh

[[6  - Find the largest files and directories]]


