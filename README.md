# Git get [![Build Status](https://travis-ci.com/pietvanzoen/git-get.svg?branch=master)](https://travis-ci.com/pietvanzoen/git-get)

Like `go get`, `git-get` organizes repos in directories matching the path of the clone url.

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

## Tips

* Use `git get` alongside [autojump](https://github.com/wting/autojump) to effortlessly navigate your folder structure.
* `git get` will only output the cloned directory path to stdout. So you can setup a helper function in your dotfiles like this for easy cloning: `gg() { cd $(git get $1) }`
