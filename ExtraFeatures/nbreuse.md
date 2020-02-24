# Jupyter 资源监控

jupyter 也可以实现监控资源使用情况，它显示当前笔记本计算机及其子代（内核，终端等）正在使用多少资源。它显示在笔记本计算机本身的主工具栏中，每5s刷新一次。


## Step 1 直接安装 nbresuse

```
pip3 install nbresuse
```

如果您的jupyter notebook<5.3，则需要手动启用扩展名。
```
jupyter serverextension enable --py nbresuse --sys-prefix
jupyter nbextension install --py nbresuse --sys-prefix
jupyter nbextension enable --py nbresuse --sys-prefix
```

## Step 2 重启jupyter

在弹出的主页面里，能看到增加了一个Nbextensions标签页，在这个页面里，勾选 nbreuse 选项即启用了代码美化功能，如图所示：

![](/image/nbreuse1.png)

设置完成后，我们来看看效果：

![](/image/nbreuse.png)
