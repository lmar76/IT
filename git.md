# Archive export

git archive --format tar.gz --output filename --prefix prefix master

E.g.:

```sh
$ git archive --format tar.gz --output ~/sara-config.tar.gz --prefix sara-config/ master
```

# How to tell which commit a tag points to in Git?

git log tagname

or:

git rev-list tagname

# List files being tracked

To list files being tracked under branch branch:

git ls-tree -r branch --name-only

E.g.:

```sh
$ git ls-tree -r master --name-only
```

# Notebooks repository

Rebasing after modifying a notebook:

git rebase -X ours dev
