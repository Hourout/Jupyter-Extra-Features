# Jupyter 插入常用代码片

在我们平时写代码过程中存在很多可以复用的代码片，俗称“搬砖”。

比如说每次代码开头都需要import一大堆包和一些常用的数据操作、绘图指令。

为了便捷的复用这些指令，Snippets功能为我们提供了一键插入预先设置的代码片段的功能，从此再也不用辛苦的输入那些常用的指令，甚至copy-paste都免了，轻轻一点代码出现！

此扩展插件为Notebook工具栏添加了一个下拉菜单，允许将代码片段单元格轻松插入当前Notebook中。

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

在弹出的主页面里，能看到增加了一个Nbextensions标签页，在这个页面里，勾选 Snippets 或 Snippets Menu 选项即启用了插入常用代码片功能，如图所示：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Snippets1.png)

设置完成后，我们来看看效果：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Snippets2.gif)

需要注意的是，Snippets默认只有一个example功能，若要自定义你的代码块，你需要找到你的jupyter存储Nbextensions的路径，可以在jupyter中运行以下代码查找：
```
get_ipython().getoutput('jupyter --data-dir')
```
找到文件夹后在Nbextensions文件夹中找到~/jupyter/nbextensions/snippets/snippets.json文件，没有可以自己创建，snippets.json默认只有以下代码：
```
{
    "snippets" : [
        {
            "name" : "example",
            "code" : [
                "# This is an example snippet!",
                "# To create your own, add a new snippet block to the",
                "# snippets.json file in your jupyter data directory under nbextensions:",
                "# $(jupyter --data-dir)/nbextensions/snippets/snippets.json",
                "import this"
            ]
        }
    ]
}
```
要想自己自定义新的代码段，可以参照以下写法：
```
{
    "snippets" : [
        {
            "name" : "example",
            "code" : [
                "# This is an example snippet!",
                "# To create your own, add a new snippet block to the",
                "# snippets.json file in your jupyter data directory under nbextensions:",
                "# $(jupyter --data-dir)/nbextensions/snippets/snippets.json",
                "import this"
            ]
        },
        {
            "name" : "some imports",
            "code" : [
                "import numpy as np",
                "import matplotlib as mpl",
                "print('spam')"
            ]
        }
    ]
}
```
这样你的Snippets就会出现"some imports"的选项了，如下所示：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Snippets3.png)
