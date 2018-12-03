# Git get [![Build Status](https://travis-ci.com/pietvanzoen/git-get.svg?branch=master)](https://travis-ci.com/pietvanzoen/git-get)

Like `go get`, `git-get` organizes repos in directories according to 1) host, 2) user, and 3) project name.

## Example

`git get git@github.com:pietvanzoen/dotfiles.git` will clone the project into `$GIT_PATH/github.com/pietvanzoen/dotfiles`.

## Installation

```bash
cd <where-you-want-the-script>
curl -O https://gist.githubusercontent.com/pietvanzoen/92c47aa810506ec113e42667fc6e1b7d/raw/git-get
chmod +x git-get
git config --global alias.get '!<path-to-script>/git-get'
```

Then add `export GIT_PATH=$HOME/repos` into your shell profile such as `.bash_profile`, `.bashrc` or `.zshrc` and close and restart your shell.
