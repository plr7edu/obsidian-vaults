- Used for moving files and also renaming them.
-  Quite similar to the cp command in terms of flags and functionality.

## You can rename files like this :-

### `$ mv oldfile newfile`

![[2021-08-03_194846.png]]
## Or you can actually move a file to a different directory :- 

### `$ mv file2 /home/pete/Documents`

![[2021-08-03_195237.png]]

## And move more than one file :-

### `$ mv file_1 file_2 /somedirectory`

![[2021-08-03_200132.png]]

## You can rename directories as well :-
### `$ mv directory1 directory2`

![[2021-08-03_200406.png]]

## Overwrite

- Like cp, if you mv a file or directory it will overwrite anything in the same directory.
So you can use the -i flag to prompt you before overwriting anything.

### `$ mv -i directory1 directory2`
![[2021-08-03_200902.png]]

## Move file with backup

- Let’s say you did want to mv a file to overwrite the previous one.
- You can also make a backup of that file and it will just rename the old version with a ~.

### `$ mv -b directory1 directory2`

![[2021-08-03_201404.png]]

