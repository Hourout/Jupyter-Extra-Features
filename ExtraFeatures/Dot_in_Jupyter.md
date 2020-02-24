# Dot in Jupyter

为Jupyter 增加 dot的内核要求系统需要安装 graphviz。

## Step 1 安装 graphviz 
- macos系统
```
brew install graphviz
```
- ubuntu
```
sudo apt-get inatall graphviz
```
- centos7
```
sudo yum inatall graphviz
```

## Step 2 用pip安装 dot kernel
```
pip3 install dot_kernel
```

## Step 3 将dot kernel 添加到jupyter中
```
install-dot-kernel
```

## Step 4 重启Jupyter
重启后就能看见Dot内核了，如图所示，

![](/image/dot1.png)

![](/image/dot0.jpeg)

举个例子，输入如下代码：
```
// The graph name and the semicolons are optional
 graph graphname {
     a -- b -- c;
     b -- d;
 }
 ```
![](/image/dot2.png)

附：[graphviz/dot语言教程](https://github.com/laixintao/learn-dot)
