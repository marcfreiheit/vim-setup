# Vim setup

## Pre-Reqs

You must have installed:

- python (brew install python3)
- cmake (brew install cmake)
- typescript
- [powerline fonts](https://github.com/powerline/fonts)

## Installation

Run the following commands to install this vim setup:

```
pushd ~
git clone --recurse-submodules -j8 git@github.com:marcfreiheit/vim-setup.git .vim
ln .vim/.vimrc .vimrc
pushd .vim/bundle/YouCompleteMe
python install.py
popd
# Install dependency of tsuquyomi
pushd ~/.vim/bundle/vimproc.vim
make
popd
popd
```
