# 搭建Jupyter Notebook远程云服务器

## 1、安装jupyter
```
pip3 install jupyter
```
可能遇到问题
安装jupyter后，使用时显示找不到命令(-bash: jupyter: command not found)
解决方法
首先打开终端，在根目录下，找到jupyter是否存在
```
find -name jupyter
```
![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/fwq1.png)
发现了jupyter位置，注意bin文件是存放命令的，所以我们把它添加到环境变量
```
sudo vim /etc/profile
# 添加如下代码
export PATH=$PATH:~/.local/bin
# 退出编辑
source  /etc/profile
```
![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/fwq2.png)

之后再启动jupyter，就可以了。
![](https://github.com/Hourout/Jupyter-Extra-Features/blob/master/image/fwq3.png)

# 2、生成Jupyter Notebook配置文件
```
jupyter notebook --generate-config
```

# 3、自动密码设置
从笔记本电脑版本5.0开始，您可以使用单个命令输入并存储笔记本电脑服务器的密码。
jupyter笔记本密码将提示您输入密码，并将哈希密码记录在您的密码中 jupyter_notebook_config.json。
```
$ jupyter notebook password
Enter password:  ****
Verify password: ****
[NotebookPasswordApp] Wrote hashed password to /Users/you/.jupyter/jupyter_notebook_config.json
```

# 4、设置服务器配置文件
```
vim ~/.jupyter/jupyter_notebook_config.py
```

在末尾增加以下几行配置信息（此配置信息，也可在启动Jupyter时在参数中添加，但我认为那样看起来比较乱）
```
c.NotebookApp.ip = '*' #所有绑定服务器的IP都能访问，若想只在特定ip访问，输入ip地址即可
c.NotebookApp.port = 6666 #将端口设置为自己喜欢的吧，默认是8888
c.NotebookApp.open_browser = False #我们并不想在服务器上直接打开Jupyter Notebook，所以设置成False
c.NotebookApp.notebook_dir = '/root/jupyter_projects' #这里是设置Jupyter的根目录，若不设置将默认root的根目录，不安全
c.NotebookApp.allow_root = True # 为了安全，Jupyter默认不允许以root权限启动jupyter 
```

# 5、启动Jupyter 远程服务器
```
nohup jupyter notebook --allow-root &
```
