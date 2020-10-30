# Settings

## General

```vim
if has("autocmd")
  filetype plugin indent on
	autocmd FileType python setlocal et sw=4 sts=4 sta
	autocmd FileType xml setlocal ts=4 sw=4 sts=4 sta
	autocmd FileType xsd setlocal ts=4 sw=4 sts=4 sta
	autocmd FileType xslt setlocal ts=4 sw=4 sts=4 sta
endif

if exists("+autochdir")
	set autochdir
endif

map <F12> :colo evening <enter>
```

Additional option for Python:`tw=78`

## Descrizione

**tabstop** oppure **ts**: larghezza del carattere TAB, quando incontrato nel file. Noi non useremo caratteri TAB quindi questa impostazione ò essere ignorata (e non è  riportata infatti nell'esempio precedente). Viene elencata qui solo per chiarezza e completezza.

**expandtab** oppure **et**: riempe con spazi le indentazioni generate dalla pressione del tasto TAB.

**softtabstop** oppure **sts**: larghezza di un rientro causato dalla pressione di un TAB. Il rientro è reato inserendo spazi se è settato, altrimenti viene usata una combinazione di spazi e caratteri TAB (questi ultimi hanno larghezza ts).

**shiftwidth** oppure **sw** larghezza di un rientro dell'indentazione automatica. È usato anche per definire la larghezza del rientro che si aggiunge o toglie ad un blocco di testo quando si seleziona (con v) e poi si indenta/deindenta con > o con <.

**smarttab** oppure **sta**: In combinazione con le opzioni precedenti questa impostazione permette di cancellare un rientro (4 spazi reali nel nostro caso) con una sola pressione del tasto BS (o BackSpace).

# Syntax

## Set syntax language

```vim
:set syntax=language
```
