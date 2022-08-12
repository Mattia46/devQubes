# Qubes Dev AppWm

#### Pre-requisite
 upgrade Debian to Testing source.list

#### Dev Template packages
 nvim
 tmux
 tree
 node
 zsh
 silversearcher-ag

#### Dev App WM
 ```bash
 # packer
 git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim

 # typescript server
 npm install -g typescript typescript-language-server
 ```

#### Dev WM Symlinks
```bash
git clone git@github.com:Mattia46/devQubes.git
ln -s devQubes/nvim ~/.config/nvim
ln -s devQubes/zshrc ~/.zshrc
ln -s devQubes/gitconfig ~/.gitconfig
ln -s devQubes/tmux.conf ~/.tmux.conf
ln -s devQubes/fonts/* ~/.local/share/fonts/ => then fc-cache
vim +PackerInstall
```
