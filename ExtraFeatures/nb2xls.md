# Jupyter notebooks 转换成 Excel 电子表格

将Jupyter笔记本转换为Excel Spreadsheets（xlsx），通过新的“Download As”选项或通过命令行上的nbconvert转换。

- 功能适配 Pandas DataFrames等表格。还导出图像数据，如matplotlib输出。
- 尽可能支持Markdown（某些元素仍需要工作）。
- 输入（代码）单元格不包含在电子表格中。
- 这允许您与非程序员共享您的结果，以便他们仍然可以轻松地使用数据。

## Step 1 首先安装表格转换库 nb2xls

```
pip install nb2xls
```

## Step 2 然后重启jupyter

- 方法一

重新启动Jupyter以在“文件”菜单中的“Download As”下选择新的“Excel电子表格（.xlsx）”选项。

- 方法二

要从命令行运行，请尝试：
```
jupyter nbconvert --to xls Examples/ExcelTest.ipynb
```
或者
```
jupyter nbconvert --to nb2xls.XLSExporter Examples/ExcelTest.ipynb
```
这应该在与指定的ipynb文件相同的文件夹中输出ExcelTest.xlsx。

设置完成后，我们来看看效果：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Jupyter2Excel.png)
