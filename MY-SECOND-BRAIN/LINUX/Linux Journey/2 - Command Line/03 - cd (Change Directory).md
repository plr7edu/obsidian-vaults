-  Now that you know where you are, let’s see if we can move around the filesystem a bit.
- Remember we’ll need to navigate our way using paths.
- There are two different ways to specify a path, with absolute and relative paths.

## Absolute path :

-   This is the path from the root directory.
-   The root is the head honcho.
-   The root directory is commonly shown as a slash.
-   Every time your path starts with / it means you are starting from the root directory.

 <u>For example, /home/pete/Desktop</u>

### `$ cd /home/pete/Pictures`

## Relative path:

-   This is the path from where you are currently in filesystem.

-  If I was in location /home/pete/Documents and wanted to get to a directory inside Documents called taxes, I don’t have to specify the whole path from root like /home/pete/Documents/taxes, I can just go to taxes/ instead

<u>Now from this directory I have a folder inside called Hawaii, I can navigate to that folder with:</u>

### `$ cd Hawaii`

### (.) Current Directory

> . (current directory). This is the directory you are currently in. 

![[2021-08-03_050746.png]]

### (..) Parent Directory

> .. (parent directory). Takes you to the directory above your current.

![[2021-08-03_050843.png]]

### (~) Home Directory

> **~ (home directory). This directory defaults to your “home directory”. Such as /home/pete.

![[2021-08-03_051002.png]]

### (-) Previous Directory

>    - (previous directory). This will take you to the previous directory you were just at.

![[2021-08-03_051121.png]]

### (cd) Defaults to your "Home Directory"

> (cd) This directory defaults to your “home directory”. Such as /home/pete.

![[2021-08-03_051744.png]]

