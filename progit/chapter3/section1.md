# 3.1 Branches in a Nutshell

## 基础知识

分支，指向某个commit。在了解分支之前，先了解commit对象。该对象储存了两类信息，当前commit的数据，即sanpshot和父分支。

1. **Snapshot**

Snapshot储存了文件结构（tree），和文件的版本信息（blob）

![image-20190819162259135](assets/section1/image-20190819162259135.png)

2. **父分支**

指向前一个或多个commit对象。若是当前对象是首次commit，则没有父分支。

![image-20190819162129816](assets/section1/image-20190819162129816.png)

## Branch的概念

A branch本质上是一个指向某个commit object的pointer；HEAD指向当前所在branch

![image-20190819163549440](assets/section1/image-20190819163549440.png)

diverged branches的概念，两个有着common ancestor的branches指向了不同的commit objects

![image-20190819164544666](assets/section1/image-20190819164544666.png)



## Creating a New Branch

```
$ git branch testing
```

创建了一个名为testing的branch，指向当前commit

![image-20190819163709917](assets/section1/image-20190819163709917.png)

如果想直接switch到这个branch，使用

```
$ git checkout -b testing
```



## Switching Branches

```
$ git checkout testing
```

将HEAD指向testing，之后若再做出commit，那只是对testing这个branch的指向作出改变

![image-20190819164202816](assets/section1/image-20190819164202816.png)

如果之后，再移动到master这个branch，工作区所有的文件都会被复原到`f30ab`这个commit中储存的snapshot下

