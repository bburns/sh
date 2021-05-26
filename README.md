# sh

Settings for bash and zsh and various applications.


## Install

To install, clone this repository -

    cd ~
    git clone https://github.com/bburns/sh
    cd sh


## Aliases

For Mac, add some lines to .zshrc and reload -

    echo "source ~/sh/alias/common" >> ~/.zshrc
    echo "source ~/sh/alias/macos" >> ~/.zshrc
    source ~/.zshrc

For Raspberry Pi, add some lines to .bashrc and reload -

    echo "source ~/sh/alias/common" >> ~/.bashrc
    echo "source ~/sh/alias/pi" >> ~/.bashrc
    source ~/.bashrc


## Git

For git config, edit ~/.gitconfig to look like this - 

    [include]
    path = ~/sh/git/.gitconfig

    [github]
    user = bburns
    oauth-token =
    token = <your github token>

Changes will be available immediately.
