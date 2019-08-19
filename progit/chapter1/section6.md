# 1.6 First-Time Git Setup

Git配置的基本命令`git config`

Git的配置文件储存位置按优先级排列：Repo中的`config`文件，也是默认值；`~/.gitconfig`，只影响当前用户，使用`--global`；`/etc/gitconfig`，影响所有用户，使用`--system`；

## Your Identity

```console
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

一个观察，如果参数有空格，需要用文本分隔符；如果没有，则可以省略。

## Your Editor

## Checking Your Settings

检查所有config

```console
$ git config --list
```

检查单个key

```console
$ git config user.name
```

查看所有配置文件的命令

```console
$ git config --list --show-origin
```

