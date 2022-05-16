- Let’s start making some copies of these files. Much like copy and pasting files in other operating systems, the shell gives us an even simpler way of doing that.

### `$ cp mycoolfile /home/pete/Documents/cooldocs`

- mycoolfile is the file you want to copy and /home/pete/Documents/cooldocs is where you are copying the file to.

- You can copy multiple files and directories as well as use wildcards.

- A wildcard is a character that can be substituted for a pattern based selection, giving you more flexibility with searches. You can use wildcards in every command for more flexibility.

#### * Wildcard
 - * the wildcard of wildcards, it's used to represent all single characters or any string.

![[2021-08-03_160147.png]]

#### ? (One Character)
- ? used to represent one character

![[2021-08-03_161402.png]]

#### [] Represent any character
-   [] used to represent any character within the brackets

![[2021-08-03_162200.png]]

![[2021-08-03_161935.png]]

#### -r flag

-   A useful command is to use the -r flag, this will recursively copy the files and directories within a directory.
-   Try to do a cp on a directory that contains a couple of files to your Documents directory.
-   Didn’t work did it? Well that’s because you’ll need to copy over the files and directories inside as well with -r command.

![[2021-08-03_162515.png]]

![[2021-08-03_163413.png]]

#### Overwritten

- One thing to note, if you copy a file over to a directory that has the same filename,
the file will be overwritten with whatever you are copying over

![[2021-08-03_164847.png]]

#### - i (Interactive)

- This is no Bueno if you have a file that you don’t want to get accidentally overwritten.

You can use the -i flag (interactive) to prompt you before overwriting a file.

![[2021-08-03_165456.png]]

