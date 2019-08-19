# 2.4 Undoing Things

## Add Staged Files To The Previous Commit

场景：已经[commit](#Commit)掉，发现有些files忘记stage了，但是又不想又写一次同样的message，可以执行以下操作

```
$ git commit -m 'initial commit'
$ git add forgotten_file
$ git commit --amend //看这里
```

## Unstaging a Staged File

场景：stage掉两个files，但是本来想分开commit的

```
$ git add *
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage) //看这里，git有提示你怎么unstage

    renamed:    README.md -> README
    modified:   CONTRIBUTING.md
```

## Unmodifying a Modified File

场景：某个file还没被stage掉，想复原回以前的样子

```
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory) ////看这里，git有提示你怎么unmodify

    modified:   CONTRIBUTING.md
```

