- The ls command will list directories and files in the current directory by default, however you can specify which path you want to list the directories of.

```
$ ls
$ ls /home/pete
```

- <mark>ls</mark> is a quite useful tool, it also shows you detailed information about the files and directories you are looking at.

- Also note that not all files in a directory will be visible.

- Filenames that start with . are hidden, you can view them however with the ls command and pass the <mark>-a</mark> flag to it (a for all).

### `$ ls -a`

![[2021-08-03_055155.png|1000]]

- There is also one more useful ls flag, <mark>-l </mark>for long, this shows a detailed list of files in a long format.

- This will show you detailed information, starting from the

 ➡left: file permissions, number of links, owner name, owner group, file size, timestamp of last modification, and file/directory name

### `$ ls -l`

![[2022-04-27_165459.png]]

![[2021-08-03_061201.png]]

-   Commands have things called flags (or arguments or options, whatever you want to call it) to add more functionality.
-   See how we added -a and -l, well you can add them both together with -la.
-   The order of the flags determines which order it goes in, most of the time this doesn’t really matter so you can also do ls -al and it would still work.

### `$ ls -la`
### `$ ls -al`

![[2021-08-03_123454.png]]

###  ls -R: recursively list directory contents

![[2021-08-03_123726.png]]

### ls -r: reverse order while sorting

![[2021-08-03_123918.png]]

### ls -t: sort by modification time, newest first

![[2021-08-03_124044.png]]
