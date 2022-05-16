- With all these files we have on the system it can get a little hectic trying to find a specific one.

- Well there’s a command we can use for that, find!

## -name

### `$ find /home -name puppies.jpg`

![[2021-08-04_043158.png]]

<mark>With find you’ll have to specify the directory you’ll be searching it, what you’re searching for, in this case we are trying to find a file by the name of Song.mp3.</mark>


## -type (Directory)

### `$ find /home -type d -name MyFolder`

You can see that I set the type of file I’m trying to find as (d) for directory and I’m still searching by the name of MyFolder.

![[2021-08-04_043816.png]]

- One cool thing to note is that find doesn’t stop at the directory you are searching,

- It will look inside any subdirectories that directory may have as well.

![[2021-08-04_043959.png]]