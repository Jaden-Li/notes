# 3.6 Rebasing

在Git中，有两种合并分支的方法，一种是`merge`，还有一种是`rebase`

## The Basic Rebase

conflict产生

![Simple divergent history.](https://git-scm.com/book/en/v2/images/basic-rebase-1.png)

使用rebase，把experiment的改变叠加在base上（C3）

```
$ git checkout experiment
$ git rebase master
```

![Rebasing the change introduced in `C4` onto `C3`.](https://git-scm.com/book/en/v2/images/basic-rebase-3.png)

最后，将master fast-forward一下

```
$ git checkout master
$ git merge experiment
```

![Fast-forwarding the master branch.](https://git-scm.com/book/en/v2/images/basic-rebase-4.png)

## More Interesting Rebases

如果有两条需要rebase，如下图

![A history with a topic branch off another topic branch.](https://git-scm.com/book/en/v2/images/interesting-rebase-1.png)

比方说，先base client onto master

```
$ git rebase --onto master server client
```

这条命令在说，把client拿出来，找出和server的区别，然后将这些区别叠加在master branch上。接下来可以把master fast-forward一下

```
$ git checkout master
$ git merge client
```

![Fast-forwarding your master branch to include the client branch changes.](https://git-scm.com/book/en/v2/images/interesting-rebase-3.png)

第二条需要rebase的线是server

```
$ git rebase master server
```



![Rebasing your server branch on top of your master branch.](https://git-scm.com/book/en/v2/images/interesting-rebase-4.png)

rebase后，常规操作，merge

```console
$ git checkout master
$ git merge server
```

最后，清理掉不需要的branch

![Final commit history.](https://git-scm.com/book/en/v2/images/interesting-rebase-5.png)

## The Perils of Rebasing

不要在remote上rebase东西

> **Do not rebase commits that exist outside your repository and people may have based work on them.**

## Rebase When You Rebase

真的有人干出了rebase remote commits这种事情，Git有办法解决

## Rebase vs. Merge

General Guideline：本地使用rebase