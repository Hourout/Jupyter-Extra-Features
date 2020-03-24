# Hive in Jupyter

为Jupyter 增加 hive的内核。

## Step 1 用pip安装 hive_kernel
```
pip3 install hive_kernel
```

## Step 2 将hive kernel 添加到jupyter中
```
python3 -m hive_kernel.install
```

## Step 3 重启Jupyter
重启后就能看见Hive内核了，如图所示，

![](/image/hive2.png)

使用方法

1: 设置 hive host and port

2: 然后写 hive sql 代码

![](/image/hive1.png)
