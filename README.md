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
* Clone and change directory in the same command. Add this to your shell environment files: `gg() { cd $(git get $1) }`

## See also

* [ghq](https://github.com/motemen/ghq) - A more feature full approach to managing repos in a `go get` way. Written in go.
* [h](https://github.com/zimbatm/h) - Combines the ideas of `git get` with `autojump` into one package. Written in python.
