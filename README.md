# 介绍

这个repo包括了：

- 读书笔记
  - `公务员`包含国考和省考相关的资料；
  - `progit`包含Pro Git的读书笔记
- 一些废话
  - 放在`other`中

# 如何查看

将想看的文件克隆至本地，用Terminal定位至该文件夹，创建book.json，复制并保存以下命令

```json
{
	"plugins": [
    "mathjax",
    "page-toc-button"
],
	"pluginsConfig": {
 		"page-toc-button": {
            "maxTocDepth": 2,
            "minTocSize": 2
           }
    }

}
```

然后运行一下命令

```
$ gitbook serve
```
