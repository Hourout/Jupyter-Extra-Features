# Jupyter Widgets 魔法工具包

Widgets是在jupyter里具有代表性的多事件python对象，通常作为滑块、文本框等控件使用。Widgets可用于构建交互式图形用户界面。 通过以下命令来安装它们：
```
# Using pip
pip install ipywidgets
jupyter nbextension enable --py widgetsnbextension
# Using conda
conda install -c conda-forge ipywidgets
```

其中包含了一系列优秀的可视化交互控件，从参数调整到文件遍历，从颜色拾取到绘图风格变换，丰富且有用的小工具你一定会喜欢的。

## 交互控件

这是IPython中widgets最简单的使用方法。

交互功能（ipywidgets.interact）会自动为代码和数据创建用户界面（UI）控件。

在数据探索过程中，通常要一次又一次地重新运行相同的单元，而每次都只会稍微改变下输入参数，这种致操作方式效率十分低下。理想解决方案是使用交互式控件，无需重写或重新运行代码即可更改输入。 

使用IPython widgets（ipywidgets），您可以使用一行代码构建交互式控件。该库允许我们将Jupyter Notebooks从静态文档转换为交互式仪表板，非常适合数据的探索和可视化数据。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets1.png)

我们可以使用 @interact 修饰器快速将任何普通函数转换为交互式控件，例如改变x的取值：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets2.png)

快速循环遍历所有图像，而无需重新运行单元程序。 如果调试卷积神经网络并想要检查网络错分类的图像，这招就很管用。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets3.png)

Widgets在数据探索方面的用途是多种多样的。 还可以用来便捷地分析两列数据间的相关性，对于数据科学家和统计学家十分有用。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets4.png)

## 播放控件

Play widget能以一定速度按照整数序列来循环播放动画，并可以通过滑块的值来控制播放相关参数。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets5.png)

## 日期选择器控件

日期选择器控件Date picker可在Chrome和IE Edge中使用，但目前暂时无法在Firefox或Safari中使用，因为它们不支持HTML日期输入字段。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets6.png)

## 颜色选择控件

Color picker 可以调出调色板，供你选择最中意的颜色：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets7.png)

## 表格控件

表格控件Tab可以构建类似excel的表格，便于展示和可视化数据：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets8.png)

## Widgets for Plots 绘图控件

交互式控件对于选择数据绘制特别有用，我们同样可以使用@interact修饰器将数据可视化函数转为控件：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets9.png)

这里，cufflinks+plotly的组合用来实现交互式绘图。如果绘图的更新速度有点慢，我们可以使用@interact_manual，手动点击按钮来进行更新。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets10.gif)

## Qgrid

Qgrid主要关注DataFrame对象。 它使用SlickGrid在Jupyter notebook中渲染pandas DataFrame。 这使您可以使用直观的滚动、排序和筛选控件来浏览DataFrame，还可以通过双击单元格来编辑DataFrame，可以便捷高效的查看dataframe中的数据：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/widgets11.gif)
