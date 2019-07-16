# Jupyter 使用Julia语言

Jupyter命名由来最初的思想是来自julia、python 和 R 三种编程语言的简称，所以当然我们也要让jupyter支持Julia语言啦。

安装方法也很简单，只要在julia语言的环境下安装一个 "IJulia" 就好了。

## Step 1 安装Julia语言
Julia语言的安装非常简单，和python一样直接去对应官网下载文件按照提示下一步就可以了，最好下载1.1以上版本。 

下载地址：[Julia官网下载地址](https://julialang.org/downloads/)

## Step 2 配置jupyter路径（可选）
在安装IJulia时，如果你没有事先配置好jupyter路径，那么它会自动下载安装一个jupyter。

建议大家在使用jupyter时，只是将Julia添加进去，因为这样可以玩转更多语言。

如果你只是为了体验Julia，无所谓Python和Jupyter的版本，那你可以跳过这一步骤。

- 首先找到你的jupyter路径，打开终端，运行如下命令
```
where jupyter
```
返回你的jupyter路径

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/julia1.png)

- 接着打开Julia语言终端，输入命令
 ```
 ENV["JUPYTER"]="C:\\Users\\JinqingLee\\AppData\\Local\\Programs\\Python\\Python36\\Scripts\\jupyter"
 ```

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/julia2.png)

## Step 3 安装 jupyter IJulia 内核
- 在1.0以后的版本，安装 IJulia 内核正确做法是在英文模式下按]键入pkg模式（中文模式会输入】）

然后直接在Julia语言终端继续输入命令
```
add IJulia
```
若出现请求超时，多试几次即可

- 另一种方式则是采用using模式，直接在Julia语言终端输入命令
```
using Pkg
Pkg.add("IJulia")
```

## Step 4 重启jupyter
重新启动后就可以看到如下页面：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/julia3.png)

然后就可以在jupyter上进行编程了

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/julia4.png)
