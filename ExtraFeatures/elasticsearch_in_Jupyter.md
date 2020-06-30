# Elasticsearch in Jupyter

为Jupyter 增加 elasticsearch 的内核。

## Step 1 用pip安装 elasticsearch_kernel
```
pip3 install elasticsearch_kernel
```

## Step 2 将elasticsearch kernel 添加到jupyter中
```
python3 -m elasticsearch_kernel.install
```

## Step 3 重启Jupyter
重启后就能看见 Elasticsearch 内核了，如图所示，

![](/image/elasticsearch1.png)

使用方法

1: 设置 elasticsearch host and port

2: 然后写 elasticsearch sql 代码

![](/image/elasticsearch2.png)
