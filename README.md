# vim

## apt installs
```
sudo apt install git curl python3-pip exuberant-ctags ack-grep
sudo pip3 install pynvim flake8 pylint isort

sudo apt-get install fonts-powerline
```

## Nerd Fonts
1. Download https://www.nerdfonts.com/font-downloads hermit hermut
2. Unzip and copy to ~/.fonts or ~/.local/share/fonts
3. `fc-cache -fv` rebuild font cache

## Powerline Fonts
1. https://github.com/powerline/fonts
2. https://vi.stackexchange.com/questions/3359/how-do-i-fix-the-status-bar-symbols-in-the-airline-plugin

## ZSH and Powerlevel
- https://gist.github.com/kevin-smets/8568070

## GIT
- see https://github.com/tpope/vim-fugitive
- `Gblame` show commits and annotations
- `Gstatus` show git status

## Comments (using https://github.com/preservim/nerdcommenter)
- " " + c + " ": Toggle comment
- " " + cc : Comment
- " " + cn : Nested comments 
    
## Line Commands
*Move line*
  :m 12 	move current line to after line 12

`yy` copy line

`CTRL - V` (mark line vertically) then `Shift-I` (insert) or `x` (remove) (Line Comments)

## Window Commands
- `Control+W followed by W` to toggle between open windows and,
- `Control+W followed by H/J/K/L` to move to the left/bottom/top/right window accordingly.

## NERDTree
- `cd` selected branch used as workdir
- `C`  selected branch as root NERDTree dir
