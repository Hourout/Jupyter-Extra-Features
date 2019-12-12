# Jupyter 使用R语言

Jupyter命名由来最初的思想是来自julia、python 和 R 三种编程语言的简称，所以当然我们也要让jupyter支持R语言啦。

安装方法也很简单，只要在R语言的环境下安装一个 "IRkernel" 就好了。

## Step 1 安装R语言
R语言的安装非常简单，和python一样直接去对应官网下载文件按照提示下一步就可以了。 

下载地址：[R官网下载地址](https://cloud.r-project.org/)

CentOS系统可以命令在线安装：
```
1.通过如下命令安装并启用 EPEL （如果已经安装过，直接执行第二步）

yum install epel-release

2.使用如下命令安装R

yum install R

3.安装完成之后，直接在终端输入R然后回车之后出现类似如下内容则表示安装成功

[root@siger-node1 local]# R
```

## Step 2 安装 Rstudio (可选，不喜欢客户端的 IDE 可以直接跳过)
对于大多数工程师来说，IDE还是离不开的工具，R的IDE还是推荐Rstudio的，有免费版，可以满足大部分需求。

下载地址：[Rstudio下载地址](https://www.rstudio.com/products/rstudio/download/)

## Step 3 构建 jupyter R内核
首先我们打开R的命令行，如果不知道也可以直接打开Rsudio，在坐下角的console里写如下命令：

先安装一些依赖包
```R
install.packages(c('repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'))
```
接着在线安装 jupyter 的 R 内核
```R
devtools::install_github('IRkernel/IRkernel')
```
安装过程中可能会请求超时，多试几次就好了。

如果提示以下原因

"Skipping install of 'IRkernel' from a github remote, the SHA1 (719bbf5e) has not changed since last install.

 Use `force = TRUE` to force installation"
  
就使用强制安装
```R
devtools::install_github('IRkernel/IRkernel', force = TRUE)
```

## Step 4 安装 jupyter R内核
- 只在当前用户下安装
```R
IRkernel::installspec()
```
- 在系统下安装
```R
IRkernel::installspec(user = FALSE)
```

## Step 5 重启jupyter
重新启动后就可以看到如下页面：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Rkernel.png)

然后就可以在jupyter上进行编程了

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/Rexample.png)
