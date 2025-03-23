# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## MkDocs 还挺有趣的！


[😋](pcl.html)



## 网站搭建

1. 本地创建项目
2. 启动服务
3. 添加页面
4. 本地预览
5. 发布站点

[参考文档](https://mkdocs-like-code.readthedocs.io/zh-cn/latest/get-started/create-program/)


### 多设备内容同步

两台电脑分别更新这个网站：huawei lenovo

一台设备更新内容后，会通过 mkdocs build 和 mkdocs gh-deploy，把内容更新到网站。
这个时候，主要更新的是 joul2.github.io/docs 这个网站中的内容。更新的是 github 中 docs 仓库的 gh-pages 分支。

为了便于另一台设备无缝衔接，还需要把本地的 docs 中所有修改的内容 push 到 github 中 docs 仓库的 main 分支。

我是怎么做的：

1. 在两台电脑都装好了 git
2. 用的是 git-gui。
3. 参考菜鸟教程先配置一些东西：https://www.runoob.com/w3cnote/git-gui-window.html
4. 之后 stage changed，commit，push，一般就能把本地的改动，同步push到main分支里。
5. 之后另一个电脑设置好 remote
6. 最后pull一下就行。这里我设置的有点问题，git gui 没有配置好。所以 pull 不成功的话，就打开 git bash，然后输入git pull \<remote name\>  \<branch name\> --allow-unrelated-histories
