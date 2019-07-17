# Jupyter 单元格分置

Jupyter 的默认窗口设置每个cell都是从上到下依次排列的，就像下面这样：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Split_Cells_Notebook1.png)

很多IDE都支持多窗口编辑、查看代码。当然jupyter也可以实现这样的功能。在notebook中split功能为我们贴心地准备了这个功能，只需轻轻一点就可以将原先垂直顺序排列的单元格变成水平排列，更好的查看与分析代码和计算结果。通过该扩展插件可以将Notebook的单元格分开，再将它们相邻放置。

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

在弹出的主页面里，能看到增加了一个Nbextensions标签页，在这个页面里，勾选 Split Cells Notebook 选项即启用了单元格分置功能，如图所示：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Split_Cells_Notebook2.png)

设置完成后，我们来看看效果：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Split_Cells_Notebook3.gif)
