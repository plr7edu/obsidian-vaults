- Now I think we have too many files, let’s remove some files.

- To remove files you can use the rm command. The rm (remove) command is used to delete files and directories.

## `$ rm file1`

![[2021-08-03_202728.png]]


<mark>Take caution when using rm, there is no magical trash can that you can fish out removed files. Once they are gone, they are gone for good, so be careful.</mark>

## rm -f

- Fortunately there are some safety measures put into place, so the average joe can’t just remove a bunch of important files.

- Write-protected files will prompt you for confirmation before deleting them.

- If a directory is write-protected it will also not be easily removed.

Now if you don’t care about any of that, you can absolutely remove a bunch of files.

### `$ rm -f file1`

![[2021-08-04_041531.png|]]

<mark>-f or force option tells rm to remove all files, whether they are write protected or not, without prompting the user (as long as you have the appropriate permissions).</mark>

## rm -i

### `$ rm -i file`

![[2021-08-04_042000.png]]

<mark>Adding the -i flag like many of the other commands, will give you a prompt on whether you want to actually remove the files or directories.</mark>

## rm -r (Recursive)

### `$ rm -r directory`

![[2021-08-04_042347.png]]

<mark>You can’t just rm a directory by default, you’ll need to add the -r flag (recursive) to remove all the files and any subdirectories it may have.</mark>

## rmdir

### `$ rmdir directory`

- You can remove a empty directory with the rmdir command.


![[2021-08-04_042808.png]]