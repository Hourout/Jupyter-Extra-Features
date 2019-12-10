# python 环境搭建

参考[Python最佳实践指南](https://pythonguidecn.readthedocs.io/zh/latest/)

## 安装python
python安装我们我们推荐安装python3.6.5版本及以上，能够覆盖绝大多数的python生态，不建议使用python2.7
数据科学家推荐使用3.7.0+

### windows系统
- 打开 [python官网](https://www.python.org/downloads/windows/),下载你喜欢的版本，注意32位和64位的区别；
- 点击下载的.exe格式文件，如果有添加环境变量选项记得一定要勾选，点击推荐安装直到结束完成；
- 电脑cmd终端打开输入python即可。

### linux系统
#### Ubantu16.04+

#### CentOS7.5+
1、首先安装gcc编译器，gcc有些系统版本已经默认安装，通过  gcc --version  查看，没安装的先安装gcc
```
yum -y install gcc
```
2、安装其它依赖包，（注：不要缺少，否则有可能安装python出错，python3.7.0以下的版本可不装 libffi-devel ）
```
yum -y install zlib-devel bzip2-devel openssl-devel ncurses-devel sqlite-devel readline-devel tk-devel gdbm-devel db4-devel libpcap-devel xz-devel libffi-devel
```
3、下载python3.7.0源码，根据需求下载
在https://www.python.org/ftp/python/ 中选择自己需要的python源码包，我下载的是python3.7.0
```
wget https://www.python.org/ftp/python/3.7.0/Python-3.7.0.tgz
```
3、解压Python-3.7.0.tgz
```
tar -zxvf Python-3.7.0.tgz
```
4、建立一个空文件夹，用于存放python3程序
```
mkdir /usr/local/python3
```
5、执行配置文件，编译，编译安装
```
cd Python-3.7.0
./configure --prefix=/usr/local/python3
make && make install
```
安装完成没有提示错误便安装成功了

6、建立软连接
```
ln -s /usr/local/python3/bin/python3.7 /usr/bin/python3
ln -s /usr/local/python3/bin/pip3.7 /usr/bin/pip3
```
7、测试一下python3是否可以用
```
[root@mini Python-3.7.0]# python3
Python 3.7.0 (default, Jul 28 2018, 22:47:29)
[GCC 4.8.5 20150623 (Red Hat 4.8.5-28)] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print("hello world!")
hello world!
>>> exit()
[root@mini Python-3.7.0]# pip3 --version
pip 10.0.1 from /usr/local/python3/lib/python3.7/site-packages/pip (python 3.7)
```
可以看到python3.7.0可以正常使用

注：
安装完之后可能导致yum不能用，报错为：
```
# yum -y install redis 
  File "/usr/bin/yum", line 30
    except KeyboardInterrupt, e:
                            ^
SyntaxError: invalid syntax
```
解决办法：
```
vi /usr/bin/yum  和 /usr/libexec/urlgrabber-ext-down
```
将第一行"#!/usr/bin/python" 改为 "#!/usr/bin/python2.7"即可。
