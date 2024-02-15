## README

New Dotfiles Setup Flow

### 1. Prerequisites

(WSL Only) Symlink repos folder 

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

Install `tmux`