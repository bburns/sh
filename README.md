# sh

Settings for bash and zsh and various applications.


## Install

To install, clone this repository -

    cd ~
    git clone https://github.com/bburns/sh
    cd sh


## Aliases

Add lines to .zshrc or .bash -

    echo "source ~/sh/alias/common" >> ~/.zshrc
    echo "source ~/sh/alias/macos" >> ~/.zshrc

    echo "source ~/sh/alias/common" >> ~/.bashrc
    echo "source ~/sh/alias/macos" >> ~/.bashrc

Then restart terminal or reload file -

    source ~/.zshrc

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
