# Git get [![Build Status](https://travis-ci.com/pietvanzoen/git-get.svg?branch=master)](https://travis-ci.com/pietvanzoen/git-get)

Like `go get`, `git-get` organizes repos in directories according to 1) host, 2) user, and 3) project name.

## Example

`git get git@github.com:pietvanzoen/dotfiles.git` will clone the project into `$GIT_PATH/github.com/pietvanzoen/dotfiles`.

## Installation

```bash
git clone https://github.com/pietvanzoen/git-get.git
cd git-get
INSTALL_DIR=<path to directory in your $PATH> ./install
```

If `$INSTALL_DIR` is not specified it will default to `$HOME/bin`.

That's it! `git get` automatically call `git-get`.
