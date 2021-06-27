# sh

Settings for bash, zsh, and git.


## Setup

To install, clone this repository -

    cd ~
    git clone https://github.com/bburns/sh
    cd sh


## Setup Aliases

For Mac, add some lines to .zshrc and reload -

    echo "source ~/sh/alias/common" >> ~/.zshrc
    echo "source ~/sh/alias/macos" >> ~/.zshrc
    source ~/.zshrc

For Raspberry Pi, add some lines to .bashrc and reload -

    echo "source ~/sh/alias/common" >> ~/.bashrc
    echo "source ~/sh/alias/pi" >> ~/.bashrc
    source ~/.bashrc


## Setup Git

For git config, edit ~/.gitconfig to look like this - 

    [include]
    path = ~/sh/git/.gitconfig

    [github]
    user = bburns
    oauth-token =
    token = <your github token>

Changes will be available immediately.


## Developing

To add more aliases, edit one of

    alias/common
    alias/macos
    alias/pi

or add an alias with eg

    echo "alias pok='pokpok -p'" >> alias/common

Then commit all changes to repo and push to GitHub

    git add .
    git commit -m "added alias"
    git push

To load the new aliases, all terminals will need to be restarted, or say (an alias)

    reload


## License

MIT
