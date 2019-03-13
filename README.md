# dotfiles
Repo to keep my dotfiles in sync
Repo made based on [this](https://news.ycombinator.com/item?id=11070797) comment.

## Repo created using
```
git init --bare $HOME/.myconf
alias config='/usr/bin/git --git-dir=$HOME/.myconf/ --work-tree=$HOME'
config config status.showUntrackedFiles no
```
and adding files with
```
config add <filepath>
```
## To use the dotfiles quickly
Clone the repo with
```
git clone --separate-git-dir=$HOME/.myconf /path/to/repo $HOME/myconf-tmp
rm -r ~/myconf-tmp/
alias config='/usr/bin/git --git-dir=$HOME/.myconf/ --work-tree=$HOME'
```
Then use the alias ```config``` to work with the repo
