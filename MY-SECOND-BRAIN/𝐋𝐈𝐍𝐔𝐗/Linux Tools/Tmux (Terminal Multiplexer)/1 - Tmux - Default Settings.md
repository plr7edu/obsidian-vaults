
- Install tmux 

```bash
sudo apt install tmux  # Debian
sudo dnf install tmux  # Fedora
sudo pacman -S tmux    # Arch
```

![[2023-03-29_11-14.png]]

# Basic

1. Default tmux prefix 
```
CTRL + B
```

2. Horizontal Panes
```
CTRL + B + SHIFT + ""
Prefix,then SHIFT + ""
```

![[2023-03-29_13-15.png]]

3. Vertical Panes
```
CTRL + B + SHIFT + %
Prefix,then SHIFT + %
```

![[2023-03-29_13-16.png]]

4. Close Panes
```
Prefix,then x (This prompt for your conformation)
CTRL + D (This is easy) / Type : exit
```

![[2023-03-29_13-18.png]]

5. Switch between panes 
```
Prefix,then ←,↑,→,↓
```

6. Resize current pane 
```
CTRL + B , ↑
CTRL + B , ↓
CTRL + B , →
CTRL + B , ←
```

7. Zoom into a panes / Unzoom into a panes
```
Prefix,then z
```

![[2023-03-29_13-19.png]]

# Window

1. Create a new window
```
Prefix,then c
```

![[2023-03-29_13-23.png]]
2. Move to previous window
```
Prefix,p
```

3. Move to next window
```
Prefix,n
```

4. Kill a window
```
Prefix,&
```

![[2023-03-29_13-24.png]]
5. Rename a window
```
Prefix ,
```

![[2023-03-29_13-25.png]]

# Session

1. Disconnect your tmux session
```
Prefix , d
```

![[2023-03-29_13-26.png]]
2. Go back your tmux session
```
tmux attach / tmux a
```

3. List all open tmux session
```
tmux list-sessions / tmux ls (abbreviation)
```

![[2023-03-29_13-09.png]]
4. Target a tmux session
```
tmux attach -t 1
tmux a -t my-project (abbreviation)
```

5. Rename a tmux session
```
prefix, $
```

![[2023-03-29_13-33.png]]

![[2023-03-29_13-33_1.png]]

![[2023-03-29_13-36.png]]

6. Create  a  new tmux session with custom name
```
tmux new -s "my-project"
```

![[2023-03-29_13-40 1.png]]

7. Show sesion list with preview
```
prefix, s
```

![[2023-03-29_13-46 1.png]]

