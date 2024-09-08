## Install vundle to install vim plugins
1. Clone vundle repository
```bash
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
2. Configurate vundle on vimrc file
```text
    |  1 set nocompatible
. Plugin 'VundleVim/Vundle.vim'                                                      |  2 filetype off
  Plugin 'preservim/nerdtree'                                                        |  3 " set the runtime path to include Vundle and initialize
* Helptags                                                                           |  4 set rtp+=~/.vim/bundle/Vundle.vim
```
## Vim orginal shortcuts
## Window
- `split window vertically:` :vsp -> vim split 
	- To split with `filename:` :vsp <file_name>
- `split window horizontally:` :sp -> split
- To move between the window, using: `crl + w + h/j/k/l`
## Navigation

## Plugin session
- NERD Tree: Show the tree of folders
- 