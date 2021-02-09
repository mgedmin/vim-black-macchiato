# vim-black-macchiato

## Description

This is a Vim plugin that provides integration with [black-macchiato][bm-url], which is a partial formatter for Python.

## Installation

### Vundle

```
Plugin 'smbl64/vim-black-macchiato'
```

## vim-plug

```
Plug 'smbl64/vim-black-macchiato'
```

## Features

You can use the `BlackMacchiato` command in normal mode to run `black-macchiato` on current line, or in visual mode to run it on the selection.

### Keybindings 

Put these in your `.vimrc` file:

```
autocmd FileType python xmap <buffer> <Leader>f <plug>(BlackMacchiatoSelection)
autocmd FileType python nmap <buffer> <Leader>f <plug>(BlackMacchiatoCurrentLine)
```

## Settings

### The `g:black_macchiato_path` option

Set this to your `black-macchiato` installation path. 

Default: `"black-macchiato"`

[bm-url]: https://github.com/wbolster/black-macchiato

