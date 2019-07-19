# Java in Jupyter

默认系统已经预装好java和python3，java版本应满足"Java JDK > = 9"

## Step 1 下载 java 内核压缩包
手动下载也行，可以关注是否有新版
```
wget https://github.com/SpencerPark/IJava/releases/download/v1.3.0/ijava-1.3.0.zip
```

## Step 2 解压下载得压缩包
也可以手动解压
```
unzip ijava-1.3.0.zip
```
解压后得到一个 install.py 的文件，和一个 java 文件夹

## Step 3 安装 java 内核

在第二步解压后的文件夹中，执行以下命令安装：
```
python install.py --sys-prefix
```

## Step 4 重启jupyter
重新启动后就可以看到如下页面：

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/java_in_jupyter.png)

然后就可以在jupyter上进行编程了

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/java_in_jupyter1.png)
