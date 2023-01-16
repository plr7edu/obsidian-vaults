1. Install stow

### `sudo pacman -S stow` (Arch)

### `sudo apt install -y stow` (Debian)

2. Check adopt all the config files :-

> stow --adopt -nvt ~ * 

==-n = Simulation Mode

![[Stow1.png]]

3. Adopt all the config files

> stow --adopt -vt ~ *

![[Stow2.png]]

![[Stow3.png]]

### Unlink an application config from stow

> stow –vDt ~ bash

![[Stow unlink.png]]

[[10  - Add,Commit & Push to gitlab]]

