# 4.3 Generating Your SSH Public Key

## 基础

ssh储存在`~/.ssh`中，如果要生成SSH，执行以下命令

```console
$ ssh-keygen -o
```

然后打开`id_dsa.pub`复制即可

```console
$ cat ~/.ssh/id_rsa.pub
```

