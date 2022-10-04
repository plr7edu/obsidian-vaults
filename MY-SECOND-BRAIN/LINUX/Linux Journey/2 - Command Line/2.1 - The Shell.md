## What is the shell?
- The shell is basically a program that takes your commands from the keyboard and sends them to the operating system to perform.

- If you’ve ever used a GUI, you’ve probably seen programs such as “Terminal” or “Console” these are just programs that launch a shell for you.

![[Shell.png]]

- We will use the shell program bash (Bourne Again shell), almost all Linux distributions will default to the bash shell.

- There are other shells available such as  <mark>zsh , fish, </mark> but we won’t get into any of those.

```
username@hostname:current_directory

pete@icebox:/home/pete $
```

**(Depending on the distribution your shell prompt might change)

![[2021-08-03_041440.png]]

### Notice the $ at the end of the prompt?

- Different shells will have different prompts, in our case the <mark>$</mark> is for a normal user using Bash, Bourne or Korn shell, you don't add the prompt symbol when you type the command, just know that it's there.


#### Let’s start with a simple command,


1. echo

![[2021-08-03_041926.png]]

> The echo command just prints out the text arguments to the display.

2. date

![[2021-08-03_042320.png]]

> **The date command just prints out the date time information.

3. whoami

![[2021-08-03_042455.png]]

> The echo command just prints out the user name.