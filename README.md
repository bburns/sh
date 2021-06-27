# sh

Settings for bash, zsh, and git.


## Setup

To install, clone this repository -

    cd ~
    git clone https://github.com/bburns/sh
    cd sh


## Setup Aliases

For Mac, add some lines to .zshrc and reload -

    echo "source ~/sh/aliases/common" >> ~/.zshrc
    echo "source ~/sh/aliases/macos" >> ~/.zshrc
    source ~/.zshrc

For Raspberry Pi, add some lines to .bashrc and reload -

    echo "source ~/sh/aliases/common" >> ~/.bashrc
    echo "source ~/sh/aliases/pi" >> ~/.bashrc
    source ~/.bashrc


## Setup Git

For git config, edit ~/.gitconfig to look like this - 

    [include]
    path = ~/sh/git/.gitconfig

    [github]
    user = <your userid>
    token = <your github token>
    oauth-token =

Changes will be available immediately.


## Developing

To add more aliases, edit one of

    aliases/common
    aliases/mac
    aliases/pi

or add an alias with eg

    echo "alias pok='pokpok -p'" >> aliases/common

Then commit all changes to repo and push to GitHub

    git add .
    git commit -m "added alias"
    git push

To load the new aliases, all terminals will need to be restarted, or say (an alias)

    reload

or on Mac could restart zshell with

    exec zsh


## License

MIT
