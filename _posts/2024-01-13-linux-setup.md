---
title: 'Setting up linux on a new machine (again)'
date: 2024-01-03
permalink: /posts/2024/01/blog-post-1/
tags:
  - pc
---

Every so often, my linux setup becomes irreperable, and I just have to reinstall (when the cost-analysis on the time it takes to debug outweights restarting fresh)...

Here are some notes for myself on setting a new ubuntu 22.04 machine. 


## Dev-related

### Setup `nodejs`

Ref: https://askubuntu.com/questions/426750/how-can-i-update-my-nodejs-to-the-latest-version

Recommended to use `nvm`; run

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash
```

then after `source ~/.bashrc`, run

```
nvm install node
```

To update later on, 

```
nvm install node
nvm alias default node
```

### Setup nvim

Ref: https://builtin.com/software-engineering-perspectives/neovim-configuration

0. Install

1. By default, the config directory is not touched, so first run `mkdir ~/.config/nvim`, then create `init.vim` file for configuration via `nvim ~/.config/nvim/init.vim`

2. Install `vim-plug` (following https://github.com/junegunn/vim-plug/wiki/tutorial)
Example `init.vim` file content:

```
" Plugins will be downloaded under the specified directory.
call plug#begin(has('nvim') ? stdpath('data') . '/plugged' : '~/.vim/plugged')

" Declare the list of plugins.
Plug 'tpope/vim-sensible'
Plug 'junegunn/seoul256.vim'

" List ends here. Plugins become visible to Vim after this call.
call plug#end()


set nocompatible            " disable compatibility to old-time vi
set showmatch               " show matching 
set ignorecase              " case insensitive 
set mouse=v                 " middle-click paste with 
set hlsearch                " highlight search 
set incsearch               " incremental search
set tabstop=4               " number of columns occupied by a tab 
set softtabstop=4           " see multiple spaces as tabstops so <BS> does the right thing
set expandtab               " converts tabs to white space
set shiftwidth=4            " width for autoindents
set autoindent              " indent a new line the same amount as the line just typed
set number                  " add line numbers
set wildmode=longest,list   " get bash-like tab completions
" set cc=80                  " set an 80 column border for good coding style
filetype plugin indent on   "allow auto-indenting depending on file type
syntax on                   " syntax highlighting
set mouse=a                 " enable mouse click
set clipboard=unnamedplus   " using system clipboard
filetype plugin on
set cursorline              " highlight current cursorline
set ttyfast                 " Speed up scrolling in Vim
" set spell                 " enable spell check (may need to download language package)
" set noswapfile            " disable creating swap file
" set backupdir=~/.cache/vim " Directory to store backup files.

call plug#begin()
 " Plugin Section
 Plug 'dracula/vim'
 Plug 'ryanoasis/vim-devicons'
 Plug 'SirVer/ultisnips'
 Plug 'honza/vim-snippets'
 Plug 'scrooloose/nerdtree'
 Plug 'preservim/nerdcommenter'
 Plug 'mhinz/vim-startify'
 Plug 'neoclide/coc.nvim', {'branch': 'release'}
call plug#end()
```

### Setup conda/python

Install miniconda etc.

### Setup julia

Ref: https://julialang.org/downloads/platform/

```
wget https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-linux-x86_64.tar.gz
tar zxvf julia-1.10.0-linux-x86_64.tar.gz
```

Then `vim ~/.bashrc` to add

```
export PATH="$PATH:/path/to/<Julia directory>/bin"
```

### Setup c++

1. Get g++ (via `sudo apt-get install build-essential`)
2. Install cmake: `sudo apt install cmake`
3. Setup vcpkg
3.1. Clone repo, then generate script
3.2. Add to path:

```
export PATH="$PATH:/home/yuri/vcpkg"
```
  
3.3. Add as alias

```
export VCPKG_ROOT="/home/yuri/vcpkg"
```

4. Likely to run into compile error; checking log, seems to require

```
sudo apt-get install pkg-config
```

Also, using python3 seems to require `autoconf` and `libtool`

```
sudo apt-get install autoconf automake autoconf-archive
```

### Git repository settings

Repos that require a token: use the https git clone command, but insert `<token>@` between `https://` and `github.com/.../repo.git`


### Setup GT VPN

Follow article (GT login required): https://gatech.service-now.com/home?id=kb_article_view&sysparm_article=KB0026837



### Setting up Arduino

Refs:
- https://www.arduino.cc/en/Guide
- https://forum.arduino.cc/t/ubuntu-arduino-ide-not-showing-any-ports/1043925/10

1. Download IDE, make sure to change permission to executable (for AppImage)
2. Make sure to add rule for access in file `/etc/udev/rules.d/99-arduino.rules`:

```
SUBSYSTEMS=="usb", ATTRS{idVendor}=="2341", GROUP="plugdev", MODE="0666"
```

3. Add current user in dialout group via

```
sudo adduser $USER dialout
```

4. Uninstall `brltty` if it is installed via `sudo apt purge brltty`


## Apps

- To install early on: `git`, `nvim`, `bat` (aliased as `batcat`)


### Using AppImages (e.g. Obsidian)

- Obsidian: Might require `sudo apt install -y libfuse2`
- Mendeley: https://www.mendeley.com/download-reference-manager/linux
- Need to make `*.desktop` for making icon
  - In `~/.local/share/applications`, make `APPNAME.desktop` file. For example, `obsidian.desktop` could look like:

```
[Desktop Entry]
Name=obsidian
Icon=/home/yuri/Apps/obsidian_icon.png
Exec=/home/yuri/Apps/Obsidian-1.5.3.AppImage
Type=Application
```

- Using git: on linux, there is at the beginning an auth error; requires running `git config --global user.email "yuri.shimane@gmail.com"` on the Vault repo (on terminal)


