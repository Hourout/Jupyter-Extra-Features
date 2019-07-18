# Jupyter 魔法函数

使用魔法函数可以简单的实现一些单纯python要很麻烦才能实现的功能。

- %：行魔法函数，只对本行代码生效。 
- %%：Cell魔法函数，在整个Cell中生效，必须放于Cell首行。 
- %lsmagic：列出所有的魔法函数 
- %magic查看各个魔法函数的说明 
- ?后面加上魔法函数名称，可以查看该函数的说明

一些常用魔法函数的示例：

| 魔法函数 | 作用 |
|--- |--- |
| %%writefile | 调用外部python脚本 |
| %run | 调用外部python脚本 |
| %timeit | 测试单行语句的执行时间 |
| %%timeit | 测试整个单元中代码的执行时间 |
| % matplotlib inline | 显示 matplotlib 包生成的图形 |
| %%writefile | 写入文件 |
| %pdb | 调试程序 |
| %pwd | 查看当前工作目录 |
| %ls | 查看目录文件列表 |
| %reset | 清除全部变量 |
| %who | 查看所有全局变量的名称，若给定类型参数，只返回该类型的变量列表 |
| %whos | 显示所有的全局变量名称、类型、值/信息 |
| %xmode Plain | 设置为当异常发生时只展示简单的异常信息 |
| %xmode Verbose | 设置为当异常发生时展示详细的异常信息 |
| %debug | bug调试，输入quit退出调试 |
| %env | 列出全部环境变量 |

注意这些命令是在Python kernel中适用的，其他 kernel 不一定适用
