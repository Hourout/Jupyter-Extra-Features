# Jupyter 代码美化

jupyter 也可以实现像其它诸如 PyCharm、Spyder 等PythonIDE所具有的代码美化功能，但默认不会安装此功能，本篇文章将介绍如何实现 Jupyter Notebook 代码美化功能。


## Step 1 首先安装 nbextensions

```
pip install jupyter_contrib_nbextensions
jupyter contrib nbextension install --user
```

## Step 2 然后安装 nbextensions_configurator
```
pip install jupyter_nbextensions_configurator
jupyter nbextensions_configurator enable --user
```

如果提示缺少依赖，就使用pip安装对应依赖即可。

## Step 3 接着安装 jupyter-black
```
pip install black [--user]
# Installation dependency package
pip install yapf
```

jupyter-black 扩展提供以下功能

- 工具栏按钮
- 用于重新格式化当前代码单元的键盘快捷键（默认值：Ctrl-B）
- 用于重新格式化整个代码单元的键盘快捷键（默认值：Ctrl-Shift-B）

语法应该是正确的。该扩展还将指出基本语法错误。

## Step 4 最后重启jupyter

在弹出的主页面里，能看到增加了一个Nbextensions标签页，在这个页面里，勾选 Code prettify 选项即启用了代码美化功能，如图所示：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/prettify1.png)

在notebook中会出现一个小图标

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/prettify2.png)

设置完成后，我们来看看效果：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/prettify3.gif)
