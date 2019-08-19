# 3.5 Remote Branches

## 基础知识

![Server and local repositories after cloning.](https://git-scm.com/book/en/v2/images/remote-branches-1.png)

远程的branch和本地的区别：远程有/。即使远程的master发生了改变，只要你不连接远程，它在本地还是不变。

[更新远程master](chapter2/section5.html/fetching-and-pulling-from-your-remotes)

## Pushing

```
$ git push <remote> <branch>
```

关于`<branch>`，`git push origin serverfix:awesomebranch`表示把本地名为serverfix的分支push到远程的awesomebranch上。

如何把远程的分支merge到本地当前的branch中：

```
$ git merge origin/serverfix
```

如何复制远程的分支到本地

```
$ git checkout -b <branch> <remote>/<branch>
```

## Tracking Branches

把远程的branch复制到本地，就是Tracking branches，特殊之处在于，使用`git pull`会直接merge branch

```
$ git branch -vv
```

查看本地branch，包含Tracking branches的信息，包括tracking branches是ahead还是behind remote branches，但这些信息都是cached，如果想要最新的信息，首先执行以下命令

```
$ git fetch --all
```



## Pulling

`git pull`是`git fetch`和`git merge`的结合，通常不建议使用。

## Deleting Remote Branches

删除掉服务端的branches

```
$ git push origin --delete <branch name>
```

