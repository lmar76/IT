# Vim and Neovim notes

## Options

Set syntax highlighting:

```vim
:set syntax=<language>
```

## Plugins

Vim/Neovim plugins.

- Conquer of Completion:
  - description: code completion
  - compatibility: vim, neovim
  - links: https://github.com/neoclide/coc.nvim

- lazy.nvim
  - description: plugin manager
  - compatibility: neovim
  - links: https://github.com/folke/lazy.nvim

- packer.nvim
  - description: plugin manager
  - compatibility: neovim
  - links: https://github.com/wbthomason/packer.nvim

- vim-plug
  - description: plugin manager
  - compatibility: vim, neovim
  - links: https://github.com/junegunn/vim-plug

## Distributions

Vim/Neovim distributions/configurations.

- kickstart.nvim
  - description: A starting point for Neovim
  - compatibility: neovim
  - links: https://github.com/nvim-lua/kickstart.nvim

- LazyVim
  - description: Neovim setup powered by lazy.nvim
  - compatibility: neovim
  - links:
    - https://www.lazyvim.org/
    - https://github.com/LazyVim/LazyVim

## Lua API for Neovim

Check status of `vim` object:

```vim
:lua print(vim.inspect(vim))
```
