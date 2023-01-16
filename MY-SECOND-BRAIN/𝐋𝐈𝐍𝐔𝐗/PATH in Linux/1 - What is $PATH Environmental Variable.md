- When you type a command on the command line, you’re basically telling the shell to run an executable file with the given name.

- In Linux, these executable programs like [ls](https://linuxize.com/post/how-to-list-files-in-linux-using-the-ls-command/) , [find](https://linuxize.com/post/how-to-find-files-in-linux-using-the-command-line/) , [file](https://linuxize.com/post/linux-file-command/) and others, usually live inside several different directories on your system.

- Any file with executable permissions stored in these directories can be run from any location.

- The most common directories that hold executable programs are

> /bin,
> /sbin,
> /usr/sbin,
> /usr/local/bin 
> /usr/local/sbin.

## What is $PATH in Linux ?
- The $PATH environmental variable is a colon-delimited list of directories that tells the shell which directories to search for executable files.

To check what directories are in your $PATH, you can use either the printenv or [echo](https://linuxize.com/post/echo-command-in-linux-with-examples/) command : - 

1. printenv

![[printenv.png]]


2. echo $PATH

![[Echo Path.png]]

[[2 - Adding a Directory to your $PATH]]
