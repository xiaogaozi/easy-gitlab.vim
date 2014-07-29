# easy-gitlab.vim

This plugin was forked from
[github-vim](https://github.com/solars/github-vim), but use with [GitLab](https://about.gitlab.com).

## Description

This is a quick and dirty Vim plugin to use some GitLab features locally from Vim.

It enables you to:

- Open a link to the corresponding GitLab file of a local Vim selection
- Add a comment to the corresponding GitLab commit of a locally selected line

## Installation

Install using [pathogen.vim](https://github.com/tpope/vim-pathogen), [Vundle](https://github.com/gmarik/Vundle.vim), [NeoBundle](https://github.com/Shougo/neobundle.vim), or your favorite Vim package manager.

## Usage

Set `g:easy_gitlab_url` in your `~/.vimrc` file:

```
let g:easy_gitlab_url = 'http://git.example.com'
```

Then you can:

- Open selection: create a selection in visual mode and press `glo`
- Comment commit: on the relevant line press `glc` in normal mode

To remap the keybinding in your `~/.vimrc` use:

- `map <F5> <Plug>GitlabOpen`
- `map <F6> <Plug>GitlabComment`
