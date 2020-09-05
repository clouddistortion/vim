# vim

## apt installs
```
sudo apt install git curl python3-pip exuberant-ctags ack-grep
sudo pip3 install pynvim flake8 pylint isort

sudo apt-get install fonts-powerline
pip3 install yapf
```

## Fancy Fonts Install
* Download https://github.com/ryanoasis/nerd-fonts/blob/master/patched-fonts/Hermit/Medium/complete/Hurmit%20Medium%20Nerd%20Font%20Complete.otf
* e.g. on Manjaro
** mkdir -p ~/.local/share/fonts/ 
** cp Hurmit Medium Nerd Font Complete.otf to fonts folder
** run fc-cache


## File Creation
- :edit ~/projects/main.go
- :NERDTree + m : Menu in NERDTree for creating subnodes

## Format
`F3` Autoformat

## Terminal or Commands
* `:! <command> [Enter]` run a command 
* `<CTRL>-Z (do stuff in the terminal 'fg' to go back`

## Nerd Fonts
1. Download https://www.nerdfonts.com/font-downloads hermit hermut
2. Unzip and copy to ~/.fonts or ~/.local/share/fonts
3. `fc-cache -fv` rebuild font cache

## Powerline Fonts
1. https://github.com/powerline/fonts
2. https://vi.stackexchange.com/questions/3359/how-do-i-fix-the-status-bar-symbols-in-the-airline-plugin

## ZSH and Powerlevel
- https://gist.github.com/kevin-smets/8568070

## Rename Variable
- `gd`+ `c`+ `gn` (new name) `ESC` --> . (next) or :%norm . (all)

## Jump
- `CTRL-O`  : jump back
- `CTRL-I`  : jump forward
- `,d`      : jump to method definition
-

## GIT
- see https://github.com/tpope/vim-fugitive
- `Gblame` show commits and annotations
- `Gstatus` show git status

## Go
### Go (execute)
- `<Space> r` :GoRun
- `<Space> b` :GoBuild

### Autocomplete (e.g. Go)
`Ctrl + X Ctrl + O`

### Go Documentation
`:GoDoc` #resize with :resize 20
`:GoDocBrowser` #jump to documentation in browser

### Go code outline
`<F8>`
`:GoDef` or `gd` go to the definition of a e.g. method (back ctrl-o)

## Comments (using https://github.com/preservim/nerdcommenter)
- " " + c + " ": Toggle comment
- " " + cc : Comment
- " " + cn : Nested comments 
    
## Line Commands
*Move line*
  :m 12 	move current line to after line 12

### Move lines
### Normal mode
nnoremap <C-j> :m .+1<CR>==
nnoremap <C-k> :m .-2<CR>==
 
### Insert mode
inoremap <C-j> <ESC>:m .+1<CR>==gi
inoremap <C-k> <ESC>:m .-2<CR>==gi
 
### Visual mode
vnoremap <C-j> :m '>+1<CR>gv=gv
vnoremap <C-k> :m '<-2<CR>gv=gv

`yy` copy line

`CTRL - V` (mark line vertically) then `Shift-I` (insert) or `x` (remove) (Line Comments)

## Window Commands
- `Control+W followed by W` to toggle between open windows and,
- `Control+W followed by H/J/K/L` to move to the left/bottom/top/right window accordingly.

## NERDTree
- `cd` selected branch used as workdir
- `C`  selected branch as root NERDTree dir
- `F6` toggle NERDTree
- `,t` select current file in NERDTree
