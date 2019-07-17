# Jupyter 折叠单元格

代码写的太长、注释写的太多、整个note太乱了，又长又没有清晰的结构该如何是好呀？

Collapsible Headings允许Notebook根据标题来分隔的可折叠部分。

如果Notebook中有很多不整洁的代码，我们就可以折叠起来免除了反复滚动的烦恼，同时也为整个notebook带来了整洁的视觉体验。

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

## Step 3 最后重启jupyter

在弹出的主页面里，能看到增加了一个Nbextensions标签页，在这个页面里，勾选 Collapsible Headings 选项即启用了折叠单元格功能，如图所示：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Collapsible_Headings1.png)

设置完成后，我们来看看效果：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Collapsible_Headings2.gif)
