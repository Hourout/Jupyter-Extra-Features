# Mysql in Jupyter

为Jupyter 增加 mysql的内核。

## Step 1 用pip安装 mysql_kernel
```
pip3 install mysql_kernel
```

## Step 2 将mysql kernel 添加到jupyter中
```
python3 -m mysql_kernel.install
```

## Step 3 重启Jupyter
重启后就能看见Mysql内核了，如图所示，

![](/image/mysql1.png)

使用方法

1: 设置 mysql host and port

2: 然后写 mysql 代码

![](/image/mysql2.png)
