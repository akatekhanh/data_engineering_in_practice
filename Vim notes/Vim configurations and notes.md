## Vim map key meaning
`remap` is an **option** that makes mappings work recursively. By default, it is on and I'd recommend you leave it that way. The rest are **mapping commands**, described below:

`:map` and `:noremap` are **recursive** and **non-recursive** versions of the various mapping commands. For example, if we run:

```
:map j gg           (moves the cursor to the first line)
:map Q j            (moves the cursor to the first line)
:noremap W j        (moves the cursor down one line)
```

Then:

- `j` will be mapped to `gg`.
- `Q` will _also_ be mapped to `gg`, because `j` will be expanded for the recursive mapping.
- `W` will be mapped to `j` (and not to `gg`) because `j` will not be expanded for the non-recursive mapping.
For each of these sets of mappings, there is a [mapping](http://vim.wikia.com/wiki/Mapping_keys_in_Vim_-_Tutorial_%28Part_1%29#Creating_keymaps) that works in normal, visual, select and operator modes (`:map` and `:noremap`), one that works in normal mode (`:nmap` and `:nnoremap`), one in visual mode (`:xmap` and `:xnoremap`) and so on.
## Install vundle to install vim plugins
1. Clone vundle repository
```bash
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
2. Configurate vundle on vimrc file
```text
set nocompatible
filetype off
set rtp+=~/.vim/bundle/Vundle.vim
```
3. Vim Color schema
```text
Plugin 'flazz/vim-colorschemes'
```
> We need to apply the color for this theme
## Vim orginal shortcuts
## Window
- `split window vertically:` :vsp -> vim split 
	- To split with `filename:` :vsp <file_name>
- `split window horizontally:` :sp -> split
- To move between the window, using: `crl + w + h/j/k/l`
## Navigation

## Plugin session
### 1. NERD Tree: Show the tree of folders 
