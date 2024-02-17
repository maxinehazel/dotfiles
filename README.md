# README

New Dotfiles Setup Flow

## WSL

### 1. Prerequisites

Symlink repos folder 

`$ ln -s /mnt/c/Users/krebs/repos /home/krebs/repos`

Generate New SSH Key 

```
$ ssh-keygen -t ed25519 -C "krebs.maxine@gmail.com"
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/<private_key>
```

Install `gh`

https://github.com/cli/cli

Install `fish`

```
$ sudo apt-add-repository ppa:fish-shell/release-3
$ sudo apt update
$ sudo apt install fish

$ chsh -s $(which fish)
```

Install `tmux`

`$ sudo apt install tmux -y`

Install `asdf`

```
$ git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.14.0
```

Install `stow`

`$ sudo apt install stow`

### 2. The Thing

Run stow

`$ stow -t /home/krebs .`

### Experimental

Install NeoVim and (sigh) NvChad

```
$ sudo apt install neovim 
$ git clone https://github.com/NvChad/NvChad ~/.config/nvim --depth 1 && nvim

```
