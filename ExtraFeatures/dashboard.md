# Jupyter 主面板介绍

打开Notebook，可以看到主面板。在菜单栏中有Files、Running、Clusters三个选项。用到最多的是Files，我们可以在这里完成notebook的新建、重命名、复制等操作。具体功能如下：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard1.png)

在Running中，可以看到正在运行的notebook，我们可以选择结束正在运行的程序。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard2.png)

一个notebook的编辑界面主要由四部分组成：名称、菜单栏、工具条以及单元(Cell)，如下图所示：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard3.png)

## 名称
在这里，我们可以修改notebook的名字，直接点击当前名称，弹出对话框进行修改： 

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard4.png)

## 菜单栏
菜单栏中有File、Edit、View、Insert、Cell、Kernel、Help等功能，下面逐一介绍。

### File
File中的按钮选项如下图所示：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard5.png)

具体功能如下表：

| 选项 | 功能 |
|--- |--- |
| New Notebook | 新建一个notebook |
| Open… | 在新的页面中打开主面板 |
| Make a Copy… | 复制当前notebook生成一个新的notebook |
| Rename… | notebook重命名 |
| Save and Checkpoint | 将当前notebook状态存为一个Checkpoint |
| Revert to Checkpoint | 恢复到此前存过的Checkpoint |
| Print Preview | 打印预览 |
| Download as | 下载notebook存为某种类型的文件 |
| Close and Halt | 停止运行并退出该notebook |

### Edit
Edit中的按钮选项如下图所示：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard6.png)

具体功能如下表：

| 选项 | 功能 |
|--- |--- |
| Cut Cells | 剪切单元 |
| Copy Cells | 复制单元 |
| Paste Cells Above | 在当前单元上方粘贴上复制的单元 |
| Paste Cells Below | 在当前单元下方粘贴上复制的单元 |
| Paste Cells & Replace | 替换当前的单元为复制的单元 |
| Delete Cells | 删除单元 |
| Undo Delete Cells | 撤回删除操作 |
| Split Cell | 从鼠标位置处拆分当前单元为两个单元 |
| Merge Cell Above | 当前单元和上方单元合并 |
| Merge Cell Below | 当前单元和下方单元合并 |
| Move Cell Up | 将当前单元上移一层 |
| Move Cell Down | 将当前单元下移一层 |
| Edit Notebook Metadata | 编辑notebook的元数据 |
| Find and Replace | 查找替换，支持多种替换方式：区分大小写、使用JavaScript正则表达式、在选中单元或全部单元中替换 |

### View
View中的按钮选项如下图所示：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard7.png)

具体功能如下表：

| 选项 | 功能 |
|--- |--- |
| Toggle Header | 隐藏/显示Jupyter notebook的logo和名称 |
| Toggle Toolbar | 隐藏/显示Jupyter notebook的工具条 |
| Cell Toolbar | 更改单元展示式样 |

View中的功能可以让用户更好的展示自己的notebook，但对编写代码、实现功能没有影响。

### Insert

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard8.png)

功能：在当前单元上方/下方插入新的单元。

### Cell

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard9.png)

| 选项 | 功能 |
|--- |--- |
| Run Cells | 运行单元内代码 |
| Run Cells and Select Below | 运行单元内代码并将光标移动到下一单元 |
| Run Cells and Insert Below | 运行单元内代码并在下方新建一单元 |
| Run All | 运行所有单元内的代码 |
| Run All Above | 运行该单元（不含）上方所有单元内的代码 |
| Run All Below | 运行该单元（含）下方所有单元内的代码 |
| Cell Type | 选择单元内容的性质 |
| Current Outputs | 对当前单元的输出结果进行隐藏/显示/滚动/清除 |
| All Output | 对所有单元的输出结果进行隐藏/显示/滚动/清除 |

### Kernel

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard10.png)

| 选项 | 功能 |
|--- |--- |
| Interrupt | 中断与内核连接（等同于ctrl-c） |
| Restart | 重启内核 |
| Restart & Clear Output | 重启内核并清空现有输出结果 |
| Restart & Run All | 重启内核并重新运行notebook中的所有代码 |
| Reconnect | 重新连接到内核 |
| Change kernel | 切换内核 |

### Help

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard11.png)

| 选项 | 功能 |
|--- |--- |
| User Interface Tour | 用户使用指南，非常棒的功能，带你全面了解notebook |
| Keyboard Shortcuts | 快捷键大全 |
| Notebook Help | notebook使用指南 |
| Markdown | Markdown使用指南 |
| Python…pandas | 各类使用指南 |
| About | 关于Jupyter Notebook的一些信息 |

### 工具条
工具条中的功能基本上在菜单中都可以实现，这里是为了能更快捷的操作，将一些常用按钮放了出来。下图是对各按钮的解释。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard12.png)

### 单元(Cell)
在单元中我们可以编辑文字、编写代码、绘制图片等等。对于单元的详细内容放在第五节中介绍。

对于Notebook中的单元，有两种模式：命令模式(Command Mode)与编辑模式(Edit Mode)，在不同模式下我们可以进行不同的操作。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard13.png)

如上图，在编辑模式(Edit Mode)下，右上角出现一只铅笔的图标，单元左侧边框线呈现出绿色，点Esc键或运行单元格(ctrl-enter)切换回命令模式。

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard14.png)

在命令模式(Command Mode)下，铅笔图标消失，单元左侧边框线呈现蓝色，按Enter键或者双击cell变为编辑状态。

- 命令模式下的快捷键

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard15.png)

- 编辑模式下的快捷键

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard16.png)

注意不要死记硬背，在使用过程中需要什么就去查，多用用就能记住了。

#### Cell的四种功能
Cell有四种功能：Code、Markdown、Raw NBConvert、Heading，这四种功能可以互相切换。Code用于写代码，Markdown用于文本编辑，Raw NBConvert中的文字或代码等都不会被运行，Heading是用于设置标题的，这个功能已经包含在Markdown中了。四种功能的切换可以使用快捷键或者工具条。

Code用于写代码，三类提示符及含义如下：

| 选项 | 功能 |
|--- |--- |
| In[ ] | 程序未运行 |
| In[num] | 程序运行后 |
| In[*] | 程序正在运行 |

Markdown用于编辑文本，给出常用的Markdown用法：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/dashboard17.png)

其他非常用的用法需要时可以再查阅。
