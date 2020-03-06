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

`./install` installs as symlinks into `~/` making a `filename.bak` for any file it's about to overwrite with a symlink unless it's pointing to ourselves already.
