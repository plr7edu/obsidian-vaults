1. Create "dotfiles" directory

### `mkdir dotfiles
2. Move the configuration files you care about to an equivalent file path in ==~/.dotfiles 

### `mv ~/.bash_profile ~/.dotfiles/
### `mv ~/.bashrc ~/.dotfiles/

3. You can use the "ln" command on linux and macOS to create symbolic links form a source file or directory to a new location :-


### `ln –sf ~/.dotfiles/.bachrc ~/.bashrc

![[Untitled picture30.png|700]]


[[5  - Setup Git for using GitLab (Including SSH Key)]]
