# Bash in Jupyter

为Jupyter 增加 bash的内核要求系统需要python3版本，目前不支持python2，windows系统需要事先安装bash shell。

## Step 1 安装 bash_kernel python库
```
pip install bash_kernel
```

## Step 2 用python3安装 bash kernel
```
python -m bash_kernel.install
```

## Step 3 重启Jupyter
重启后就能看见Bash内核了，如图所示，

![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/bash_in_jupyter.png)
