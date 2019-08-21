# 3.5 Remote Branches

## 基础知识

remote references和remote-tracking branches都储存了远程分支的状态，但他们是两个不同的概念，区别如下：

- 被储存的位置不同：前者存在**远程**仓库，后者存在**本地**仓库
- 储存的分支状态的时间点不同：前者**实时**更新，后者储存**最近一次**连接远程仓库时远程分支的状态
- 后者以`<remote>/<branch>`的形式显示，`origin`是`<remote>`的默认名

[使用fetch来更新远程分支状态](chapter2/section5.html/fetching-and-pulling-from-your-remotes)

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

