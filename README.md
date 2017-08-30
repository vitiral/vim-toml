# vim-toml

Vim syntax for [TOML](https://github.com/toml-lang/toml).

## Installation

### Pathogen

Set up [Pathogen](https://github.com/tpope/vim-pathogen) then clone/submodule this repo into `~/.vim/bundle/toml`, or wherever you've pointed your Pathogen.

### Vundle

Set up [Vundle](https://github.com/VundleVim/Vundle.vim) then add `Plugin 'cespare/vim-toml'` to your vimrc and run `:PluginInstall` from a fresh vim.

### vim-plug

Set up [vim-plug](https://github.com/junegunn/vim-plug). In your .vimrc, between the lines for `call plug#begin()` and `call plug#end()`, add the line `Plug 'cespare/vim-toml'`. Then run `:PlugInstall` from a fresh vim instance.

## Configuration
If you regularily deal with toml files which have literal strings greater than 500 lines, you can add this to your `.vimrc`:
```
autocmd FileType toml
    \ autocmd Syntax <buffer> syntax sync minlines=2000
```

Replace `minlines=2000` with whatever number you want.

## Contributing

Contributions are very welcome! Just open a PR.
