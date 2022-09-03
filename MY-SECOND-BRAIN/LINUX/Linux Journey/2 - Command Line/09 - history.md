In your shell, there is a history of the commands that you previously entered, you can actually look through these commands.

This is quite useful when you want to find and run a command you used previously without actually typing it again.

### `$ history`

![[2021-08-03_141924.png]]

<mark>Want to run the same command you did before, just hit the up arrow.</mark>

- Want to run the previous command without typing it again?

- Use !!. If you typed cat log.txt and want to run it again, you can actually just go !! and it will run the last command you ran.

![[2021-08-03_142209.png|1000]]

- Another history shortcut is ctrl-R, this is the reverse search command, if you hit ctrl-R and you start typing parts of the command you want it will show you matches and you can just navigate through them by hitting the ctrl-R key again.

- Once you found the command you want to use again, just hit the Enter key.

![[2021-08-03_144220.png]]

use the clear command to clear up your display

### `$ clear`

## <u>Tab Key in Command Line</u>

- one of the most useful features in any command-line environment is tab completion.

- If you start typing the beginning of a command, file, directory, etc and hit the Tab key, it will autocomplete based on what it finds in the directory you are searching as long as you don’t have any other files that start with those letters.

- For example if you were trying to run the command chrome, you can type chr and press Tab and it will autocomplete chrome.
