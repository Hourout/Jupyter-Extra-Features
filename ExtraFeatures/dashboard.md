# Jupyter 主面板介绍

打开Notebook，可以看到主面板。在菜单栏中有Files、Running、Clusters三个选项。用到最多的是Files，我们可以在这里完成notebook的新建、重命名、复制等操作。具体功能如下：


在Running中，可以看到正在运行的notebook，我们可以选择结束正在运行的程序。


一个notebook的编辑界面主要由四部分组成：名称、菜单栏、工具条以及单元(Cell)，如下图所示：


## 名称
在这里，我们可以修改notebook的名字，直接点击当前名称，弹出对话框进行修改： 


## 菜单栏
菜单栏中有File、Edit、View、Insert、Cell、Kernel、Help等功能，下面逐一介绍。


### File
File中的按钮选项如下图所示：

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

具体功能如下表：

| 选项 | 功能 |
|--- |--- |
| Toggle Header | 隐藏/显示Jupyter notebook的logo和名称 |
| Toggle Toolbar | 隐藏/显示Jupyter notebook的工具条 |
| Cell Toolbar | 更改单元展示式样 |

View中的功能可以让用户更好的展示自己的notebook，但对编写代码、实现功能没有影响。

### Insert



功能：在当前单元上方/下方插入新的单元。

### Cell

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

| 选项 | 功能 |
|--- |--- |
| Interrupt | 中断与内核连接（等同于ctrl-c） |
| Restart | 重启内核 |
| Restart & Clear Output | 重启内核并清空现有输出结果 |
| Restart & Run All | 重启内核并重新运行notebook中的所有代码 |
| Reconnect | 重新连接到内核 |
| Change kernel | 切换内核 |


