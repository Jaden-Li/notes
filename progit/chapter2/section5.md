# 2.5 Working with Remotes

## Showing Your Remotes

```
$ git remote
```

会显示remote的名字，要查看remote的URL，增加`-v`

## Adding Remote Repositories

```
$ git remote add <shortname> <url>
```

现在你可以用shortname代指这个远程仓库

## Fetching and Pulling from Your Remotes

```
$ git fetch <remote>
```

`git fetch`会把远程仓库有的，但是你没有的，全都拿下来。而`git pull`除了fetch还会merge

![Remote tracking branch for `teamone/master`.](https://git-scm.com/book/en/v2/images/remote-branches-5.png)

## Pushing to Your Remotes

```
$ git push <remote> <branch>
```

要成功执行这个命令，需要具备两个条件，首先你有write access，然后没有其他正在push的人

## Inspecting a Remote

```
$ git remote show <remote>
```

展示Remote更多的信息

## Renaming and Removing Remotes

```
$ git remote rename pb paul
```

比方要把`pb`重命名为`paul`

```
$ git remote remove paul
```

如果你想移除`paul`

