## Apply patch

git apply patch *filename*, where *filename* is a `.patch` file. E.g.:

```console
git apply patch biomasspy.patch
```

## Archive export

git archive --format tar.gz --output *filename* --prefix *prefix* *branch*

E.g.:

```sh
$ git archive --format tar.gz --output ~/sara-config.tar.gz --prefix sara-config/ master
```

## Delete branches

Delete branch locally:

```
git branch -d localBranchName
```

Delete branch remotely:

```
git push origin --delete remoteBranchName
```

## How to tell which commit a tag points to in Git?

git log *tagname*

or:

git rev-list *tagname*

## List files being tracked

To list files being tracked under branch branch:

git ls-tree -r *branch* --name-only

E.g.:

```console
git ls-tree -r master --name-only
```

## Notebooks repository

Workflow:

1. Update notebook on branch. Clear outputs and save.
2. Commit and push.
3. Change to master.
4. Rebase.
5. Execute notebook.
6. Commit with `--amend` option.
7. Force push.

Rebasing after modifying a notebook:

git rebase -X ours *branch*

E.g.:

```sh
$ git rebase -X ours development
```

Commit with `--amend` option:

git commit -a --amend -m *comment*

E.g.:

```sh
$ git commit -a --amend -m 'Notebook re-executed'
```

Force push:

git push --force

## Reset repository

```sh
$ git reset --hard
```
