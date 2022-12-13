# Settings

## General

```vim
set nocompatible            " disable compatibility to old-time vi
set showmatch               " show matching 
"set ignorecase             " case insensitive 
set hlsearch                " highlight search 
set incsearch               " incremental search
set tabstop=4               " number of columns occupied by a tab 
set softtabstop=4           " see multiple spaces as tabstops so <BS> does the right thing
set expandtab               " converts tabs to white space
set shiftwidth=4            " width for autoindents
set autoindent              " indent a new line the same amount as the line just typed
"set number                 " add line numbers
set wildmode=longest,list   " get bash-like tab completions
set cc=80                   " set an 80 column border for good coding style
set mouse=a                 " enable mouse click
set clipboard=unnamedplus   " using system clipboard
set cursorline              " highlight current cursorline
set ttyfast                 " Speed up scrolling in Vim
set spell                   " enable spell check (may need to download language package)
set sta
set autochdir

filetype plugin indent on   " allow auto-indenting depending on file type
filetype plugin on
syntax enable               " syntax highlighting

colo evening
```

Additional option for latex:`tw=78`

## Descrizione

**tabstop** oppure **ts**: larghezza del carattere TAB, quando incontrato nel file. Noi non useremo caratteri TAB quindi questa impostazione ò essere ignorata (e non è  riportata infatti nell'esempio precedente). Viene elencata qui solo per chiarezza e completezza.

**expandtab** oppure **et**: riempe con spazi le indentazioni generate dalla pressione del tasto TAB.

**softtabstop** oppure **sts**: larghezza di un rientro causato dalla pressione di un TAB. Il rientro è reato inserendo spazi se è settato, altrimenti viene usata una combinazione di spazi e caratteri TAB (questi ultimi hanno larghezza ts).

**shiftwidth** oppure **sw** larghezza di un rientro dell'indentazione automatica. È usato anche per definire la larghezza del rientro che si aggiunge o toglie ad un blocco di testo quando si seleziona (con v) e poi si indenta/deindenta con > o con <.

**smarttab** oppure **sta**: In combinazione con le opzioni precedenti questa impostazione permette di cancellare un rientro (4 spazi reali nel nostro caso) con una sola pressione del tasto BS (o BackSpace).

# Plugins

Plugin Manager: [junegunn/vim-plug](https://github.com/junegunn/vim-plug)

Conquer of Completion: [neoclide/coc.nvim](https://github.com/neoclide/coc.nvim)

# Syntax

## Set syntax language

```vim
:set syntax=language
```
