dotfiles
========

My personal configuration

Prepare
--------

* Homebrew

```
 $ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
 $ brew doctor
 $ brew update
```

* Zsh

```
 $ brew install zsh
 $ sudo vi /etc/shells (最終行に/usr/local/bin/zshを追加)
 $ chsh -s /usr/local/bin/zsh
```

Install
--------

```
 $ git clone git://github.com/mikikohei/dotfiles.git ~/dotfiles
```

Setup
--------

```
 $ cd ~/dotfiles
 $ ./setup.sh
 $ brew bundle
```

This script create a symbolic link as following:

* .zlogin -> ~/.zprezto/runcoms/zlogin
* .zlogout -> ~/.zprezto/runcoms/zlogout
* .zpreztorc -> ~/.zprezto/runcoms/zpreztorc
* .zprofile -> ~/.zprezto/runcoms/zprofile
* .zshenv -> ~/.zprezto/runcoms/zshenv
* .zshrc -> ~/.zprezto/runcoms/zshrc
* .vimrc -> ~/dotfiles/.vimrc
* .dein.toml -> ~/dotfiles/.dein.toml
* .dein_lazy.toml -> ~/dotfiles/.dein_lazy.toml
* .gitconfig -> ~/dotfiles/.gitconfig
* .gitignore_global -> ~/dotfiles/.gitignore_global
