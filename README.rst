Macintosh
=================================================================================

Tutorial
---------------------------------------------------------------------------------

- Switching from Windows to Mac: https://www.youtube.com/watch?v=I96nVmnzUqE

Cloning HD
---------------------------------------------------------------------------------

**Cek Disk**

- Cek disk speed (app): Disk Speed Test
- Info: performa SSD adalah 6 kali lipat lebih cepat

**Cloning**

- turn on, kemudian tekan cmd+R
- akan masuk ke macOS Utilities > Disk Utility
- format external hardisk (target)
   - Name: Mac OS
   - Format: Mac Os Extended (Journaled)
- pilih external hardisk > restore from main > image
- close 
- shutdown (kiri atas)

**Booting from external**

- tekan alt langsung setelah tekan tombol power 
- akan ada 2 pilihan booting hardisk, pilih yang ada simbol usb

General
---------------------------------------------------------------------------------

- Cek penggunaan memori: Finder > Applications > Utilities > Activity Monitor
- Buka storages (termasuk shared folders): $ cd /Volumes
- Buka pdf preview dari terminal: $ open tes.pdf 
- Copy, Cut, Paste: cmd+C, cmd+X, cmd+V
- Select all: cmd+A
- Right click: ctrl+click atau double tap
- Delete: fn+backspace
- Force quit: cmd+alt+esc

Users
---------------------------------------------------------------------------------

$ cd /Users

show all contents

$ ls -a

Apps
---------------------------------------------------------------------------------
Brew
*********************************************************************************

- website: https://brew.sh
- definisi: cek di wikipedia

Git
*********************************************************************************

- install: $ brew install git

Vim
*********************************************************************************

**Definisi**

vimrc adalah sebuah file yang berisi initialization. 

**Lokasi vimrc**

- cek lokasi vimrc: $ vim --version
- system vimrc file: "$VIM/vimrc"
- user vimrc file: "$HOME/.vimrc"
- 2nd user vimrc file: "$~/.vim/vimrc"

**Cek vim initialization**

- $ vim
- $ :help initialization

vimrc dicari secara urut dan hanya file yang pertama kali ditemukan yang akan
dibaca.  Di Unix, urutannya adalah:

- $HOME/.vimrc atau
- $HOME/.vim/vimrc 

**Isi vimrc**

set number
set textwidth=80

Tmux
*********************************************************************************

- Tutorial: https://fideloper.com/mac-vim-tmux

Pandoc
*********************************************************************************

**Install**

- $ brew install pandoc
- $ brew install pandoc-citeproc

**Konversi**

- txt to html: $ pandoc -s tes.txt -o tes.html
- rst to pdf: $ pandoc tes.rst --pdf-engine=pdflatex -o tes.pdf

Themes
*********************************************************************************

- MacOS Catalina Wallpapers: https://www.gnome-look.org/p/1362975/
- Font: Lucida grande

iTerm2
*********************************************************************************

- iTerm2 adalah terminal emulator untuk MacOS
- Tutorial: https://medium.com/@Clovis_app/configuration-of-a-beautiful-efficient-terminal-and-prompt-on-osx-in-7-minutes-827c29391961 
- Install: https://iterm2.com
- Color schemes: https://iterm2colorschemes.comi
  + apply color scheme: iTerm2 > Preferences > Profiles > Colors > Color presets > import
  + favourite color: cobalt2
- Install font
  + apply font: iTerm2 > Preferences > Profiles > Text > Change Font
  + favourite font: SourceCodePro+powerline
- Install zsh and Oh my Zsh:
  + zsh: brew install zsh zsh-completions
  + Oh my Zsh: $ sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
- Install Theme
  + Install: $ git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
  + Edit ~/.zshrc: ZSH_THEME="powerlevel9k/powerlevel9k"

Alias
*********************************************************************************

- configuration file: .zshrc
- referensi: https://scriptingosx.com/2019/07/moving-to-zsh-part-4-aliases-and-functions/
