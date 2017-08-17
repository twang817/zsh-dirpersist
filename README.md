# zsh-dirpersist

This is a copy of the [dirpersist][1] library from [oh-my-zsh][2], packaged as a zsh plugin to be used with your favorite zsh plugin manager.

[1]: https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/dirpersist
[2]: https://github.com/robbyrussell/oh-my-zsh
[3]: http://zsh.sourceforge.net/

## Requirements

* [ZSH][3] >= 4.3.0

## Install

### antigen

    antigen bundle twang817/zsh-dirpersist

### zgen

    zgen load twang817/zsh-dirpersist
    
### antibody

    antibody bundle twang817/zsh-dirpersist
    
## Usage

Dirpersist hooks into `chpwd_functions` in ZSH and will persist your directory stack across terminal sessions.

## Tips

`cd -<TAB>` will show you your dirstack at any point in time:

```
cd -<TAB>
directory stack
0 -- ~/.dotfiles/zsh/completion
1 -- ~/.dotfiles/zsh/completions/gvm
2 -- ~/.dotfiles/zsh/completions
3 -- ~/.dotfiles/zsh/configs/gvm
4 -- ~/.dotfiles/zsh/configs/fzf
5 -- ~/.dotfiles/zsh/configs
6 -- ~/.dotfiles/zsh/ssh-agent
7 -- ~/.dotfiles/zsh/ssh-identities
8 -- ~/.dotfiles/zsh/plugins
11 -- ~/.dotfiles/zsh/clipboard
12 -- ~/.dotfiles/zsh
15 -- ~/.dotfiles/zsh
16 -- ~/.dotfiles/zsh/bundles
17 -- ~
```
