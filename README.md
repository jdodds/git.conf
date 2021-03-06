![](https://github.com/jdodds/git.conf/workflows/shellcheck/badge.svg)
---
# git.conf

what it says on the tin.

## things you might care about:
+ we set `eol=true` and don't use `autocrlf`. If you want crlf locally, you'll need to change that
+ `git show-alias` is the most useful alias
+ `branch.sort -committerdate` sorts `git branch` by most recently updated
+ `help.autoCorrect 1` makes git just run the command instead of mocking you
+ `rerere` is on
+ `showbranch` defaults to having `HEAD` and `master`
+ `~/.gitconfig.local` gets sourced
+ if you have [delta](https://github.com/dandavison/delta) we use it for `core.pager`, it's set in `~/.gitconfig.local`


## installing

`./install` symlinks this gitconfig to your `$HOME/.gitconfig`, creating a backup first. We also use `$HOME/.gitconfig.local` to set `core.pager`, but don't touch it if you're already using delta and preserve the rest of it's contents in-file.
