- There are situations where you may want to add other directories to the $PATH variable.

-   For example, some programs may be installed in different locations, or you may want to have a dedicated directory for your personal scrips, but be able to run them without specifying the absolute path to the executable files. 

- To do this, you simply need to add the directory to your $PATH.

- Let’s say you have a directory called bin located in your Home directory in which you keep your shell scripts. To add the directory to your $PATH type in : -

### `export PATH="$HOME/bin:$PATH"

However, this change is only ==temporary== and valid only in the current shell session.

## Make the change permanent : -

- To make the change permanent, you need to define the $PATH variable in the shell configuration files. In most Linux distributions when you start a new session, environment variables are read from the following files:

-   Global shell specific configuration files such as /etc/environment and /etc/profile. Use this file if you want the new directory to be added to all system users $PATH.

-   Per-user shell specific configuration files. For example, if you are using Bash, you can set the $PATH variable in the ~/.bashrc file. If you are using Zsh the file name is ~/.zshrc.

In this example, we’ll set the variable in the ~/.bashrc file. Open the file with your [text editor](https://linuxize.com/post/how-to-use-nano-text-editor/) and add the following line at the end of it : -

### `nano ~/.bashrc`

> # Add bin directory to PATH
> export PATH="$HOME/bin:$PATH"

- Add this two line to .bashrc file.

Save the file and load the new $PATH into the current shell session using the [source](https://linuxize.com/post/bash-source-command/) command :- 

### `source ~/.bashrc

- To confirm that the directory was successfully added, print the value of your $PATH by typing :-

### `echo $PATH

![[Echo Path1.png .png]]

