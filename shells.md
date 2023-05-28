## Bash

Reference Manual: https://www.gnu.org/software/bash/manual/bash.html

## Zsh

Homepage: https://www.zsh.org/

## Block auto-logout

To avoid auto-logout

exec env TMOUT=0 *shell*

E.g.:

```console
exec env TMOUT=0 bash
```
