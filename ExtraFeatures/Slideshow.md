# Jupyter 幻灯片放映

Notebooks是教学和编写可解释代码的有效工具。无论是给同学讲解代码还是给老板汇报进展，一份动态、顺滑、有代码有图片的报告总会带来很好的效果。 

Jupyter Notebooks可轻松转换为幻灯片，将你的工作转换为图文并茂的生动报告，也许我们就不再需要PPT啦~

我们可以通过以下两个方式来实现：

- Jupyter的内置幻灯片

在你的notebook中，可以通过工具栏导航到 View → Cell Toolbar → Slideshow。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Slideshow1.png)

这时每个单元格顶部都会出现一个浅灰色条，您可以根据不同的五种特性自定义幻灯片，其中幻灯片是主要的呈现形式，还包括可以上下滑动的自幻灯片和浮动的碎片。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Slideshow2.png)

在设置完成后转到notebook所在的目录，执行以下代码：
```
jupyter nbconvert *.ipynb --to slides --post serve
```
其中 *.ipynb 就是你的文件全名

幻灯片将显示在本地8000端口。此外目录中将生成.html文件，您也可以从那里双击访问幻灯片。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Slideshow3.gif)

- RISE（Reveal.js  plugin）

jupyter的问题在于无法再运行幻灯片的时候运行代码，而RISE提供了边演示便运行的解决方案。

RISE是Reveal.js — Jupyter/IPython Slideshow Extension的首字母缩写。 

它利用reveal.js来运行幻灯片。这非常有用，因为它能在不必退出幻灯片的情况下运行代码。 使用如下命令进行安装：
```
# Using Conda
conda install -c conda-forge rise
# Using pip
pip install RISE
```
在适当的目录安装JS和 CSS:
```
jupyter-nbextension install rise --py --sys-prefix
# enable the nbextension
jupyter-nbextension enable rise --py --sys-prefix
```
现在我们就会发现一个新的扩展，上面写着“Enter/Exit RISE Slideshow.”。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Slideshow4.png)

边演示便运行真的很爽，是时候向老板展示你真正的实力了。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Slideshow5.gif)
