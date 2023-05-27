# Vim and Neovim notes

## Options

Set syntax highlighting:

```vim
:set syntax=<language>
```

## Plugins

- Conquer of Completion:
  - description: code completion
  - compatibility: vim, neovim
  - homepage: https://github.com/neoclide/coc.nvim

- vim-plug
  - description: plugin manager
  - compatibility: vim, neovim
  - homepage: https://github.com/junegunn/vim-plug

## Lua API for Neovim

Check status of `vim` object:

```vim
:lua print(vim.inspect(vim))
```
