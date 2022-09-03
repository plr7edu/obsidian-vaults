### `$ echo Hello World > peanuts.txt`

What just happened?

- Well check the directory where you ran that command and lo and behold you should see a file called peanuts.txt,

- look inside that file and you should see the text Hello World.

- Lots of things just happened in one command so let's break it down.

![[2021-08-17_085156.png]]

1.First let's break down the first part : -


#### `$ echo Hello World`

- We know this prints out Hello World to the screen,

but how?

- Processes use I/O streams to receive input and return output.



![[2021-08-17_090004.png]]


<mark>By default the echo command takes the input (standard input or stdin)
from the keyboard and returns the output (standard output or stdout) to the screen.</mark>

- So that's why when you type echo Hello World in your shell, you get Hello World on the screen.

**However, I/O redirection allows us to change this default behavior giving us greater file flexibility.

2.Let's proceed to the next part of the command :-

### `>`

- The > is a redirection operator that allows us the change where standard output goes.

- It allows us to send the output of echo Hello World to a file instead of the screen.

- If the file does not already exist it will create it for us.

- However, if it does exist it will overwrite it (you can add a shell flag to prevent this depending on what shell you are using).


- And that's basically how stdout redirection works!

---

- Well let's say I didn't want to overwrite my peanuts.txt,

- luckily there is a redirection operator for that as well, >> :-

### `$ echo Hello World >> peanuts.txt`

![[2021-08-17_092225.png]]

- This will append Hello World to the end of the peanuts.txt file,

- If the file doesn't already exist it will create it for us like it did with the > redirector!

(Examples)


![[2021-08-17_100039.png]]

![[2021-08-17_100147.png]]

![[2021-08-17_100324.png]]

What redirector do you use to append output to a file?

`>>`
`📁`

